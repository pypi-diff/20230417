# Comparing `tmp/buildbot-3.7.0.tar.gz` & `tmp/buildbot-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/buildbot-3.7.0.tar", last modified: Sun Dec  4 11:50:48 2022, max compression
+gzip compressed data, was "dist/buildbot-3.8.0.tar", last modified: Mon Apr 17 01:19:57 2023, max compression
```

## Comparing `buildbot-3.7.0.tar` & `buildbot-3.8.0.tar`

### file list

```diff
@@ -1,802 +1,803 @@
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15122 2022-12-04 11:48:49.000000 buildbot-3.7.0/COPYING
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3926 2022-12-04 11:48:49.000000 buildbot-3.7.0/CREDITS
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1158 2022-12-04 11:48:49.000000 buildbot-3.7.0/MANIFEST.in
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    26185 2022-12-04 11:50:48.000000 buildbot-3.7.0/NEWS
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5252 2022-12-04 11:50:48.000000 buildbot-3.7.0/PKG-INFO
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3703 2022-12-04 11:48:49.000000 buildbot-3.7.0/README.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      161 2022-12-04 11:48:49.000000 buildbot-3.7.0/UPGRADING
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/VERSION
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4595 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3283 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/asyncio.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7730 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/buildbot_net_usage_data.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      794 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/buildrequest.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/changes/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/changes/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5539 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/changes/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9050 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/changes/bitbucket.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7363 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/changes/changes.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6923 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/changes/filter.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21126 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/changes/gerritchangesource.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10637 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/changes/github.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18829 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/changes/gitpoller.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14891 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/changes/hgpoller.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    19102 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/changes/mail.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      945 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/changes/manager.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14167 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/changes/p4poller.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6335 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/changes/pb.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    19021 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/changes/svnpoller.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/clients/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/clients/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2651 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/clients/sendchange.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    31367 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/clients/tryclient.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1942 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/clients/usersclient.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/config/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      915 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/config/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6278 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/config/builder.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1463 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/config/checks.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1666 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/config/errors.py
--rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)    31012 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/config/master.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/configurators/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1640 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/configurators/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4034 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/configurators/janitor.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/data/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7952 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3790 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/build_data.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5381 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/builders.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12087 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/buildrequests.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9430 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/builds.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8972 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/buildsets.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8824 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/changes.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4139 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/changesources.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10662 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/connector.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1205 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/exceptions.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3855 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/forceschedulers.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11529 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/graphql.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5181 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/logchunks.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5241 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/logs.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7125 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/masters.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1213 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/patches.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5283 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/properties.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14664 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/resultspec.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1726 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/root.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4713 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/schedulers.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2764 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/sourcestamps.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5597 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/steps.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5508 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/test_result_sets.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3423 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/test_results.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12340 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/types.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6785 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/data/workers.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/db/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      823 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5687 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6170 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/build_data.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5977 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/builders.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9599 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/buildrequests.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10634 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/builds.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9627 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/buildsets.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15216 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/changes.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3932 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/changesources.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6459 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/connector.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2992 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/dbconfig.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8846 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/enginestrategy.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      756 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/exceptions.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16888 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/logs.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3966 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/masters.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1660 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/migrate_utils.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/db/migrations/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      333 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/migrations/README
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1942 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/migrations/alembic.ini
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/db/migrations/versions/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      375 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/migrations/versions/059_2021-09-07_alembic_initial.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/migrations/versions/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    45219 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/model.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9704 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/pool.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8250 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/schedulers.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7256 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/sourcestamps.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6772 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/state.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7222 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/steps.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1128 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/tags.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4640 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/test_result_sets.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12267 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/test_results.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/db/types/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/types/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1245 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/types/json.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9250 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/users.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9732 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/db/workers.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      862 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/errors.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10553 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/interfaces.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16251 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/locks.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/machine/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      705 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/machine/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1540 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/machine/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6527 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/machine/generic.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6536 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/machine/latent.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1217 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/machine/manager.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10768 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/manhole.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18825 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/master.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/monkeypatches/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2424 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/monkeypatches/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1107 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/monkeypatches/decorators.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1329 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/monkeypatches/servicechecks.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/mq/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/mq/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2556 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/mq/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2843 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/mq/connector.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3298 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/mq/simple.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4087 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/mq/wamp.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6389 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/pbutil.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/plugins/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1620 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/plugins/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9719 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/plugins/db.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/process/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      774 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    13811 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/botmaster.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    32837 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/build.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    17858 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/builder.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14139 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/buildrequest.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18471 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/buildrequestdistributor.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    34856 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/buildstep.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2893 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/cache.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1787 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/debug.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9756 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/factory.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7019 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/log.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4872 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/logobserver.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1363 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/measured_service.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    13898 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/metrics.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    31577 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/properties.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    20302 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/remotecommand.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5859 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/remotetransfer.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2768 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/results.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      876 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/subunitlogobserver.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/process/users/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/users/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1683 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/users/manager.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8822 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/users/manual.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4277 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/users/users.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7387 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/process/workerforbuilder.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/reporters/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4136 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6938 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/bitbucket.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16118 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/bitbucketserver.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/reporters/generators/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/generators/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4919 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/generators/build.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3544 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/generators/buildrequest.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5038 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/generators/buildset.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9205 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/generators/utils.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2745 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/generators/worker.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16587 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/gerrit.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9285 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/gerrit_verify_status.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10952 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/github.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8121 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/gitlab.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2638 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/http.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21132 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/irc.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    13369 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/mail.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16298 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/message.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3627 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/pushjet.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4501 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/pushover.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    39367 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/telegram.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10054 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/utils.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    50456 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/words.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3067 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/reporters/zulip.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3440 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/revlinks.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1275 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scheduler.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/schedulers/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/schedulers/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    17054 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/schedulers/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10875 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/schedulers/basic.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14043 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/schedulers/canceller.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6075 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/schedulers/canceller_buildset.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6317 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/schedulers/dependent.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      854 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/schedulers/filter.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    31109 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/schedulers/forcesched.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      944 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/schedulers/manager.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18014 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/schedulers/timed.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4840 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/schedulers/triggerable.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18077 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/schedulers/trysched.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/scripts/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10758 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1309 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/buildbot_tac.tmpl
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1928 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/checkconfig.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3661 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/cleanupdb.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3707 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/create_master.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1553 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/dataspec.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7918 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/devproxy.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1791 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/gengraphql.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6591 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/logwatcher.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3337 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/reconfig.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1114 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/restart.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    29948 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/runner.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4051 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/sample.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2058 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/sendchange.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5229 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/start.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2379 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/stop.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      825 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/trycmd.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1469 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/tryserver.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5184 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/upgrade_master.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1672 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/user.py
--rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)    22405 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/scripts/windows_service.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/secrets/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      705 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/secrets/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1552 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/secrets/manager.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/secrets/providers/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      705 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/secrets/providers/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1019 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/secrets/providers/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3232 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/secrets/providers/file.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2460 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/secrets/providers/passwordstore.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3801 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/secrets/providers/vault.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6902 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/secrets/providers/vault_hvac.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1615 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/secrets/secret.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/spec/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    31395 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/api.raml
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/spec/types/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3911 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/build.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1653 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/build_data.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1161 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/builder.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3358 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/buildrequest.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3821 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/buildset.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3863 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/change.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1371 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/changesource.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      893 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/forcescheduler.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       69 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/identifier.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3202 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/log.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2811 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/logchunk.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1876 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/master.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      954 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/patch.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      100 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/rootlink.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1427 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/scheduler.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1830 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/sourcedproperties.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1867 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/sourcestamp.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      272 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/spec.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3291 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/step.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2820 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/test_result.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6556 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/test_result_set.raml
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1614 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/spec/types/worker.raml
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/statistics/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1857 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/statistics/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12664 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/statistics/capture.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3510 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/statistics/stats_service.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/statistics/storage_backends/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      705 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/statistics/storage_backends/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      997 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/statistics/storage_backends/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2114 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/statistics/storage_backends/influxdb_client.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/steps/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2688 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/cmake.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3799 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/cppcheck.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2767 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/download_secret_to_worker.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3625 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/gitdiffinfo.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6664 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/http.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8288 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/master.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2408 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/maxq.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3659 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/mswin.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/steps/package/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      831 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/package/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/steps/package/deb/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/package/deb/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2881 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/package/deb/lintian.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7509 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/package/deb/pbuilder.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/steps/package/rpm/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1124 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/package/rpm/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5344 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/package/rpm/mock.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4852 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/package/rpm/rpmbuild.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2436 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/package/rpm/rpmlint.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1134 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/package/util.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14973 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/python.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16001 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/python_twisted.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    20997 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/shell.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4999 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/shellsequence.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/steps/source/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      779 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/source/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12455 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/source/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8733 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/source/bzr.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12327 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/source/cvs.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7579 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/source/darcs.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1967 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/source/gerrit.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    27093 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/source/git.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1000 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/source/github.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2139 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/source/gitlab.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    13170 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/source/mercurial.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12627 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/source/mtn.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15586 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/source/p4.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    19634 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/source/repo.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    17214 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/source/svn.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5705 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/subunit.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    19721 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/transfer.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15145 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/trigger.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18337 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/vstudio.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10850 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/steps/worker.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/test/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7133 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/test/fake/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1742 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/botmaster.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2631 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/bworkermanager.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1148 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/change.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2834 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/connection.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4046 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/docker.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6471 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/endpoint.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3186 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/fakebuild.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    24317 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/fakedata.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5362 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/fakemaster.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4021 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/fakemq.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2885 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/fakeprotocol.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2063 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/fakestats.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6598 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/httpclientservice.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2417 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/kube.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7509 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/latent.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2441 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/libvirt.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4314 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/logfile.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2509 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/machine.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1807 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/msgmanager.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6145 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/openstack.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1801 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/pbmanager.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1398 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/private_tempdir.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6029 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/reactor.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      404 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/secrets.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1022 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/state.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2191 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/step.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3426 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/web.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6092 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fake/worker.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/test/fakedb/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4346 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2075 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4104 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/build_data.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5367 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/builders.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7439 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/buildrequests.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7813 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/builds.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9535 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/buildsets.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9236 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/changes.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4564 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/changesources.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5073 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/connector.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5043 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/logs.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3035 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/masters.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6188 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/row.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7964 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/schedulers.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6315 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/sourcestamps.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4175 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/state.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6119 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/steps.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1656 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/tags.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4318 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/test_result_sets.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8457 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/test_results.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5288 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/users.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9264 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fakedb/workers.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/test/fuzz/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fuzz/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3301 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/fuzz/test_lru.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/test/integration/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/__init__.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/test/integration/interop/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      839 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/interop/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3282 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/interop/test_commandmixin.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4670 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/interop/test_compositestepmixin.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4832 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/interop/test_integration_secrets.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2381 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/interop/test_interruptcommand.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2555 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/interop/test_setpropertyfromcommand.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8011 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/interop/test_transfer.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2367 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/interop/test_worker_reconnect.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/test/integration/pki/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5558 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/pki/127.0.0.1.crt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1704 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/pki/127.0.0.1.key
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/test/integration/pki/ca/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1777 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/pki/ca/ca.crt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2235 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_URLs.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3544 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_configs.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4928 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_custom_buildstep.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4225 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_customservices.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12978 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_graphql.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3285 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_integration_force_with_patch.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4303 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_integration_mastershell.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2830 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_integration_scheduler_reconfigure.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5219 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_integration_secrets_with_vault.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5629 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_integration_secrets_with_vault_hvac.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2472 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_integration_template.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2605 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_integration_with_secrets.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    17635 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_locks.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4718 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_log_finish.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3221 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_master.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6921 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_notifier.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2366 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_process_botmaster.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11648 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_setup_entrypoints.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2542 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_stop_build.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5824 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_stop_trigger.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9963 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_telegram_bot.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4834 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_trigger.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10220 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_try_client.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2317 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_try_client_e2e.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10473 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_upgrade.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3117 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_usePty.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2416 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_virtual_builder.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9939 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_worker.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    13887 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_worker_comm.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4940 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_worker_kubernetes.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    63614 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_worker_latent.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4859 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_worker_marathon.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6272 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_worker_proxy.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5344 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_worker_upcloud.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11402 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_worker_workerside.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6367 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/integration/test_www.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2281 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/reactor.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/test/regressions/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/regressions/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2611 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/regressions/test_bad_change_properties_rows.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4231 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/regressions/test_oldpaths.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1932 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/regressions/test_steps_shell_WarningCountingShellCommand.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2823 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/runprocess.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    33416 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/steps.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2061 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/test_extra_coverage.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/test/unit/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3471 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_asyncio.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6034 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_buildbot_net_usage_data.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9502 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_clients_sendchange.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5422 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_clients_tryclient.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3409 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_clients_usersclient.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1259 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_configurator_base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8384 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_contrib_buildbot_cvs_mail.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5545 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_download_secret_to_worker.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2539 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_fake_httpclientservice.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4697 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_fake_secrets_manager.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3896 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_interpolate_secrets.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4167 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_janitor_configurator.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    27588 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_locks.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8592 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_machine_generic.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7737 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_master.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4869 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_mq.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1901 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_mq_base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3377 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_mq_connector.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2849 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_mq_simple.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9812 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_mq_wamp.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10098 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_plugins.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6342 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_revlinks.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4411 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_secret_in_file.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8301 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_secret_in_hvac.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5192 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_secret_in_passwordstore.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7508 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_secret_in_vault.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2088 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_secret_rendered_service.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21492 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_stats_service.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5389 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_steps_git_diffinfo.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/test/unit/test_templates_dir/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       13 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_templates_dir/builds.html
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/test/unit/test_templates_dir/plugin/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       43 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_templates_dir/plugin/plugin.jade
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7921 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_test_util_validation.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5699 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_test_util_warnings.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    17133 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_util.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8036 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_util_queue.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2294 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_version.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4292 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/unit/test_wamp_connector.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/test/util/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3747 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/changesource.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2280 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/config.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2708 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/configurators.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2736 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/connector_component.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11475 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/db.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2173 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/decorators.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1425 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/dirs.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4181 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/endpoint.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1307 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/fuzz.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15929 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/integration.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4734 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/interfaces.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1907 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/logging.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3971 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/migration.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5963 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/misc.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2857 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/patch_delay.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2097 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/pbmanager.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      969 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/properties.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2514 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/protocols.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3257 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/querylog.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8055 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/reporter.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3416 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/sandboxed_worker.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10092 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/scheduler.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2060 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/sourcesteps.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2099 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/tuplematching.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    22974 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/validation.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3861 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/warnings.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8030 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/test/util/www.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/util/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14791 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1548 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/_notifier.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1681 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/async_sort.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2713 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/backoff.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1391 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/bbcollections.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1711 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/codebase.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2309 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/config.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10256 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/croniter.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3775 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/debounce.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3568 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/deferwaiter.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2775 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/eventual.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12438 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/git.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1696 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/giturlparse.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8207 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/httpclientservice.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2019 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/identifiers.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9649 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/kubeclientservice.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1962 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/latent.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3585 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/lineboundaries.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7191 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/lru.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6234 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/maildir.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1718 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/misc.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2353 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/netstrings.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3687 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/path_expand_user.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2661 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/pathmatch.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5300 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/poll.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1771 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/private_tempdir.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2614 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/protocol.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1436 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/pullrequest.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5683 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/queue.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4301 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/raml.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10821 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/runprocess.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2895 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/sautils.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    20367 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/service.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9049 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/ssfilter.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1475 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/ssl.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1659 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/state.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3055 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/subscription.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5750 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/test_result_submitter.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      922 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/util/tuplematch.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/wamp/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/wamp/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6038 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/wamp/connector.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1385 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/warnings.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/worker/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      930 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    27700 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15305 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/docker.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    24359 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/ec2.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4825 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/kubernetes.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    22525 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/latent.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9321 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/libvirt.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2322 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/local.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6030 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/manager.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4665 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/marathon.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14998 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/openstack.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/worker/protocols/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/protocols/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5291 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/protocols/base.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/worker/protocols/manager/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/protocols/manager/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4745 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/protocols/manager/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16316 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/protocols/manager/msgpack.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3472 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/protocols/manager/pb.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16442 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/protocols/msgpack.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4105 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/protocols/null.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10737 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/protocols/pb.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8409 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/worker/upcloud.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/www/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7833 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/auth.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/www/authz/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      266 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/authz/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3462 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/authz/authz.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7733 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/authz/endpointmatchers.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3059 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/authz/roles.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9042 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/avatar.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6827 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/change_hook.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8575 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/config.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3735 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/graphql.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/buildbot/www/hooks/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        7 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/hooks/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3546 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/hooks/base.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2609 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/hooks/bitbucket.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6217 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/hooks/bitbucketcloud.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6722 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/hooks/bitbucketserver.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14474 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/hooks/github.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10571 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/hooks/gitlab.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2856 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/hooks/gitorious.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2255 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/hooks/poller.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6888 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/ldapuserinfo.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15374 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/oauth2.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1566 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/plugin.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3878 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/resource.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    17067 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/rest.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15693 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/service.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4744 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/sse.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9968 2022-12-04 11:48:49.000000 buildbot-3.7.0/buildbot/www/ws.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/docs/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5742 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/Makefile
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/docs/_images/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      909 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/Makefile
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21741 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/auth_rules.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    35904 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/auth_rules.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   289235 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/auth_rules_src.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3553 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/badges-badgeio.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9176 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/bitbucket-status-push.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    66019 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/changes.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   226083 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/changes.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   350488 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/changes_src.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    55985 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/forcedialog1.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9338 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/full_logo.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    23908 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/full_logo.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14232 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/header-text-transparent.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    96212 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/icon.blend
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2142 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/js-data-module-mvvm.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3884 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/js-data-module-wrappers.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   141026 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/master.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   180121 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/master.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   231416 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/master_src.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    38839 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/multimaster.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    50350 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/multimaster.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   306716 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/multimaster_src.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    66724 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/overview.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   109003 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/overview.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    68913 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/overview_src.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2024 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/success_normal.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    62274 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/vault_multipart_key.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    47787 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/vault_simple_key.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    52463 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/workers.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   168390 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/workers.svg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)   144624 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_images/workers_src.svg
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/docs/_static/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1076 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_static/buildbot_rtd.css
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21460 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_static/icon.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1180 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_static/icon.svg
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/docs/_templates/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       98 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/_templates/localtoc.html
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/docs/bbdocs/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/bbdocs/__init__.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2019 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/bbdocs/api_index.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    17822 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/bbdocs/ext.py
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8455 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/buildbot.1
--rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)    11822 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/conf.py
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/docs/developer/
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/docs/developer/_images/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    53561 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/_images/stats-service.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6096 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/auth.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      980 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/authz.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3039 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/br-claiming.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      712 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/classes.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4421 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-auth.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      714 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-avatar.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8862 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-basescheduler.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1059 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-build.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3996 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-buildfactory.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    25869 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-buildsteps.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1210 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-changesources.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6817 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-forcesched.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      545 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-iconfigurator.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      775 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-iproperties.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      461 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-irenderable.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3419 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-log.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4756 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-logobserver.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6909 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-protocols.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10500 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-remotecommands.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5144 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-resultspec.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      346 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-worker.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1233 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-workermanager.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1808 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/cls-www.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    19481 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/config.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    24282 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/data.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    20333 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/database.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1304 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/encodings.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      436 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/general.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      785 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/index.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3194 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/master-overview.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    41051 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/master-worker-msgpack.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15968 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/master-worker.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3816 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/metrics.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11359 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/mq.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3474 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/plugins-publish.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8592 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/pull-request.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5927 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/quickstart.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7493 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/rest.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2515 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/results.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5347 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/schedulers.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4866 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/secrets.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21940 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/stats-service.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11336 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/style.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    19947 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/tests.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    62607 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/utils.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9089 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/www-base-app.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9184 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/www-data-module.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8217 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/developer/www-server.rst
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/docs/examples/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7644 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/examples/git_gerrit.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11845 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/examples/gitlab.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2035 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/examples/hello.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5864 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/examples/repo_gerrit.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11904 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/examples/twisted_master.cfg
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1394 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/index.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      307 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/indices.rst
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/docs/manual/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    32853 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/cmdline.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18618 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/concepts.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    69490 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/customization.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9023 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/deploy.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      315 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/index.rst
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/docs/manual/installation/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3521 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/installation/buildmaster.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      598 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/installation/components.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      136 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/installation/index.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4356 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/installation/installation.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9347 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/installation/misc.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6350 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/installation/requirements.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15599 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/installation/worker.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4496 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/introduction.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1107 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/optimization.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2407 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/plugins.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      439 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/resources.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12183 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/manual/secretsmanagement.rst
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/docs/relnotes/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      381 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.3.1.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1384 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.3.2.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3225 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.3.3.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1394 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.3.4.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2566 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.3.5.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4717 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.4.0.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      870 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.4.1.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1273 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.4.2.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5033 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.4.3.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3516 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.5.0.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9535 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.6.0.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4465 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.6.1.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3171 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.6.2.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5496 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.6.3.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2865 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.6.4.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4674 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.6.5.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1502 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.6.6.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5206 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.7.0.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3989 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.7.1.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5707 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.7.10.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2073 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.7.11.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2586 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.7.12.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2847 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.7.2.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3187 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.7.3.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5827 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.7.4.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6699 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.7.5.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8892 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.7.6.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3800 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.7.7.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4234 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.7.8.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4598 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.7.9.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3188 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.8.0.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2134 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.8.1.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1878 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.8.10.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4701 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.8.12.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3056 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.8.2.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2337 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.8.3.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4744 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.8.4.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3702 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.8.5.txt
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8729 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.8.6.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11292 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.8.7.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6668 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.8.8.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18603 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.8.9.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    31328 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.9.0.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21087 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.9.0b1.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2529 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.9.0b2.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1894 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.9.0b3.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      804 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.9.0b4.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      723 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.9.0b5.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1558 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.9.0b6.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1298 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.9.0b7.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    22987 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.9.0b8.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3845 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.9.0b9.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3530 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.9.0rc1.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1746 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.9.0rc2.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      869 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.9.0rc3.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      623 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.9.0rc4.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7159 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.9.1.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    33722 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/0.9.2-0.9.15.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16525 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/1.x.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    41820 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/2.x.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    26185 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/relnotes/index.rst
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/docs/tutorial/
-drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2022-12-04 11:50:48.000000 buildbot-3.7.0/docs/tutorial/_images/
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    29673 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/tutorial/_images/builders.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    48591 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/tutorial/_images/force-build.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    33658 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/tutorial/_images/index.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    39220 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/tutorial/_images/irc-testrun.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    37741 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/tutorial/_images/runtests-success.png
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5310 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/tutorial/docker.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9454 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/tutorial/firstrun.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18445 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/tutorial/fiveminutes.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      156 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/tutorial/further.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)      119 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/tutorial/index.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11921 2022-12-04 11:48:49.000000 buildbot-3.7.0/docs/tutorial/tour.rst
--rw-r--r--   0 buildbot  (1000) buildbot  (1000)       35 2022-12-04 11:48:49.000000 buildbot-3.7.0/setup.cfg
--rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)    22981 2022-12-04 11:48:49.000000 buildbot-3.7.0/setup.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15122 2023-04-17 01:17:21.000000 buildbot-3.8.0/COPYING
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3926 2023-04-17 01:17:21.000000 buildbot-3.8.0/CREDITS
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1158 2023-04-17 01:17:21.000000 buildbot-3.8.0/MANIFEST.in
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    28214 2023-04-17 01:19:57.000000 buildbot-3.8.0/NEWS
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4752 2023-04-17 01:19:57.000000 buildbot-3.8.0/PKG-INFO
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3703 2023-04-17 01:17:21.000000 buildbot-3.8.0/README.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      161 2023-04-17 01:17:21.000000 buildbot-3.8.0/UPGRADING
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        5 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/VERSION
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4595 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3283 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/asyncio.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7958 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/buildbot_net_usage_data.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      794 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/buildrequest.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/changes/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/changes/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5539 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/changes/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9050 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/changes/bitbucket.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7363 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/changes/changes.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6923 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/changes/filter.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21126 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/changes/gerritchangesource.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10637 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/changes/github.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18829 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/changes/gitpoller.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14891 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/changes/hgpoller.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    19102 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/changes/mail.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      945 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/changes/manager.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14167 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/changes/p4poller.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6335 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/changes/pb.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    19021 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/changes/svnpoller.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/clients/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/clients/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2651 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/clients/sendchange.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    31367 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/clients/tryclient.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1942 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/clients/usersclient.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/config/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      915 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/config/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6278 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/config/builder.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1463 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/config/checks.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1666 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/config/errors.py
+-rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)    31012 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/config/master.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/configurators/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1640 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/configurators/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4034 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/configurators/janitor.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/data/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7952 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3790 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/build_data.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5381 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/builders.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12087 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/buildrequests.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9430 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/builds.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8972 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/buildsets.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8824 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/changes.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4139 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/changesources.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10662 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/connector.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1205 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/exceptions.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3855 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/forceschedulers.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11529 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/graphql.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5181 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/logchunks.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5241 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/logs.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7125 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/masters.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1213 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/patches.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5283 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/properties.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14664 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/resultspec.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1726 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/root.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4713 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/schedulers.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2764 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/sourcestamps.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5597 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/steps.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5508 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/test_result_sets.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3423 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/test_results.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12340 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/types.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6785 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/data/workers.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/db/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      823 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5687 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6170 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/build_data.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5977 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/builders.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9599 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/buildrequests.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10634 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/builds.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9627 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/buildsets.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15216 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/changes.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3932 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/changesources.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6459 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/connector.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2992 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/dbconfig.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8846 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/enginestrategy.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      756 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/exceptions.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16888 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/logs.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3966 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/masters.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1660 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/migrate_utils.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/db/migrations/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      333 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/migrations/README
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1942 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/migrations/alembic.ini
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/db/migrations/versions/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      375 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/migrations/versions/059_2021-09-07_alembic_initial.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/migrations/versions/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    45219 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/model.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9704 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/pool.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8250 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/schedulers.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7256 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/sourcestamps.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6772 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/state.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7222 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/steps.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1128 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/tags.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4640 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/test_result_sets.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12267 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/test_results.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/db/types/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/types/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1245 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/types/json.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9250 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/users.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9732 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/db/workers.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      862 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/errors.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10553 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/interfaces.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16251 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/locks.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/machine/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      705 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/machine/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1540 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/machine/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6527 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/machine/generic.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6536 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/machine/latent.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1217 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/machine/manager.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10768 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/manhole.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18825 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/master.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/monkeypatches/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2424 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/monkeypatches/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1107 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/monkeypatches/decorators.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1329 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/monkeypatches/servicechecks.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/mq/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/mq/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2556 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/mq/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2843 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/mq/connector.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3298 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/mq/simple.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4087 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/mq/wamp.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6389 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/pbutil.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/plugins/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1620 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/plugins/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9719 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/plugins/db.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/process/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      774 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    13811 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/botmaster.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    32837 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/build.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    17858 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/builder.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14139 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/buildrequest.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18471 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/buildrequestdistributor.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    34875 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/buildstep.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2893 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/cache.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1787 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/debug.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9756 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/factory.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7019 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/log.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4872 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/logobserver.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1363 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/measured_service.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    13898 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/metrics.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    31577 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/properties.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    20302 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/remotecommand.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5859 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/remotetransfer.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2768 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/results.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      876 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/subunitlogobserver.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/process/users/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/users/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1683 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/users/manager.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8822 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/users/manual.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4277 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/users/users.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7387 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/process/workerforbuilder.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/reporters/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4136 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6938 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/bitbucket.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16118 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/bitbucketserver.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/reporters/generators/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/generators/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4919 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/generators/build.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3544 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/generators/buildrequest.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5038 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/generators/buildset.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9205 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/generators/utils.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2745 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/generators/worker.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16587 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/gerrit.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9285 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/gerrit_verify_status.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10952 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/github.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8121 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/gitlab.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2638 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/http.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21132 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/irc.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    13369 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/mail.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16298 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/message.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3627 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/pushjet.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4501 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/pushover.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    39367 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/telegram.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10057 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/utils.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    50456 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/words.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3067 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/reporters/zulip.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3440 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/revlinks.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1275 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scheduler.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/schedulers/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/schedulers/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    17054 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/schedulers/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10875 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/schedulers/basic.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14043 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/schedulers/canceller.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6075 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/schedulers/canceller_buildset.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6317 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/schedulers/dependent.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      854 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/schedulers/filter.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    31109 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/schedulers/forcesched.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      944 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/schedulers/manager.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18014 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/schedulers/timed.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4840 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/schedulers/triggerable.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18077 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/schedulers/trysched.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/scripts/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10758 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1309 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/buildbot_tac.tmpl
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1928 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/checkconfig.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3661 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/cleanupdb.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3707 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/create_master.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1553 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/dataspec.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7918 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/devproxy.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1791 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/gengraphql.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6591 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/logwatcher.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3337 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/reconfig.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1114 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/restart.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    29948 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/runner.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4051 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/sample.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2058 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/sendchange.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5229 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/start.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2379 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/stop.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      825 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/trycmd.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1469 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/tryserver.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5184 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/upgrade_master.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1672 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/user.py
+-rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)    22405 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/scripts/windows_service.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/secrets/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      705 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/secrets/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1552 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/secrets/manager.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/secrets/providers/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      705 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/secrets/providers/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1019 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/secrets/providers/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3232 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/secrets/providers/file.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2460 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/secrets/providers/passwordstore.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3801 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/secrets/providers/vault.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6902 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/secrets/providers/vault_hvac.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1615 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/secrets/secret.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/spec/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    31395 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/api.raml
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/spec/types/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3911 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/build.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1653 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/build_data.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1161 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/builder.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3358 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/buildrequest.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3821 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/buildset.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3863 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/change.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1371 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/changesource.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      893 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/forcescheduler.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       69 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/identifier.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3202 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/log.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2811 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/logchunk.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1876 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/master.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      954 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/patch.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      100 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/rootlink.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1427 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/scheduler.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1830 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/sourcedproperties.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1867 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/sourcestamp.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      272 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/spec.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3291 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/step.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2820 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/test_result.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6556 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/test_result_set.raml
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1614 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/spec/types/worker.raml
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/statistics/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1857 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/statistics/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12456 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/statistics/capture.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3510 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/statistics/stats_service.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/statistics/storage_backends/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      705 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/statistics/storage_backends/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      997 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/statistics/storage_backends/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2114 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/statistics/storage_backends/influxdb_client.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/steps/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2688 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/cmake.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3799 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/cppcheck.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2767 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/download_secret_to_worker.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3625 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/gitdiffinfo.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6664 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/http.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8288 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/master.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2408 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/maxq.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3659 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/mswin.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/steps/package/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      831 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/package/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/steps/package/deb/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/package/deb/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2881 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/package/deb/lintian.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7509 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/package/deb/pbuilder.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/steps/package/rpm/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1124 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/package/rpm/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5344 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/package/rpm/mock.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4852 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/package/rpm/rpmbuild.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2436 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/package/rpm/rpmlint.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1134 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/package/util.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14973 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/python.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16001 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/python_twisted.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21151 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/shell.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4999 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/shellsequence.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/steps/source/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      779 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/source/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12455 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/source/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8733 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/source/bzr.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12327 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/source/cvs.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7579 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/source/darcs.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1967 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/source/gerrit.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    27093 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/source/git.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1000 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/source/github.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2139 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/source/gitlab.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    13170 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/source/mercurial.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12627 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/source/mtn.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15586 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/source/p4.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    19634 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/source/repo.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    17214 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/source/svn.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5705 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/subunit.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    19721 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/transfer.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15145 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/trigger.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18337 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/vstudio.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10850 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/steps/worker.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/test/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7153 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/test/fake/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1742 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/botmaster.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2631 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/bworkermanager.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1148 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/change.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2834 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/connection.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4046 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/docker.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6471 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/endpoint.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3186 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/fakebuild.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    24317 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/fakedata.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5362 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/fakemaster.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4021 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/fakemq.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2885 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/fakeprotocol.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2063 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/fakestats.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6598 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/httpclientservice.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2417 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/kube.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7621 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/latent.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2441 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/libvirt.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4314 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/logfile.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2509 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/machine.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1807 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/msgmanager.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6145 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/openstack.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1801 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/pbmanager.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1398 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/private_tempdir.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6029 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/reactor.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      404 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/secrets.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1022 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/state.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2191 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/step.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3426 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/web.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6092 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fake/worker.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/test/fakedb/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4346 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2075 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4104 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/build_data.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5367 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/builders.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7439 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/buildrequests.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7813 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/builds.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9535 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/buildsets.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9236 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/changes.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4564 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/changesources.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5073 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/connector.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5043 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/logs.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3035 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/masters.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6188 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/row.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7964 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/schedulers.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6315 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/sourcestamps.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4175 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/state.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6119 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/steps.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1656 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/tags.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4318 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/test_result_sets.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8457 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/test_results.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5288 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/users.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9264 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fakedb/workers.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/test/fuzz/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fuzz/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3301 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/fuzz/test_lru.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/test/integration/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/__init__.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/test/integration/interop/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      839 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/interop/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3291 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/interop/test_commandmixin.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4642 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/interop/test_compositestepmixin.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5038 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/interop/test_integration_secrets.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2495 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/interop/test_interruptcommand.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2560 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/interop/test_setpropertyfromcommand.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7870 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/interop/test_transfer.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2356 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/interop/test_worker_reconnect.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/test/integration/pki/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5558 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/pki/127.0.0.1.crt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1704 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/pki/127.0.0.1.key
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/test/integration/pki/ca/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1777 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/pki/ca/ca.crt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2321 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_URLs.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3544 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_configs.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4928 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_custom_buildstep.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4225 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_customservices.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3416 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_download_secret_to_worker.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12978 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_graphql.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3322 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_integration_force_with_patch.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4306 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_integration_mastershell.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2906 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_integration_scheduler_reconfigure.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5348 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_integration_secrets_with_vault.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5756 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_integration_secrets_with_vault_hvac.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2564 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_integration_template.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2702 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_integration_with_secrets.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    17635 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_locks.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4709 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_log_finish.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3222 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_master.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7129 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_notifier.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2366 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_process_botmaster.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11648 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_setup_entrypoints.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2530 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_stop_build.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6140 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_stop_trigger.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9963 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_telegram_bot.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4977 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_trigger.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10357 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_try_client.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2401 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_try_client_e2e.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10473 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_upgrade.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3190 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_usePty.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2512 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_virtual_builder.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9939 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_worker.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    13887 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_worker_comm.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5121 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_worker_kubernetes.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    65074 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_worker_latent.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5105 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_worker_marathon.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6257 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_worker_proxy.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5345 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_worker_upcloud.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11402 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_worker_workerside.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6367 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/integration/test_www.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2281 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/reactor.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/test/regressions/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/regressions/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2611 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/regressions/test_bad_change_properties_rows.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4231 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/regressions/test_oldpaths.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1932 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/regressions/test_steps_shell_WarningCountingShellCommand.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2823 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/runprocess.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    33383 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/steps.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2061 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/test_extra_coverage.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/test/unit/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3471 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_asyncio.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6034 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_buildbot_net_usage_data.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9502 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_clients_sendchange.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5422 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_clients_tryclient.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3409 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_clients_usersclient.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1259 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_configurator_base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8384 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_contrib_buildbot_cvs_mail.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5545 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_download_secret_to_worker.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2539 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_fake_httpclientservice.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4697 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_fake_secrets_manager.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3896 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_interpolate_secrets.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4167 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_janitor_configurator.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    27588 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_locks.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8592 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_machine_generic.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7737 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_master.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4869 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_mq.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1901 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_mq_base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3377 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_mq_connector.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2849 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_mq_simple.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9812 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_mq_wamp.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10098 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_plugins.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6342 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_revlinks.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4411 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_secret_in_file.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8301 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_secret_in_hvac.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5192 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_secret_in_passwordstore.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7508 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_secret_in_vault.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2088 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_secret_rendered_service.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21492 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_stats_service.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5389 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_steps_git_diffinfo.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/test/unit/test_templates_dir/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       13 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_templates_dir/builds.html
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/test/unit/test_templates_dir/plugin/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       43 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_templates_dir/plugin/plugin.jade
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7921 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_test_util_validation.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5699 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_test_util_warnings.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    17256 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_util.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8036 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_util_queue.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2294 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_version.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4292 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/unit/test_wamp_connector.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/test/util/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3747 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/changesource.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2280 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/config.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2708 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/configurators.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2736 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/connector_component.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11475 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/db.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2173 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/decorators.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1425 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/dirs.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4181 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/endpoint.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1307 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/fuzz.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15976 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/integration.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4537 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/interfaces.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1907 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/logging.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3971 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/migration.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5963 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/misc.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2857 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/patch_delay.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2097 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/pbmanager.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      969 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/properties.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2514 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/protocols.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3257 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/querylog.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8055 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/reporter.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3416 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/sandboxed_worker.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10092 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/scheduler.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2060 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/sourcesteps.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2099 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/tuplematching.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    22974 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/validation.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3861 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/warnings.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8030 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/test/util/www.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/util/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14885 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1548 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/_notifier.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1681 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/async_sort.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2713 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/backoff.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1391 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/bbcollections.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1711 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/codebase.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2309 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/config.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10256 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/croniter.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3775 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/debounce.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3568 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/deferwaiter.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2775 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/eventual.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12988 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/git.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1696 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/giturlparse.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8207 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/httpclientservice.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2019 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/identifiers.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9649 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/kubeclientservice.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1962 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/latent.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3585 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/lineboundaries.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7191 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/lru.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6234 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/maildir.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1718 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/misc.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2353 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/netstrings.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3687 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/path_expand_user.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2661 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/pathmatch.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5300 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/poll.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1771 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/private_tempdir.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2614 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/protocol.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1436 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/pullrequest.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5683 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/queue.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4301 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/raml.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11408 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/runprocess.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2895 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/sautils.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    20367 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/service.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9049 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/ssfilter.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1475 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/ssl.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1659 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/state.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3055 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/subscription.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5750 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/test_result_submitter.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      922 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/util/tuplematch.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/wamp/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/wamp/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6046 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/wamp/connector.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1385 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/warnings.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/worker/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      930 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    27700 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15305 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/docker.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    24359 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/ec2.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4825 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/kubernetes.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    24854 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/latent.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9423 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/libvirt.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2322 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/local.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6030 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/manager.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4665 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/marathon.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14998 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/openstack.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/worker/protocols/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/protocols/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5291 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/protocols/base.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/worker/protocols/manager/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/protocols/manager/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4745 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/protocols/manager/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16316 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/protocols/manager/msgpack.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3472 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/protocols/manager/pb.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16605 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/protocols/msgpack.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4105 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/protocols/null.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10737 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/protocols/pb.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8409 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/worker/upcloud.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/www/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7833 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/auth.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/www/authz/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      266 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/authz/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3462 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/authz/authz.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7733 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/authz/endpointmatchers.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3059 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/authz/roles.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9042 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/avatar.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6827 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/change_hook.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8575 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/config.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3735 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/graphql.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/buildbot/www/hooks/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        7 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/hooks/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3546 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/hooks/base.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2609 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/hooks/bitbucket.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6217 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/hooks/bitbucketcloud.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6722 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/hooks/bitbucketserver.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14802 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/hooks/github.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10571 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/hooks/gitlab.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2856 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/hooks/gitorious.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2255 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/hooks/poller.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6952 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/ldapuserinfo.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15374 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/oauth2.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1566 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/plugin.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3878 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/resource.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    17067 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/rest.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15693 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/service.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4744 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/sse.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9968 2023-04-17 01:17:21.000000 buildbot-3.8.0/buildbot/www/ws.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/docs/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5742 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/Makefile
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/docs/_images/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      909 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/Makefile
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21741 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/auth_rules.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    35904 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/auth_rules.svg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)   289235 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/auth_rules_src.svg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3553 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/badges-badgeio.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9176 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/bitbucket-status-push.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    66019 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/changes.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)   226083 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/changes.svg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)   350488 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/changes_src.svg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    55985 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/forcedialog1.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9338 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/full_logo.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    23908 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/full_logo.svg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    14232 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/header-text-transparent.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    96212 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/icon.blend
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2142 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/js-data-module-mvvm.svg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3884 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/js-data-module-wrappers.svg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)   141026 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/master.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)   180121 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/master.svg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)   231416 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/master_src.svg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    38839 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/multimaster.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    50350 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/multimaster.svg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)   306716 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/multimaster_src.svg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    66724 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/overview.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)   109003 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/overview.svg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    68913 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/overview_src.svg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2024 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/success_normal.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    62274 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/vault_multipart_key.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    47787 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/vault_simple_key.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    52463 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/workers.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)   168390 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/workers.svg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)   144624 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_images/workers_src.svg
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/docs/_static/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1076 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_static/buildbot_rtd.css
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21460 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_static/icon.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1180 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_static/icon.svg
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/docs/_templates/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       98 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/_templates/localtoc.html
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/docs/bbdocs/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/bbdocs/__init__.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2019 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/bbdocs/api_index.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    17822 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/bbdocs/ext.py
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8455 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/buildbot.1
+-rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)    11822 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/conf.py
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/docs/developer/
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/docs/developer/_images/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    53561 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/_images/stats-service.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6096 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/auth.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      980 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/authz.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3039 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/br-claiming.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      712 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/classes.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4421 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-auth.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      714 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-avatar.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8862 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-basescheduler.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1059 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-build.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3996 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-buildfactory.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    25869 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-buildsteps.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1210 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-changesources.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6817 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-forcesched.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      545 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-iconfigurator.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      775 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-iproperties.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      461 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-irenderable.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3419 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-log.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4756 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-logobserver.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6909 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-protocols.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    10500 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-remotecommands.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5144 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-resultspec.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      346 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-worker.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1233 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-workermanager.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1808 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/cls-www.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    19481 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/config.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    24282 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/data.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    20333 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/database.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1304 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/encodings.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      436 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/general.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      785 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/index.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3194 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/master-overview.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    41051 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/master-worker-msgpack.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15968 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/master-worker.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3816 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/metrics.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11359 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/mq.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3474 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/plugins-publish.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8592 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/pull-request.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5947 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/quickstart.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7493 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/rest.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2515 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/results.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5347 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/schedulers.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4866 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/secrets.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21940 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/stats-service.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11336 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/style.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    19947 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/tests.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    62607 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/utils.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9089 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/www-base-app.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9184 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/www-data-module.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8217 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/developer/www-server.rst
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/docs/examples/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7644 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/examples/git_gerrit.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11845 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/examples/gitlab.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2035 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/examples/hello.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5864 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/examples/repo_gerrit.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11904 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/examples/twisted_master.cfg
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1394 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/index.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      307 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/indices.rst
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/docs/manual/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    32853 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/cmdline.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18618 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/concepts.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    69782 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/customization.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9023 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/deploy.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      315 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/index.rst
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/docs/manual/installation/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3521 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/installation/buildmaster.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      598 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/installation/components.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      136 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/installation/index.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4356 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/installation/installation.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9347 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/installation/misc.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6350 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/installation/requirements.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    15599 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/installation/worker.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4496 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/introduction.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1107 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/optimization.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2407 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/plugins.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      439 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/resources.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    12183 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/manual/secretsmanagement.rst
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/docs/relnotes/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      381 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.3.1.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1384 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.3.2.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3225 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.3.3.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1394 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.3.4.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2566 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.3.5.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4717 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.4.0.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      870 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.4.1.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1273 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.4.2.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5033 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.4.3.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3516 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.5.0.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9535 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.6.0.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4465 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.6.1.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3171 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.6.2.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5496 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.6.3.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2865 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.6.4.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4674 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.6.5.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1502 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.6.6.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5206 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.7.0.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3989 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.7.1.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5707 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.7.10.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2073 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.7.11.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2586 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.7.12.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2847 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.7.2.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3187 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.7.3.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5827 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.7.4.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6699 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.7.5.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8892 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.7.6.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3800 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.7.7.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4234 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.7.8.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4598 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.7.9.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3188 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.8.0.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2134 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.8.1.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1878 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.8.10.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4701 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.8.12.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3056 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.8.2.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2337 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.8.3.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     4744 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.8.4.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3702 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.8.5.txt
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     8729 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.8.6.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11292 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.8.7.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     6668 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.8.8.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18603 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.8.9.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    31328 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.9.0.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    21087 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.9.0b1.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     2529 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.9.0b2.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1894 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.9.0b3.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      804 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.9.0b4.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      723 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.9.0b5.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1558 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.9.0b6.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1298 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.9.0b7.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    22987 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.9.0b8.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3845 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.9.0b9.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     3530 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.9.0rc1.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     1746 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.9.0rc2.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      869 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.9.0rc3.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      623 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.9.0rc4.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     7159 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.9.1.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    33722 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/0.9.2-0.9.15.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    16525 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/1.x.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    41820 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/2.x.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    28214 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/relnotes/index.rst
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/docs/tutorial/
+drwxr-xr-x   0 buildbot  (1000) buildbot  (1000)        0 2023-04-17 01:19:57.000000 buildbot-3.8.0/docs/tutorial/_images/
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    29673 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/tutorial/_images/builders.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    48591 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/tutorial/_images/force-build.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    33658 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/tutorial/_images/index.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    39220 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/tutorial/_images/irc-testrun.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    37741 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/tutorial/_images/runtests-success.png
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     5310 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/tutorial/docker.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)     9454 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/tutorial/firstrun.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    18445 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/tutorial/fiveminutes.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      156 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/tutorial/further.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)      119 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/tutorial/index.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)    11921 2023-04-17 01:17:21.000000 buildbot-3.8.0/docs/tutorial/tour.rst
+-rw-r--r--   0 buildbot  (1000) buildbot  (1000)       35 2023-04-17 01:17:21.000000 buildbot-3.8.0/setup.cfg
+-rwxr-xr-x   0 buildbot  (1000) buildbot  (1000)    23081 2023-04-17 01:17:21.000000 buildbot-3.8.0/setup.py
```

### Comparing `buildbot-3.7.0/COPYING` & `buildbot-3.8.0/COPYING`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/CREDITS` & `buildbot-3.8.0/CREDITS`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/MANIFEST.in` & `buildbot-3.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/NEWS` & `buildbot-3.8.0/NEWS`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,56 @@
     Buildbot uses towncrier to manage its release notes.
     towncrier helps to avoid the need for rebase when several people work at the same time on the release notes files.
 
     Each PR should come with a file in the newsfragment directory
 
 .. towncrier release notes start
 
+Buildbot ``3.8.0`` ( ``2023-04-16`` )
+=====================================
+
+Bug fixes
+---------
+
+- Fixed compatibility issues with Python 3.11.
+- Fixed compatibility with Autobahn v22.4.1 and newer.
+- Fixed issue with overriding `env` when calling `ShellMixin.makeRemoteShellCommand`
+- Buildbot will now include the previous location of moved files when evaluating a Github commit.
+  This fixes an issue where a commit that moves a file out of a folder, would not be shown in the
+  web UI for a builder that is tracking that same folder.
+- Improved reliability of Buildbot log watching to follow log files even after rotation.
+  This improves reliability of Buildbot start and restart scripts.
+- Fixed handling of occasional errors that happen when attempting to kill a master-side process that has already exited.
+- Fixed a race condition in PyLint step that may lead to step throwing exceptions.
+- Fixed compatibility with qemu 6.1 and newer when using LibVirtWorker with ``cheap_copy=True`` (default).
+- Fixed an issue with secrets provider stripping newline from ssh keys sent in git steps.
+- Fixed occasional errors that happen when killing processes on Windows. TASKKILL command may return
+  code 255 when process has already exited.
+- Fixed deleting secrets from worker that contain '~' in their destination path.
+
+Changes
+-------
+
+- Buildbot now requires NodeJS 14.18 or newer to build the frontend.
+- The URLs emitted by the Buildbot APIs have been changed to include slash after the hash (``#``)
+  symbol to be compatible with what React web UI supports.
+
+Improved Documentation
+----------------------
+
+- Replace statement "https is unsupported" with a more detailed disclaimer.
+
+Features
+--------
+
+- Add a way to disable default ``WarningCountingShellCommand`` parser.
+- Added health check API that latent workers can use to specify that a particular worker will not connect and build should not wait for it and mark itself as failure immediately.
+- Implemented a way to customize TLS setting for ``LdapUserInfo``.
+
+
 Buildbot ``3.7.0`` ( ``2022-12-04`` )
 =====================================
 
 Bug fixes
 ---------
 
 - Improved statistics capture to avoid negative build duration.
```

### Comparing `buildbot-3.7.0/PKG-INFO` & `buildbot-3.8.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,100 @@
 Metadata-Version: 2.1
 Name: buildbot
-Version: 3.7.0
+Version: 3.8.0
 Summary: The Continuous Integration Framework
 Home-page: http://buildbot.net/
 Author: Brian Warner
 Author-email: warner-buildbot@lothar.com
 Maintainer: Dustin J. Mitchell
 Maintainer-email: dustin@v.igoro.us
-License: UNKNOWN
-Description: Buildbot: The Continuous Integration Framework
-        ==============================================
-        
-        :Site: https://buildbot.net
-        :Original author: Brian Warner <warner-buildbot @ lothar . com>
-        :Current maintainer: `The Botherders <https://github.com/buildbot/botherders>`_.
-        
-        .. contents::
-           :local:
-        
-        Buildbot is an open-source continuous integration framework for automating software build, test, and release processes.
-        
-        * Buildbot is easy to set up, but very extensible and customizable.
-          It supports arbitrary build processes, and is not limited to common build processes for particular languages (e.g., autotools or ant)
-        * Buildbot supports building and testing on a variety of platforms.
-          Developers, who do not have the facilities to test their changes everywhere before committing, will know shortly afterwards whether they have broken the build or not.
-        * Buildbot allows to track various metrics (warning counts, lint checks, image size, compile time, etc) over time.
-        * Buildbot has minimal requirements for workers: using virtualenv, only a Python installation is required.
-        * Workers can be run behind a NAT firewall and communicate with the master.
-        * Buildbot has a variety of status-reporting tools to get information about builds in front of developers in a timely manner.
-        
-        Documentation
-        -------------
-        
-        See https://docs.buildbot.net/current/ for documentation of the current version of Buildbot.
-        
-        Docker container
-        ----------------
-        Buildbot comes with a ready to use docker container available at buildbot/buildbot-master
-        Following environment variables are supported for configuration:
-        
-        * ``BUILDBOT_CONFIG_URL``: http url to a config tarball.
-            The tarball must be in the .tar.gz format.
-            The tarball must contain a directory, which will contain a master.cfg file in it.
-            The tarball may contain a twisted.tac file in it, which can be used to configure the twisted logging system (e.g to log in logstash instead of the default stdout).
-            The tarball will be extracted in a directory named ``$BUILDBOT_CONFIG_DIR`` in the master directory, and can contain additional python module that the master.cfg can load.
-            If ``BUILDBOT_CONFIG_URL`` does not end with .tar.gz, it is considered to be an URL to the direct ``master.cfg``
-        
-        * ``BUILDBOT_CONFIG_DIR`` directory where to extract the config tarball within the master directory.
-          It is important so that you can do relative imports in your master.cfg like it is done in the metabbotcfg (https://github.com/buildbot/metabbotcfg)
-        
-        
-        Requirements
-        ------------
-        
-        See https://docs.buildbot.net/current/manual/installation/index.html
-        
-        Briefly: python, Twisted, Jinja2, simplejson, and SQLite.
-        Simplejson and SQLite are included with recent versions of Python.
-        
-        Contributing
-        -------------
-        
-        Please send your patches to https://github.com/buildbot/buildbot/
-        
-        Support
-        -------
-        
-        Please send questions, file bugs, etc, on the Buildbot Github project https://github.com/buildbot/buildbot/issues.
-        Alternatively, write to the buildbot-devel mailing list reachable through https://buildbot.net/.
-        
-        Copying
-        -------
-        
-        Buildbot is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, version 2.
-        
-        This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
-        See the GNU General Public License for more details.
-        
-        For full details, please see the file named COPYING in the top directory of the source tree.
-        You should have received a copy of the GNU General Public License along with this program.
-        If not, see <http://www.gnu.org/licenses/>.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: test
 Provides-Extra: bundle
 Provides-Extra: tls
 Provides-Extra: docs
+License-File: COPYING
+
+Buildbot: The Continuous Integration Framework
+==============================================
+
+:Site: https://buildbot.net
+:Original author: Brian Warner <warner-buildbot @ lothar . com>
+:Current maintainer: `The Botherders <https://github.com/buildbot/botherders>`_.
+
+.. contents::
+   :local:
+
+Buildbot is an open-source continuous integration framework for automating software build, test, and release processes.
+
+* Buildbot is easy to set up, but very extensible and customizable.
+  It supports arbitrary build processes, and is not limited to common build processes for particular languages (e.g., autotools or ant)
+* Buildbot supports building and testing on a variety of platforms.
+  Developers, who do not have the facilities to test their changes everywhere before committing, will know shortly afterwards whether they have broken the build or not.
+* Buildbot allows to track various metrics (warning counts, lint checks, image size, compile time, etc) over time.
+* Buildbot has minimal requirements for workers: using virtualenv, only a Python installation is required.
+* Workers can be run behind a NAT firewall and communicate with the master.
+* Buildbot has a variety of status-reporting tools to get information about builds in front of developers in a timely manner.
+
+Documentation
+-------------
+
+See https://docs.buildbot.net/current/ for documentation of the current version of Buildbot.
+
+Docker container
+----------------
+Buildbot comes with a ready to use docker container available at buildbot/buildbot-master
+Following environment variables are supported for configuration:
+
+* ``BUILDBOT_CONFIG_URL``: http url to a config tarball.
+    The tarball must be in the .tar.gz format.
+    The tarball must contain a directory, which will contain a master.cfg file in it.
+    The tarball may contain a twisted.tac file in it, which can be used to configure the twisted logging system (e.g to log in logstash instead of the default stdout).
+    The tarball will be extracted in a directory named ``$BUILDBOT_CONFIG_DIR`` in the master directory, and can contain additional python module that the master.cfg can load.
+    If ``BUILDBOT_CONFIG_URL`` does not end with .tar.gz, it is considered to be an URL to the direct ``master.cfg``
+
+* ``BUILDBOT_CONFIG_DIR`` directory where to extract the config tarball within the master directory.
+  It is important so that you can do relative imports in your master.cfg like it is done in the metabbotcfg (https://github.com/buildbot/metabbotcfg)
+
+
+Requirements
+------------
+
+See https://docs.buildbot.net/current/manual/installation/index.html
+
+Briefly: python, Twisted, Jinja2, simplejson, and SQLite.
+Simplejson and SQLite are included with recent versions of Python.
+
+Contributing
+-------------
+
+Please send your patches to https://github.com/buildbot/buildbot/
+
+Support
+-------
+
+Please send questions, file bugs, etc, on the Buildbot Github project https://github.com/buildbot/buildbot/issues.
+Alternatively, write to the buildbot-devel mailing list reachable through https://buildbot.net/.
+
+Copying
+-------
+
+Buildbot is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, version 2.
+
+This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU General Public License for more details.
+
+For full details, please see the file named COPYING in the top directory of the source tree.
+You should have received a copy of the GNU General Public License along with this program.
+If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `buildbot-3.7.0/README.rst` & `buildbot-3.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/__init__.py` & `buildbot-3.8.0/buildbot/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/asyncio.py` & `buildbot-3.8.0/buildbot/asyncio.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/buildbot_net_usage_data.py` & `buildbot-3.8.0/buildbot/buildbot_net_usage_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,24 +39,32 @@
 # This can't change! or we will need to make sure we are compatible with all
 # released version of buildbot >=0.9.0
 PHONE_HOME_URL = "https://events.buildbot.net/events/phone_home"
 
 
 def linux_distribution():
     os_release = "/etc/os-release"
-    meta_data = {'ID': "unknown_linux", 'VERSION_ID': "unknown_version"}
+    meta_data = {}
     if os.path.exists(os_release):
         with open("/etc/os-release", encoding='utf-8') as f:
             for line in f:
                 try:
                     k, v = line.strip().split("=")
                     meta_data[k] = v.strip('""')
                 except Exception:
                     pass
-    return meta_data['ID'], meta_data['VERSION_ID']
+
+    linux_id = meta_data.get("ID", "unknown_linux")
+
+    linux_version = "unknown_version"
+    # Pre-release versions of Debian contain VERSION_CODENAME but not VERSION_ID
+    for version_key in ["VERSION_ID", "VERSION_CODENAME"]:
+        linux_version = meta_data.get(version_key, linux_version)
+
+    return linux_id, linux_version
 
 
 def get_distro():
     system = platform.system()
     if system == "Linux":
         dist = linux_distribution()
         return f"{dist[0]}:{dist[1]}"
```

### Comparing `buildbot-3.7.0/buildbot/buildrequest.py` & `buildbot-3.8.0/buildbot/buildrequest.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/changes/base.py` & `buildbot-3.8.0/buildbot/changes/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/changes/bitbucket.py` & `buildbot-3.8.0/buildbot/changes/bitbucket.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/changes/changes.py` & `buildbot-3.8.0/buildbot/changes/changes.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/changes/filter.py` & `buildbot-3.8.0/buildbot/changes/filter.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/changes/gerritchangesource.py` & `buildbot-3.8.0/buildbot/changes/gerritchangesource.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/changes/github.py` & `buildbot-3.8.0/buildbot/changes/github.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/changes/gitpoller.py` & `buildbot-3.8.0/buildbot/changes/gitpoller.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/changes/hgpoller.py` & `buildbot-3.8.0/buildbot/changes/hgpoller.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/changes/mail.py` & `buildbot-3.8.0/buildbot/changes/mail.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/changes/manager.py` & `buildbot-3.8.0/buildbot/changes/manager.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/changes/p4poller.py` & `buildbot-3.8.0/buildbot/changes/p4poller.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/changes/pb.py` & `buildbot-3.8.0/buildbot/changes/pb.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/changes/svnpoller.py` & `buildbot-3.8.0/buildbot/changes/svnpoller.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/clients/sendchange.py` & `buildbot-3.8.0/buildbot/clients/sendchange.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/clients/tryclient.py` & `buildbot-3.8.0/buildbot/clients/tryclient.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/clients/usersclient.py` & `buildbot-3.8.0/buildbot/clients/usersclient.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/config/__init__.py` & `buildbot-3.8.0/buildbot/config/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/config/builder.py` & `buildbot-3.8.0/buildbot/config/builder.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/config/checks.py` & `buildbot-3.8.0/buildbot/config/checks.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/config/errors.py` & `buildbot-3.8.0/buildbot/config/errors.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/config/master.py` & `buildbot-3.8.0/buildbot/config/master.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/configurators/__init__.py` & `buildbot-3.8.0/buildbot/configurators/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/configurators/janitor.py` & `buildbot-3.8.0/buildbot/configurators/janitor.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/base.py` & `buildbot-3.8.0/buildbot/data/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/build_data.py` & `buildbot-3.8.0/buildbot/data/build_data.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/builders.py` & `buildbot-3.8.0/buildbot/data/builders.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/buildrequests.py` & `buildbot-3.8.0/buildbot/data/buildrequests.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/builds.py` & `buildbot-3.8.0/buildbot/data/builds.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/buildsets.py` & `buildbot-3.8.0/buildbot/data/buildsets.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/changes.py` & `buildbot-3.8.0/buildbot/data/changes.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/changesources.py` & `buildbot-3.8.0/buildbot/data/changesources.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/connector.py` & `buildbot-3.8.0/buildbot/data/connector.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/exceptions.py` & `buildbot-3.8.0/buildbot/data/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/forceschedulers.py` & `buildbot-3.8.0/buildbot/data/forceschedulers.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/graphql.py` & `buildbot-3.8.0/buildbot/data/graphql.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/logchunks.py` & `buildbot-3.8.0/buildbot/data/logchunks.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/logs.py` & `buildbot-3.8.0/buildbot/data/logs.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/masters.py` & `buildbot-3.8.0/buildbot/data/masters.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/patches.py` & `buildbot-3.8.0/buildbot/data/patches.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/properties.py` & `buildbot-3.8.0/buildbot/data/properties.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/resultspec.py` & `buildbot-3.8.0/buildbot/data/resultspec.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/root.py` & `buildbot-3.8.0/buildbot/data/root.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/schedulers.py` & `buildbot-3.8.0/buildbot/data/schedulers.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/sourcestamps.py` & `buildbot-3.8.0/buildbot/data/sourcestamps.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/steps.py` & `buildbot-3.8.0/buildbot/data/steps.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/test_result_sets.py` & `buildbot-3.8.0/buildbot/data/test_result_sets.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/test_results.py` & `buildbot-3.8.0/buildbot/data/test_results.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/types.py` & `buildbot-3.8.0/buildbot/data/types.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/data/workers.py` & `buildbot-3.8.0/buildbot/data/workers.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/__init__.py` & `buildbot-3.8.0/buildbot/db/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/base.py` & `buildbot-3.8.0/buildbot/db/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/build_data.py` & `buildbot-3.8.0/buildbot/db/build_data.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/builders.py` & `buildbot-3.8.0/buildbot/db/builders.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/buildrequests.py` & `buildbot-3.8.0/buildbot/db/buildrequests.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/builds.py` & `buildbot-3.8.0/buildbot/db/builds.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/buildsets.py` & `buildbot-3.8.0/buildbot/db/buildsets.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/changes.py` & `buildbot-3.8.0/buildbot/db/changes.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/changesources.py` & `buildbot-3.8.0/buildbot/db/changesources.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/connector.py` & `buildbot-3.8.0/buildbot/db/connector.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/dbconfig.py` & `buildbot-3.8.0/buildbot/db/dbconfig.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/enginestrategy.py` & `buildbot-3.8.0/buildbot/db/enginestrategy.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/exceptions.py` & `buildbot-3.8.0/buildbot/db/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/logs.py` & `buildbot-3.8.0/buildbot/db/logs.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/masters.py` & `buildbot-3.8.0/buildbot/db/masters.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/migrate_utils.py` & `buildbot-3.8.0/buildbot/db/migrate_utils.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/migrations/alembic.ini` & `buildbot-3.8.0/buildbot/db/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/model.py` & `buildbot-3.8.0/buildbot/db/model.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/pool.py` & `buildbot-3.8.0/buildbot/db/pool.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/schedulers.py` & `buildbot-3.8.0/buildbot/db/schedulers.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/sourcestamps.py` & `buildbot-3.8.0/buildbot/db/sourcestamps.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/state.py` & `buildbot-3.8.0/buildbot/db/state.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/steps.py` & `buildbot-3.8.0/buildbot/db/steps.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/tags.py` & `buildbot-3.8.0/buildbot/db/tags.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/test_result_sets.py` & `buildbot-3.8.0/buildbot/db/test_result_sets.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/test_results.py` & `buildbot-3.8.0/buildbot/db/test_results.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/types/json.py` & `buildbot-3.8.0/buildbot/db/types/json.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/users.py` & `buildbot-3.8.0/buildbot/db/users.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/db/workers.py` & `buildbot-3.8.0/buildbot/db/workers.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/errors.py` & `buildbot-3.8.0/buildbot/errors.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/interfaces.py` & `buildbot-3.8.0/buildbot/interfaces.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/locks.py` & `buildbot-3.8.0/buildbot/locks.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/machine/__init__.py` & `buildbot-3.8.0/buildbot/machine/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/machine/base.py` & `buildbot-3.8.0/buildbot/machine/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/machine/generic.py` & `buildbot-3.8.0/buildbot/machine/generic.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/machine/latent.py` & `buildbot-3.8.0/buildbot/machine/latent.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/machine/manager.py` & `buildbot-3.8.0/buildbot/machine/manager.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/manhole.py` & `buildbot-3.8.0/buildbot/manhole.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/master.py` & `buildbot-3.8.0/buildbot/master.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/monkeypatches/__init__.py` & `buildbot-3.8.0/buildbot/monkeypatches/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/monkeypatches/decorators.py` & `buildbot-3.8.0/buildbot/monkeypatches/decorators.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/monkeypatches/servicechecks.py` & `buildbot-3.8.0/buildbot/monkeypatches/servicechecks.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/mq/base.py` & `buildbot-3.8.0/buildbot/mq/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/mq/connector.py` & `buildbot-3.8.0/buildbot/mq/connector.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/mq/simple.py` & `buildbot-3.8.0/buildbot/mq/simple.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/mq/wamp.py` & `buildbot-3.8.0/buildbot/mq/wamp.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/pbutil.py` & `buildbot-3.8.0/buildbot/pbutil.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/plugins/__init__.py` & `buildbot-3.8.0/buildbot/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/plugins/db.py` & `buildbot-3.8.0/buildbot/plugins/db.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/base.py` & `buildbot-3.8.0/buildbot/process/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/botmaster.py` & `buildbot-3.8.0/buildbot/process/botmaster.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/build.py` & `buildbot-3.8.0/buildbot/process/build.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/builder.py` & `buildbot-3.8.0/buildbot/process/builder.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/buildrequest.py` & `buildbot-3.8.0/buildbot/process/buildrequest.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/buildrequestdistributor.py` & `buildbot-3.8.0/buildbot/process/buildrequestdistributor.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/buildstep.py` & `buildbot-3.8.0/buildbot/process/buildstep.py`

 * *Files 0% similar despite different names*

```diff
@@ -911,16 +911,18 @@
             del kwargs['interruptSignal']
 
         # lazylogfiles are handled below
         del kwargs['lazylogfiles']
 
         # merge the builder's environment with that supplied here
         builderEnv = self.build.builder.config.env
-        kwargs['env'] = yield self.build.render(builderEnv)
-        kwargs['env'].update(self.env)
+        kwargs['env'] = {
+            **(yield self.build.render(builderEnv)),
+            **kwargs['env'],
+        }
         kwargs['stdioLogName'] = stdioLogName
 
         # default the workdir appropriately
         if not kwargs.get('workdir') and not self.workdir:
             if callable(self.build.workdir):
                 kwargs['workdir'] = self.build.workdir(self.build.sources)
             else:
```

### Comparing `buildbot-3.7.0/buildbot/process/cache.py` & `buildbot-3.8.0/buildbot/process/cache.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/debug.py` & `buildbot-3.8.0/buildbot/process/debug.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/factory.py` & `buildbot-3.8.0/buildbot/process/factory.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/log.py` & `buildbot-3.8.0/buildbot/process/log.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/logobserver.py` & `buildbot-3.8.0/buildbot/process/logobserver.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/measured_service.py` & `buildbot-3.8.0/buildbot/process/measured_service.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/metrics.py` & `buildbot-3.8.0/buildbot/process/metrics.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/properties.py` & `buildbot-3.8.0/buildbot/process/properties.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/remotecommand.py` & `buildbot-3.8.0/buildbot/process/remotecommand.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/remotetransfer.py` & `buildbot-3.8.0/buildbot/process/remotetransfer.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/results.py` & `buildbot-3.8.0/buildbot/process/results.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/subunitlogobserver.py` & `buildbot-3.8.0/buildbot/process/subunitlogobserver.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/users/manager.py` & `buildbot-3.8.0/buildbot/process/users/manager.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/users/manual.py` & `buildbot-3.8.0/buildbot/process/users/manual.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/users/users.py` & `buildbot-3.8.0/buildbot/process/users/users.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/process/workerforbuilder.py` & `buildbot-3.8.0/buildbot/process/workerforbuilder.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/base.py` & `buildbot-3.8.0/buildbot/reporters/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/bitbucket.py` & `buildbot-3.8.0/buildbot/reporters/bitbucket.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/bitbucketserver.py` & `buildbot-3.8.0/buildbot/reporters/bitbucketserver.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/generators/build.py` & `buildbot-3.8.0/buildbot/reporters/generators/build.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/generators/buildrequest.py` & `buildbot-3.8.0/buildbot/reporters/generators/buildrequest.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/generators/buildset.py` & `buildbot-3.8.0/buildbot/reporters/generators/buildset.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/generators/utils.py` & `buildbot-3.8.0/buildbot/reporters/generators/utils.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/generators/worker.py` & `buildbot-3.8.0/buildbot/reporters/generators/worker.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/gerrit.py` & `buildbot-3.8.0/buildbot/reporters/gerrit.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/gerrit_verify_status.py` & `buildbot-3.8.0/buildbot/reporters/gerrit_verify_status.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/github.py` & `buildbot-3.8.0/buildbot/reporters/github.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/gitlab.py` & `buildbot-3.8.0/buildbot/reporters/gitlab.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/http.py` & `buildbot-3.8.0/buildbot/reporters/http.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/irc.py` & `buildbot-3.8.0/buildbot/reporters/irc.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/mail.py` & `buildbot-3.8.0/buildbot/reporters/mail.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/message.py` & `buildbot-3.8.0/buildbot/reporters/message.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/pushjet.py` & `buildbot-3.8.0/buildbot/reporters/pushjet.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/pushover.py` & `buildbot-3.8.0/buildbot/reporters/pushover.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/telegram.py` & `buildbot-3.8.0/buildbot/reporters/telegram.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/utils.py` & `buildbot-3.8.0/buildbot/reporters/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,25 +219,25 @@
     blamelist = list(blamelist)
     blamelist.sort()
     return blamelist
 
 
 def getURLForBuild(master, builderid, build_number):
     prefix = master.config.buildbotURL
-    return prefix + f"#builders/{builderid}/builds/{build_number}"
+    return prefix + f"#/builders/{builderid}/builds/{build_number}"
 
 
 def getURLForBuildrequest(master, buildrequestid):
     prefix = master.config.buildbotURL
-    return f"{prefix}#buildrequests/{buildrequestid}"
+    return f"{prefix}#/buildrequests/{buildrequestid}"
 
 
 def get_url_for_log(master, builderid, build_number, step_number, log_slug):
     prefix = master.config.buildbotURL
-    return f"{prefix}#builders/{builderid}/builds/{build_number}/" + \
+    return f"{prefix}#/builders/{builderid}/builds/{build_number}/" + \
         f"steps/{step_number}/logs/{log_slug}"
 
 
 @renderer
 def URLForBuild(props):
     build = props.getBuild()
     return build.getUrl()
```

### Comparing `buildbot-3.7.0/buildbot/reporters/words.py` & `buildbot-3.8.0/buildbot/reporters/words.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/reporters/zulip.py` & `buildbot-3.8.0/buildbot/reporters/zulip.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/revlinks.py` & `buildbot-3.8.0/buildbot/revlinks.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scheduler.py` & `buildbot-3.8.0/buildbot/scheduler.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/schedulers/base.py` & `buildbot-3.8.0/buildbot/schedulers/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/schedulers/basic.py` & `buildbot-3.8.0/buildbot/schedulers/basic.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/schedulers/canceller.py` & `buildbot-3.8.0/buildbot/schedulers/canceller.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/schedulers/canceller_buildset.py` & `buildbot-3.8.0/buildbot/schedulers/canceller_buildset.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/schedulers/dependent.py` & `buildbot-3.8.0/buildbot/schedulers/dependent.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/schedulers/filter.py` & `buildbot-3.8.0/buildbot/schedulers/filter.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/schedulers/forcesched.py` & `buildbot-3.8.0/buildbot/schedulers/forcesched.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/schedulers/manager.py` & `buildbot-3.8.0/buildbot/schedulers/manager.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/schedulers/timed.py` & `buildbot-3.8.0/buildbot/schedulers/timed.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/schedulers/triggerable.py` & `buildbot-3.8.0/buildbot/schedulers/triggerable.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/schedulers/trysched.py` & `buildbot-3.8.0/buildbot/schedulers/trysched.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/base.py` & `buildbot-3.8.0/buildbot/scripts/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/buildbot_tac.tmpl` & `buildbot-3.8.0/buildbot/scripts/buildbot_tac.tmpl`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/checkconfig.py` & `buildbot-3.8.0/buildbot/scripts/checkconfig.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/cleanupdb.py` & `buildbot-3.8.0/buildbot/scripts/cleanupdb.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/create_master.py` & `buildbot-3.8.0/buildbot/scripts/create_master.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/dataspec.py` & `buildbot-3.8.0/buildbot/scripts/dataspec.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/devproxy.py` & `buildbot-3.8.0/buildbot/scripts/devproxy.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/gengraphql.py` & `buildbot-3.8.0/buildbot/scripts/gengraphql.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/logwatcher.py` & `buildbot-3.8.0/buildbot/scripts/logwatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         if platform.system().lower() == 'sunos' and os.path.exists('/usr/xpg4/bin/tail'):
             tailBin = "/usr/xpg4/bin/tail"
         elif platform.system().lower() == 'haiku' and os.path.exists('/bin/tail'):
             tailBin = "/bin/tail"
         else:
             tailBin = "/usr/bin/tail"
 
-        args = ("tail", "-f", "-n", "0", self.logfile)
+        args = ("tail", "-F", "-n", "0", self.logfile)
         self.p = self._reactor.spawnProcess(self.pp, tailBin, args,
                                             env=os.environ)
         self.running = True
         d = defer.maybeDeferred(self._start)
         return d
 
     def _start(self):
```

### Comparing `buildbot-3.7.0/buildbot/scripts/reconfig.py` & `buildbot-3.8.0/buildbot/scripts/reconfig.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/restart.py` & `buildbot-3.8.0/buildbot/scripts/restart.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/runner.py` & `buildbot-3.8.0/buildbot/scripts/runner.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/sample.cfg` & `buildbot-3.8.0/buildbot/scripts/sample.cfg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/sendchange.py` & `buildbot-3.8.0/buildbot/scripts/sendchange.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/start.py` & `buildbot-3.8.0/buildbot/scripts/start.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/stop.py` & `buildbot-3.8.0/buildbot/scripts/stop.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/trycmd.py` & `buildbot-3.8.0/buildbot/scripts/trycmd.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/tryserver.py` & `buildbot-3.8.0/buildbot/scripts/tryserver.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/upgrade_master.py` & `buildbot-3.8.0/buildbot/scripts/upgrade_master.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/user.py` & `buildbot-3.8.0/buildbot/scripts/user.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/scripts/windows_service.py` & `buildbot-3.8.0/buildbot/scripts/windows_service.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/secrets/__init__.py` & `buildbot-3.8.0/buildbot/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/secrets/manager.py` & `buildbot-3.8.0/buildbot/secrets/manager.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/secrets/providers/__init__.py` & `buildbot-3.8.0/buildbot/secrets/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/secrets/providers/base.py` & `buildbot-3.8.0/buildbot/secrets/providers/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/secrets/providers/file.py` & `buildbot-3.8.0/buildbot/secrets/providers/file.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/secrets/providers/passwordstore.py` & `buildbot-3.8.0/buildbot/secrets/providers/passwordstore.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/secrets/providers/vault.py` & `buildbot-3.8.0/buildbot/secrets/providers/vault.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/secrets/providers/vault_hvac.py` & `buildbot-3.8.0/buildbot/secrets/providers/vault_hvac.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/secrets/secret.py` & `buildbot-3.8.0/buildbot/secrets/secret.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/api.raml` & `buildbot-3.8.0/buildbot/spec/api.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/build.raml` & `buildbot-3.8.0/buildbot/spec/types/build.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/build_data.raml` & `buildbot-3.8.0/buildbot/spec/types/build_data.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/builder.raml` & `buildbot-3.8.0/buildbot/spec/types/builder.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/buildrequest.raml` & `buildbot-3.8.0/buildbot/spec/types/buildrequest.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/buildset.raml` & `buildbot-3.8.0/buildbot/spec/types/buildset.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/change.raml` & `buildbot-3.8.0/buildbot/spec/types/change.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/changesource.raml` & `buildbot-3.8.0/buildbot/spec/types/changesource.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/forcescheduler.raml` & `buildbot-3.8.0/buildbot/spec/types/forcescheduler.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/log.raml` & `buildbot-3.8.0/buildbot/spec/types/log.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/logchunk.raml` & `buildbot-3.8.0/buildbot/spec/types/logchunk.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/master.raml` & `buildbot-3.8.0/buildbot/spec/types/master.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/patch.raml` & `buildbot-3.8.0/buildbot/spec/types/patch.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/scheduler.raml` & `buildbot-3.8.0/buildbot/spec/types/scheduler.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/sourcedproperties.raml` & `buildbot-3.8.0/buildbot/spec/types/sourcedproperties.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/sourcestamp.raml` & `buildbot-3.8.0/buildbot/spec/types/sourcestamp.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/step.raml` & `buildbot-3.8.0/buildbot/spec/types/step.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/test_result.raml` & `buildbot-3.8.0/buildbot/spec/types/test_result.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/test_result_set.raml` & `buildbot-3.8.0/buildbot/spec/types/test_result_set.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/spec/types/worker.raml` & `buildbot-3.8.0/buildbot/spec/types/worker.raml`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/statistics/__init__.py` & `buildbot-3.8.0/buildbot/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/statistics/capture.py` & `buildbot-3.8.0/buildbot/statistics/capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,18 +283,15 @@
                 divisor = 60
             elif report_in == 'hours':
                 divisor = 60 * 60
             if end_time < start_time:
                 duration = datetime.timedelta(0)
             else:
                 duration = end_time - start_time
-            # cannot use duration.total_seconds() on Python 2.6
-            duration = ((duration.microseconds + (duration.seconds +
-                                                  duration.days * 24 * 3600) * 1e6) / 1e6)
-            return duration / divisor
+            return duration.total_seconds() / divisor
 
         if not callback:
             callback = default_callback
         super().__init__(builder_name, callback, "duration")
 
     def _retValParams(self, msg):
         return [msg['started_at'], msg['complete_at']]
```

### Comparing `buildbot-3.7.0/buildbot/statistics/stats_service.py` & `buildbot-3.8.0/buildbot/statistics/stats_service.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/statistics/storage_backends/__init__.py` & `buildbot-3.8.0/buildbot/statistics/storage_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/statistics/storage_backends/base.py` & `buildbot-3.8.0/buildbot/statistics/storage_backends/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/statistics/storage_backends/influxdb_client.py` & `buildbot-3.8.0/buildbot/statistics/storage_backends/influxdb_client.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/cmake.py` & `buildbot-3.8.0/buildbot/steps/cmake.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/cppcheck.py` & `buildbot-3.8.0/buildbot/steps/cppcheck.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/download_secret_to_worker.py` & `buildbot-3.8.0/buildbot/steps/download_secret_to_worker.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/gitdiffinfo.py` & `buildbot-3.8.0/buildbot/steps/gitdiffinfo.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/http.py` & `buildbot-3.8.0/buildbot/steps/http.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/master.py` & `buildbot-3.8.0/buildbot/steps/master.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/maxq.py` & `buildbot-3.8.0/buildbot/steps/maxq.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/mswin.py` & `buildbot-3.8.0/buildbot/steps/mswin.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/package/__init__.py` & `buildbot-3.8.0/buildbot/steps/package/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/package/deb/lintian.py` & `buildbot-3.8.0/buildbot/steps/package/deb/lintian.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/package/deb/pbuilder.py` & `buildbot-3.8.0/buildbot/steps/package/deb/pbuilder.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/package/rpm/__init__.py` & `buildbot-3.8.0/buildbot/steps/package/rpm/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/package/rpm/mock.py` & `buildbot-3.8.0/buildbot/steps/package/rpm/mock.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/package/rpm/rpmbuild.py` & `buildbot-3.8.0/buildbot/steps/package/rpm/rpmbuild.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/package/rpm/rpmlint.py` & `buildbot-3.8.0/buildbot/steps/package/rpm/rpmlint.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/package/util.py` & `buildbot-3.8.0/buildbot/steps/package/util.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/python.py` & `buildbot-3.8.0/buildbot/steps/python.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/python_twisted.py` & `buildbot-3.8.0/buildbot/steps/python_twisted.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/shell.py` & `buildbot-3.8.0/buildbot/steps/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,22 +231,27 @@
     directoryLeavePattern = "make.*: Leaving directory"
     suppressionFile = None
 
     commentEmptyLineRe = re.compile(r"^\s*(#.*)?$")
     suppressionLineRe = re.compile(
         r"^\s*(.+?)\s*:\s*(.+?)\s*(?:[:]\s*([0-9]+)(?:-([0-9]+))?\s*)?$")
 
+    class Sentinel:
+        pass
+
+    _sentinel = Sentinel()
+
     def __init__(self,
-                 warningPattern=None, warningExtractor=None, maxWarnCount=None,
+                 warningPattern=_sentinel, warningExtractor=None, maxWarnCount=None,
                  directoryEnterPattern=None, directoryLeavePattern=None,
                  suppressionFile=None, suppressionList=None, **kwargs):
         # See if we've been given a regular expression to use to match
         # warnings. If not, use a default that assumes any line with "warning"
         # present is a warning. This may lead to false positives in some cases.
-        if warningPattern:
+        if not isinstance(warningPattern, self.Sentinel):
             self.warningPattern = warningPattern
         if directoryEnterPattern:
             self.directoryEnterPattern = directoryEnterPattern
         if directoryLeavePattern:
             self.directoryLeavePattern = directoryLeavePattern
         if suppressionFile:
             self.suppressionFile = suppressionFile
@@ -269,17 +274,18 @@
 
         self.suppressions = []
         self.directoryStack = []
 
         self.warnCount = 0
         self.loggedWarnings = []
 
-        self.addLogObserver(
-            'stdio',
-            logobserver.LineConsumerLogObserver(self.warningLogConsumer))
+        if self.warningPattern is not None:
+            self.addLogObserver(
+                'stdio',
+                logobserver.LineConsumerLogObserver(self.warningLogConsumer))
 
     def addSuppression(self, suppressionList):
         """
         This method can be used to add patters of warnings that should
         not be counted.
 
         It takes a single argument, a list of patterns.
```

### Comparing `buildbot-3.7.0/buildbot/steps/shellsequence.py` & `buildbot-3.8.0/buildbot/steps/shellsequence.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/source/__init__.py` & `buildbot-3.8.0/buildbot/steps/source/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/source/base.py` & `buildbot-3.8.0/buildbot/steps/source/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/source/bzr.py` & `buildbot-3.8.0/buildbot/steps/source/bzr.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/source/cvs.py` & `buildbot-3.8.0/buildbot/steps/source/cvs.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/source/darcs.py` & `buildbot-3.8.0/buildbot/steps/source/darcs.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/source/gerrit.py` & `buildbot-3.8.0/buildbot/steps/source/gerrit.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/source/git.py` & `buildbot-3.8.0/buildbot/steps/source/git.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/source/github.py` & `buildbot-3.8.0/buildbot/steps/source/github.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/source/gitlab.py` & `buildbot-3.8.0/buildbot/steps/source/gitlab.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/source/mercurial.py` & `buildbot-3.8.0/buildbot/steps/source/mercurial.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/source/mtn.py` & `buildbot-3.8.0/buildbot/steps/source/mtn.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/source/p4.py` & `buildbot-3.8.0/buildbot/steps/source/p4.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/source/repo.py` & `buildbot-3.8.0/buildbot/steps/source/repo.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/source/svn.py` & `buildbot-3.8.0/buildbot/steps/source/svn.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/subunit.py` & `buildbot-3.8.0/buildbot/steps/subunit.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/transfer.py` & `buildbot-3.8.0/buildbot/steps/transfer.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/trigger.py` & `buildbot-3.8.0/buildbot/steps/trigger.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/vstudio.py` & `buildbot-3.8.0/buildbot/steps/vstudio.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/steps/worker.py` & `buildbot-3.8.0/buildbot/steps/worker.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/__init__.py` & `buildbot-3.8.0/buildbot/test/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,14 @@
 
 # this warning happens sometimes on python3.4
 warnings.filterwarnings('ignore', r"The value of convert_charrefs will become True in 3.5")
 
 # Twisted 18.4+ adds a deprecation warning and still use the deprecated API in its own code!
 warnings.filterwarnings('ignore', ".*getClientIP was deprecated.*", DeprecationWarning)
 
-# Python 3.7 adds a deprecation warning formatargspec.
-# The signature api that replaces it is not available in 2.7
-warnings.filterwarnings('ignore', ".*`formatargspec` is deprecated.*", DeprecationWarning)
-
 # Python 3.7 adds a deprecation importing ABCs from collection.
 # Such imports are made in dependencies (e.g moto, werzeug, pyparsing)
 warnings.filterwarnings('ignore', ".*Using or importing the ABCs from 'collections'.*",
                         DeprecationWarning)
 
 # more 3.7 warning from moto
 warnings.filterwarnings('ignore', r".*Use 'list\(elem\)' or iteration over elem instead.*",
@@ -139,7 +135,11 @@
 warnings.filterwarnings('ignore', ".*stream argument is deprecated. Use stream parameter",
                         category=DeprecationWarning)
 
 # Botocore imports deprecated urllib3.contrib.pyopenssl for backwards compatibility that we don't
 # use. See https://github.com/boto/botocore/issues/2744
 warnings.filterwarnings('ignore', ".*'urllib3.contrib.pyopenssl' module is deprecated",
                         category=DeprecationWarning)
+
+# pipes is still used in astroid and buildbot_worker in default installation
+warnings.filterwarnings('ignore', "'pipes' is deprecated and slated for removal in Python 3.13",
+                        category=DeprecationWarning)
```

### Comparing `buildbot-3.7.0/buildbot/test/fake/botmaster.py` & `buildbot-3.8.0/buildbot/test/fake/botmaster.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/bworkermanager.py` & `buildbot-3.8.0/buildbot/test/fake/bworkermanager.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/change.py` & `buildbot-3.8.0/buildbot/test/fake/change.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/connection.py` & `buildbot-3.8.0/buildbot/test/fake/connection.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/docker.py` & `buildbot-3.8.0/buildbot/test/fake/docker.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/endpoint.py` & `buildbot-3.8.0/buildbot/test/fake/endpoint.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/fakebuild.py` & `buildbot-3.8.0/buildbot/test/fake/fakebuild.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/fakedata.py` & `buildbot-3.8.0/buildbot/test/fake/fakedata.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/fakemaster.py` & `buildbot-3.8.0/buildbot/test/fake/fakemaster.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/fakemq.py` & `buildbot-3.8.0/buildbot/test/fake/fakemq.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/fakeprotocol.py` & `buildbot-3.8.0/buildbot/test/fake/fakeprotocol.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/fakestats.py` & `buildbot-3.8.0/buildbot/test/fake/fakestats.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/httpclientservice.py` & `buildbot-3.8.0/buildbot/test/fake/httpclientservice.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/kube.py` & `buildbot-3.8.0/buildbot/test/fake/kube.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/latent.py` & `buildbot-3.8.0/buildbot/test/fake/latent.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     stop_instance() is executed.
     """
 
     def __init__(self, case, name, kind=None, build_wait_timeout=600,
                  starts_without_substantiate=None, **kwargs):
         self.case = case
         self.build_wait_timeout = build_wait_timeout
+        self.has_crashed = False
         self.worker = ControllableLatentWorker(name, self, **kwargs)
         self.remote_worker = None
 
         if starts_without_substantiate is not None:
             self.worker.starts_without_substantiate = \
                 starts_without_substantiate
 
@@ -222,7 +223,10 @@
         self._controller.state = States.STOPPING
 
         if self._controller.auto_stop_flag:
             yield self._controller.do_stop_instance()
             return True
         self._controller._stop_deferred = defer.Deferred()
         return (yield self._controller._stop_deferred)
+
+    def check_instance(self):
+        return not self._controller.has_crashed
```

### Comparing `buildbot-3.7.0/buildbot/test/fake/libvirt.py` & `buildbot-3.8.0/buildbot/test/fake/libvirt.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/logfile.py` & `buildbot-3.8.0/buildbot/test/fake/logfile.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/machine.py` & `buildbot-3.8.0/buildbot/test/fake/machine.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/msgmanager.py` & `buildbot-3.8.0/buildbot/test/fake/msgmanager.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/openstack.py` & `buildbot-3.8.0/buildbot/test/fake/openstack.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/pbmanager.py` & `buildbot-3.8.0/buildbot/test/fake/pbmanager.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/private_tempdir.py` & `buildbot-3.8.0/buildbot/test/fake/private_tempdir.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/reactor.py` & `buildbot-3.8.0/buildbot/test/fake/reactor.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/state.py` & `buildbot-3.8.0/buildbot/test/fake/state.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/step.py` & `buildbot-3.8.0/buildbot/test/fake/step.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/web.py` & `buildbot-3.8.0/buildbot/test/fake/web.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fake/worker.py` & `buildbot-3.8.0/buildbot/test/fake/worker.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/__init__.py` & `buildbot-3.8.0/buildbot/test/fakedb/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/base.py` & `buildbot-3.8.0/buildbot/test/fakedb/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/build_data.py` & `buildbot-3.8.0/buildbot/test/fakedb/build_data.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/builders.py` & `buildbot-3.8.0/buildbot/test/fakedb/builders.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/buildrequests.py` & `buildbot-3.8.0/buildbot/test/fakedb/buildrequests.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/builds.py` & `buildbot-3.8.0/buildbot/test/fakedb/builds.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/buildsets.py` & `buildbot-3.8.0/buildbot/test/fakedb/buildsets.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/changes.py` & `buildbot-3.8.0/buildbot/test/fakedb/changes.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/changesources.py` & `buildbot-3.8.0/buildbot/test/fakedb/changesources.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/connector.py` & `buildbot-3.8.0/buildbot/test/fakedb/connector.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/logs.py` & `buildbot-3.8.0/buildbot/test/fakedb/logs.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/masters.py` & `buildbot-3.8.0/buildbot/test/fakedb/masters.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/row.py` & `buildbot-3.8.0/buildbot/test/fakedb/row.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/schedulers.py` & `buildbot-3.8.0/buildbot/test/fakedb/schedulers.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/sourcestamps.py` & `buildbot-3.8.0/buildbot/test/fakedb/sourcestamps.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/state.py` & `buildbot-3.8.0/buildbot/test/fakedb/state.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/steps.py` & `buildbot-3.8.0/buildbot/test/fakedb/steps.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/tags.py` & `buildbot-3.8.0/buildbot/test/fakedb/tags.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/test_result_sets.py` & `buildbot-3.8.0/buildbot/test/fakedb/test_result_sets.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/test_results.py` & `buildbot-3.8.0/buildbot/test/fakedb/test_results.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/users.py` & `buildbot-3.8.0/buildbot/test/fakedb/users.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fakedb/workers.py` & `buildbot-3.8.0/buildbot/test/fakedb/workers.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/fuzz/test_lru.py` & `buildbot-3.8.0/buildbot/test/fuzz/test_lru.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/interop/__init__.py` & `buildbot-3.8.0/buildbot/test/integration/interop/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/interop/test_commandmixin.py` & `buildbot-3.8.0/buildbot/test/integration/interop/test_commandmixin.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,16 +23,34 @@
 
 
 # This integration test creates a master and worker environment,
 # and makes sure the command mixin is working.
 class CommandMixinMaster(RunMasterBase):
 
     @defer.inlineCallbacks
+    def setup_config(self):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import schedulers
+
+        c['schedulers'] = [
+            schedulers.AnyBranchScheduler(name="sched", builderNames=["testy"])
+        ]
+
+        f = BuildFactory()
+        f.addStep(TestCommandMixinStep())
+        c['builders'] = [
+            BuilderConfig(name="testy", workernames=["local1"], factory=f)
+        ]
+        yield self.setup_master(c)
+
+    @defer.inlineCallbacks
     def test_commandmixin(self):
-        yield self.setupConfig(masterConfig())
+        yield self.setup_config()
 
         change = dict(branch="master",
                       files=["foo.c"],
                       author="me@foo.com",
                       committer="me@foo.com",
                       comments="good stuff",
                       revision="HEAD",
@@ -77,28 +95,7 @@
         yield self.runRmdir('composite_mixin_test')
 
         hasPath = yield self.pathExists('composite_mixin_test')
         if hasPath:
             return results.FAILURE
 
         return results.SUCCESS
-
-
-# master configuration
-def masterConfig():
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import schedulers
-
-    c['schedulers'] = [
-        schedulers.AnyBranchScheduler(
-            name="sched",
-            builderNames=["testy"])]
-
-    f = BuildFactory()
-    f.addStep(TestCommandMixinStep())
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      factory=f)]
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/interop/test_compositestepmixin.py` & `buildbot-3.8.0/buildbot/test/integration/interop/test_compositestepmixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,57 +18,14 @@
 
 from buildbot.process import results
 from buildbot.process.buildstep import BuildStep
 from buildbot.steps.worker import CompositeStepMixin
 from buildbot.test.util.integration import RunMasterBase
 
 
-# This integration test creates a master and worker environment,
-# and makes sure the composite step mixin is working.
-class CompositeStepMixinMaster(RunMasterBase):
-
-    @defer.inlineCallbacks
-    def test_compositemixin_rmdir_list(self):
-        yield self.do_compositemixin_test(is_list_mkdir=False, is_list_rmdir=True)
-
-    @defer.inlineCallbacks
-    def test_compositemixin(self):
-        yield self.do_compositemixin_test(is_list_mkdir=False, is_list_rmdir=False)
-
-    @defer.inlineCallbacks
-    def do_compositemixin_test(self, is_list_mkdir, is_list_rmdir):
-        yield self.setupConfig(masterConfig(is_list_mkdir=is_list_mkdir,
-                                            is_list_rmdir=is_list_rmdir))
-
-        change = dict(branch="master",
-                      files=["foo.c"],
-                      author="me@foo.com",
-                      committer="me@foo.com",
-                      comments="good stuff",
-                      revision="HEAD",
-                      project="none"
-                      )
-        build = yield self.doForceBuild(wantSteps=True, useChange=change,
-                                        wantLogs=True)
-        self.assertEqual(build['buildid'], 1)
-        self.assertEqual(build['results'], results.SUCCESS)
-
-
-class CompositeStepMixinMasterPb(CompositeStepMixinMaster):
-    proto = "pb"
-
-
-class CompositeStepMixinMasterMsgPack(CompositeStepMixinMaster):
-    proto = "msgpack"
-
-    @defer.inlineCallbacks
-    def test_compositemixin_mkdir_rmdir_lists(self):
-        yield self.do_compositemixin_test(is_list_mkdir=True, is_list_rmdir=True)
-
-
 class TestCompositeMixinStep(BuildStep, CompositeStepMixin):
 
     def __init__(self, is_list_mkdir, is_list_rmdir):
         super().__init__()
         self.logEnviron = False
         self.is_list_mkdir = is_list_mkdir
         self.is_list_rmdir = is_list_rmdir
@@ -114,27 +71,67 @@
             has_path = yield self.pathExists(path)
             if has_path:
                 return results.FAILURE
 
         return results.SUCCESS
 
 
-# master configuration
-def masterConfig(is_list_mkdir=True, is_list_rmdir=True):
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import schedulers
-
-    c['schedulers'] = [
-        schedulers.AnyBranchScheduler(
-            name="sched",
-            builderNames=["testy"])]
-
-    f = BuildFactory()
-    f.addStep(TestCompositeMixinStep(is_list_mkdir=is_list_mkdir,
-                                     is_list_rmdir=is_list_rmdir))
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      factory=f)]
-    return c
+# This integration test creates a master and worker environment,
+# and makes sure the composite step mixin is working.
+class CompositeStepMixinMaster(RunMasterBase):
+
+    @defer.inlineCallbacks
+    def setup_config(self, is_list_mkdir=True, is_list_rmdir=True):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import schedulers
+
+        c['schedulers'] = [
+            schedulers.AnyBranchScheduler(name="sched", builderNames=["testy"])
+        ]
+
+        f = BuildFactory()
+        f.addStep(TestCompositeMixinStep(is_list_mkdir=is_list_mkdir,
+                                         is_list_rmdir=is_list_rmdir))
+        c['builders'] = [
+            BuilderConfig(name="testy", workernames=["local1"], factory=f)
+        ]
+
+        yield self.setup_master(c)
+
+    @defer.inlineCallbacks
+    def test_compositemixin_rmdir_list(self):
+        yield self.do_compositemixin_test(is_list_mkdir=False, is_list_rmdir=True)
+
+    @defer.inlineCallbacks
+    def test_compositemixin(self):
+        yield self.do_compositemixin_test(is_list_mkdir=False, is_list_rmdir=False)
+
+    @defer.inlineCallbacks
+    def do_compositemixin_test(self, is_list_mkdir, is_list_rmdir):
+        yield self.setup_config(is_list_mkdir=is_list_mkdir, is_list_rmdir=is_list_rmdir)
+
+        change = dict(branch="master",
+                      files=["foo.c"],
+                      author="me@foo.com",
+                      committer="me@foo.com",
+                      comments="good stuff",
+                      revision="HEAD",
+                      project="none"
+                      )
+        build = yield self.doForceBuild(wantSteps=True, useChange=change,
+                                        wantLogs=True)
+        self.assertEqual(build['buildid'], 1)
+        self.assertEqual(build['results'], results.SUCCESS)
+
+
+class CompositeStepMixinMasterPb(CompositeStepMixinMaster):
+    proto = "pb"
+
+
+class CompositeStepMixinMasterMsgPack(CompositeStepMixinMaster):
+    proto = "msgpack"
+
+    @defer.inlineCallbacks
+    def test_compositemixin_mkdir_rmdir_lists(self):
+        yield self.do_compositemixin_test(is_list_mkdir=True, is_list_rmdir=True)
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/interop/test_integration_secrets.py` & `buildbot-3.8.0/buildbot/test/integration/interop/test_integration_secrets.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,24 +29,64 @@
     def sendMessage(self, reports):
         assert self.auth == ('user', 'myhttppasswd')
         self.reported = True
 
 
 class SecretsConfig(RunMasterBase):
 
+    @defer.inlineCallbacks
+    def setup_config(self, use_interpolation):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import schedulers, steps, util
+
+        fake_reporter = FakeSecretReporter('http://example.com/hook',
+                                           auth=('user', Interpolate('%(secret:httppasswd)s')))
+
+        c['services'] = [fake_reporter]
+        c['schedulers'] = [
+            schedulers.ForceScheduler(
+                name="force",
+                builderNames=["testy"])]
+
+        c['secretsProviders'] = [FakeSecretStorage(secretdict={"foo": "secretvalue",
+                                                               "something": "more",
+                                                               'httppasswd': 'myhttppasswd'})]
+        f = BuildFactory()
+
+        if use_interpolation:
+            if os.name == "posix":
+                # on posix we can also check whether the password was passed to the command
+                command = Interpolate('echo %(secret:foo)s | ' +
+                                      'sed "s/secretvalue/The password was there/"')
+            else:
+                command = Interpolate('echo %(secret:foo)s')
+        else:
+            command = ['echo', util.Secret('foo')]
+
+        f.addStep(steps.ShellCommand(command=command))
+
+        c['builders'] = [
+            BuilderConfig(name="testy",
+                          workernames=["local1"],
+                          factory=f)]
+        yield self.setup_master(c)
+
+        return fake_reporter
+
     # Note that the secret name must be long enough so that it does not crash with random directory
     # or file names in the build dictionary.
     @parameterized.expand([
         ('with_interpolation', True),
         ('plain_command', False),
     ])
     @defer.inlineCallbacks
     def test_secret(self, name, use_interpolation):
-        c = masterConfig(use_interpolation)
-        yield self.setupConfig(c)
+        fake_reporter = yield self.setup_config(use_interpolation)
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True)
         self.assertEqual(build['buildid'], 1)
 
         # check the command line
         res = yield self.checkBuildStepLogExist(build, "echo <foo>")
 
         # also check the secrets are replaced in argv
@@ -56,26 +96,27 @@
         if os.name == "posix" and use_interpolation:
             res &= yield self.checkBuildStepLogExist(build, "The password was there")
 
         self.assertTrue(res)
         # at this point, build contains all the log and steps info that is in the db
         # we check that our secret is not in there!
         self.assertNotIn("secretvalue", repr(build))
-        self.assertTrue(c['services'][0].reported)
+        self.assertTrue(fake_reporter.reported)
 
     @parameterized.expand([
         ('with_interpolation', True),
         ('plain_command', False),
     ])
     @defer.inlineCallbacks
     def test_secretReconfig(self, name, use_interpolation):
-        c = masterConfig(use_interpolation)
-        yield self.setupConfig(c)
-        c['secretsProviders'] = [FakeSecretStorage(
-            secretdict={"foo": "different_value", "something": "more"})]
+        yield self.setup_config(use_interpolation)
+        self.master_config_dict['secretsProviders'] = [
+            FakeSecretStorage(secretdict={"foo": "different_value", "something": "more"})
+        ]
+
         yield self.master.reconfig()
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True)
         self.assertEqual(build['buildid'], 1)
         res = yield self.checkBuildStepLogExist(build, "echo <foo>")
         self.assertTrue(res)
         # at this point, build contains all the log and steps info that is in the db
         # we check that our secret is not in there!
@@ -84,45 +125,7 @@
 
 class SecretsConfigPB(SecretsConfig):
     proto = "pb"
 
 
 class SecretsConfigMsgPack(SecretsConfig):
     proto = "msgpack"
-
-
-# master configuration
-def masterConfig(use_interpolation):
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import schedulers, steps, util
-
-    c['services'] = [FakeSecretReporter('http://example.com/hook',
-                                        auth=('user', Interpolate('%(secret:httppasswd)s')))]
-    c['schedulers'] = [
-        schedulers.ForceScheduler(
-            name="force",
-            builderNames=["testy"])]
-
-    c['secretsProviders'] = [FakeSecretStorage(secretdict={"foo": "secretvalue",
-                                                           "something": "more",
-                                                           'httppasswd': 'myhttppasswd'})]
-    f = BuildFactory()
-
-    if use_interpolation:
-        if os.name == "posix":
-            # on posix we can also check whether the password was passed to the command
-            command = Interpolate('echo %(secret:foo)s | ' +
-                                  'sed "s/secretvalue/The password was there/"')
-        else:
-            command = Interpolate('echo %(secret:foo)s')
-    else:
-        command = ['echo', util.Secret('foo')]
-
-    f.addStep(steps.ShellCommand(command=command))
-
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      factory=f)]
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/interop/test_interruptcommand.py` & `buildbot-3.8.0/buildbot/test/integration/interop/test_interruptcommand.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,56 +21,53 @@
 from buildbot.test.util.integration import RunMasterBase
 from buildbot.util import asyncSleep
 
 
 class InterruptCommand(RunMasterBase):
     """Make sure we can interrupt a command"""
 
+    @defer.inlineCallbacks
+    def setup_config(self):
+        c = {}
+        from buildbot.plugins import schedulers, steps, util
+
+        class SleepAndInterrupt(steps.ShellSequence):
+            @defer.inlineCallbacks
+            def run(self):
+                if self.worker.worker_system == "nt":
+                    sleep = "waitfor SomethingThatIsNeverHappening /t 100 >nul 2>&1"
+                else:
+                    sleep = ["sleep", "100"]
+                d = self.runShellSequence([util.ShellArg(sleep)])
+                yield asyncSleep(1)
+                self.interrupt("just testing")
+                res = yield d
+                return res
+
+        c['schedulers'] = [
+            schedulers.ForceScheduler(
+                name="force",
+                builderNames=["testy"])]
+
+        f = util.BuildFactory()
+        f.addStep(SleepAndInterrupt())
+        c['builders'] = [
+            util.BuilderConfig(name="testy",
+                               workernames=["local1"],
+                               factory=f)]
+
+        yield self.setup_master(c)
+
     @flaky(bugNumber=4404, onPlatform='win32')
     @defer.inlineCallbacks
     def test_interrupt(self):
-        yield self.setupConfig(masterConfig())
+        yield self.setup_config()
         build = yield self.doForceBuild(wantSteps=True)
         self.assertEqual(build['steps'][-1]['results'], CANCELLED)
 
 
 class InterruptCommandPb(InterruptCommand):
     proto = "pb"
 
 
 class InterruptCommandMsgPack(InterruptCommand):
     proto = "msgpack"
-
-
-# master configuration
-
-
-def masterConfig():
-    c = {}
-    from buildbot.plugins import schedulers, steps, util
-
-    class SleepAndInterrupt(steps.ShellSequence):
-        @defer.inlineCallbacks
-        def run(self):
-            if self.worker.worker_system == "nt":
-                sleep = "waitfor SomethingThatIsNeverHappening /t 100 >nul 2>&1"
-            else:
-                sleep = ["sleep", "100"]
-            d = self.runShellSequence([util.ShellArg(sleep)])
-            yield asyncSleep(1)
-            self.interrupt("just testing")
-            res = yield d
-            return res
-
-    c['schedulers'] = [
-        schedulers.ForceScheduler(
-            name="force",
-            builderNames=["testy"])]
-
-    f = util.BuildFactory()
-    f.addStep(SleepAndInterrupt())
-    c['builders'] = [
-        util.BuilderConfig(name="testy",
-                           workernames=["local1"],
-                           factory=f)]
-
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/interop/test_setpropertyfromcommand.py` & `buildbot-3.8.0/buildbot/test/integration/interop/test_setpropertyfromcommand.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,23 +16,42 @@
 
 from twisted.internet import defer
 from twisted.internet import reactor
 from twisted.internet import task
 
 from buildbot.test.util.integration import RunMasterBase
 
+
 # This integration test helps reproduce http://trac.buildbot.net/ticket/3024
 # we make sure that we can reconfigure the master while build is running
+class SetPropertyFromCommand(RunMasterBase):
 
+    @defer.inlineCallbacks
+    def setup_config(self):
+        c = {}
+        from buildbot.plugins import schedulers, steps, util
+
+        c['schedulers'] = [
+            schedulers.ForceScheduler(
+                name="force",
+                builderNames=["testy"])]
+
+        f = util.BuildFactory()
+        f.addStep(steps.SetPropertyFromCommand(
+            property="test", command=["echo", "foo"]))
+        c['builders'] = [
+            util.BuilderConfig(name="testy",
+                               workernames=["local1"],
+                               factory=f)]
 
-class SetPropertyFromCommand(RunMasterBase):
+        yield self.setup_master(c)
 
     @defer.inlineCallbacks
     def test_setProp(self):
-        yield self.setupConfig(masterConfig())
+        yield self.setup_config()
         oldNewLog = self.master.data.updates.addLog
 
         @defer.inlineCallbacks
         def newLog(*arg, **kw):
             # Simulate db delay. We usually don't test race conditions
             # with delays, but in integrations test, that would be pretty
             # tricky
@@ -48,34 +67,7 @@
 
 class SetPropertyFromCommandPB(SetPropertyFromCommand):
     proto = "pb"
 
 
 class SetPropertyFromCommandMsgPack(SetPropertyFromCommand):
     proto = "msgpack"
-
-
-# master configuration
-
-num_reconfig = 0
-
-
-def masterConfig():
-    global num_reconfig
-    num_reconfig += 1
-    c = {}
-    from buildbot.plugins import schedulers, steps, util
-
-    c['schedulers'] = [
-        schedulers.ForceScheduler(
-            name="force",
-            builderNames=["testy"])]
-
-    f = util.BuildFactory()
-    f.addStep(steps.SetPropertyFromCommand(
-        property="test", command=["echo", "foo"]))
-    c['builders'] = [
-        util.BuilderConfig(name="testy",
-                           workernames=["local1"],
-                           factory=f)]
-
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/interop/test_transfer.py` & `buildbot-3.8.0/buildbot/test/integration/interop/test_transfer.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,78 +16,136 @@
 
 
 import os
 import shutil
 
 from twisted.internet import defer
 
+from buildbot.process.buildstep import BuildStep
 from buildbot.process.results import FAILURE
 from buildbot.process.results import SUCCESS
+from buildbot.steps.transfer import DirectoryUpload
+from buildbot.steps.transfer import FileDownload
+from buildbot.steps.transfer import FileUpload
+from buildbot.steps.transfer import MultipleFileUpload
+from buildbot.steps.transfer import StringDownload
+from buildbot.steps.worker import CompositeStepMixin
 from buildbot.test.util.decorators import flaky
 from buildbot.test.util.integration import RunMasterBase
 
 # This integration test creates a master and worker environment
 # and make sure the transfer steps are working
 
 # When new protocols are added, make sure you update this test to exercise
 # your proto implementation
 
 
 class TransferStepsMasterPb(RunMasterBase):
     proto = "pb"
 
-    def readMasterDirContents(self, top):
-        contents = {}
-        for root, _, files in os.walk(top):
-            for name in files:
-                fn = os.path.join(root, name)
-                with open(fn, encoding='utf-8') as f:
-                    contents[fn] = f.read()
-        return contents
+    @defer.inlineCallbacks
+    def setup_config(self, bigfilename):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import schedulers
 
-    def get_config_single_step(self, step):
+        c['schedulers'] = [
+            schedulers.ForceScheduler(
+                name="force",
+                builderNames=["testy"])]
+
+        f = BuildFactory()
+        # do a bunch of transfer to exercise the protocol
+        f.addStep(StringDownload("filecontent", workerdest="dir/file1.txt"))
+        f.addStep(StringDownload("filecontent2", workerdest="dir/file2.txt"))
+        # create 8 MB file
+        with open(bigfilename, 'w', encoding='utf-8') as o:
+            buf = "xxxxxxxx" * 1024
+            for _ in range(1000):
+                o.write(buf)
+        f.addStep(FileDownload(mastersrc=bigfilename, workerdest="bigfile.txt"))
+        f.addStep(FileUpload(workersrc="dir/file2.txt", masterdest="master.txt"))
+        f.addStep(FileDownload(mastersrc="master.txt", workerdest="dir/file3.txt"))
+        f.addStep(DirectoryUpload(workersrc="dir", masterdest="dir"))
+        c['builders'] = [
+            BuilderConfig(name="testy", workernames=["local1"], factory=f)
+        ]
+        yield self.setup_master(c)
+
+    @defer.inlineCallbacks
+    def setup_config_glob(self):
         c = {}
         from buildbot.config import BuilderConfig
         from buildbot.process.factory import BuildFactory
-        from buildbot.plugins import steps, schedulers
+        from buildbot.plugins import schedulers
+
+        class CustomStep(BuildStep, CompositeStepMixin):
+            @defer.inlineCallbacks
+            def run(self):
+                content = yield self.getFileContentFromWorker(
+                    "dir/file1.txt", abandonOnFailure=True)
+                assert content == "filecontent"
+                return SUCCESS
+
+        c['schedulers'] = [
+            schedulers.ForceScheduler(
+                name="force", builderNames=["testy"])
+        ]
+
+        f = BuildFactory()
+        f.addStep(StringDownload("filecontent", workerdest="dir/file1.txt"))
+        f.addStep(StringDownload("filecontent2", workerdest="dir/notafile1.txt"))
+        f.addStep(StringDownload("filecontent2", workerdest="dir/only1.txt"))
+        f.addStep(
+            MultipleFileUpload(
+                workersrcs=["dir/file*.txt", "dir/not*.txt", "dir/only?.txt"],
+                masterdest="dest/",
+                glob=True))
+        f.addStep(CustomStep())
+        c['builders'] = [
+            BuilderConfig(name="testy", workernames=["local1"], factory=f)
+        ]
+        yield self.setup_master(c)
+
+    @defer.inlineCallbacks
+    def setup_config_single_step(self, step):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import schedulers
 
         c['schedulers'] = [
             schedulers.ForceScheduler(
                 name="force",
                 builderNames=["testy"])]
 
         f = BuildFactory()
 
-        f.addStep(steps.FileUpload(workersrc="dir/noexist_path", masterdest="master_dest"))
+        f.addStep(FileUpload(workersrc="dir/noexist_path", masterdest="master_dest"))
         c['builders'] = [
             BuilderConfig(name="testy",
                           workernames=["local1"],
                           factory=f)
         ]
-        return c
+        yield self.setup_master(c)
 
-    def get_non_existing_file_upload_config(self):
-        from buildbot.plugins import steps
-        step = steps.FileUpload(workersrc="dir/noexist_path", masterdest="master_dest")
-        return self.get_config_single_step(step)
-
-    def get_non_existing_directory_upload_config(self):
-        from buildbot.plugins import steps
-        step = steps.DirectoryUpload(workersrc="dir/noexist_path", masterdest="master_dest")
-        return self.get_config_single_step(step)
-
-    def get_non_existing_multiple_file_upload_config(self):
-        from buildbot.plugins import steps
-        step = steps.MultipleFileUpload(workersrcs=["dir/noexist_path"], masterdest="master_dest")
-        return self.get_config_single_step(step)
+    def readMasterDirContents(self, top):
+        contents = {}
+        for root, _, files in os.walk(top):
+            for name in files:
+                fn = os.path.join(root, name)
+                with open(fn, encoding='utf-8') as f:
+                    contents[fn] = f.read()
+        return contents
 
     @flaky(bugNumber=4407, onPlatform='win32')
     @defer.inlineCallbacks
     def test_transfer(self):
-        yield self.setupConfig(masterConfig(bigfilename=self.mktemp()))
+        yield self.setup_config(bigfilename=self.mktemp())
 
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True)
         self.assertEqual(build['results'], SUCCESS)
         dirContents = self.readMasterDirContents("dir")
         self.assertEqual(
             dirContents,
             {os.path.join('dir', 'file1.txt'): 'filecontent',
@@ -96,123 +154,53 @@
 
         # cleanup our mess (worker is cleaned up by parent class)
         shutil.rmtree("dir")
         os.unlink("master.txt")
 
     @defer.inlineCallbacks
     def test_globTransfer(self):
-        yield self.setupConfig(masterGlobConfig())
+        yield self.setup_config_glob()
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True)
         self.assertEqual(build['results'], SUCCESS)
         dirContents = self.readMasterDirContents("dest")
         self.assertEqual(dirContents, {
             os.path.join('dest', 'file1.txt'): 'filecontent',
             os.path.join('dest', 'notafile1.txt'): 'filecontent2',
             os.path.join('dest', 'only1.txt'): 'filecontent2'
         })
 
         # cleanup
         shutil.rmtree("dest")
 
     @defer.inlineCallbacks
     def test_no_exist_file_upload(self):
-        yield self.setupConfig(self.get_non_existing_file_upload_config())
+        step = FileUpload(workersrc="dir/noexist_path", masterdest="master_dest")
+        yield self.setup_config_single_step(step)
+
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True)
         self.assertEqual(build['results'], FAILURE)
         res = yield self.checkBuildStepLogExist(build, "Cannot open file")
         self.assertTrue(res)
 
     @defer.inlineCallbacks
     def test_no_exist_directory_upload(self):
-        yield self.setupConfig(self.get_non_existing_directory_upload_config())
+        step = DirectoryUpload(workersrc="dir/noexist_path", masterdest="master_dest")
+        yield self.setup_config_single_step(step)
+
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True)
         self.assertEqual(build['results'], FAILURE)
         res = yield self.checkBuildStepLogExist(build, "Cannot open file")
         self.assertTrue(res)
 
     @defer.inlineCallbacks
     def test_no_exist_multiple_file_upload(self):
-        yield self.setupConfig(self.get_non_existing_multiple_file_upload_config())
+        step = MultipleFileUpload(workersrcs=["dir/noexist_path"], masterdest="master_dest")
+        yield self.setup_config_single_step(step)
+
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True)
         self.assertEqual(build['results'], FAILURE)
         res = yield self.checkBuildStepLogExist(build, "Cannot open file")
         self.assertTrue(res)
 
 
 class TransferStepsMasterNull(TransferStepsMasterPb):
     proto = "null"
-
-
-# master configuration
-def masterConfig(bigfilename):
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import steps, schedulers
-
-    c['schedulers'] = [
-        schedulers.ForceScheduler(
-            name="force",
-            builderNames=["testy"])]
-
-    f = BuildFactory()
-    # do a bunch of transfer to exercise the protocol
-    f.addStep(steps.StringDownload("filecontent", workerdest="dir/file1.txt"))
-    f.addStep(steps.StringDownload("filecontent2", workerdest="dir/file2.txt"))
-    # create 8 MB file
-    with open(bigfilename, 'w', encoding='utf-8') as o:
-        buf = "xxxxxxxx" * 1024
-        for _ in range(1000):
-            o.write(buf)
-    f.addStep(
-        steps.FileDownload(
-            mastersrc=bigfilename, workerdest="bigfile.txt"))
-    f.addStep(
-        steps.FileUpload(workersrc="dir/file2.txt", masterdest="master.txt"))
-    f.addStep(
-        steps.FileDownload(mastersrc="master.txt", workerdest="dir/file3.txt"))
-    f.addStep(steps.DirectoryUpload(workersrc="dir", masterdest="dir"))
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      factory=f)
-    ]
-    return c
-
-
-def masterGlobConfig():
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import steps, schedulers
-    from buildbot.steps.worker import CompositeStepMixin
-
-    class CustomStep(steps.BuildStep, CompositeStepMixin):
-        @defer.inlineCallbacks
-        def run(self):
-            content = yield self.getFileContentFromWorker(
-                "dir/file1.txt", abandonOnFailure=True)
-            assert content == "filecontent"
-            return SUCCESS
-
-    c['schedulers'] = [
-        schedulers.ForceScheduler(
-            name="force", builderNames=["testy"])
-    ]
-
-    f = BuildFactory()
-    f.addStep(steps.StringDownload("filecontent", workerdest="dir/file1.txt"))
-    f.addStep(
-        steps.StringDownload(
-            "filecontent2", workerdest="dir/notafile1.txt"))
-    f.addStep(steps.StringDownload("filecontent2", workerdest="dir/only1.txt"))
-    f.addStep(
-        steps.MultipleFileUpload(
-            workersrcs=["dir/file*.txt", "dir/not*.txt", "dir/only?.txt"],
-            masterdest="dest/",
-            glob=True))
-    f.addStep(CustomStep())
-    c['builders'] = [
-        BuilderConfig(
-            name="testy", workernames=["local1"], factory=f)
-    ]
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/interop/test_worker_reconnect.py` & `buildbot-3.8.0/buildbot/test/integration/interop/test_worker_reconnect.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,41 +33,37 @@
 
 
 class WorkerReconnectPb(RunMasterBase):
     """integration test for testing worker disconnection and reconnection"""
     proto = "pb"
 
     @defer.inlineCallbacks
+    def setup_config(self):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import schedulers
+
+        c['schedulers'] = [
+            schedulers.AnyBranchScheduler(name="sched", builderNames=["testy"]),
+            schedulers.ForceScheduler(name="force", builderNames=["testy"])
+        ]
+
+        f = BuildFactory()
+        f.addStep(DisconnectingStep())
+        c['builders'] = [
+            BuilderConfig(name="testy", workernames=["local1"], factory=f)
+        ]
+        yield self.setup_master(c)
+
+    @defer.inlineCallbacks
     def test_eventually_reconnect(self):
         DisconnectingStep.disconnection_list = []
-        yield self.setupConfig(masterConfig())
+        yield self.setup_config()
+
         build = yield self.doForceBuild()
         self.assertEqual(build['buildid'], 2)
         self.assertEqual(len(DisconnectingStep.disconnection_list), 2)
 
 
 class WorkerReconnectMsgPack(WorkerReconnectPb):
     proto = "msgpack"
-
-
-# master configuration
-def masterConfig():
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import schedulers
-
-    c['schedulers'] = [
-        schedulers.AnyBranchScheduler(
-            name="sched",
-            builderNames=["testy"]),
-        schedulers.ForceScheduler(
-            name="force",
-            builderNames=["testy"])]
-
-    f = BuildFactory()
-    f.addStep(DisconnectingStep())
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      factory=f)]
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/pki/127.0.0.1.crt` & `buildbot-3.8.0/buildbot/test/integration/pki/127.0.0.1.crt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/pki/127.0.0.1.key` & `buildbot-3.8.0/buildbot/test/integration/pki/127.0.0.1.key`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/pki/ca/ca.crt` & `buildbot-3.8.0/buildbot/test/integration/pki/ca/ca.crt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_URLs.py` & `buildbot-3.8.0/buildbot/test/integration/test_URLs.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,42 +25,41 @@
 
 
 class UrlForBuildMaster(RunMasterBase):
 
     proto = "null"
 
     @defer.inlineCallbacks
+    def setup_config(self):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import steps, schedulers, util
+
+        c['schedulers'] = [
+            schedulers.ForceScheduler(
+                name="force",
+                builderNames=["testy"])]
+
+        f = BuildFactory()
+        # do a bunch of transfer to exercise the protocol
+        f.addStep(steps.ShellCommand(command=["echo", util.URLForBuild]))
+        c['builders'] = [
+            BuilderConfig(name="testy",
+                          workernames=["local1"],
+                          factory=f)
+        ]
+        yield self.setup_master(c)
+
+    @defer.inlineCallbacks
     def test_url(self):
-        yield self.setupConfig(masterConfig())
+        yield self.setup_config()
 
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True)
         self.assertEqual(build['results'], SUCCESS)
         if runtime.platformType == 'win32':
-            command = "echo http://localhost:8080/#builders/1/builds/1"
+            command = "echo http://localhost:8080/#/builders/1/builds/1"
         else:
-            command = "echo 'http://localhost:8080/#builders/1/builds/1'"
+            command = "echo 'http://localhost:8080/#/builders/1/builds/1'"
 
         self.assertIn(command,
                       build['steps'][1]['logs'][0]['contents']['content'])
-
-
-# master configuration
-def masterConfig():
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import steps, schedulers, util
-
-    c['schedulers'] = [
-        schedulers.ForceScheduler(
-            name="force",
-            builderNames=["testy"])]
-
-    f = BuildFactory()
-    # do a bunch of transfer to exercise the protocol
-    f.addStep(steps.ShellCommand(command=["echo", util.URLForBuild]))
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      factory=f)
-    ]
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_configs.py` & `buildbot-3.8.0/buildbot/test/integration/test_configs.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_custom_buildstep.py` & `buildbot-3.8.0/buildbot/test/integration/test_custom_buildstep.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_customservices.py` & `buildbot-3.8.0/buildbot/test/integration/test_customservices.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_graphql.py` & `buildbot-3.8.0/buildbot/test/integration/test_graphql.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_integration_force_with_patch.py` & `buildbot-3.8.0/buildbot/test/integration/test_integration_force_with_patch.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,51 +43,50 @@
         if patch:
             yield self.patch(patch)
         return SUCCESS
 
 
 class ShellMaster(RunMasterBase):
 
+    @defer.inlineCallbacks
+    def setup_config(self):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import steps, schedulers, util
+
+        c['schedulers'] = [
+            schedulers.ForceScheduler(
+                name="force",
+                codebases=[util.CodebaseParameter(
+                    "foo", patch=util.PatchParameter())],
+                builderNames=["testy"])]
+
+        f = BuildFactory()
+        f.addStep(MySource(codebase='foo'))
+        # if the patch was applied correctly, then make will work!
+        f.addStep(steps.ShellCommand(command=["make"]))
+        c['builders'] = [
+            BuilderConfig(name="testy", workernames=["local1"], factory=f)
+        ]
+
+        yield self.setup_master(c)
+
     @skipUnlessPlatformIs("posix")  # make is not installed on windows
     @defer.inlineCallbacks
     def test_shell(self):
-        yield self.setupConfig(masterConfig())
+        yield self.setup_config()
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True,
                                         forceParams={'foo_patch_body': PATCH})
         self.assertEqual(build['buildid'], 1)
         # if makefile was not properly created, we would have a failure
         self.assertEqual(build['results'], SUCCESS)
 
     @defer.inlineCallbacks
     def test_shell_no_patch(self):
-        yield self.setupConfig(masterConfig())
+        yield self.setup_config()
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True)
         self.assertEqual(build['buildid'], 1)
         # if no patch, the source step is happy, but the make step cannot find makefile
         self.assertEqual(build['steps'][1]['results'], SUCCESS)
         self.assertEqual(build['steps'][2]['results'], FAILURE)
         self.assertEqual(build['results'], FAILURE)
-
-
-# master configuration
-def masterConfig():
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import steps, schedulers, util
-
-    c['schedulers'] = [
-        schedulers.ForceScheduler(
-            name="force",
-            codebases=[util.CodebaseParameter(
-                "foo", patch=util.PatchParameter())],
-            builderNames=["testy"])]
-
-    f = BuildFactory()
-    f.addStep(MySource(codebase='foo'))
-    # if the patch was applied correctly, then make will work!
-    f.addStep(steps.ShellCommand(command=["make"]))
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      factory=f)]
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_integration_mastershell.py` & `buildbot-3.8.0/buildbot/test/integration/test_integration_mastershell.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,74 +27,75 @@
 
 
 # This integration test creates a master and worker environment,
 # with one builders and a shellcommand step
 # meant to be a template for integration steps
 class ShellMaster(RunMasterBase):
 
-    def config_for_master_command(self, **kwargs):
+    @defer.inlineCallbacks
+    def setup_config_for_master_command(self, **kwargs):
         c = {}
 
         c['schedulers'] = [
             schedulers.AnyBranchScheduler(name="sched", builderNames=["testy"])
         ]
 
         f = BuildFactory()
         f.addStep(steps.MasterShellCommand(**kwargs))
         c['builders'] = [
             BuilderConfig(name="testy", workernames=["local1"], factory=f)
         ]
-        return c
+        yield self.setup_master(c)
 
     def get_change(self):
         return {
             "branch": "master",
             "files": ["foo.c"],
             "author": "me@foo.com",
             "committer": "me@foo.com",
             "comments": "good stuff",
             "revision": "HEAD",
             "project": "none"
         }
 
     @defer.inlineCallbacks
     def test_shell(self):
-        yield self.setupConfig(self.config_for_master_command(command='echo hello'))
+        yield self.setup_config_for_master_command(command='echo hello')
 
         build = yield self.doForceBuild(wantSteps=True, useChange=self.get_change(), wantLogs=True)
         self.assertEqual(build['buildid'], 1)
         self.assertEqual(build['steps'][1]['state_string'], 'Ran')
 
     @defer.inlineCallbacks
     def test_logs(self):
-        yield self.setupConfig(self.config_for_master_command(command=[
+        yield self.setup_config_for_master_command(command=[
             sys.executable, '-c', 'print("hello")'
-        ]))
+        ])
 
         build = yield self.doForceBuild(wantSteps=True, useChange=self.get_change(), wantLogs=True)
         self.assertEqual(build['buildid'], 1)
         res = yield self.checkBuildStepLogExist(build, "hello")
         self.assertTrue(res)
         self.assertEqual(build['steps'][1]['state_string'], 'Ran')
 
     @defer.inlineCallbacks
     def test_fails(self):
-        yield self.setupConfig(self.config_for_master_command(command=[
+        yield self.setup_config_for_master_command(command=[
             sys.executable, '-c', 'exit(1)'
-        ]))
+        ])
 
         build = yield self.doForceBuild(wantSteps=True, useChange=self.get_change(), wantLogs=True)
         self.assertEqual(build['buildid'], 1)
         self.assertEqual(build['steps'][1]['state_string'], 'failed (1) (failure)')
 
     @defer.inlineCallbacks
     def test_interrupt(self):
-        yield self.setupConfig(self.config_for_master_command(name='sleep', command=[
+        yield self.setup_config_for_master_command(name='sleep', command=[
             sys.executable, '-c', "while True: pass"
-        ]))
+        ])
 
         d = self.doForceBuild(wantSteps=True, useChange=self.get_change(), wantLogs=True)
 
         @defer.inlineCallbacks
         def on_new_step(_, data):
             if data['name'] == 'sleep':
                 # wait until the step really starts
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_integration_scheduler_reconfigure.py` & `buildbot-3.8.0/buildbot/test/integration/test_integration_scheduler_reconfigure.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,42 @@
 
 
 # This integration test creates a master and worker environment,
 # with one builders and a shellcommand step
 # meant to be a template for integration steps
 class ShellMaster(RunMasterBase):
 
+    def create_config(self):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import steps
+
+        c['schedulers'] = [
+            schedulers.AnyBranchScheduler(
+                name="sched1",
+                builderNames=["testy1"]),
+            schedulers.ForceScheduler(
+                name="sched2",
+                builderNames=["testy2"])
+        ]
+        f = BuildFactory()
+        f.addStep(steps.ShellCommand(command='echo hello'))
+        c['builders'] = [
+            BuilderConfig(name=name,
+                          workernames=["local1"],
+                          factory=f)
+            for name in ['testy1', 'testy2']
+        ]
+        return c
+
     @defer.inlineCallbacks
     def test_shell(self):
-        cfg = masterConfig()
-        yield self.setupConfig(cfg)
+        cfg = self.create_config()
+        yield self.setup_master(cfg)
 
         change = dict(branch="master",
                       files=["foo.c"],
                       author="me@foo.com",
                       committer="me@foo.com",
                       comments="good stuff",
                       revision="HEAD",
@@ -48,33 +72,7 @@
                 builderNames=["testy1"])
         ]
         yield self.master.reconfig()
         build = yield self.doForceBuild(wantSteps=True, useChange=change, wantLogs=True)
         self.assertEqual(build['buildid'], 1)
         builder = yield self.master.data.get(('builders', build['builderid']))
         self.assertEqual(builder['name'], 'testy2')
-
-
-# master configuration
-def masterConfig():
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import steps
-
-    c['schedulers'] = [
-        schedulers.AnyBranchScheduler(
-            name="sched1",
-            builderNames=["testy1"]),
-        schedulers.ForceScheduler(
-            name="sched2",
-            builderNames=["testy2"])
-    ]
-    f = BuildFactory()
-    f.addStep(steps.ShellCommand(command='echo hello'))
-    c['builders'] = [
-        BuilderConfig(name=name,
-                      workernames=["local1"],
-                      factory=f)
-        for name in ['testy1', 'testy2']
-    ]
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_integration_secrets_with_vault.py` & `buildbot-3.8.0/buildbot/test/integration/test_integration_secrets_with_vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,21 +60,50 @@
             subprocess.check_call(['docker', 'exec',
                                    '-e', 'VAULT_ADDR=http://127.0.0.1:8200/',
                                    'vault_for_buildbot',
                                    'vault', 'kv', 'put', 'secret/key1/key2', 'id=val'])
         except (FileNotFoundError, subprocess.CalledProcessError) as e:
             raise SkipTest("Vault integration needs docker environment to be setup") from e
 
+    @defer.inlineCallbacks
+    def setup_config(self, secret_specifier):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import schedulers
+
+        c['schedulers'] = [
+            schedulers.ForceScheduler(
+                name="force",
+                builderNames=["testy"])]
+
+        # note that as of December 2018, the vault docker image default to kv
+        # version 2 to be enabled by default
+        c['secretsProviders'] = [HashiCorpVaultSecretProvider(
+            vaultToken='my_vaulttoken',
+            vaultServer="http://localhost:8200",
+            apiVersion=2
+        )]
+
+        f = BuildFactory()
+        f.addStep(ShellCommand(command=Interpolate(f'echo {secret_specifier} | base64')))
+
+        c['builders'] = [
+            BuilderConfig(name="testy",
+                          workernames=["local1"],
+                          factory=f)]
+        yield self.setup_master(c)
+
     def remove_container(self):
         subprocess.call(['docker', 'rm', '-f', 'vault_for_buildbot'])
 
     @defer.inlineCallbacks
     def do_secret_test(self, secret_specifier, expected_obfuscation, expected_value):
         with assertProducesWarning(DeprecatedApiWarning):
-            yield self.setupConfig(masterConfig(secret_specifier=secret_specifier))
+            yield self.setup_config(secret_specifier=secret_specifier)
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True)
         self.assertEqual(build['buildid'], 1)
 
         patterns = [
             f"echo {expected_obfuscation}",
             base64.b64encode((expected_value + "\n").encode('utf-8')).decode('utf-8'),
         ]
@@ -93,36 +122,7 @@
     @defer.inlineCallbacks
     def test_any_key(self):
         yield self.do_secret_test('%(secret:anykey/anyvalue)s', '<anykey/anyvalue>', 'anyword')
 
     @defer.inlineCallbacks
     def test_nested_key(self):
         yield self.do_secret_test('%(secret:key1/key2/id)s', '<key1/key2/id>', 'val')
-
-
-def masterConfig(secret_specifier):
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import schedulers
-
-    c['schedulers'] = [
-        schedulers.ForceScheduler(
-            name="force",
-            builderNames=["testy"])]
-
-    # note that as of December 2018, the vault docker image default to kv
-    # version 2 to be enabled by default
-    c['secretsProviders'] = [HashiCorpVaultSecretProvider(
-        vaultToken='my_vaulttoken',
-        vaultServer="http://localhost:8200",
-        apiVersion=2
-    )]
-
-    f = BuildFactory()
-    f.addStep(ShellCommand(command=Interpolate(f'echo {secret_specifier} | base64')))
-
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      factory=f)]
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_integration_secrets_with_vault_hvac.py` & `buildbot-3.8.0/buildbot/test/integration/test_integration_secrets_with_vault_hvac.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,44 @@
 
 
 # Test needs to be explicitly disabled on Windows, as docker may be present there, but not able
 # to properly launch images.
 @skipUnlessPlatformIs('posix')
 class TestVaultHvac(RunMasterBase):
 
+    @defer.inlineCallbacks
+    def setup_config(self, secret_specifier):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import schedulers
+
+        c['schedulers'] = [
+            schedulers.ForceScheduler(name="force", builderNames=["testy"])
+        ]
+
+        # note that as of August 2021, the vault docker image default to kv
+        # version 2 to be enabled by default
+        c['secretsProviders'] = [
+            HashiCorpVaultKvSecretProvider(authenticator=VaultAuthenticatorToken('my_vaulttoken'),
+                                           vault_server="http://localhost:8200",
+                                           secrets_mount="secret")
+        ]
+
+        f = BuildFactory()
+        f.addStep(ShellCommand(command=Interpolate(f'echo {secret_specifier} | base64')))
+
+        c['builders'] = [
+            BuilderConfig(name="testy",
+                          workernames=["local1"],
+                          factory=f)
+        ]
+
+        yield self.setup_master(c)
+
     def start_container(self, image_tag):
         try:
             image = f'vault:{image_tag}'
             subprocess.check_call(['docker', 'pull', image])
 
             subprocess.check_call(['docker', 'run', '-d',
                                    '-e', 'SKIP_SETCAP=yes',
@@ -71,15 +101,15 @@
 
     def remove_container(self):
         subprocess.call(['docker', 'rm', '-f', 'vault_for_buildbot'])
 
     @defer.inlineCallbacks
     def do_secret_test(self, image_tag, secret_specifier, expected_obfuscation, expected_value):
         self.start_container(image_tag)
-        yield self.setupConfig(master_config(secret_specifier=secret_specifier))
+        yield self.setup_config(secret_specifier=secret_specifier)
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True)
         self.assertEqual(build['buildid'], 1)
 
         patterns = [
             f"echo {expected_obfuscation}",
             base64.b64encode((expected_value + "\n").encode('utf-8')).decode('utf-8'),
         ]
@@ -104,37 +134,7 @@
         yield self.do_secret_test(image_tag, '%(secret:anykey|anyvalue)s', '<anykey|anyvalue>',
                                   'anyword')
 
     @parameterized.expand(all_tags)
     @defer.inlineCallbacks
     def test_nested_key(self, image_tag):
         yield self.do_secret_test(image_tag, '%(secret:key1/key2|id)s', '<key1/key2|id>', 'val')
-
-
-def master_config(secret_specifier):
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import schedulers
-
-    c['schedulers'] = [
-        schedulers.ForceScheduler(name="force", builderNames=["testy"])
-    ]
-
-    # note that as of August 2021, the vault docker image default to kv
-    # version 2 to be enabled by default
-    c['secretsProviders'] = [
-        HashiCorpVaultKvSecretProvider(authenticator=VaultAuthenticatorToken('my_vaulttoken'),
-                                       vault_server="http://localhost:8200",
-                                       secrets_mount="secret")
-    ]
-
-    f = BuildFactory()
-    f.addStep(ShellCommand(command=Interpolate(f'echo {secret_specifier} | base64')))
-
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      factory=f)
-    ]
-
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_integration_template.py` & `buildbot-3.8.0/buildbot/test/integration/test_integration_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,47 +21,46 @@
 
 # This integration test creates a master and worker environment,
 # with one builder and a shellcommand step
 # meant to be a template for integration steps
 class ShellMaster(RunMasterBase):
 
     @defer.inlineCallbacks
+    def setup_config(self):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import steps, schedulers
+
+        c['schedulers'] = [
+            schedulers.AnyBranchScheduler(
+                name="sched",
+                builderNames=["testy"]),
+            schedulers.ForceScheduler(
+                name="force",
+                builderNames=["testy"])]
+
+        f = BuildFactory()
+        f.addStep(steps.ShellCommand(command='echo hello'))
+        c['builders'] = [
+            BuilderConfig(name="testy",
+                          workernames=["local1"],
+                          factory=f)]
+        c['www'] = {'graphql': True}
+        yield self.setup_master(c)
+
+    @defer.inlineCallbacks
     def test_shell(self):
-        yield self.setupConfig(masterConfig())
+        yield self.setup_config()
         # if you don't need change, you can just remove this change, and useChange parameter
         change = dict(branch="master",
                       files=["foo.c"],
                       author="me@foo.com",
                       committer="me@foo.com",
                       comments="good stuff",
                       revision="HEAD",
                       project="none"
                       )
         build = yield self.doForceBuild(wantSteps=True, useChange=change, wantLogs=True,
                                         wantProperties=True)
         self.assertEqual(build['buildid'], 1)
         self.assertEqual(build['properties']['owners'], (['me@foo.com'], 'Build'))
-
-
-# master configuration
-def masterConfig():
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import steps, schedulers
-
-    c['schedulers'] = [
-        schedulers.AnyBranchScheduler(
-            name="sched",
-            builderNames=["testy"]),
-        schedulers.ForceScheduler(
-            name="force",
-            builderNames=["testy"])]
-
-    f = BuildFactory()
-    f.addStep(steps.ShellCommand(command='echo hello'))
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      factory=f)]
-    c['www'] = {'graphql': True}
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_integration_with_secrets.py` & `buildbot-3.8.0/buildbot/test/integration/test_integration_with_secrets.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,50 +19,49 @@
 from buildbot.test.fake.secrets import FakeSecretStorage
 from buildbot.test.util.integration import RunMasterBase
 
 
 class SecretsConfig(RunMasterBase):
 
     @defer.inlineCallbacks
+    def setup_config(self, use_with=False):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import schedulers, steps
+
+        c['schedulers'] = [
+            schedulers.ForceScheduler(
+                name="force",
+                builderNames=["testy"])]
+
+        c['secretsProviders'] = [FakeSecretStorage(
+            secretdict={"foo": "bar", "something": "more"})]
+        f = BuildFactory()
+        if use_with:
+            secrets_list = [("pathA", Interpolate('%(secret:something)s'))]
+            with f.withSecrets(secrets_list):
+                f.addStep(steps.ShellCommand(command=Interpolate('echo %(secret:foo)s')))
+        else:
+            f.addSteps([steps.ShellCommand(command=Interpolate('echo %(secret:foo)s'))],
+                       withSecrets=[("pathA", Interpolate('%(secret:something)s'))])
+        c['builders'] = [
+            BuilderConfig(name="testy",
+                          workernames=["local1"],
+                          factory=f)]
+        yield self.setup_master(c)
+
+    @defer.inlineCallbacks
     def test_secret(self):
-        yield self.setupConfig(masterConfig())
+        yield self.setup_config()
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True)
         self.assertEqual(build['buildid'], 1)
         res = yield self.checkBuildStepLogExist(build, "<foo>")
         self.assertTrue(res)
 
     @defer.inlineCallbacks
     def test_withsecrets(self):
-        yield self.setupConfig(masterConfig(use_with=True))
+        yield self.setup_config(use_with=True)
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True)
         self.assertEqual(build['buildid'], 1)
         res = yield self.checkBuildStepLogExist(build, "<foo>")
         self.assertTrue(res)
-
-
-# master configuration
-def masterConfig(use_with=False):
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import schedulers, steps
-
-    c['schedulers'] = [
-        schedulers.ForceScheduler(
-            name="force",
-            builderNames=["testy"])]
-
-    c['secretsProviders'] = [FakeSecretStorage(
-        secretdict={"foo": "bar", "something": "more"})]
-    f = BuildFactory()
-    if use_with:
-        secrets_list = [("pathA", Interpolate('%(secret:something)s'))]
-        with f.withSecrets(secrets_list):
-            f.addStep(steps.ShellCommand(command=Interpolate('echo %(secret:foo)s')))
-    else:
-        f.addSteps([steps.ShellCommand(command=Interpolate('echo %(secret:foo)s'))],
-                   withSecrets=[("pathA", Interpolate('%(secret:something)s'))])
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      factory=f)]
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_locks.py` & `buildbot-3.8.0/buildbot/test/integration/test_locks.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_log_finish.py` & `buildbot-3.8.0/buildbot/test/integration/test_log_finish.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 from buildbot.process.results import SUCCESS
 from buildbot.test.util.integration import RunMasterBase
 
 
 class TestLog(RunMasterBase):
     # master configuration
 
-    def masterConfig(self, step):
+    @defer.inlineCallbacks
+    def setup_config(self, step):
         c = {}
         from buildbot.config import BuilderConfig
         from buildbot.process.factory import BuildFactory
         from buildbot.plugins import schedulers
 
         c['schedulers'] = [
             schedulers.AnyBranchScheduler(
@@ -38,30 +39,30 @@
 
         f = BuildFactory()
         f.addStep(step)
         c['builders'] = [
             BuilderConfig(name="testy",
                           workernames=["local1"],
                           factory=f)]
-        return c
+        yield self.setup_master(c)
 
     @defer.inlineCallbacks
     def test_shellcommand(self):
         testcase = self
 
         class MyStep(steps.ShellCommand):
 
             def _newLog(self, name, type, logid, logEncoding):
                 r = super()._newLog(name, type, logid, logEncoding)
                 testcase.curr_log = r
                 return r
 
         step = MyStep(command='echo hello')
 
-        yield self.setupConfig(self.masterConfig(step))
+        yield self.setup_config(step)
 
         change = dict(branch="master",
                       files=["foo.c"],
                       author="me@foo.com",
                       committer="me@foo.com",
                       comments="good stuff",
                       revision="HEAD",
@@ -80,15 +81,15 @@
             def _newLog(self, name, type, logid, logEncoding):
                 r = super()._newLog(name, type, logid, logEncoding)
                 testcase.curr_log = r
                 return r
 
         step = MyStep(command='echo hello')
 
-        yield self.setupConfig(self.masterConfig(step))
+        yield self.setup_config(step)
 
         change = dict(branch="master",
                       files=["foo.c"],
                       author="me@foo.com",
                       committer="me@foo.com",
                       comments="good stuff",
                       revision="HEAD",
@@ -108,15 +109,15 @@
                 r = super()._newLog(name, type, logid, logEncoding)
                 testcase.curr_log = r
                 testcase.patch(r, "finish", lambda: defer.fail(RuntimeError('Could not finish')))
                 return r
 
         step = MyStep(command='echo hello')
 
-        yield self.setupConfig(self.masterConfig(step))
+        yield self.setup_config(step)
 
         change = dict(branch="master",
                       files=["foo.c"],
                       author="me@foo.com",
                       committer="me@foo.com",
                       comments="good stuff",
                       revision="HEAD",
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_master.py` & `buildbot-3.8.0/buildbot/test/integration/test_master.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 class RunMaster(RunMasterBase, www.RequiresWwwMixin):
 
     proto = 'pb'
 
     @defer.inlineCallbacks
     def do_test_master(self):
-        yield self.setupConfig(BuildmasterConfig, startWorker=False)
+        yield self.setup_master(BuildmasterConfig, startWorker=False)
 
         # hang out for a fraction of a second, to let startup processes run
         yield deferLater(reactor, 0.01, lambda: None)
 
     # run this test twice, to make sure the first time shut everything down
     # correctly; if this second test fails, but the first succeeds, then
     # something is not cleaning up correctly in stopService.
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_notifier.py` & `buildbot-3.8.0/buildbot/test/integration/test_notifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,28 +37,73 @@
 
     if not ESMTPSenderFactory:
         skip = ("twisted-mail unavailable, "
                 "see: https://twistedmatrix.com/trac/ticket/8770")
 
     @defer.inlineCallbacks
     def create_master_config(self, build_set_summary=False):
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import steps, schedulers, reporters
+
         self.mailDeferred = defer.Deferred()
 
         # patch MailNotifier.sendmail to know when the mail has been sent
         def sendMail(_, mail, recipients):
             self.mailDeferred.callback((mail.as_string(), recipients))
         self.patch(MailNotifier, "sendMail", sendMail)
 
         self.notification = defer.Deferred()
 
         def sendNotification(_, params):
             self.notification.callback(params)
         self.patch(PushoverNotifier, "sendNotification", sendNotification)
 
-        yield self.setupConfig(masterConfig(build_set_summary=build_set_summary))
+        c = {}
+        c['schedulers'] = [
+            schedulers.AnyBranchScheduler(
+                name="sched",
+                builderNames=["testy"])
+        ]
+        f = BuildFactory()
+        f.addStep(steps.ShellCommand(command='echo hello'))
+        c['builders'] = [
+            BuilderConfig(name="testy",
+                          workernames=["local1"],
+                          factory=f)
+        ]
+
+        formatter = MessageFormatter(template='This is a message.')
+        formatter_worker = MessageFormatterMissingWorker(template='No worker.')
+
+        if build_set_summary:
+            generators_mail = [
+                BuildSetStatusGenerator(mode='all'),
+                WorkerMissingGenerator(workers='all'),
+            ]
+            generators_pushover = [
+                BuildSetStatusGenerator(mode='all', message_formatter=formatter),
+                WorkerMissingGenerator(workers=['local1'], message_formatter=formatter_worker),
+            ]
+        else:
+            generators_mail = [
+                BuildStatusGenerator(mode='all'),
+                WorkerMissingGenerator(workers='all'),
+            ]
+            generators_pushover = [
+                BuildStatusGenerator(mode='all', message_formatter=formatter),
+                WorkerMissingGenerator(workers=['local1'], message_formatter=formatter_worker),
+            ]
+
+        c['services'] = [
+            reporters.MailNotifier("bot@foo.com", generators=generators_mail),
+            reporters.PushoverNotifier('1234', 'abcd', generators=generators_pushover)
+        ]
+
+        yield self.setup_master(c)
 
     @defer.inlineCallbacks
     def doTest(self, what):
         change = dict(branch="master",
                       files=["foo.c"],
                       author="author@foo.com",
                       committer="me@foo.com",
@@ -78,15 +123,17 @@
         self.assertEqual(build['buildid'], 1)
         self.assertEqual(params, {
             'title': f"☺ Buildbot (Buildbot): {what} - build successful (master)",
             'message': "This is a message."
         })
 
     def assertEncodedIn(self, text, mail):
-        # python 2.6 default transfer in base64 for utf-8
+        # The default transfer encoding is base64 for utf-8 even when it could be represented
+        # accurately by quoted 7bit encoding. TODO: it is possible to override it,
+        # see https://bugs.python.org/issue12552
         if "base64" not in mail:
             self.assertIn(text, mail)
         else:  # b64encode and remove '=' padding (hence [:-1])
             encodedBytes = base64.b64encode(unicode2bytes(text)).rstrip(b"=")
             encodedText = bytes2unicode(encodedBytes)
             self.assertIn(encodedText, mail)
 
@@ -114,55 +161,7 @@
         self.assertEqual(recipients, ['admin@worker.org'])
         self.assertIn("Subject: Buildbot Buildbot worker local1 missing", mail)
         self.assertIn("disconnected at long time ago", mail)
         self.assertEncodedIn("worker named local1 went away", mail)
         params = yield self.notification
         self.assertEqual(params, {'title': "Buildbot Buildbot worker local1 missing",
                                   'message': b"No worker."})
-
-
-# master configuration
-def masterConfig(build_set_summary):
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import steps, schedulers, reporters
-    c['schedulers'] = [
-        schedulers.AnyBranchScheduler(
-            name="sched",
-            builderNames=["testy"])
-    ]
-    f = BuildFactory()
-    f.addStep(steps.ShellCommand(command='echo hello'))
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      factory=f)
-    ]
-
-    formatter = MessageFormatter(template='This is a message.')
-    formatter_worker = MessageFormatterMissingWorker(template='No worker.')
-
-    if build_set_summary:
-        generators_mail = [
-            BuildSetStatusGenerator(mode='all'),
-            WorkerMissingGenerator(workers='all'),
-        ]
-        generators_pushover = [
-            BuildSetStatusGenerator(mode='all', message_formatter=formatter),
-            WorkerMissingGenerator(workers=['local1'], message_formatter=formatter_worker),
-        ]
-    else:
-        generators_mail = [
-            BuildStatusGenerator(mode='all'),
-            WorkerMissingGenerator(workers='all'),
-        ]
-        generators_pushover = [
-            BuildStatusGenerator(mode='all', message_formatter=formatter),
-            WorkerMissingGenerator(workers=['local1'], message_formatter=formatter_worker),
-        ]
-
-    c['services'] = [
-        reporters.MailNotifier("bot@foo.com", generators=generators_mail),
-        reporters.PushoverNotifier('1234', 'abcd', generators=generators_pushover)
-    ]
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_process_botmaster.py` & `buildbot-3.8.0/buildbot/test/integration/test_process_botmaster.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_setup_entrypoints.py` & `buildbot-3.8.0/buildbot/test/integration/test_setup_entrypoints.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_stop_build.py` & `buildbot-3.8.0/buildbot/test/integration/test_stop_build.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,35 @@
 
 from buildbot.test.util.integration import RunMasterBase
 
 
 class ShellMaster(RunMasterBase):
 
     @defer.inlineCallbacks
+    def setup_config(self):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import steps, schedulers
+
+        c['schedulers'] = [
+            schedulers.AnyBranchScheduler(name="sched", builderNames=["testy"]),
+            schedulers.ForceScheduler(name="force", builderNames=["testy"])
+        ]
+
+        f = BuildFactory()
+        f.addStep(steps.ShellCommand(command='sleep 100', name='sleep'))
+        c['builders'] = [
+            BuilderConfig(name="testy", workernames=["local1"], factory=f)
+        ]
+        yield self.setup_master(c)
+
+    @defer.inlineCallbacks
     def test_shell(self):
-        yield self.setupConfig(masterConfig())
+        yield self.setup_config()
 
         @defer.inlineCallbacks
         def newStepCallback(_, data):
             # when the sleep step start, we kill it
             if data['name'] == 'sleep':
                 brs = yield self.master.data.get(('buildrequests',))
                 brid = brs[-1]['buildrequestid']
@@ -41,31 +60,7 @@
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True, wantProperties=True)
         self.assertEqual(build['buildid'], 1)
 
         # make sure the cancel reason is transferred all the way to the step log
         cancel_log = build['steps'][1]['logs'][-1]
         self.assertEqual(cancel_log['name'], 'cancelled')
         self.assertIn('cancelled by test', cancel_log['contents']['content'])
-
-
-# master configuration
-def masterConfig():
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import steps, schedulers
-
-    c['schedulers'] = [
-        schedulers.AnyBranchScheduler(
-            name="sched",
-            builderNames=["testy"]),
-        schedulers.ForceScheduler(
-            name="force",
-            builderNames=["testy"])]
-
-    f = BuildFactory()
-    f.addStep(steps.ShellCommand(command='sleep 100', name='sleep'))
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      factory=f)]
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_stop_trigger.py` & `buildbot-3.8.0/buildbot/test/integration/test_stop_trigger.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,98 +23,96 @@
 from buildbot.config import BuilderConfig
 from buildbot.plugins import schedulers
 from buildbot.plugins import steps
 from buildbot.process.factory import BuildFactory
 from buildbot.process.results import CANCELLED
 from buildbot.test.util.integration import RunMasterBase
 
+
 # This integration test creates a master and worker environment,
 # with two builders and a trigger step linking them. the triggered build never ends
 # so that we can reliably stop it recursively
-
-
-# master configurations
-def setupTriggerConfiguration(triggeredFactory, nextBuild=None):
-    c = {}
-
-    c['schedulers'] = [
-        schedulers.Triggerable(
-            name="trigsched",
-            builderNames=["triggered"]),
-        schedulers.AnyBranchScheduler(
-            name="sched",
-            builderNames=["main"])]
-
-    f = BuildFactory()
-    f.addStep(steps.Trigger(schedulerNames=['trigsched'],
-                            waitForFinish=True,
-                            updateSourceStamp=True))
-    f.addStep(steps.ShellCommand(command='echo world'))
-
-    mainBuilder = BuilderConfig(name="main",
-                                workernames=["local1"],
-                                factory=f)
-
-    triggeredBuilderKwargs = {'name': "triggered",
-                              'workernames': ["local1"],
-                              'factory': triggeredFactory}
-
-    if nextBuild is not None:
-        triggeredBuilderKwargs['nextBuild'] = nextBuild
-
-    triggeredBuilder = BuilderConfig(**triggeredBuilderKwargs)
-
-    c['builders'] = [mainBuilder, triggeredBuilder]
-    return c
-
-
-def triggerRunsForever():
-    f2 = BuildFactory()
-
-    # Infinite sleep command.
-    if sys.platform == 'win32':
-        # Ping localhost infinitely.
-        # There are other options, however they either don't work in
-        # non-interactive mode (e.g. 'pause'), or doesn't available on all
-        # Windows versions (e.g. 'timeout' and 'choice' are available
-        # starting from Windows 7).
-        cmd = 'ping -t 127.0.0.1'.split()
-    else:
-        cmd = textwrap.dedent("""\
-            while :
-            do
-              echo "sleeping";
-              sleep 1;
-            done
-            """)
-
-    f2.addStep(steps.ShellCommand(command=cmd))
-
-    return setupTriggerConfiguration(f2)
-
-
-def triggeredBuildIsNotCreated():
-    f2 = BuildFactory()
-    f2.addStep(steps.ShellCommand(command="echo 'hello'"))
-
-    def nextBuild(*args, **kwargs):
-        return defer.succeed(None)
-    return setupTriggerConfiguration(f2, nextBuild=nextBuild)
-
-
 class TriggeringMaster(RunMasterBase):
     timeout = 120
     change = dict(branch="master",
                   files=["foo.c"],
                   author="me@foo.com",
                   committer="me@foo.com",
                   comments="good stuff",
                   revision="HEAD",
                   project="none")
 
+    @defer.inlineCallbacks
+    def setup_trigger_config(self, triggeredFactory, nextBuild=None):
+        c = {}
+
+        c['schedulers'] = [
+            schedulers.Triggerable(
+                name="trigsched",
+                builderNames=["triggered"]),
+            schedulers.AnyBranchScheduler(
+                name="sched",
+                builderNames=["main"])]
+
+        f = BuildFactory()
+        f.addStep(steps.Trigger(schedulerNames=['trigsched'],
+                                waitForFinish=True,
+                                updateSourceStamp=True))
+        f.addStep(steps.ShellCommand(command='echo world'))
+
+        mainBuilder = BuilderConfig(name="main",
+                                    workernames=["local1"],
+                                    factory=f)
+
+        triggeredBuilderKwargs = {'name': "triggered",
+                                  'workernames': ["local1"],
+                                  'factory': triggeredFactory}
+
+        if nextBuild is not None:
+            triggeredBuilderKwargs['nextBuild'] = nextBuild
+
+        triggeredBuilder = BuilderConfig(**triggeredBuilderKwargs)
+
+        c['builders'] = [mainBuilder, triggeredBuilder]
+        yield self.setup_master(c)
+
+    @defer.inlineCallbacks
+    def setup_config_trigger_runs_forever(self):
+        f2 = BuildFactory()
+
+        # Infinite sleep command.
+        if sys.platform == 'win32':
+            # Ping localhost infinitely.
+            # There are other options, however they either don't work in
+            # non-interactive mode (e.g. 'pause'), or doesn't available on all
+            # Windows versions (e.g. 'timeout' and 'choice' are available
+            # starting from Windows 7).
+            cmd = 'ping -t 127.0.0.1'.split()
+        else:
+            cmd = textwrap.dedent("""\
+                while :
+                do
+                  echo "sleeping";
+                  sleep 1;
+                done
+                """)
+
+        f2.addStep(steps.ShellCommand(command=cmd))
+
+        yield self.setup_trigger_config(f2)
+
+    @defer.inlineCallbacks
+    def setup_config_triggered_build_not_created(self):
+        f2 = BuildFactory()
+        f2.addStep(steps.ShellCommand(command="echo 'hello'"))
+
+        def nextBuild(*args, **kwargs):
+            return defer.succeed(None)
+        yield self.setup_trigger_config(f2, nextBuild=nextBuild)
+
     def assertBuildIsCancelled(self, b):
         self.assertTrue(b['complete'])
         self.assertEqual(b['results'], CANCELLED, repr(b))
 
     @defer.inlineCallbacks
     def runTest(self, newBuildCallback, flushErrors=False):
         newConsumer = yield self.master.mq.startConsuming(
@@ -129,29 +127,29 @@
         for b in builds:
             self.assertBuildIsCancelled(b)
         if flushErrors:
             self.flushLoggedErrors()
 
     @defer.inlineCallbacks
     def testTriggerRunsForever(self):
-        yield self.setupConfig(triggerRunsForever())
+        yield self.setup_config_trigger_runs_forever()
         self.higherBuild = None
 
         def newCallback(_, data):
             if self.higherBuild is None:
                 self.higherBuild = data['buildid']
             else:
                 self.master.data.control(
                     "stop", {}, ("builds", self.higherBuild))
                 self.higherBuild = None
         yield self.runTest(newCallback, flushErrors=True)
 
     @defer.inlineCallbacks
     def testTriggerRunsForeverAfterCmdStarted(self):
-        yield self.setupConfig(triggerRunsForever())
+        yield self.setup_config_trigger_runs_forever()
         self.higherBuild = None
 
         def newCallback(_, data):
             if self.higherBuild is None:
                 self.higherBuild = data['buildid']
             else:
 
@@ -161,12 +159,12 @@
                     self.higherBuild = None
                 reactor.callLater(5.0, f)
 
         yield self.runTest(newCallback, flushErrors=True)
 
     @defer.inlineCallbacks
     def testTriggeredBuildIsNotCreated(self):
-        yield self.setupConfig(triggeredBuildIsNotCreated())
+        yield self.setup_config_triggered_build_not_created()
 
         def newCallback(_, data):
             self.master.data.control("stop", {}, ("builds", data['buildid']))
         yield self.runTest(newCallback)
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_telegram_bot.py` & `buildbot-3.8.0/buildbot/test/integration/test_telegram_bot.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_trigger.py` & `buildbot-3.8.0/buildbot/test/integration/test_trigger.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 
 expectedOutputRegex = \
     r"""\*\*\* BUILD 1 \*\*\* ==> build successful \(success\)
     \*\*\* STEP worker_preparation \*\*\* ==> worker local1 ready \(success\)
     \*\*\* STEP shell \*\*\* ==> 'echo hello' \(success\)
         log:stdio \({loglines}\)
     \*\*\* STEP trigger \*\*\* ==> triggered trigsched, 1 success \(success\)
-       url:trigsched #2 \(http://localhost:8080/#buildrequests/2\)
-       url:success: build #1 \(http://localhost:8080/#builders/(1|2)/builds/1\)
+       url:trigsched #2 \(http://localhost:8080/#/buildrequests/2\)
+       url:success: build #1 \(http://localhost:8080/#/builders/(1|2)/builds/1\)
     \*\*\* STEP shell_1 \*\*\* ==> 'echo world' \(success\)
         log:stdio \({loglines}\)
 \*\*\* BUILD 2 \*\*\* ==> build successful \(success\)
     \*\*\* STEP worker_preparation \*\*\* ==> worker local1 ready \(success\)
     \*\*\* STEP shell \*\*\* ==> 'echo ola' \(success\)
         log:stdio \({loglines}\)
 """
@@ -48,16 +48,55 @@
                   committer="me@foo.com",
                   comments="good stuff",
                   revision="HEAD",
                   project="none"
                   )
 
     @defer.inlineCallbacks
+    def setup_config(self, addFailure=False):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import steps, schedulers
+
+        c['schedulers'] = [
+            schedulers.Triggerable(
+                name="trigsched",
+                builderNames=["build"]),
+            schedulers.AnyBranchScheduler(
+                name="sched",
+                builderNames=["testy"])]
+
+        f = BuildFactory()
+        f.addStep(steps.ShellCommand(command='echo hello'))
+        f.addStep(steps.Trigger(schedulerNames=['trigsched'],
+                                waitForFinish=True,
+                                updateSourceStamp=True))
+        f.addStep(steps.ShellCommand(command='echo world'))
+        f2 = BuildFactory()
+        f2.addStep(steps.ShellCommand(command='echo ola'))
+        c['builders'] = [
+            BuilderConfig(name="testy",
+                          workernames=["local1"],
+                          factory=f),
+            BuilderConfig(name="build",
+                          workernames=["local1"],
+                          factory=f2)]
+        if addFailure:
+            f3 = BuildFactory()
+            f3.addStep(steps.ShellCommand(command='false'))
+            c['builders'].append(BuilderConfig(name="build2", workernames=["local1"], factory=f3))
+            c['builders'].append(BuilderConfig(name="build3", workernames=["local1"], factory=f2))
+            c['schedulers'][0] = schedulers.Triggerable(name="trigsched",
+                                                        builderNames=["build", "build2", "build3"])
+        yield self.setup_master(c)
+
+    @defer.inlineCallbacks
     def test_trigger(self):
-        yield self.setupConfig(masterConfig())
+        yield self.setup_config()
 
         build = yield self.doForceBuild(wantSteps=True, useChange=self.change, wantLogs=True)
 
         self.assertEqual(
             build['steps'][2]['state_string'], 'triggered trigsched, 1 success')
         builds = yield self.master.data.get(("builds",))
         self.assertEqual(len(builds), 2)
@@ -68,55 +107,15 @@
         # test hosts
         loglines = builds[1]['steps'][1]['logs'][0]['num_lines']
         self.assertRegex(dump.getvalue(),
                          expectedOutputRegex.format(loglines=loglines))
 
     @defer.inlineCallbacks
     def test_trigger_failure(self):
-        yield self.setupConfig(masterConfig(addFailure=True))
+        yield self.setup_config(addFailure=True)
 
         build = yield self.doForceBuild(wantSteps=True, useChange=self.change, wantLogs=True)
 
         self.assertEqual(
             build['steps'][2]['state_string'], 'triggered trigsched, 2 successes, 1 failure')
         builds = yield self.master.data.get(("builds",))
         self.assertEqual(len(builds), 4)
-
-
-# master configuration
-def masterConfig(addFailure=False):
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import steps, schedulers
-
-    c['schedulers'] = [
-        schedulers.Triggerable(
-            name="trigsched",
-            builderNames=["build"]),
-        schedulers.AnyBranchScheduler(
-            name="sched",
-            builderNames=["testy"])]
-
-    f = BuildFactory()
-    f.addStep(steps.ShellCommand(command='echo hello'))
-    f.addStep(steps.Trigger(schedulerNames=['trigsched'],
-                            waitForFinish=True,
-                            updateSourceStamp=True))
-    f.addStep(steps.ShellCommand(command='echo world'))
-    f2 = BuildFactory()
-    f2.addStep(steps.ShellCommand(command='echo ola'))
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      factory=f),
-        BuilderConfig(name="build",
-                      workernames=["local1"],
-                      factory=f2)]
-    if addFailure:
-        f3 = BuildFactory()
-        f3.addStep(steps.ShellCommand(command='false'))
-        c['builders'].append(BuilderConfig(name="build2", workernames=["local1"], factory=f3))
-        c['builders'].append(BuilderConfig(name="build3", workernames=["local1"], factory=f2))
-        c['schedulers'][0] = schedulers.Triggerable(name="trigsched",
-                                                    builderNames=["build", "build2", "build3"])
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_try_client.py` & `buildbot-3.8.0/buildbot/test/integration/test_try_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,21 +89,51 @@
         jobdir.createDirectory()
         self.jobdir = jobdir.path
         for sub in 'new', 'tmp', 'cur':
             jobdir.child(sub).createDirectory()
         return self.jobdir
 
     @defer.inlineCallbacks
+    def setup_config(self, extra_config):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.buildstep import BuildStep
+        from buildbot.process.factory import BuildFactory
+        from buildbot.process import results
+
+        class MyBuildStep(BuildStep):
+
+            def run(self):
+                return results.SUCCESS
+
+        c['change_source'] = []
+        c['schedulers'] = []  # filled in above
+        f1 = BuildFactory()
+        f1.addStep(MyBuildStep(name='one'))
+        f1.addStep(MyBuildStep(name='two'))
+        c['builders'] = [
+            BuilderConfig(name="a", workernames=["local1"], factory=f1),
+        ]
+        c['title'] = "test"
+        c['titleURL'] = "test"
+        c['buildbotURL'] = "http://localhost:8010/"
+        c['mq'] = {'debug': True}
+        # test wants to influence the config, but we still return a new config
+        # each time
+        c.update(extra_config)
+        yield self.setup_master(c)
+
+    @defer.inlineCallbacks
     def startMaster(self, sch):
         extra_config = {
             'schedulers': [sch],
         }
         self.sch = sch
 
-        yield self.setupConfig(masterConfig(extra_config))
+        yield self.setup_config(extra_config)
 
         # wait until the scheduler is active
         yield waitFor(lambda: self.sch.active)
 
         # and, for Try_Userpass, until it's registered its port
         if isinstance(self.sch, trysched.Try_Userpass):
             def getSchedulerPort():
@@ -267,37 +297,7 @@
             "using 'ssh' connect method",
             'job created',
             'job has been delivered',
             'waiting for builds with ssh is not supported'
         ])
         buildsets = yield self.master.db.buildsets.getBuildsets()
         self.assertEqual(len(buildsets), 1)
-
-
-def masterConfig(extra_config):
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.buildstep import BuildStep
-    from buildbot.process.factory import BuildFactory
-    from buildbot.process import results
-
-    class MyBuildStep(BuildStep):
-
-        def run(self):
-            return results.SUCCESS
-
-    c['change_source'] = []
-    c['schedulers'] = []  # filled in above
-    f1 = BuildFactory()
-    f1.addStep(MyBuildStep(name='one'))
-    f1.addStep(MyBuildStep(name='two'))
-    c['builders'] = [
-        BuilderConfig(name="a", workernames=["local1"], factory=f1),
-    ]
-    c['title'] = "test"
-    c['titleURL'] = "test"
-    c['buildbotURL'] = "http://localhost:8010/"
-    c['mq'] = {'debug': True}
-    # test wants to influence the config, but we still return a new config
-    # each time
-    c.update(extra_config)
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_try_client_e2e.py` & `buildbot-3.8.0/buildbot/test/integration/test_try_client_e2e.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,43 +23,42 @@
 
 
 # This integration test tests that the try command line works end2end
 class TryClientE2E(RunMasterBase):
     timeout = 15
 
     @defer.inlineCallbacks
+    def setup_config(self):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import steps, schedulers
+
+        c['schedulers'] = [
+            schedulers.Try_Userpass(name="try",
+                                    builderNames=["testy"],
+                                    port='tcp:0',
+                                    userpass=[("alice", "pw1")])
+        ]
+        f = BuildFactory()
+        f.addStep(steps.ShellCommand(command='echo hello'))
+        c['builders'] = [
+            BuilderConfig(name="testy",
+                          workernames=["local1"],
+                          factory=f)]
+        yield self.setup_master(c)
+
+    @defer.inlineCallbacks
     def test_shell(self):
-        yield self.setupConfig(masterConfig())
+        yield self.setup_config()
 
         def trigger_callback():
             port = self.master.pbmanager.dispatchers['tcp:0'].port.getHost().port
 
             def thd():
                 os.system(f"buildbot try --connect=pb --master=127.0.0.1:{port} -b testy "
                           "--property=foo:bar --username=alice --passwd=pw1 --vc=none")
             reactor.callInThread(thd)
 
         build = yield self.doForceBuild(wantSteps=True, triggerCallback=trigger_callback,
                                         wantLogs=True, wantProperties=True)
         self.assertEqual(build['buildid'], 1)
-
-
-# master configuration
-def masterConfig():
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import steps, schedulers
-
-    c['schedulers'] = [
-        schedulers.Try_Userpass(name="try",
-                                builderNames=["testy"],
-                                port='tcp:0',
-                                userpass=[("alice", "pw1")])
-    ]
-    f = BuildFactory()
-    f.addStep(steps.ShellCommand(command='echo hello'))
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      factory=f)]
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_upgrade.py` & `buildbot-3.8.0/buildbot/test/integration/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_usePty.py` & `buildbot-3.8.0/buildbot/test/integration/test_usePty.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,18 +23,40 @@
 from buildbot.test.util.integration import RunMasterBase
 
 
 # This integration test creates a master and worker environment,
 # with one builder and a shellcommand step, which use usePTY
 class ShellMaster(RunMasterBase):
 
+    @defer.inlineCallbacks
+    def setup_config(self, usePTY):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import steps, schedulers
+
+        c['schedulers'] = [
+            schedulers.ForceScheduler(
+                name="force",
+                builderNames=["testy"])]
+
+        f = BuildFactory()
+        f.addStep(steps.ShellCommand(
+            command='if [ -t 1 ] ; then echo in a terminal; else echo "not a terminal"; fi',
+            usePTY=usePTY))
+        c['builders'] = [
+            BuilderConfig(name="testy",
+                          workernames=["local1"],
+                          factory=f)]
+        yield self.setup_master(c)
+
     @skipUnlessPlatformIs('posix')
     @defer.inlineCallbacks
     def test_usePTY(self):
-        yield self.setupConfig(masterConfig(usePTY=True))
+        yield self.setup_config(usePTY=True)
 
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True)
         self.assertEqual(build['buildid'], 1)
         res = yield self.checkBuildStepLogExist(build, "in a terminal", onlyStdout=True)
         self.assertTrue(res)
 
         # Twisted versions less than 17.1.0 would issue a warning:
@@ -46,36 +68,13 @@
         # https://github.com/twisted/twisted/commit/23fa3cc05549251ea4118e4e03354d58df87eaaa
         if parse_version(twistedVersion) < parse_version("17.1.0"):
             self.flushWarnings()
 
     @skipUnlessPlatformIs('posix')
     @defer.inlineCallbacks
     def test_NOusePTY(self):
-        yield self.setupConfig(masterConfig(usePTY=False))
+        yield self.setup_config(usePTY=False)
 
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True)
         self.assertEqual(build['buildid'], 1)
         res = yield self.checkBuildStepLogExist(build, "not a terminal", onlyStdout=True)
         self.assertTrue(res)
-
-
-# master configuration
-def masterConfig(usePTY):
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import steps, schedulers
-
-    c['schedulers'] = [
-        schedulers.ForceScheduler(
-            name="force",
-            builderNames=["testy"])]
-
-    f = BuildFactory()
-    f.addStep(steps.ShellCommand(
-        command='if [ -t 1 ] ; then echo in a terminal; else echo "not a terminal"; fi',
-        usePTY=usePTY))
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      factory=f)]
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_virtual_builder.py` & `buildbot-3.8.0/buildbot/test/integration/test_virtual_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,43 +21,42 @@
 
 # This integration test creates a master and worker environment,
 # with one builder and a shellcommand step
 # meant to be a template for integration steps
 class ShellMaster(RunMasterBase):
 
     @defer.inlineCallbacks
+    def setup_config(self):
+        c = {}
+        from buildbot.config import BuilderConfig
+        from buildbot.process.factory import BuildFactory
+        from buildbot.plugins import steps, schedulers
+
+        c['schedulers'] = [
+            schedulers.ForceScheduler(
+                name="force",
+                builderNames=["testy"])]
+
+        f = BuildFactory()
+        f.addStep(steps.ShellCommand(command='echo hello'))
+        c['builders'] = [
+            BuilderConfig(name="testy",
+                          workernames=["local1"],
+                          properties={
+                              'virtual_builder_name': 'virtual_testy',
+                              'virtual_builder_description': 'I am a virtual builder',
+                              'virtual_builder_tags': ['virtual'],
+                          },
+                          factory=f)]
+        yield self.setup_master(c)
+
+    @defer.inlineCallbacks
     def test_shell(self):
-        yield self.setupConfig(masterConfig())
+        yield self.setup_config()
         build = yield self.doForceBuild(wantSteps=True, wantLogs=True)
         self.assertEqual(build['buildid'], 1)
         builders = yield self.master.data.get(("builders",))
         self.assertEqual(len(builders), 2)
         self.assertEqual(builders[1], {
             'masterids': [], 'tags': ['virtual', '_virtual_'],
             'description': 'I am a virtual builder', 'name': 'virtual_testy', 'builderid': 2})
         self.assertEqual(build['builderid'], builders[1]['builderid'])
-
-
-# master configuration
-def masterConfig():
-    c = {}
-    from buildbot.config import BuilderConfig
-    from buildbot.process.factory import BuildFactory
-    from buildbot.plugins import steps, schedulers
-
-    c['schedulers'] = [
-        schedulers.ForceScheduler(
-            name="force",
-            builderNames=["testy"])]
-
-    f = BuildFactory()
-    f.addStep(steps.ShellCommand(command='echo hello'))
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["local1"],
-                      properties={
-                          'virtual_builder_name': 'virtual_testy',
-                          'virtual_builder_description': 'I am a virtual builder',
-                          'virtual_builder_tags': ['virtual'],
-                      },
-                      factory=f)]
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_worker.py` & `buildbot-3.8.0/buildbot/test/integration/test_worker.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_worker_comm.py` & `buildbot-3.8.0/buildbot/test/integration/test_worker_comm.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_worker_kubernetes.py` & `buildbot-3.8.0/buildbot/test/integration/test_worker_kubernetes.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,74 +58,72 @@
                 "variable TEST_KUBERNETES is set")
         if 'masterFQDN' not in os.environ:
             raise SkipTest(
                 "you need to export masterFQDN. You have example in the test file. "
                 "Make sure that you're spawned worker can callback this IP")
 
     @defer.inlineCallbacks
+    def setup_config(self, num_concurrent, extra_steps=None):
+        if extra_steps is None:
+            extra_steps = []
+        c = {}
+
+        c['schedulers'] = [
+            schedulers.ForceScheduler(name="force", builderNames=["testy"])
+        ]
+        triggereables = []
+        for i in range(num_concurrent):
+            c['schedulers'].append(
+                schedulers.Triggerable(
+                    name="trigsched" + str(i), builderNames=["build"]))
+            triggereables.append("trigsched" + str(i))
+
+        f = BuildFactory()
+        f.addStep(steps.ShellCommand(command='echo hello'))
+        f.addStep(
+            steps.Trigger(
+                schedulerNames=triggereables,
+                waitForFinish=True,
+                updateSourceStamp=True))
+        f.addStep(steps.ShellCommand(command='echo world'))
+        f2 = BuildFactory()
+        f2.addStep(steps.ShellCommand(command='echo ola'))
+        for step in extra_steps:
+            f2.addStep(step)
+        c['builders'] = [
+            BuilderConfig(name="testy", workernames=["kubernetes0"], factory=f),
+            BuilderConfig(
+                name="build",
+                workernames=["kubernetes" + str(i) for i in range(num_concurrent)],
+                factory=f2)
+        ]
+        masterFQDN = os.environ.get('masterFQDN')
+        c['workers'] = [
+            kubernetes.KubeLatentWorker(
+                'kubernetes' + str(i),
+                'buildbot/buildbot-worker',
+                kube_config=kubeclientservice.KubeCtlProxyConfigLoader(
+                    namespace=os.getenv("KUBE_NAMESPACE", "default")),
+                masterFQDN=masterFQDN) for i in range(num_concurrent)
+        ]
+        # un comment for debugging what happens if things looks locked.
+        # c['www'] = {'port': 8080}
+        c['protocols'] = {"pb": {"port": "tcp:9989"}}
+
+        yield self.setup_master(c, startWorker=False)
+
+    @defer.inlineCallbacks
     def test_trigger(self):
-        yield self.setupConfig(
-            masterConfig(num_concurrent=NUM_CONCURRENT), startWorker=False)
+        yield self.setup_config(num_concurrent=NUM_CONCURRENT)
         yield self.doForceBuild()
 
         builds = yield self.master.data.get(("builds", ))
         # if there are some retry, there will be more builds
         self.assertEqual(len(builds), 1 + NUM_CONCURRENT)
         for b in builds:
             self.assertEqual(b['results'], SUCCESS)
 
 
 class KubernetesMasterTReq(KubernetesMaster):
     def setup(self):
         super().setUp()
         self.patch(kubernetes.KubeClientService, 'PREFER_TREQ', True)
-
-
-# master configuration
-def masterConfig(num_concurrent, extra_steps=None):
-    if extra_steps is None:
-        extra_steps = []
-    c = {}
-
-    c['schedulers'] = [
-        schedulers.ForceScheduler(name="force", builderNames=["testy"])
-    ]
-    triggereables = []
-    for i in range(num_concurrent):
-        c['schedulers'].append(
-            schedulers.Triggerable(
-                name="trigsched" + str(i), builderNames=["build"]))
-        triggereables.append("trigsched" + str(i))
-
-    f = BuildFactory()
-    f.addStep(steps.ShellCommand(command='echo hello'))
-    f.addStep(
-        steps.Trigger(
-            schedulerNames=triggereables,
-            waitForFinish=True,
-            updateSourceStamp=True))
-    f.addStep(steps.ShellCommand(command='echo world'))
-    f2 = BuildFactory()
-    f2.addStep(steps.ShellCommand(command='echo ola'))
-    for step in extra_steps:
-        f2.addStep(step)
-    c['builders'] = [
-        BuilderConfig(name="testy", workernames=["kubernetes0"], factory=f),
-        BuilderConfig(
-            name="build",
-            workernames=["kubernetes" + str(i) for i in range(num_concurrent)],
-            factory=f2)
-    ]
-    masterFQDN = os.environ.get('masterFQDN')
-    c['workers'] = [
-        kubernetes.KubeLatentWorker(
-            'kubernetes' + str(i),
-            'buildbot/buildbot-worker',
-            kube_config=kubeclientservice.KubeCtlProxyConfigLoader(
-                namespace=os.getenv("KUBE_NAMESPACE", "default")),
-            masterFQDN=masterFQDN) for i in range(num_concurrent)
-    ]
-    # un comment for debugging what happens if things looks locked.
-    # c['www'] = {'port': 8080}
-    c['protocols'] = {"pb": {"port": "tcp:9989"}}
-
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_worker_latent.py` & `buildbot-3.8.0/buildbot/test/integration/test_worker_latent.py`

 * *Files 1% similar despite different names*

```diff
@@ -659,14 +659,51 @@
             set(brids),
             {req['buildrequestid'] for req in unclaimed_build_requests}
         )
         yield controller.start_instance(False)
         yield controller.auto_stop(True)
 
     @defer.inlineCallbacks
+    def test_stalled_substantiation_then_check_instance_fails_get_requeued(self):
+        """
+        If a latent worker substantiate, but not connect and check_instance() indicates a crash,
+        the build request should become unclaimed as soon as check_instance_interval passes
+        """
+        controller, builder_id = yield self.create_single_worker_config(
+            controller_kwargs={'check_instance_interval': 10}
+        )
+        controller.auto_connect_worker = False
+
+        # Trigger a buildrequest
+        _, brids = yield self.create_build_request([builder_id])
+
+        unclaimed_build_requests = []
+        yield self.master.mq.startConsuming(
+            lambda key, request: unclaimed_build_requests.append(request),
+            ('buildrequests', None, 'unclaimed'))
+
+        # The worker startup succeeds, but it doe not connect and check_instance() later
+        # indicates a crash.
+        yield controller.start_instance(True)
+
+        self.reactor.advance(10)
+        controller.has_crashed = True
+        self.reactor.advance(10)
+
+        # Flush the errors logged by the failure.
+        self.flushLoggedErrors(LatentWorkerFailedToSubstantiate)
+
+        # When the substantiation fails, the buildrequest becomes unclaimed.
+        self.assertEqual(
+            set(brids),
+            {req['buildrequestid'] for req in unclaimed_build_requests}
+        )
+        yield controller.auto_stop(True)
+
+    @defer.inlineCallbacks
     def test_sever_connection_before_ping_then_timeout_get_requeued(self):
         """
         If a latent worker connects, but its connection is severed without
         notification in the TCP layer, we successfully wait until TCP times
         out and requeue the build.
         """
         controller, builder_id = yield self.create_single_worker_config(
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_worker_marathon.py` & `buildbot-3.8.0/buildbot/test/integration/test_worker_marathon.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,80 +50,79 @@
     def setUp(self):
         if "BBTEST_MARATHON_URL" not in os.environ:
             raise SkipTest(
                 "marathon integration tests only run when environment variable BBTEST_MARATHON_URL"
                 " is with url to Marathon api ")
 
     @defer.inlineCallbacks
+    def setup_config(self, num_concurrent, extra_steps=None):
+        if extra_steps is None:
+            extra_steps = []
+        c = {}
+
+        c['schedulers'] = [
+            schedulers.ForceScheduler(
+                name="force",
+                builderNames=["testy"])]
+        triggereables = []
+        for i in range(num_concurrent):
+            c['schedulers'].append(
+                schedulers.Triggerable(
+                    name="trigsched" + str(i),
+                    builderNames=["build"]))
+            triggereables.append("trigsched" + str(i))
+
+        f = BuildFactory()
+        f.addStep(steps.ShellCommand(command='echo hello'))
+        f.addStep(steps.Trigger(schedulerNames=triggereables,
+                                waitForFinish=True,
+                                updateSourceStamp=True))
+        f.addStep(steps.ShellCommand(command='echo world'))
+        f2 = BuildFactory()
+        f2.addStep(steps.ShellCommand(command='echo ola'))
+        for step in extra_steps:
+            f2.addStep(step)
+        c['builders'] = [
+            BuilderConfig(name="testy",
+                          workernames=["marathon0"],
+                          factory=f),
+            BuilderConfig(name="build",
+                          workernames=["marathon" + str(i)
+                                       for i in range(num_concurrent)],
+                          factory=f2)]
+        url = os.environ.get('BBTEST_MARATHON_URL')
+        creds = os.environ.get('BBTEST_MARATHON_CREDS')
+        if creds is not None:
+            user, password = creds.split(":")
+        else:
+            user = password = None
+        masterFQDN = os.environ.get('masterFQDN')
+        marathon_extra_config = {
+        }
+        c['workers'] = [
+            MarathonLatentWorker('marathon' + str(i), url, user, password,
+                                 'buildbot/buildbot-worker:master',
+                                 marathon_extra_config=marathon_extra_config,
+                                 masterFQDN=masterFQDN)
+            for i in range(num_concurrent)
+        ]
+        # un comment for debugging what happens if things looks locked.
+        # c['www'] = {'port': 8080}
+        # if the masterFQDN is forced (proxy case), then we use 9989 default port
+        # else, we try to find a free port
+        if masterFQDN is not None:
+            c['protocols'] = {"pb": {"port": "tcp:9989"}}
+        else:
+            c['protocols'] = {"pb": {"port": "tcp:0"}}
+
+        yield self.setup_master(c, startWorker=False)
+
+    @defer.inlineCallbacks
     def test_trigger(self):
-        yield self.setupConfig(masterConfig(num_concurrent=NUM_CONCURRENT), startWorker=False)
+        yield self.setup_master(num_concurrent=NUM_CONCURRENT)
         yield self.doForceBuild()
 
         builds = yield self.master.data.get(("builds",))
         # if there are some retry, there will be more builds
         self.assertEqual(len(builds), 1 + NUM_CONCURRENT)
         for b in builds:
             self.assertEqual(b['results'], SUCCESS)
-
-
-# master configuration
-def masterConfig(num_concurrent, extra_steps=None):
-    if extra_steps is None:
-        extra_steps = []
-    c = {}
-
-    c['schedulers'] = [
-        schedulers.ForceScheduler(
-            name="force",
-            builderNames=["testy"])]
-    triggereables = []
-    for i in range(num_concurrent):
-        c['schedulers'].append(
-            schedulers.Triggerable(
-                name="trigsched" + str(i),
-                builderNames=["build"]))
-        triggereables.append("trigsched" + str(i))
-
-    f = BuildFactory()
-    f.addStep(steps.ShellCommand(command='echo hello'))
-    f.addStep(steps.Trigger(schedulerNames=triggereables,
-                            waitForFinish=True,
-                            updateSourceStamp=True))
-    f.addStep(steps.ShellCommand(command='echo world'))
-    f2 = BuildFactory()
-    f2.addStep(steps.ShellCommand(command='echo ola'))
-    for step in extra_steps:
-        f2.addStep(step)
-    c['builders'] = [
-        BuilderConfig(name="testy",
-                      workernames=["marathon0"],
-                      factory=f),
-        BuilderConfig(name="build",
-                      workernames=["marathon" + str(i)
-                                   for i in range(num_concurrent)],
-                      factory=f2)]
-    url = os.environ.get('BBTEST_MARATHON_URL')
-    creds = os.environ.get('BBTEST_MARATHON_CREDS')
-    if creds is not None:
-        user, password = creds.split(":")
-    else:
-        user = password = None
-    masterFQDN = os.environ.get('masterFQDN')
-    marathon_extra_config = {
-    }
-    c['workers'] = [
-        MarathonLatentWorker('marathon' + str(i), url, user, password,
-                             'buildbot/buildbot-worker:master',
-                             marathon_extra_config=marathon_extra_config,
-                             masterFQDN=masterFQDN)
-        for i in range(num_concurrent)
-    ]
-    # un comment for debugging what happens if things looks locked.
-    # c['www'] = {'port': 8080}
-    # if the masterFQDN is forced (proxy case), then we use 9989 default port
-    # else, we try to find a free port
-    if masterFQDN is not None:
-        c['protocols'] = {"pb": {"port": "tcp:9989"}}
-    else:
-        c['protocols'] = {"pb": {"port": "tcp:0"}}
-
-    return c
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_worker_proxy.py` & `buildbot-3.8.0/buildbot/test/integration/test_worker_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,18 +150,18 @@
             print("---- ------ ----")
             with open(self.queue.get(), encoding='utf-8') as file:
                 print(file.read())
             print("---- ------ ----")
             os.unlink(get_log_path())
 
     @defer.inlineCallbacks
-    def setupConfig(self, config_dict, startWorker=True):
+    def setup_master(self, config_dict, startWorker=True):
         proxy_connection_string = f"tcp:127.0.0.1:{self.target_port}"
-        yield RunMasterBase.setupConfig(self, config_dict, startWorker,
-                                        proxy_connection_string=proxy_connection_string)
+        yield super().setup_master(config_dict, startWorker,
+                                   proxy_connection_string=proxy_connection_string)
 
 
 # Use interoperability test cases to test the HTTP proxy tunneling.
 
 class ProxyCommandMixinMasterPB(RunMasterBehindProxy, test_commandmixin.CommandMixinMasterPB):
     pass
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_worker_upcloud.py` & `buildbot-3.8.0/buildbot/test/integration/test_worker_upcloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         if "BBTEST_UPCLOUD_CREDS" not in os.environ:
             raise SkipTest(
                 "upcloud integration tests only run when environment variable BBTEST_UPCLOUD_CREDS"
                 " is set to valid upcloud credentials ")
 
     @defer.inlineCallbacks
     def test_trigger(self):
-        yield self.setupConfig(masterConfig(num_concurrent=1), startWorker=False)
+        yield self.setup_master(masterConfig(num_concurrent=1), startWorker=False)
         yield self.doForceBuild()
 
         builds = yield self.master.data.get(("builds",))
         # if there are some retry, there will be more builds
         self.assertEqual(len(builds), 1 + NUM_CONCURRENT)
         for b in builds:
             self.assertEqual(b['results'], SUCCESS)
```

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_worker_workerside.py` & `buildbot-3.8.0/buildbot/test/integration/test_worker_workerside.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/integration/test_www.py` & `buildbot-3.8.0/buildbot/test/integration/test_www.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/reactor.py` & `buildbot-3.8.0/buildbot/test/reactor.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/regressions/test_bad_change_properties_rows.py` & `buildbot-3.8.0/buildbot/test/regressions/test_bad_change_properties_rows.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/regressions/test_oldpaths.py` & `buildbot-3.8.0/buildbot/test/regressions/test_oldpaths.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/regressions/test_steps_shell_WarningCountingShellCommand.py` & `buildbot-3.8.0/buildbot/test/regressions/test_steps_shell_WarningCountingShellCommand.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/runprocess.py` & `buildbot-3.8.0/buildbot/test/runprocess.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/steps.py` & `buildbot-3.8.0/buildbot/test/steps.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,52 +43,57 @@
     @return The list of keys missing in d1, the list of keys missing in d2, and the differences
     in any nested keys
     """
     d1_keys = set(d1.keys())
     d2_keys = set(d2.keys())
     both = d1_keys & d2_keys
 
-    missing_in_d1 = []
-    missing_in_d2 = []
+    missing_in_d1 = {}
+    missing_in_d2 = {}
     different = []
 
     for k in both:
         if isinstance(d1[k], dict) and isinstance(d2[k], dict):
-            missing_in_v1, missing_in_v2, different_in_v = _dict_diff(
-                d1[k], d2[k])
-            missing_in_d1.extend([f'{k}.{m}' for m in missing_in_v1])
-            missing_in_d2.extend([f'{k}.{m}' for m in missing_in_v2])
+            missing_in_v1, missing_in_v2, different_in_v = _dict_diff(d1[k], d2[k])
+
+            for sub_key in missing_in_v1:
+                missing_in_d1[f'{k}.{sub_key}'] = d2[k][sub_key]
+            for sub_key in missing_in_v2:
+                missing_in_d2[f'{k}.{sub_key}'] = d1[k][sub_key]
+
             for child_k, left, right in different_in_v:
                 different.append((f'{k}.{child_k}', left, right))
             continue
         if d1[k] != d2[k]:
             different.append((k, d1[k], d2[k]))
-    missing_in_d1.extend(d2_keys - both)
-    missing_in_d2.extend(d1_keys - both)
+
+    for k in d2_keys - both:
+        missing_in_d1[k] = d2[k]
+    for k in d1_keys - both:
+        missing_in_d2[k] = d1[k]
     return missing_in_d1, missing_in_d2, different
 
 
 def _describe_cmd_difference(exp_command, exp_args, got_command, got_args):
     if exp_command != got_command:
         return (f'Expected command type {exp_command} got {got_command}. Expected args '
                 f'{exp_args!r}')
     if exp_args == got_args:
         return ""
     text = ""
     missing_in_exp, missing_in_cmd, diff = _dict_diff(exp_args, got_args)
     if missing_in_exp:
-        missing_dict = {key: got_args[key] for key in missing_in_exp}
-        text += f'Keys in command missing from expectation: {missing_dict!r}\n'
+        text += f'Keys in command missing from expectation: {missing_in_exp!r}\n'
     if missing_in_cmd:
-        missing_dict = {key: exp_args[key] for key in missing_in_cmd}
-        text += f'Keys in expectation missing from command: {missing_dict!r}\n'
+        text += f'Keys in expectation missing from command: {missing_in_cmd!r}\n'
     if diff:
         formatted_diff = [f'"{d[0]}":\nexpected: {d[1]!r}\ngot:      {d[2]!r}\n' for d in diff]
         text += ('Key differences between expectation and command: {0}\n'.format(
             '\n'.join(formatted_diff)))
+
     return text
 
 
 class ExpectRemoteRef:
 
     """
     Define an expected RemoteReference in the args to an L{Expect} class
```

### Comparing `buildbot-3.7.0/buildbot/test/test_extra_coverage.py` & `buildbot-3.8.0/buildbot/test/test_extra_coverage.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_asyncio.py` & `buildbot-3.8.0/buildbot/test/unit/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_buildbot_net_usage_data.py` & `buildbot-3.8.0/buildbot/test/unit/test_buildbot_net_usage_data.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_clients_sendchange.py` & `buildbot-3.8.0/buildbot/test/unit/test_clients_sendchange.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_clients_tryclient.py` & `buildbot-3.8.0/buildbot/test/unit/test_clients_tryclient.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_clients_usersclient.py` & `buildbot-3.8.0/buildbot/test/unit/test_clients_usersclient.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_configurator_base.py` & `buildbot-3.8.0/buildbot/test/unit/test_configurator_base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_contrib_buildbot_cvs_mail.py` & `buildbot-3.8.0/buildbot/test/unit/test_contrib_buildbot_cvs_mail.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_download_secret_to_worker.py` & `buildbot-3.8.0/buildbot/test/unit/test_download_secret_to_worker.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_fake_httpclientservice.py` & `buildbot-3.8.0/buildbot/test/unit/test_fake_httpclientservice.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_fake_secrets_manager.py` & `buildbot-3.8.0/buildbot/test/unit/test_fake_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_interpolate_secrets.py` & `buildbot-3.8.0/buildbot/test/unit/test_interpolate_secrets.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_janitor_configurator.py` & `buildbot-3.8.0/buildbot/test/unit/test_janitor_configurator.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_locks.py` & `buildbot-3.8.0/buildbot/test/unit/test_locks.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_machine_generic.py` & `buildbot-3.8.0/buildbot/test/unit/test_machine_generic.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_master.py` & `buildbot-3.8.0/buildbot/test/unit/test_master.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_mq.py` & `buildbot-3.8.0/buildbot/test/unit/test_mq.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_mq_base.py` & `buildbot-3.8.0/buildbot/test/unit/test_mq_base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_mq_connector.py` & `buildbot-3.8.0/buildbot/test/unit/test_mq_connector.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_mq_simple.py` & `buildbot-3.8.0/buildbot/test/unit/test_mq_simple.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_mq_wamp.py` & `buildbot-3.8.0/buildbot/test/unit/test_mq_wamp.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_plugins.py` & `buildbot-3.8.0/buildbot/test/unit/test_plugins.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_revlinks.py` & `buildbot-3.8.0/buildbot/test/unit/test_revlinks.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_secret_in_file.py` & `buildbot-3.8.0/buildbot/test/unit/test_secret_in_file.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_secret_in_hvac.py` & `buildbot-3.8.0/buildbot/test/unit/test_secret_in_hvac.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_secret_in_passwordstore.py` & `buildbot-3.8.0/buildbot/test/unit/test_secret_in_passwordstore.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_secret_in_vault.py` & `buildbot-3.8.0/buildbot/test/unit/test_secret_in_vault.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_secret_rendered_service.py` & `buildbot-3.8.0/buildbot/test/unit/test_secret_rendered_service.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_stats_service.py` & `buildbot-3.8.0/buildbot/test/unit/test_stats_service.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_steps_git_diffinfo.py` & `buildbot-3.8.0/buildbot/test/unit/test_steps_git_diffinfo.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_test_util_validation.py` & `buildbot-3.8.0/buildbot/test/unit/test_test_util_validation.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_test_util_warnings.py` & `buildbot-3.8.0/buildbot/test/unit/test_test_util_warnings.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_util.py` & `buildbot-3.8.0/buildbot/test/unit/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 #
 # Copyright Buildbot Team Members
 
 import datetime
 import locale
 import os
+import sys
 
 import mock
 
 from twisted.internet import reactor
 from twisted.internet import task
 from twisted.trial import unittest
 
@@ -377,15 +378,18 @@
         config = mock.Mock()
         util.check_functional_environment(config)
         self.assertEqual(config.error.called, False)
 
     def test_broken_locale(self):
         def err():
             raise KeyError
-        self.patch(locale, 'getdefaultlocale', err)
+        if sys.version_info >= (3, 11, 0):
+            self.patch(locale, 'getencoding', err)
+        else:
+            self.patch(locale, 'getdefaultlocale', err)
         config = mock.Mock()
         util.check_functional_environment(config)
         config.error.assert_called_with(mock.ANY)
 
 
 class StripUrlPassword(unittest.TestCase):
```

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_util_queue.py` & `buildbot-3.8.0/buildbot/test/unit/test_util_queue.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_version.py` & `buildbot-3.8.0/buildbot/test/unit/test_version.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/unit/test_wamp_connector.py` & `buildbot-3.8.0/buildbot/test/unit/test_wamp_connector.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/changesource.py` & `buildbot-3.8.0/buildbot/test/util/changesource.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/config.py` & `buildbot-3.8.0/buildbot/test/util/config.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/configurators.py` & `buildbot-3.8.0/buildbot/test/util/configurators.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/connector_component.py` & `buildbot-3.8.0/buildbot/test/util/connector_component.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/db.py` & `buildbot-3.8.0/buildbot/test/util/db.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/decorators.py` & `buildbot-3.8.0/buildbot/test/util/decorators.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/dirs.py` & `buildbot-3.8.0/buildbot/test/util/dirs.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/endpoint.py` & `buildbot-3.8.0/buildbot/test/util/endpoint.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/fuzz.py` & `buildbot-3.8.0/buildbot/test/util/fuzz.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/integration.py` & `buildbot-3.8.0/buildbot/test/util/integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 class RunMasterBase(unittest.TestCase):
     proto = "null"
 
     if Worker is None:
         skip = "buildbot-worker package is not installed"
 
     @defer.inlineCallbacks
-    def setupConfig(self, config_dict, startWorker=True, **worker_kwargs):
+    def setup_master(self, config_dict, startWorker=True, **worker_kwargs):
         """
         Setup and start a master configured
         by the function configFunc defined in the test module.
         @type config_dict: dict
         @param configFunc: The BuildmasterConfig dictionary.
         """
         # mock reactor.stop (which trial *really* doesn't
@@ -208,14 +208,15 @@
                 proto = {"null": {}}
                 workerclass = worker.LocalWorker
             config_dict['workers'] = [workerclass("local1", password=Interpolate("localpw"),
                                                   missing_timeout=0)]
             config_dict['protocols'] = proto
 
         m = yield getMaster(self, reactor, config_dict)
+        self.master_config_dict = config_dict
         self.master = m
         self.assertFalse(stop.called,
                          "startService tried to stop the reactor; check logs")
 
         if not startWorker:
             return
```

### Comparing `buildbot-3.7.0/buildbot/test/util/interfaces.py` & `buildbot-3.8.0/buildbot/test/util/interfaces.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 #
 # Copyright Buildbot Team Members
 
 
 import inspect
 import pkg_resources
+from collections import OrderedDict
 
 import zope.interface.interface
 from twisted.trial import unittest
 from zope.interface.interface import Attribute
 
 
 class InterfaceTests:
@@ -33,47 +34,47 @@
             def methodTemplate(self, arg1, arg2):
                 pass
 
         or, more useful when you will be faking out C{methodUnderTest}:
 
             self.assertArgSpecMatches(obj.methodUnderTest, self.fakeMethod)
         """
-        def filter(spec):
-            # the tricky thing here is to align args and defaults, since the
-            # defaults correspond to the *last* n elements of args.  To make
-            # things easier, we go in reverse, and keep a separate counter for
-            # the defaults
-            args = spec[0]
-            defaults = list(spec[3] if spec[3] is not None else [])
-            di = -1
-            for ai in range(len(args) - 1, -1, -1):
-                arg = args[ai]
-                if arg.startswith('_') or (arg == 'self' and ai == 0):
-                    del args[ai]
-                    if -di <= len(defaults):
-                        del defaults[di]
-                        di += 1
-                di -= 1
+        def filter(signature):
+            if len(signature.parameters) == 0:
+                return signature
+
+            parameters = OrderedDict(signature.parameters)
+            for name in parameters:
+                if name == 'self':
+                    parameters.pop('self')
+                break
+
+            delete_names = []
+            for name in parameters:
+                if name.startswith('_'):
+                    delete_names.append(name)
+            for name in delete_names:
+                parameters.pop(name)
 
-            return (args, spec[1], spec[2], defaults or None)
+            signature = signature.replace(parameters=parameters.values())
+            return signature
 
         def remove_decorators(func):
             try:
                 return func.__wrapped__
             except AttributeError:
                 return func
 
         def filter_argspec(func):
             return filter(
-                inspect.getfullargspec(remove_decorators(func)))
+                inspect.signature(remove_decorators(func)))
 
         def assert_same_argspec(expected, actual):
             if expected != actual:
-                msg = (f"Expected: {inspect.formatargspec(*expected)}; got: "
-                       f"{inspect.formatargspec(*actual)}")
+                msg = (f"Expected: {expected}; got: {actual}")
                 self.fail(msg)
 
         actual_argspec = filter_argspec(actualMethod)
 
         for fakeMethod in fakeMethods:
             fake_argspec = filter_argspec(fakeMethod)
             assert_same_argspec(actual_argspec, fake_argspec)
```

### Comparing `buildbot-3.7.0/buildbot/test/util/logging.py` & `buildbot-3.8.0/buildbot/test/util/logging.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/migration.py` & `buildbot-3.8.0/buildbot/test/util/migration.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/misc.py` & `buildbot-3.8.0/buildbot/test/util/misc.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/patch_delay.py` & `buildbot-3.8.0/buildbot/test/util/patch_delay.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/pbmanager.py` & `buildbot-3.8.0/buildbot/test/util/pbmanager.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/properties.py` & `buildbot-3.8.0/buildbot/test/util/properties.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/protocols.py` & `buildbot-3.8.0/buildbot/test/util/protocols.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/querylog.py` & `buildbot-3.8.0/buildbot/test/util/querylog.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/reporter.py` & `buildbot-3.8.0/buildbot/test/util/reporter.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/sandboxed_worker.py` & `buildbot-3.8.0/buildbot/test/util/sandboxed_worker.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/scheduler.py` & `buildbot-3.8.0/buildbot/test/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/sourcesteps.py` & `buildbot-3.8.0/buildbot/test/util/sourcesteps.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/tuplematching.py` & `buildbot-3.8.0/buildbot/test/util/tuplematching.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/validation.py` & `buildbot-3.8.0/buildbot/test/util/validation.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/warnings.py` & `buildbot-3.8.0/buildbot/test/util/warnings.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/test/util/www.py` & `buildbot-3.8.0/buildbot/test/util/www.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/__init__.py` & `buildbot-3.8.0/buildbot/util/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,18 @@
     d = defer.Deferred()
     reactor.callLater(delay, d.callback, None)
     return d
 
 
 def check_functional_environment(config):
     try:
-        locale.getdefaultlocale()
+        if sys.version_info >= (3, 11, 0):
+            locale.getencoding()
+        else:
+            locale.getdefaultlocale()
     except (KeyError, ValueError) as e:
         config.error("\n".join([
             "Your environment has incorrect locale settings. This means python cannot handle "
             "strings safely.",
             " Please check 'LANG', 'LC_CTYPE', 'LC_ALL' and 'LANGUAGE'"
             " are either unset or set to a valid locale.", str(e)
         ]))
```

### Comparing `buildbot-3.7.0/buildbot/util/_notifier.py` & `buildbot-3.8.0/buildbot/util/_notifier.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/async_sort.py` & `buildbot-3.8.0/buildbot/util/async_sort.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/backoff.py` & `buildbot-3.8.0/buildbot/util/backoff.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/bbcollections.py` & `buildbot-3.8.0/buildbot/util/bbcollections.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/codebase.py` & `buildbot-3.8.0/buildbot/util/codebase.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/config.py` & `buildbot-3.8.0/buildbot/util/config.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/croniter.py` & `buildbot-3.8.0/buildbot/util/croniter.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/debounce.py` & `buildbot-3.8.0/buildbot/util/debounce.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/deferwaiter.py` & `buildbot-3.8.0/buildbot/util/deferwaiter.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/eventual.py` & `buildbot-3.8.0/buildbot/util/eventual.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/git.py` & `buildbot-3.8.0/buildbot/util/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,27 @@
 
 
 def getSshKnownHostsContents(hostKey):
     host_name = '*'
     return f'{host_name} {hostKey}'
 
 
+def ensureSshKeyNewline(privateKey: str) -> str:
+    """Ensure key has trailing newline
+
+    Providers can be configured to strip newlines from secrets. This feature
+    breaks SSH key use within the Git module. This helper function ensures that
+    when an ssh key is provided for a git step that is contains the trailing
+    newline.
+    """
+    if privateKey.endswith("\n") or privateKey.endswith("\r") or privateKey.endswith("\r\n"):
+        return privateKey
+    return privateKey + "\n"
+
+
 class GitStepMixin(GitMixin):
 
     def setupGitStep(self):
         self.didDownloadSshPrivateKey = False
         self.setupGit(logname='Git')
 
         if not self.repourl:
@@ -274,14 +287,15 @@
         # options
         workdir = self._getSshDataWorkDir()
 
         ssh_data_path = self._getSshDataPath()
         yield self.runMkdir(ssh_data_path)
 
         private_key_path = self._getSshPrivateKeyPath(ssh_data_path)
+        private_key = ensureSshKeyNewline(private_key)
         yield self.downloadFileContentToWorker(private_key_path,
                                                private_key,
                                                workdir=workdir, mode=0o400)
 
         known_hosts_path = None
         if self.sshHostKey is not None or self.sshKnownHosts is not None:
             known_hosts_path = self._getSshHostKeyPath(ssh_data_path)
```

### Comparing `buildbot-3.7.0/buildbot/util/giturlparse.py` & `buildbot-3.8.0/buildbot/util/giturlparse.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/httpclientservice.py` & `buildbot-3.8.0/buildbot/util/httpclientservice.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/identifiers.py` & `buildbot-3.8.0/buildbot/util/identifiers.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/kubeclientservice.py` & `buildbot-3.8.0/buildbot/util/kubeclientservice.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/latent.py` & `buildbot-3.8.0/buildbot/util/latent.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/lineboundaries.py` & `buildbot-3.8.0/buildbot/util/lineboundaries.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/lru.py` & `buildbot-3.8.0/buildbot/util/lru.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/maildir.py` & `buildbot-3.8.0/buildbot/util/maildir.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/misc.py` & `buildbot-3.8.0/buildbot/util/misc.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/netstrings.py` & `buildbot-3.8.0/buildbot/util/netstrings.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/path_expand_user.py` & `buildbot-3.8.0/buildbot/util/path_expand_user.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/pathmatch.py` & `buildbot-3.8.0/buildbot/util/pathmatch.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/poll.py` & `buildbot-3.8.0/buildbot/util/poll.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/private_tempdir.py` & `buildbot-3.8.0/buildbot/util/private_tempdir.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/protocol.py` & `buildbot-3.8.0/buildbot/util/protocol.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/pullrequest.py` & `buildbot-3.8.0/buildbot/util/pullrequest.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/queue.py` & `buildbot-3.8.0/buildbot/util/queue.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/raml.py` & `buildbot-3.8.0/buildbot/util/raml.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/runprocess.py` & `buildbot-3.8.0/buildbot/util/runprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -255,23 +255,34 @@
 
     def send_signal(self, interrupt_signal):
         success = False
 
         log.msg(f'{self}: killing process using {interrupt_signal}')
 
         if runtime.platformType == "win32":
-            if interrupt_signal is not None and self.process.pid is not None:
-                if interrupt_signal == "TERM":
-                    # TODO: blocks
-                    subprocess.check_call(f"TASKKILL /PID {self.process.pid} /T")
-                    success = True
-                elif interrupt_signal == "KILL":
-                    # TODO: blocks
-                    subprocess.check_call(f"TASKKILL /F /PID {self.process.pid} /T")
-                    success = True
+            pid = self.process.pid
+            if interrupt_signal is not None and pid is not None:
+                try:
+                    if interrupt_signal == "TERM":
+                        # TODO: blocks
+                        subprocess.check_call(f"TASKKILL /PID {pid} /T")
+                        success = True
+                    elif interrupt_signal == "KILL":
+                        # TODO: blocks
+                        subprocess.check_call(f"TASKKILL /F /PID {pid} /T")
+                        success = True
+                except subprocess.CalledProcessError as e:
+                    # taskkill may return 128 or 255 as exit code when the child has already exited.
+                    # We can't handle this race condition in any other way than just interpreting
+                    # the kill action as successful
+                    if e.returncode in (128, 255):
+                        log.msg(f"{self} taskkill didn't find pid {pid} to kill")
+                        success = True
+                    else:
+                        raise
 
         # try signalling the process itself (works on Windows too, sorta)
         if not success:
             try:
                 self.process.signalProcess(interrupt_signal)
                 success = True
             except OSError as e:
```

### Comparing `buildbot-3.7.0/buildbot/util/sautils.py` & `buildbot-3.8.0/buildbot/util/sautils.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/service.py` & `buildbot-3.8.0/buildbot/util/service.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/ssfilter.py` & `buildbot-3.8.0/buildbot/util/ssfilter.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/ssl.py` & `buildbot-3.8.0/buildbot/util/ssl.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/state.py` & `buildbot-3.8.0/buildbot/util/state.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/subscription.py` & `buildbot-3.8.0/buildbot/util/subscription.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/test_result_submitter.py` & `buildbot-3.8.0/buildbot/util/test_result_submitter.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/util/tuplematch.py` & `buildbot-3.8.0/buildbot/util/tuplematch.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/wamp/connector.py` & `buildbot-3.8.0/buildbot/wamp/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """
     concatenation of all the wamp services of buildbot
     """
 
     def __init__(self, config):
         # Cannot use super() here.
         # We must explicitly call both parent constructors.
-        ApplicationSession.__init__(self)
+        ApplicationSession.__init__(self, config)
         service.AsyncMultiService.__init__(self)
         self.leaving = False
         self.setServiceParent(config.extra['parent'])
 
     @defer.inlineCallbacks
     def onJoin(self, details):
         log.msg("Wamp connection succeed!")
```

### Comparing `buildbot-3.7.0/buildbot/warnings.py` & `buildbot-3.8.0/buildbot/warnings.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/worker/__init__.py` & `buildbot-3.8.0/buildbot/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/worker/base.py` & `buildbot-3.8.0/buildbot/worker/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/worker/docker.py` & `buildbot-3.8.0/buildbot/worker/docker.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/worker/ec2.py` & `buildbot-3.8.0/buildbot/worker/ec2.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/worker/kubernetes.py` & `buildbot-3.8.0/buildbot/worker/kubernetes.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/worker/latent.py` & `buildbot-3.8.0/buildbot/worker/latent.py`

 * *Files 6% similar despite different names*

```diff
@@ -159,24 +159,28 @@
     '''
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._substantiation_notifier = Notifier()
         self._start_stop_lock = defer.DeferredLock()
         self._deferwaiter = deferwaiter.DeferWaiter()
+        self._check_instance_timer = None
 
     def checkConfig(self, name, password,
                     build_wait_timeout=60 * 10,
+                    check_instance_interval=10,
                     **kwargs):
         super().checkConfig(name, password, **kwargs)
 
     def reconfigService(self, name, password,
                         build_wait_timeout=60 * 10,
+                        check_instance_interval=10,
                         **kwargs):
         self.build_wait_timeout = build_wait_timeout
+        self.check_instance_interval = check_instance_interval
         return super().reconfigService(name, password, **kwargs)
 
     def _generate_random_password(self):
         return ''.join(random.choice(string.ascii_letters + string.digits) for _ in range(20))
 
     def getRandomPass(self):
         """
@@ -220,14 +224,17 @@
         # should use an errback.
         raise NotImplementedError
 
     def stop_instance(self, fast=False):
         # responsible for shutting down instance.
         raise NotImplementedError
 
+    def check_instance(self):
+        return True
+
     @property
     def substantiated(self):
         return self.state == States.SUBSTANTIATED and self.conn is not None
 
     def substantiate(self, wfb, build):
         log.msg(f"substantiating worker {wfb}")
 
@@ -298,14 +305,16 @@
 
             if dont_wait_to_attach and \
                     self.state == States.SUBSTANTIATING_STARTING and \
                     self.conn is not None:
                 log.msg(f"Worker {self.name} substantiated (already attached)")
                 self.state = States.SUBSTANTIATED
                 self._fireSubstantiationNotifier(True)
+            else:
+                self._start_check_instance_timer()
 
         except Exception as e:
             self.stopMissingTimer()
             self._substantiation_failed(failure.Failure(e))
             # swallow the failure as it is notified
 
     def _fireSubstantiationNotifier(self, result):
@@ -316,14 +325,16 @@
         result_msg = 'success' if result is True else 'failure'
         log.msg(f"Firing {self.name} substantiation deferred with {result_msg}")
 
         self._substantiation_notifier.notify(result)
 
     @defer.inlineCallbacks
     def attached(self, conn):
+        self._stop_check_instance_timer()
+
         if self.state != States.SUBSTANTIATING_STARTING and \
                 self.build_wait_timeout >= 0:
             msg = (f'Worker {self.name} received connection while not trying to substantiate.'
                    'Disconnecting.')
             log.msg(msg)
             self._deferwaiter.add(self._disconnect(conn))
             raise RuntimeError(msg)
@@ -416,14 +427,59 @@
     def _setBuildWaitTimer(self):
         self._clearBuildWaitTimer()
         if self.build_wait_timeout <= 0:
             return
         self.build_wait_timer = self.master.reactor.callLater(
             self.build_wait_timeout, self._soft_disconnect)
 
+    def _stop_check_instance_timer(self):
+        if self._check_instance_timer is not None:
+            if self._check_instance_timer.active():
+                self._check_instance_timer.cancel()
+            self._check_instance_timer = None
+
+    def _start_check_instance_timer(self):
+        self._stop_check_instance_timer()
+        self._check_instance_timer = self.master.reactor.callLater(
+            self.check_instance_interval, self._check_instance_timer_fired
+        )
+
+    def _check_instance_timer_fired(self):
+        self._deferwaiter.add(self._check_instance_timer_fired_impl())
+
+    @defer.inlineCallbacks
+    def _check_instance_timer_fired_impl(self):
+        self._check_instance_timer = None
+        if self.state != States.SUBSTANTIATING_STARTING:
+            # The only case when we want to recheck whether the instance has not failed is
+            # between call to start_instance() and successful attachment of the worker.
+            return
+
+        if self._start_stop_lock.locked:  # pragma: no cover
+            # This can't actually happen, because we start the timer for instance checking after
+            # start_instance() completed and in insubstantiation the state is changed from
+            # SUBSTANTIATING_STARTING as soon as the lock is acquired.
+            return
+
+        try:
+            yield self._start_stop_lock.acquire()
+            is_good = yield self.check_instance()
+            if not is_good:
+                yield self._substantiation_failed(
+                    LatentWorkerFailedToSubstantiate(
+                        self.name, 'latent worker crashed before connecting'
+                    )
+                )
+                return
+        finally:
+            self._start_stop_lock.release()
+
+        # if check passes, schedule another one until worker connects
+        self._start_check_instance_timer()
+
     @defer.inlineCallbacks
     def insubstantiate(self, fast=False, force_substantiation_build=None):
         # If force_substantiation_build is not None, we'll try to substantiate the given build
         # after insubstantiation concludes. This parameter allows to go directly to the
         # SUBSTANTIATING state without going through NOT_SUBSTANTIATED state.
 
         log.msg(f"insubstantiating worker {self}")
@@ -455,14 +511,15 @@
                 self.state = States.INSUBSTANTIATING
 
             if prev_state in [States.SUBSTANTIATING, States.SUBSTANTIATING_STARTING]:
                 self._fireSubstantiationNotifier(
                     failure.Failure(LatentWorkerSubstantiatiationCancelled()))
 
             self._clearBuildWaitTimer()
+            self._stop_check_instance_timer()
 
             if prev_state in [States.SUBSTANTIATING_STARTING, States.SUBSTANTIATED]:
                 try:
                     yield self.stop_instance(fast)
                 except Exception as e:
                     # The case of failure for insubstantiation is bad as we have a
                     # left-over costing resource There is not much thing to do here
@@ -529,14 +586,15 @@
 
         # prevent any race conditions with any future builds that are in the process of
         # being started.
         if self.state == States.NOT_SUBSTANTIATED:
             self.state = States.SHUT_DOWN
 
         self._clearBuildWaitTimer()
+        self._stop_check_instance_timer()
         res = yield super().stopService()
         return res
 
     def updateWorker(self):
         """Called to add or remove builders after the worker has connected.
 
         Also called after botmaster's builders are initially set.
```

### Comparing `buildbot-3.7.0/buildbot/worker/libvirt.py` & `buildbot-3.8.0/buildbot/worker/libvirt.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,18 @@
         I am a private method for creating (possibly cheap) copies of a
         base_image for start_instance to boot.
         """
         if not self.base_image:
             return
 
         if self.cheap_copy:
-            clone_cmd = ['qemu-img', 'create', '-b', self.base_image, '-f', 'qcow2', self.image]
+            clone_cmd = ['qemu-img', 'create',
+                         '-o', 'backing_fmt=qcow2',
+                         '-b', self.base_image,
+                         '-f', 'qcow2', self.image]
         else:
             clone_cmd = ['cp', self.base_image, self.image]
 
         log.msg(f"Cloning base image: {clone_cmd}'")
 
         try:
             rc = yield runprocess.run_process(self.master.reactor, clone_cmd, collect_stdout=False,
```

### Comparing `buildbot-3.7.0/buildbot/worker/local.py` & `buildbot-3.8.0/buildbot/worker/local.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/worker/manager.py` & `buildbot-3.8.0/buildbot/worker/manager.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/worker/marathon.py` & `buildbot-3.8.0/buildbot/worker/marathon.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/worker/openstack.py` & `buildbot-3.8.0/buildbot/worker/openstack.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/worker/protocols/base.py` & `buildbot-3.8.0/buildbot/worker/protocols/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/worker/protocols/manager/base.py` & `buildbot-3.8.0/buildbot/worker/protocols/manager/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/worker/protocols/manager/msgpack.py` & `buildbot-3.8.0/buildbot/worker/protocols/manager/msgpack.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/worker/protocols/manager/pb.py` & `buildbot-3.8.0/buildbot/worker/protocols/manager/pb.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/worker/protocols/msgpack.py` & `buildbot-3.8.0/buildbot/worker/protocols/msgpack.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,17 @@
             args['path'] = self.path_module.join(self.builder_basedirs[builderName], args['path'])
 
         if commandName == "listdir":
             args['path'] = self.path_module.join(self.builder_basedirs[builderName], args['dir'])
             del args['dir']
 
         if commandName == "rmfile":
-            args['path'] = self.path_module.join(self.builder_basedirs[builderName], args['path'])
+            args['path'] = self.path_module.join(self.builder_basedirs[builderName],
+                                                 self.path_expanduser(args['path'],
+                                                                      self.info['environ']))
 
         if commandName == "shell":
             args['workdir'] = self.path_module.join(self.builder_basedirs[builderName],
                                                     args['workdir'])
 
         if commandName == "uploadFile":
             commandName = "upload_file"
```

### Comparing `buildbot-3.7.0/buildbot/worker/protocols/null.py` & `buildbot-3.8.0/buildbot/worker/protocols/null.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/worker/protocols/pb.py` & `buildbot-3.8.0/buildbot/worker/protocols/pb.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/worker/upcloud.py` & `buildbot-3.8.0/buildbot/worker/upcloud.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/auth.py` & `buildbot-3.8.0/buildbot/www/auth.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/authz/authz.py` & `buildbot-3.8.0/buildbot/www/authz/authz.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/authz/endpointmatchers.py` & `buildbot-3.8.0/buildbot/www/authz/endpointmatchers.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/authz/roles.py` & `buildbot-3.8.0/buildbot/www/authz/roles.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/avatar.py` & `buildbot-3.8.0/buildbot/www/avatar.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/change_hook.py` & `buildbot-3.8.0/buildbot/www/change_hook.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/config.py` & `buildbot-3.8.0/buildbot/www/config.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/graphql.py` & `buildbot-3.8.0/buildbot/www/graphql.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/hooks/base.py` & `buildbot-3.8.0/buildbot/www/hooks/base.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/hooks/bitbucket.py` & `buildbot-3.8.0/buildbot/www/hooks/bitbucket.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/hooks/bitbucketcloud.py` & `buildbot-3.8.0/buildbot/www/hooks/bitbucketcloud.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/hooks/bitbucketserver.py` & `buildbot-3.8.0/buildbot/www/hooks/bitbucketserver.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/hooks/github.py` & `buildbot-3.8.0/buildbot/www/hooks/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,15 +272,23 @@
             headers=headers,
             debug=self.debug,
             verify=self.verify,
         )
         res = yield http.get(url)
         if 200 <= res.code < 300:
             data = yield res.json()
-            return [f["filename"] for f in data]
+            filenames = []
+            for f in data:
+                filenames.append(f["filename"])
+                # If a file was moved this tell us where it was moved from.
+                previous_filename = f.get("previous_filename")
+                if previous_filename is not None:
+                    filenames.append(previous_filename)
+
+            return filenames
 
         log.msg(f'Failed fetching PR files: response code {res.code}')
         return []
 
     def _process_change(self, payload, user, repo, repo_url, project, event,
                         properties):
         """
```

### Comparing `buildbot-3.7.0/buildbot/www/hooks/gitlab.py` & `buildbot-3.8.0/buildbot/www/hooks/gitlab.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/hooks/gitorious.py` & `buildbot-3.8.0/buildbot/www/hooks/gitorious.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/hooks/poller.py` & `buildbot-3.8.0/buildbot/www/hooks/poller.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/ldapuserinfo.py` & `buildbot-3.8.0/buildbot/www/ldapuserinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,16 @@
                  accountFullName,
                  accountEmail,
                  groupBase=None,
                  groupMemberPattern=None,
                  groupName=None,
                  avatarPattern=None,
                  avatarData=None,
-                 accountExtraFields=None):
+                 accountExtraFields=None,
+                 tls=None):
         # Throw import error now that this is being used
         if not ldap3:
             importlib.import_module('ldap3')
         self.uri = uri
         self.bindUser = bindUser
         self.bindPw = bindPw
         self.accountBase = accountBase
@@ -77,21 +78,22 @@
         self.groupBase = groupBase
         self.avatarPattern = avatarPattern
         self.avatarData = avatarData
         if accountExtraFields is None:
             accountExtraFields = []
         self.accountExtraFields = accountExtraFields
         self.ldap_encoding = ldap3.get_config_parameter('DEFAULT_SERVER_ENCODING')
+        self.tls = tls
 
     def connectLdap(self):
         server = urlparse(self.uri)
         netloc = server.netloc.split(":")
         # define the server and the connection
         s = ldap3.Server(netloc[0], port=int(netloc[1]), use_ssl=server.scheme == 'ldaps',
-                         get_info=ldap3.ALL)
+                         get_info=ldap3.ALL, tls=self.tls)
 
         auth = ldap3.SIMPLE
         if self.bindUser is None and self.bindPw is None:
             auth = ldap3.ANONYMOUS
 
         c = ldap3.Connection(s, auto_bind=True, client_strategy=ldap3.SYNC,
                              user=self.bindUser, password=self.bindPw,
```

### Comparing `buildbot-3.7.0/buildbot/www/oauth2.py` & `buildbot-3.8.0/buildbot/www/oauth2.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/plugin.py` & `buildbot-3.8.0/buildbot/www/plugin.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/resource.py` & `buildbot-3.8.0/buildbot/www/resource.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/rest.py` & `buildbot-3.8.0/buildbot/www/rest.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/service.py` & `buildbot-3.8.0/buildbot/www/service.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/sse.py` & `buildbot-3.8.0/buildbot/www/sse.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/buildbot/www/ws.py` & `buildbot-3.8.0/buildbot/www/ws.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/Makefile` & `buildbot-3.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/Makefile` & `buildbot-3.8.0/docs/_images/Makefile`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/auth_rules.png` & `buildbot-3.8.0/docs/_images/auth_rules.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/auth_rules.svg` & `buildbot-3.8.0/docs/_images/auth_rules.svg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/auth_rules_src.svg` & `buildbot-3.8.0/docs/_images/auth_rules_src.svg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/badges-badgeio.png` & `buildbot-3.8.0/docs/_images/badges-badgeio.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/bitbucket-status-push.png` & `buildbot-3.8.0/docs/_images/bitbucket-status-push.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/changes.png` & `buildbot-3.8.0/docs/_images/changes.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/changes.svg` & `buildbot-3.8.0/docs/_images/changes.svg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/changes_src.svg` & `buildbot-3.8.0/docs/_images/changes_src.svg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/forcedialog1.png` & `buildbot-3.8.0/docs/_images/forcedialog1.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/full_logo.png` & `buildbot-3.8.0/docs/_images/full_logo.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/full_logo.svg` & `buildbot-3.8.0/docs/_images/full_logo.svg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/header-text-transparent.png` & `buildbot-3.8.0/docs/_images/header-text-transparent.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/icon.blend` & `buildbot-3.8.0/docs/_images/icon.blend`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/js-data-module-mvvm.svg` & `buildbot-3.8.0/docs/_images/js-data-module-mvvm.svg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/js-data-module-wrappers.svg` & `buildbot-3.8.0/docs/_images/js-data-module-wrappers.svg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/master.png` & `buildbot-3.8.0/docs/_images/master.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/master.svg` & `buildbot-3.8.0/docs/_images/master.svg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/master_src.svg` & `buildbot-3.8.0/docs/_images/master_src.svg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/multimaster.png` & `buildbot-3.8.0/docs/_images/multimaster.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/multimaster.svg` & `buildbot-3.8.0/docs/_images/multimaster.svg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/multimaster_src.svg` & `buildbot-3.8.0/docs/_images/multimaster_src.svg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/overview.png` & `buildbot-3.8.0/docs/_images/overview.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/overview.svg` & `buildbot-3.8.0/docs/_images/overview.svg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/overview_src.svg` & `buildbot-3.8.0/docs/_images/overview_src.svg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/success_normal.png` & `buildbot-3.8.0/docs/_images/success_normal.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/vault_multipart_key.png` & `buildbot-3.8.0/docs/_images/vault_multipart_key.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/vault_simple_key.png` & `buildbot-3.8.0/docs/_images/vault_simple_key.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/workers.png` & `buildbot-3.8.0/docs/_images/workers.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/workers.svg` & `buildbot-3.8.0/docs/_images/workers.svg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_images/workers_src.svg` & `buildbot-3.8.0/docs/_images/workers_src.svg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_static/buildbot_rtd.css` & `buildbot-3.8.0/docs/_static/buildbot_rtd.css`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_static/icon.png` & `buildbot-3.8.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/_static/icon.svg` & `buildbot-3.8.0/docs/_static/icon.svg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/bbdocs/api_index.py` & `buildbot-3.8.0/docs/bbdocs/api_index.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/bbdocs/ext.py` & `buildbot-3.8.0/docs/bbdocs/ext.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/buildbot.1` & `buildbot-3.8.0/docs/buildbot.1`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/conf.py` & `buildbot-3.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/_images/stats-service.png` & `buildbot-3.8.0/docs/developer/_images/stats-service.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/auth.rst` & `buildbot-3.8.0/docs/developer/auth.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/authz.rst` & `buildbot-3.8.0/docs/developer/authz.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/br-claiming.rst` & `buildbot-3.8.0/docs/developer/br-claiming.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/classes.rst` & `buildbot-3.8.0/docs/developer/classes.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-auth.rst` & `buildbot-3.8.0/docs/developer/cls-auth.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-avatar.rst` & `buildbot-3.8.0/docs/developer/cls-avatar.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-basescheduler.rst` & `buildbot-3.8.0/docs/developer/cls-basescheduler.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-build.rst` & `buildbot-3.8.0/docs/developer/cls-build.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-buildfactory.rst` & `buildbot-3.8.0/docs/developer/cls-buildfactory.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-buildsteps.rst` & `buildbot-3.8.0/docs/developer/cls-buildsteps.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-changesources.rst` & `buildbot-3.8.0/docs/developer/cls-changesources.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-forcesched.rst` & `buildbot-3.8.0/docs/developer/cls-forcesched.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-iconfigurator.rst` & `buildbot-3.8.0/docs/developer/cls-iconfigurator.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-iproperties.rst` & `buildbot-3.8.0/docs/developer/cls-iproperties.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-log.rst` & `buildbot-3.8.0/docs/developer/cls-log.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-logobserver.rst` & `buildbot-3.8.0/docs/developer/cls-logobserver.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-protocols.rst` & `buildbot-3.8.0/docs/developer/cls-protocols.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-remotecommands.rst` & `buildbot-3.8.0/docs/developer/cls-remotecommands.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-resultspec.rst` & `buildbot-3.8.0/docs/developer/cls-resultspec.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-workermanager.rst` & `buildbot-3.8.0/docs/developer/cls-workermanager.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/cls-www.rst` & `buildbot-3.8.0/docs/developer/cls-www.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/config.rst` & `buildbot-3.8.0/docs/developer/config.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/data.rst` & `buildbot-3.8.0/docs/developer/data.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/database.rst` & `buildbot-3.8.0/docs/developer/database.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/encodings.rst` & `buildbot-3.8.0/docs/developer/encodings.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/index.rst` & `buildbot-3.8.0/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/master-overview.rst` & `buildbot-3.8.0/docs/developer/master-overview.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/master-worker-msgpack.rst` & `buildbot-3.8.0/docs/developer/master-worker-msgpack.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/master-worker.rst` & `buildbot-3.8.0/docs/developer/master-worker.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/metrics.rst` & `buildbot-3.8.0/docs/developer/metrics.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/mq.rst` & `buildbot-3.8.0/docs/developer/mq.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/plugins-publish.rst` & `buildbot-3.8.0/docs/developer/plugins-publish.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/pull-request.rst` & `buildbot-3.8.0/docs/developer/pull-request.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/quickstart.rst` & `buildbot-3.8.0/docs/developer/quickstart.rst`

 * *Files 1% similar despite different names*

```diff
@@ -69,29 +69,29 @@
 You will also need ``NodeJS``, and ``yarn`` installed.
 
 Prerequisites
 ~~~~~~~~~~~~~
 
 .. note::
 
-  Buildbot UI requires at least node 4 or newer and yarn.
+  Buildbot UI requires at least node 14.18 or newer and yarn.
 
 * Install LTS release of node.js.
 
   http://nodejs.org/ is a good start for Windows and OSX.
 
   For modern Linux distributions, you can often just install the distribution-provided node version if it's recent enough.
   You can use yarn from the same source.
-  The below method has been tested on Ubuntu 18.04 and should work on recent enough Debian.
+  The below method has been tested on Debian Bookworm.
 
   .. code-block:: none
 
     sudo apt install nodejs yarn
 
-  In other cases, use https://deb.nodesource.com.
+  In other cases, use https://deb.nodesource.com and https://classic.yarnpkg.com/lang/en/docs/install.
 
 .. _JSDevQuickStart:
 
 Hacking the Buildbot JavaScript
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 To effectively develop Buildbot JavaScript, you'll need a running Buildmaster configured to operate out of the source directory.
```

### Comparing `buildbot-3.7.0/docs/developer/rest.rst` & `buildbot-3.8.0/docs/developer/rest.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/results.rst` & `buildbot-3.8.0/docs/developer/results.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/schedulers.rst` & `buildbot-3.8.0/docs/developer/schedulers.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/secrets.rst` & `buildbot-3.8.0/docs/developer/secrets.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/stats-service.rst` & `buildbot-3.8.0/docs/developer/stats-service.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/style.rst` & `buildbot-3.8.0/docs/developer/style.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/tests.rst` & `buildbot-3.8.0/docs/developer/tests.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/utils.rst` & `buildbot-3.8.0/docs/developer/utils.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/www-base-app.rst` & `buildbot-3.8.0/docs/developer/www-base-app.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/www-data-module.rst` & `buildbot-3.8.0/docs/developer/www-data-module.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/developer/www-server.rst` & `buildbot-3.8.0/docs/developer/www-server.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/examples/git_gerrit.cfg` & `buildbot-3.8.0/docs/examples/git_gerrit.cfg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/examples/gitlab.cfg` & `buildbot-3.8.0/docs/examples/gitlab.cfg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/examples/hello.cfg` & `buildbot-3.8.0/docs/examples/hello.cfg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/examples/repo_gerrit.cfg` & `buildbot-3.8.0/docs/examples/repo_gerrit.cfg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/examples/twisted_master.cfg` & `buildbot-3.8.0/docs/examples/twisted_master.cfg`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/index.rst` & `buildbot-3.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/manual/cmdline.rst` & `buildbot-3.8.0/docs/manual/cmdline.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/manual/concepts.rst` & `buildbot-3.8.0/docs/manual/concepts.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/manual/customization.rst` & `buildbot-3.8.0/docs/manual/customization.rst`

 * *Files 0% similar despite different names*

```diff
@@ -634,14 +634,21 @@
         This method determines whether a started instance is compatible with the build that is about to be started.
         ``build_props`` is the properties of the build that are known before the build has been started.
         A build may be incompatible with already started instance if, for example, it requests a different amount of memory or a different Docker image.
         A deferred should be returned, whose callback should return ``True`` if build is compatible and ``False`` otherwise.
         The method may be called when the instance is not yet started and should indicate compatible build in that case.
         In the default implementation the callback returns ``True``.
 
+    .. py:method:: check_instance(self)
+
+        This method determines the health of an instance.
+        The method should return ``False`` if it determines that a serious error has occurred and worker will not connect to the master.
+        Otherwise, the method should return ``True``.
+
+
 Custom Build Classes
 --------------------
 
 The standard :class:`BuildFactory` object creates :class:`Build` objects by default.
 These Builds will each execute a collection of :class:`BuildStep`\s in a fixed sequence.
 Each step can affect the results of the build, but in general there is little intelligence to tie the different steps together.
```

### Comparing `buildbot-3.7.0/docs/manual/deploy.rst` & `buildbot-3.8.0/docs/manual/deploy.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/manual/installation/buildmaster.rst` & `buildbot-3.8.0/docs/manual/installation/buildmaster.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/manual/installation/components.rst` & `buildbot-3.8.0/docs/manual/installation/components.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/manual/installation/installation.rst` & `buildbot-3.8.0/docs/manual/installation/installation.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/manual/installation/misc.rst` & `buildbot-3.8.0/docs/manual/installation/misc.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/manual/installation/requirements.rst` & `buildbot-3.8.0/docs/manual/installation/requirements.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/manual/installation/worker.rst` & `buildbot-3.8.0/docs/manual/installation/worker.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/manual/introduction.rst` & `buildbot-3.8.0/docs/manual/introduction.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/manual/optimization.rst` & `buildbot-3.8.0/docs/manual/optimization.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/manual/plugins.rst` & `buildbot-3.8.0/docs/manual/plugins.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/manual/secretsmanagement.rst` & `buildbot-3.8.0/docs/manual/secretsmanagement.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.3.2.txt` & `buildbot-3.8.0/docs/relnotes/0.3.2.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.3.3.txt` & `buildbot-3.8.0/docs/relnotes/0.3.3.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.3.4.txt` & `buildbot-3.8.0/docs/relnotes/0.3.4.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.3.5.txt` & `buildbot-3.8.0/docs/relnotes/0.3.5.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.4.0.txt` & `buildbot-3.8.0/docs/relnotes/0.4.0.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.4.1.txt` & `buildbot-3.8.0/docs/relnotes/0.4.1.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.4.2.txt` & `buildbot-3.8.0/docs/relnotes/0.4.2.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.4.3.txt` & `buildbot-3.8.0/docs/relnotes/0.4.3.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.5.0.txt` & `buildbot-3.8.0/docs/relnotes/0.5.0.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.6.0.txt` & `buildbot-3.8.0/docs/relnotes/0.6.0.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.6.1.txt` & `buildbot-3.8.0/docs/relnotes/0.6.1.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.6.2.txt` & `buildbot-3.8.0/docs/relnotes/0.6.2.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.6.3.txt` & `buildbot-3.8.0/docs/relnotes/0.6.3.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.6.4.txt` & `buildbot-3.8.0/docs/relnotes/0.6.4.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.6.5.txt` & `buildbot-3.8.0/docs/relnotes/0.6.5.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.6.6.txt` & `buildbot-3.8.0/docs/relnotes/0.6.6.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.7.0.txt` & `buildbot-3.8.0/docs/relnotes/0.7.0.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.7.1.txt` & `buildbot-3.8.0/docs/relnotes/0.7.1.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.7.10.txt` & `buildbot-3.8.0/docs/relnotes/0.7.10.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.7.11.txt` & `buildbot-3.8.0/docs/relnotes/0.7.11.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.7.12.txt` & `buildbot-3.8.0/docs/relnotes/0.7.12.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.7.2.txt` & `buildbot-3.8.0/docs/relnotes/0.7.2.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.7.3.txt` & `buildbot-3.8.0/docs/relnotes/0.7.3.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.7.4.txt` & `buildbot-3.8.0/docs/relnotes/0.7.4.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.7.5.txt` & `buildbot-3.8.0/docs/relnotes/0.7.5.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.7.6.txt` & `buildbot-3.8.0/docs/relnotes/0.7.6.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.7.7.txt` & `buildbot-3.8.0/docs/relnotes/0.7.7.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.7.8.txt` & `buildbot-3.8.0/docs/relnotes/0.7.8.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.7.9.txt` & `buildbot-3.8.0/docs/relnotes/0.7.9.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.8.0.txt` & `buildbot-3.8.0/docs/relnotes/0.8.0.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.8.1.txt` & `buildbot-3.8.0/docs/relnotes/0.8.1.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.8.10.rst` & `buildbot-3.8.0/docs/relnotes/0.8.10.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.8.12.rst` & `buildbot-3.8.0/docs/relnotes/0.8.12.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.8.2.txt` & `buildbot-3.8.0/docs/relnotes/0.8.2.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.8.3.txt` & `buildbot-3.8.0/docs/relnotes/0.8.3.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.8.4.txt` & `buildbot-3.8.0/docs/relnotes/0.8.4.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.8.5.txt` & `buildbot-3.8.0/docs/relnotes/0.8.5.txt`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.8.6.rst` & `buildbot-3.8.0/docs/relnotes/0.8.6.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.8.7.rst` & `buildbot-3.8.0/docs/relnotes/0.8.7.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.8.8.rst` & `buildbot-3.8.0/docs/relnotes/0.8.8.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.8.9.rst` & `buildbot-3.8.0/docs/relnotes/0.8.9.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.9.0.rst` & `buildbot-3.8.0/docs/relnotes/0.9.0.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.9.0b1.rst` & `buildbot-3.8.0/docs/relnotes/0.9.0b1.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.9.0b2.rst` & `buildbot-3.8.0/docs/relnotes/0.9.0b2.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.9.0b3.rst` & `buildbot-3.8.0/docs/relnotes/0.9.0b3.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.9.0b4.rst` & `buildbot-3.8.0/docs/relnotes/0.9.0b4.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.9.0b5.rst` & `buildbot-3.8.0/docs/relnotes/0.9.0b5.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.9.0b6.rst` & `buildbot-3.8.0/docs/relnotes/0.9.0b6.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.9.0b7.rst` & `buildbot-3.8.0/docs/relnotes/0.9.0b7.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.9.0b8.rst` & `buildbot-3.8.0/docs/relnotes/0.9.0b8.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.9.0b9.rst` & `buildbot-3.8.0/docs/relnotes/0.9.0b9.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.9.0rc1.rst` & `buildbot-3.8.0/docs/relnotes/0.9.0rc1.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.9.0rc2.rst` & `buildbot-3.8.0/docs/relnotes/0.9.0rc2.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.9.0rc3.rst` & `buildbot-3.8.0/docs/relnotes/0.9.0rc3.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.9.0rc4.rst` & `buildbot-3.8.0/docs/relnotes/0.9.0rc4.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.9.1.rst` & `buildbot-3.8.0/docs/relnotes/0.9.1.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/0.9.2-0.9.15.rst` & `buildbot-3.8.0/docs/relnotes/0.9.2-0.9.15.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/1.x.rst` & `buildbot-3.8.0/docs/relnotes/1.x.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/2.x.rst` & `buildbot-3.8.0/docs/relnotes/2.x.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/relnotes/index.rst` & `buildbot-3.8.0/docs/relnotes/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,56 @@
     Buildbot uses towncrier to manage its release notes.
     towncrier helps to avoid the need for rebase when several people work at the same time on the release notes files.
 
     Each PR should come with a file in the newsfragment directory
 
 .. towncrier release notes start
 
+Buildbot ``3.8.0`` ( ``2023-04-16`` )
+=====================================
+
+Bug fixes
+---------
+
+- Fixed compatibility issues with Python 3.11.
+- Fixed compatibility with Autobahn v22.4.1 and newer.
+- Fixed issue with overriding `env` when calling `ShellMixin.makeRemoteShellCommand`
+- Buildbot will now include the previous location of moved files when evaluating a Github commit.
+  This fixes an issue where a commit that moves a file out of a folder, would not be shown in the
+  web UI for a builder that is tracking that same folder.
+- Improved reliability of Buildbot log watching to follow log files even after rotation.
+  This improves reliability of Buildbot start and restart scripts.
+- Fixed handling of occasional errors that happen when attempting to kill a master-side process that has already exited.
+- Fixed a race condition in PyLint step that may lead to step throwing exceptions.
+- Fixed compatibility with qemu 6.1 and newer when using LibVirtWorker with ``cheap_copy=True`` (default).
+- Fixed an issue with secrets provider stripping newline from ssh keys sent in git steps.
+- Fixed occasional errors that happen when killing processes on Windows. TASKKILL command may return
+  code 255 when process has already exited.
+- Fixed deleting secrets from worker that contain '~' in their destination path.
+
+Changes
+-------
+
+- Buildbot now requires NodeJS 14.18 or newer to build the frontend.
+- The URLs emitted by the Buildbot APIs have been changed to include slash after the hash (``#``)
+  symbol to be compatible with what React web UI supports.
+
+Improved Documentation
+----------------------
+
+- Replace statement "https is unsupported" with a more detailed disclaimer.
+
+Features
+--------
+
+- Add a way to disable default ``WarningCountingShellCommand`` parser.
+- Added health check API that latent workers can use to specify that a particular worker will not connect and build should not wait for it and mark itself as failure immediately.
+- Implemented a way to customize TLS setting for ``LdapUserInfo``.
+
+
 Buildbot ``3.7.0`` ( ``2022-12-04`` )
 =====================================
 
 Bug fixes
 ---------
 
 - Improved statistics capture to avoid negative build duration.
```

### Comparing `buildbot-3.7.0/docs/tutorial/_images/builders.png` & `buildbot-3.8.0/docs/tutorial/_images/builders.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/tutorial/_images/force-build.png` & `buildbot-3.8.0/docs/tutorial/_images/force-build.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/tutorial/_images/index.png` & `buildbot-3.8.0/docs/tutorial/_images/index.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/tutorial/_images/irc-testrun.png` & `buildbot-3.8.0/docs/tutorial/_images/irc-testrun.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/tutorial/_images/runtests-success.png` & `buildbot-3.8.0/docs/tutorial/_images/runtests-success.png`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/tutorial/docker.rst` & `buildbot-3.8.0/docs/tutorial/docker.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/tutorial/firstrun.rst` & `buildbot-3.8.0/docs/tutorial/firstrun.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/tutorial/fiveminutes.rst` & `buildbot-3.8.0/docs/tutorial/fiveminutes.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/docs/tutorial/tour.rst` & `buildbot-3.8.0/docs/tutorial/tour.rst`

 * *Files identical despite different names*

### Comparing `buildbot-3.7.0/setup.py` & `buildbot-3.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,16 @@
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
         'Topic :: Software Development :: Build Tools',
         'Topic :: Software Development :: Testing',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 
     'packages': [
         "buildbot",
         "buildbot.configurators",
         "buildbot.worker",
         "buildbot.worker.protocols",
```

