# Comparing `tmp/synapse-2.98.0.tar.gz` & `tmp/synapse-2.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synapse-2.98.0.tar", last modified: Fri Jun 17 21:07:39 2022, max compression
+gzip compressed data, was "synapse-2.99.0.tar", last modified: Thu Jun 23 22:53:35 2022, max compression
```

## Comparing `synapse-2.98.0.tar` & `synapse-2.99.0.tar`

### file list

```diff
@@ -1,485 +1,488 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.293636 synapse-2.98.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2022-06-17 21:06:39.000000 synapse-2.98.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      117 2022-06-17 21:06:39.000000 synapse-2.98.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2966 2022-06-17 21:07:39.293636 synapse-2.98.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1771 2022-06-17 21:06:39.000000 synapse-2.98.0/README.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2022-06-17 21:07:39.293636 synapse-2.98.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4789 2022-06-17 21:06:39.000000 synapse-2.98.0/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.205635 synapse-2.98.0/synapse/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1222 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    42912 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/axon.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      308 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/cells.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.209635 synapse-2.98.0/synapse/cmds/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/cmds/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2920 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/cmds/boss.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15812 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/cmds/cortex.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26083 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/cmds/cron.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8362 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/cmds/hive.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10999 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/cmds/trigger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    27505 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/common.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   176823 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/cortex.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9081 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/cryotank.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16632 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/daemon.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.209635 synapse-2.98.0/synapse/data/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      433 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/data/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10558 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/data/iana.tlds.mpk
--rw-r--r--   0 circleci  (3434) circleci  (3434)    28386 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/datamodel.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6846 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/exc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3209 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/glob.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.233635 synapse-2.98.0/synapse/lib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      129 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    33134 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/agenda.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    30488 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/aha.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   114530 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/ast.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12255 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/autodoc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21288 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1585 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/boss.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5904 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/cache.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   104380 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/cell.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35154 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/certdir.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3015 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/chop.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14152 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1053 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/cmd.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2026 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/cmdr.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14369 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1008 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/const.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7719 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/coro.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.233635 synapse-2.98.0/synapse/lib/crypto/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/crypto/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4860 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/crypto/coin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6522 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/crypto/ecc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3875 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/crypto/tinfoil.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      620 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/datfile.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2168 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/dyndeps.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6015 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/encoding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2682 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/gis.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2150 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/grammar.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      658 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/hashitem.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1405 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/hashset.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1730 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/health.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19149 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/hive.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    30759 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/hiveauth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    28773 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/httpapi.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/ingest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1175 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/interval.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19210 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/jsonstor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11686 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/jupyter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   131206 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/layer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9359 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/link.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    52542 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/lmdbslab.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21681 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/modelrev.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4686 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/module.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1038 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/modules.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6476 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/msgpack.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15048 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/multislabseqn.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19699 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/nexus.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    30184 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/node.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      890 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/output.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26158 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/parser.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.233635 synapse-2.98.0/synapse/lib/platforms/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      196 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/platforms/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1097 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/platforms/common.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      150 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/platforms/darwin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      149 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/platforms/freebsd.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6457 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/platforms/linux.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2069 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/platforms/windows.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6536 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/provenance.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3862 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/queue.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1124 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/ratelimit.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2878 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/reflect.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18883 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/rstorm.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4336 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/scope.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14521 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/scrape.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      663 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/share.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/slaboffs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9823 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/slabseqn.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    44145 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/snap.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4564 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/spooled.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14532 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/storm.lark
--rw-r--r--   0 circleci  (3434) circleci  (3434)   165118 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/storm.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4018 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/storm_format.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      285 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormctrl.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21682 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormhttp.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.241635 synapse-2.98.0/synapse/lib/stormlib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3556 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/auth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2425 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/backup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9660 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/cell.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1176 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/ethereum.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1717 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/hex.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11928 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/imap.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10638 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/infosec.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1467 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/ipv6.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5681 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/json.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6425 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/log.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7044 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/macro.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26268 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/model.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7610 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/modelext.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3107 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/notifications.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5063 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/oauth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    34831 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/project.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6546 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/scrape.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6954 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/smtp.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    36246 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/stix.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1682 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/storm.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2302 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3558 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/xml.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1685 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormlib/yaml.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6688 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormsvc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   335916 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormtypes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2275 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/stormwhois.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1303 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/structlog.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5095 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/task.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      840 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/thishost.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      417 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/thisplat.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      164 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/threads.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6614 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/time.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14510 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/trigger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    62521 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/types.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2459 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/urlhelp.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7161 2022-06-17 21:07:12.000000 synapse-2.98.0/synapse/lib/version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    34616 2022-06-17 21:06:39.000000 synapse-2.98.0/synapse/lib/view.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.241635 synapse-2.98.0/synapse/lookup/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/lookup/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5224 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/lookup/iana.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10406 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/lookup/iso3166.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2493 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/lookup/macho.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11071 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/lookup/pe.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16491 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/lookup/phonenum.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/mindmeld.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.245636 synapse-2.98.0/synapse/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2907 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/auth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10251 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11258 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/biz.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24468 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/crypto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13439 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/dns.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12001 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/economic.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26201 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/files.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1540 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/geopol.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15282 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/geospace.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.245636 synapse-2.98.0/synapse/models/gov/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/gov/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      876 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/gov/cn.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1032 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/gov/intl.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1328 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/gov/us.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   124294 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/inet.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    94151 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/infotech.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2640 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/language.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2323 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/material.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2409 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/media.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    48713 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/orgs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21288 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/person.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6573 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/proj.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18217 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/risk.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13692 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/syn.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15107 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/telco.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12238 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/models/transport.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.249636 synapse-2.98.0/synapse/servers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/servers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      180 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/servers/aha.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/servers/axon.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      573 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/servers/cell.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      184 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/servers/cortex.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      192 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/servers/cryotank.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      200 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/servers/jsonstor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1190 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/servers/stemcell.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    41504 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/telepath.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.281636 synapse-2.98.0/synapse/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.281636 synapse-2.98.0/synapse/tests/files/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.197635 synapse-2.98.0/synapse/tests/files/certdir/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.281636 synapse-2.98.0/synapse/tests/files/certdir/cas/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      981 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/certdir/cas/ca.crt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1704 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/certdir/cas/ca.key
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.281636 synapse-2.98.0/synapse/tests/files/certdir/hosts/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1054 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/certdir/hosts/localhost.crt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1708 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/certdir/hosts/localhost.key
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.281636 synapse-2.98.0/synapse/tests/files/certdir/users/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1432 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/certdir/users/root.crt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3272 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/certdir/users/root.key
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1062 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/certdir/users/user.crt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1704 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/certdir/users/user.key
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.281636 synapse-2.98.0/synapse/tests/files/rstorm/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       57 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/rstorm/httpresp1.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/rstorm/httpresp2.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/rstorm/httpresp3.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1486 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/rstorm/httprespmulti.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      910 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/rstorm/testsvc.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.281636 synapse-2.98.0/synapse/tests/files/stix_export/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15655 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stix_export/basic.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6559 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stix_export/custom0.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6068 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stix_export/risk0.json
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.281636 synapse-2.98.0/synapse/tests/files/stormmod/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormmod/common
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.281636 synapse-2.98.0/synapse/tests/files/stormpkg/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.281636 synapse-2.98.0/synapse/tests/files/stormpkg/docs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/docs/foobar.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/docs/foobar.svg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.281636 synapse-2.98.0/synapse/tests/files/stormpkg/dotstorm/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      128 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/dotstorm/dotstorm.yaml
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.201635 synapse-2.98.0/synapse/tests/files/stormpkg/dotstorm/storm/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.285636 synapse-2.98.0/synapse/tests/files/stormpkg/dotstorm/storm/commands/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/dotstorm/storm/commands/dotstorm.bar.storm
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.285636 synapse-2.98.0/synapse/tests/files/stormpkg/dotstorm/storm/modules/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/dotstorm/storm/modules/dotstorm.foo.storm
--rw-r--r--   0 circleci  (3434) circleci  (3434)       57 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/nocontent.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/nomime.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/nopath.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       79 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/nosuchfile.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       63 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/notitle.yaml
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.285636 synapse-2.98.0/synapse/tests/files/stormpkg/optic/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        3 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/optic/index.html
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.201635 synapse-2.98.0/synapse/tests/files/stormpkg/storm/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.285636 synapse-2.98.0/synapse/tests/files/stormpkg/storm/commands/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/storm/commands/testpkg.baz
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/storm/commands/testpkgcmd
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.285636 synapse-2.98.0/synapse/tests/files/stormpkg/storm/modules/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/storm/modules/testmod
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1492 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/testpkg.yaml
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.285636 synapse-2.98.0/synapse/tests/files/stormpkg/workflows/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       30 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/workflows/testpkg-bam.newp
--rw-r--r--   0 circleci  (3434) circleci  (3434)       47 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/workflows/testpkg-baz.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       31 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/stormpkg/workflows/testpkg-foo.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/test.dat
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.285636 synapse-2.98.0/synapse/tests/files/testcore/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       46 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/files/testcore/cell.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       70 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/nopmod.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25820 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_axon.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4540 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_cmds_boss.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17475 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_cmds_cortex.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19736 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_cmds_cron.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5912 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_cmds_hive.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7804 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_cmds_trigger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14272 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_common.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   271666 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_cortex.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4379 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_cryotank.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5124 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_daemon.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      196 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9633 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_datamodel.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      249 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_glob.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      557 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_init.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35254 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_agenda.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    34906 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_aha.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    82686 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_ast.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5576 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_autodoc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12201 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      846 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_boss.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8594 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_cache.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    64809 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_cell.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22673 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_certdir.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3189 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_chop.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9283 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_cli.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15234 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      873 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_const.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2974 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_coro.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      295 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_crypto_coin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5218 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_crypto_ecc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5372 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_crypto_tinfoil.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_datfile.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1239 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_dyndeps.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6575 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_encoding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3186 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_gis.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   116085 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_grammar.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      715 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_hashitem.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1329 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_hashset.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2265 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_health.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6379 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_hive.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14934 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_hiveauth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    50471 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_httpapi.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      839 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_interval.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6145 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_jsonstor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7755 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_jupyter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    81044 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_layer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4500 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_link.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    59604 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_lmdbslab.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11076 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_modelrev.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3923 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_module.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7680 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_msgpack.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17442 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_multislabseqn.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8350 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_nexus.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19131 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_node.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      603 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_output.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2320 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_platforms_linux.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4969 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_provenance.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      829 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_queue.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      415 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_ratelimit.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3104 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_reflect.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18632 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_rstorm.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2668 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_scope.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23942 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_scrape.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      756 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_slaboffs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4257 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_slabseqn.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23935 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_snap.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2455 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_spooled.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   157267 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_storm.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      277 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_storm_format.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23741 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormhttp.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1644 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_backup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9092 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_cell.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      797 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_ethereum.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8524 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_imap.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7389 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_infosec.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      877 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_ipv6.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2795 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_json.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2905 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_log.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4733 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_macro.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11799 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_model.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5445 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_modelext.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5336 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_oauth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8841 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_scrape.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1214 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_smtp.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12428 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_stix.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1227 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_storm.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3435 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_xml.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1358 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormlib_yaml.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39169 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormsvc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   241235 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormtypes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4779 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_stormwhois.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2960 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_structlog.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1325 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_task.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      366 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_thishost.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3555 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_time.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24298 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_trigger.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    66419 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_types.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2788 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_urlhelp.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8164 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    32951 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lib_view.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      375 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lookup_iso3166.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      290 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_lookup_phonenum.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_mindmeld.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1828 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_auth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11437 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8202 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_biz.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21277 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_crypto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15006 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_dns.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9549 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_economic.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18663 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_files.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1887 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_geopol.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18148 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_geospace.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      648 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_gov_cn.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      899 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_gov_intl.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1328 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_gov_us.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   106246 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_inet.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    58311 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_infotech.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2469 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_language.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1798 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_material.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1487 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_media.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    31199 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_orgs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13682 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_person.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22416 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_proj.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8581 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_risk.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21980 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_syn.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12620 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_telco.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6029 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_model_transport.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1098 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_servers_axon.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1465 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_servers_cortex.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1185 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_servers_cryotank.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2320 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_servers_stemcell.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3381 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_servers_univ.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    49484 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_telepath.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3520 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_aha.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6703 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_autodoc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4242 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_backup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12281 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_cellauth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4104 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_cryo_cat.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      671 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_cryo_list.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6257 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_csvtool.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6168 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_easycert.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5608 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_feed.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8492 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_genpkg.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      314 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_guid.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3262 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_healthcheck.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3944 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_hiveload.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2550 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_hivesave.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      892 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_json2mpk.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1507 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_modrole.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4153 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_moduser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1695 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_pullfile.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5611 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_pushfile.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2078 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_rstorm.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7928 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_tools_storm.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7972 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/test_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    63583 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tests/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.285636 synapse-2.98.0/synapse/tools/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.289636 synapse-2.98.0/synapse/tools/aha/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/aha/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3304 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/aha/easycert.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2609 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/aha/enroll.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2222 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/aha/list.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.289636 synapse-2.98.0/synapse/tools/aha/provision/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/aha/provision/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2722 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/aha/provision/service.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1520 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/aha/provision/user.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    27086 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/autodoc.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5922 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/backup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12234 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/cellauth.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1885 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/cmdr.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.289636 synapse-2.98.0/synapse/tools/cryo/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/cryo/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2532 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/cryo/cat.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      734 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/cryo/list.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6727 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/csvtool.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3085 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/easycert.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5706 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/feed.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8701 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/genpkg.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      300 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/guid.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3082 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/healthcheck.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.289636 synapse-2.98.0/synapse/tools/hive/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/hive/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2196 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/hive/load.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1749 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/hive/save.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1360 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/json2mpk.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2141 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/modrole.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4277 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/moduser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1178 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/promote.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2098 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/pullfile.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4082 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/pushfile.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1057 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/rstorm.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12588 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/tools/storm.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.289636 synapse-2.98.0/synapse/vendor/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.289636 synapse-2.98.0/synapse/vendor/cashaddress/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1197 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/cashaddress/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      162 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/cashaddress/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3692 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/cashaddress/base58.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4471 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/cashaddress/convert.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1719 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/cashaddress/crypto.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.289636 synapse-2.98.0/synapse/vendor/cashaddress/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/cashaddress/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3944 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/cashaddress/tests/test_cashaddress.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.289636 synapse-2.98.0/synapse/vendor/substrateinterface/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11502 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/substrateinterface/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/substrateinterface/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.289636 synapse-2.98.0/synapse/vendor/substrateinterface/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/substrateinterface/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9508 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/substrateinterface/tests/test_ss58.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.289636 synapse-2.98.0/synapse/vendor/substrateinterface/utils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1064 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/substrateinterface/utils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8241 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/substrateinterface/utils/ss58.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      263 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.289636 synapse-2.98.0/synapse/vendor/xrpl/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      981 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/xrpl/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1269 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/xrpl/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      576 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/xrpl/constants.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.289636 synapse-2.98.0/synapse/vendor/xrpl/core/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      181 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/xrpl/core/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.293636 synapse-2.98.0/synapse/vendor/xrpl/core/addresscodec/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1178 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/xrpl/core/addresscodec/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6526 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/xrpl/core/addresscodec/codec.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      254 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/xrpl/core/addresscodec/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4963 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/xrpl/core/addresscodec/main.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      235 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/xrpl/core/addresscodec/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.293636 synapse-2.98.0/synapse/vendor/xrpl/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/xrpl/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6651 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/xrpl/tests/test_codec.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4299 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/xrpl/tests/test_main.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4221 2022-06-17 21:06:40.000000 synapse-2.98.0/synapse/vendor/xrpl/tests/test_main_test_cases.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-17 21:07:39.205635 synapse-2.98.0/synapse.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2966 2022-06-17 21:07:39.000000 synapse-2.98.0/synapse.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13574 2022-06-17 21:07:39.000000 synapse-2.98.0/synapse.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-17 21:07:39.000000 synapse-2.98.0/synapse.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1070 2022-06-17 21:07:39.000000 synapse-2.98.0/synapse.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2022-06-17 21:07:39.000000 synapse-2.98.0/synapse.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.983796 synapse-2.99.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2022-06-23 22:52:43.000000 synapse-2.99.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      117 2022-06-23 22:52:43.000000 synapse-2.99.0/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2966 2022-06-23 22:53:35.983796 synapse-2.99.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1771 2022-06-23 22:52:43.000000 synapse-2.99.0/README.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2022-06-23 22:53:35.987796 synapse-2.99.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4789 2022-06-23 22:52:43.000000 synapse-2.99.0/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.935796 synapse-2.99.0/synapse/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1222 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    42912 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/axon.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      308 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/cells.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.939796 synapse-2.99.0/synapse/cmds/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/cmds/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2920 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/cmds/boss.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15812 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/cmds/cortex.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26083 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/cmds/cron.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8362 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/cmds/hive.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10999 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/cmds/trigger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    27505 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/common.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   176823 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/cortex.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9081 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/cryotank.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16632 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/daemon.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.939796 synapse-2.99.0/synapse/data/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      433 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/data/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10558 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/data/iana.tlds.mpk
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    28386 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/datamodel.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6846 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/exc.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3209 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/glob.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.947796 synapse-2.99.0/synapse/lib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      129 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    33134 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/agenda.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    30488 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/aha.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   114530 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/ast.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12255 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/autodoc.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21288 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1585 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/boss.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5904 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/cache.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   104380 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/cell.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35154 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/certdir.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3015 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/chop.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14152 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1053 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/cmd.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2026 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/cmdr.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14369 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1008 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/const.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7719 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/coro.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.947796 synapse-2.99.0/synapse/lib/crypto/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/crypto/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4860 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/crypto/coin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6522 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/crypto/ecc.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3875 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/crypto/tinfoil.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      620 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/datfile.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2168 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/dyndeps.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6015 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/encoding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2682 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/gis.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2150 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/grammar.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      658 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/hashitem.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1405 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/hashset.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1730 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/health.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19149 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/hive.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    30759 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/hiveauth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    28773 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/httpapi.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/ingest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1175 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/interval.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19210 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/jsonstor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11686 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/jupyter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   131206 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/layer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9359 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/link.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    52542 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/lmdbslab.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21681 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/modelrev.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4686 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/module.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1038 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/modules.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6476 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/msgpack.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15048 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/multislabseqn.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19699 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/nexus.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    30184 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/node.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      890 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/output.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26158 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/parser.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.947796 synapse-2.99.0/synapse/lib/platforms/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      196 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/platforms/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1097 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/platforms/common.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      150 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/platforms/darwin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      149 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/platforms/freebsd.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6465 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/platforms/linux.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2069 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/platforms/windows.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6536 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/provenance.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3862 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/queue.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1124 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/ratelimit.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2878 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/reflect.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18883 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/rstorm.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4336 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/scope.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14521 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/scrape.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      663 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/share.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/slaboffs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9823 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/slabseqn.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    44145 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/snap.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4564 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/spooled.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14532 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/storm.lark
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   165753 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/storm.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4018 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/storm_format.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      285 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormctrl.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21682 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormhttp.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.951796 synapse-2.99.0/synapse/lib/stormlib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3556 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/auth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2425 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/backup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10883 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/cell.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1176 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/ethereum.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1717 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/hex.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11928 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/imap.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10638 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/infosec.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1467 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/ipv6.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5681 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/json.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6425 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/log.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7044 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/macro.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26268 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/model.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7610 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/modelext.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3107 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/notifications.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5063 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/oauth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    34831 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/project.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6546 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/scrape.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6954 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/smtp.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    47317 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/stix.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1682 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/storm.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2302 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3558 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/xml.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1685 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormlib/yaml.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6688 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormsvc.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   335916 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormtypes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2275 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/stormwhois.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1303 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/structlog.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5095 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/task.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      840 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/thishost.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      417 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/thisplat.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      164 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/threads.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6614 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/time.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14510 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/trigger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    62521 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/types.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2459 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/urlhelp.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7161 2022-06-23 22:53:13.000000 synapse-2.99.0/synapse/lib/version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    34616 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lib/view.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.951796 synapse-2.99.0/synapse/lookup/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lookup/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5224 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lookup/iana.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10406 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lookup/iso3166.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2493 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lookup/macho.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11071 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lookup/pe.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16491 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/lookup/phonenum.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/mindmeld.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.955796 synapse-2.99.0/synapse/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2907 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/auth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10251 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11258 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/biz.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    24468 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/crypto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13439 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/dns.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12001 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/economic.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26201 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/files.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1540 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/geopol.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15282 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/geospace.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.955796 synapse-2.99.0/synapse/models/gov/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/gov/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      876 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/gov/cn.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1032 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/gov/intl.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1328 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/gov/us.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   124294 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/inet.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    95476 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/infotech.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2640 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/language.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2323 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/material.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2409 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/media.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    48713 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/orgs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21421 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/person.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6573 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/proj.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18217 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/risk.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13692 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/syn.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15107 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/telco.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12238 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/models/transport.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.955796 synapse-2.99.0/synapse/servers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/servers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      180 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/servers/aha.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      176 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/servers/axon.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      573 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/servers/cell.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      184 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/servers/cortex.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      192 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/servers/cryotank.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      200 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/servers/jsonstor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1190 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/servers/stemcell.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    41504 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/telepath.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.975796 synapse-2.99.0/synapse/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.975796 synapse-2.99.0/synapse/tests/files/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.931796 synapse-2.99.0/synapse/tests/files/certdir/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.975796 synapse-2.99.0/synapse/tests/files/certdir/cas/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      981 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/certdir/cas/ca.crt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1704 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/certdir/cas/ca.key
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.975796 synapse-2.99.0/synapse/tests/files/certdir/hosts/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1054 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/certdir/hosts/localhost.crt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1708 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/certdir/hosts/localhost.key
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.975796 synapse-2.99.0/synapse/tests/files/certdir/users/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1432 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/certdir/users/root.crt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3272 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/certdir/users/root.key
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1062 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/certdir/users/user.crt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1704 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/certdir/users/user.key
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.975796 synapse-2.99.0/synapse/tests/files/rstorm/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       57 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/rstorm/httpresp1.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/rstorm/httpresp2.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/rstorm/httpresp3.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1486 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/rstorm/httprespmulti.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      910 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/rstorm/testsvc.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.975796 synapse-2.99.0/synapse/tests/files/stix_export/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15655 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stix_export/basic.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6559 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stix_export/custom0.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6068 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stix_export/risk0.json
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.975796 synapse-2.99.0/synapse/tests/files/stix_import/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    52903 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stix_import/apt1.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4020 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stix_import/oasis-example-00.json
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.975796 synapse-2.99.0/synapse/tests/files/stormmod/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormmod/common
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.975796 synapse-2.99.0/synapse/tests/files/stormpkg/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.975796 synapse-2.99.0/synapse/tests/files/stormpkg/docs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/docs/foobar.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/docs/foobar.svg
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.975796 synapse-2.99.0/synapse/tests/files/stormpkg/dotstorm/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      128 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/dotstorm/dotstorm.yaml
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.931796 synapse-2.99.0/synapse/tests/files/stormpkg/dotstorm/storm/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.975796 synapse-2.99.0/synapse/tests/files/stormpkg/dotstorm/storm/commands/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/dotstorm/storm/commands/dotstorm.bar.storm
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.975796 synapse-2.99.0/synapse/tests/files/stormpkg/dotstorm/storm/modules/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/dotstorm/storm/modules/dotstorm.foo.storm
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       57 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/nocontent.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/nomime.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       56 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/nopath.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       79 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/nosuchfile.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       63 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/notitle.yaml
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.979796 synapse-2.99.0/synapse/tests/files/stormpkg/optic/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        3 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/optic/index.html
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.935796 synapse-2.99.0/synapse/tests/files/stormpkg/storm/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.979796 synapse-2.99.0/synapse/tests/files/stormpkg/storm/commands/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/storm/commands/testpkg.baz
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/storm/commands/testpkgcmd
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.979796 synapse-2.99.0/synapse/tests/files/stormpkg/storm/modules/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/storm/modules/testmod
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1492 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/testpkg.yaml
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.979796 synapse-2.99.0/synapse/tests/files/stormpkg/workflows/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       30 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/workflows/testpkg-bam.newp
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       47 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/workflows/testpkg-baz.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       31 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/stormpkg/workflows/testpkg-foo.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        5 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/test.dat
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.979796 synapse-2.99.0/synapse/tests/files/testcore/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       46 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/files/testcore/cell.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       70 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/nopmod.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25820 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_axon.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4540 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_cmds_boss.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17475 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_cmds_cortex.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19736 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_cmds_cron.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5912 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_cmds_hive.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7804 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_cmds_trigger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14272 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_common.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   271666 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_cortex.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4379 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_cryotank.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5124 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_daemon.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      196 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9633 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_datamodel.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      249 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_glob.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      557 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_init.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    35254 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_agenda.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    34906 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_aha.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    82686 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_ast.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5576 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_autodoc.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12201 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      846 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_boss.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8594 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_cache.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    64809 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_cell.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22673 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_certdir.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3189 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_chop.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9283 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15234 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      873 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_const.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2974 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_coro.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      295 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_crypto_coin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5218 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_crypto_ecc.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5372 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_crypto_tinfoil.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_datfile.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1239 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_dyndeps.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6575 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_encoding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3186 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_gis.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   116085 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_grammar.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      715 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_hashitem.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1329 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_hashset.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2265 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_health.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6379 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_hive.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14934 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_hiveauth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    50471 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_httpapi.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      839 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_interval.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6145 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_jsonstor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7755 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_jupyter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    81044 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_layer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4500 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_link.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    59604 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_lmdbslab.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11076 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_modelrev.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3923 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_module.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7680 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_msgpack.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17442 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_multislabseqn.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8350 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_nexus.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19131 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_node.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      603 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_output.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2320 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_platforms_linux.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4969 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_provenance.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      829 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_queue.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      415 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_ratelimit.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3104 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_reflect.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18632 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_rstorm.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2668 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_scope.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23942 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_scrape.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      756 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_slaboffs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4257 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_slabseqn.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23935 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_snap.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2455 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_spooled.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   157267 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_storm.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      277 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_storm_format.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23741 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormhttp.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1644 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_backup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10333 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_cell.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      797 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_ethereum.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8524 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_imap.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7389 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_infosec.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      877 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_ipv6.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2795 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_json.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2905 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_log.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4733 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_macro.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11799 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_model.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5445 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_modelext.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5336 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_oauth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8841 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_scrape.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1214 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_smtp.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16977 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_stix.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1227 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_storm.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3435 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_xml.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1358 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormlib_yaml.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39169 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormsvc.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   241235 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormtypes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4779 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_stormwhois.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2960 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_structlog.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1325 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_task.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      366 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_thishost.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3555 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_time.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    24298 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_trigger.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    66419 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_types.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2788 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_urlhelp.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8164 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    32951 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lib_view.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      375 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lookup_iso3166.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      290 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_lookup_phonenum.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_mindmeld.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1828 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_auth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11437 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8202 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_biz.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21277 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_crypto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15006 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_dns.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9549 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_economic.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18663 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_files.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1887 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_geopol.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18148 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_geospace.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      648 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_gov_cn.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      899 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_gov_intl.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1328 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_gov_us.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)   106246 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_inet.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    58311 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_infotech.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2469 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_language.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1798 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_material.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1487 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_media.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    31199 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_orgs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13682 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_person.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    22416 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_proj.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8581 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_risk.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21980 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_syn.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12620 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_telco.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6029 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_model_transport.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1098 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_servers_axon.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1465 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_servers_cortex.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1185 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_servers_cryotank.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2320 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_servers_stemcell.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3381 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_servers_univ.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    49484 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_telepath.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3520 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_aha.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6703 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_autodoc.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4242 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_backup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12281 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_cellauth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4104 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_cryo_cat.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      671 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_cryo_list.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8317 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_csvtool.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6168 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_easycert.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5608 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_feed.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8492 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_genpkg.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      314 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_guid.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3262 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_healthcheck.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3944 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_hiveload.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2550 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_hivesave.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      892 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_json2mpk.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1507 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_modrole.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4153 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_moduser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1695 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_pullfile.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5611 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_pushfile.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2078 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_rstorm.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7928 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_tools_storm.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7972 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/test_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    63583 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tests/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.979796 synapse-2.99.0/synapse/tools/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.979796 synapse-2.99.0/synapse/tools/aha/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/aha/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3304 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/aha/easycert.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2609 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/aha/enroll.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2222 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/aha/list.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.979796 synapse-2.99.0/synapse/tools/aha/provision/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/aha/provision/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2722 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/aha/provision/service.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1520 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/aha/provision/user.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    27086 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/autodoc.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5922 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/backup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12234 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/cellauth.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1885 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/cmdr.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.979796 synapse-2.99.0/synapse/tools/cryo/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/cryo/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2532 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/cryo/cat.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      734 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/cryo/list.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7267 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/csvtool.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3085 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/easycert.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5706 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/feed.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8701 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/genpkg.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      300 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/guid.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3082 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/healthcheck.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.983796 synapse-2.99.0/synapse/tools/hive/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/hive/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2196 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/hive/load.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1749 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/hive/save.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1360 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/json2mpk.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2141 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/modrole.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4277 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/moduser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1178 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/promote.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2098 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/pullfile.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4082 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/pushfile.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1057 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/rstorm.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12588 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/tools/storm.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.983796 synapse-2.99.0/synapse/vendor/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.983796 synapse-2.99.0/synapse/vendor/cashaddress/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1197 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/cashaddress/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      162 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/cashaddress/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3692 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/cashaddress/base58.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4471 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/cashaddress/convert.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1719 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/cashaddress/crypto.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.983796 synapse-2.99.0/synapse/vendor/cashaddress/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/cashaddress/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3944 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/cashaddress/tests/test_cashaddress.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.983796 synapse-2.99.0/synapse/vendor/substrateinterface/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11502 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/substrateinterface/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/substrateinterface/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.983796 synapse-2.99.0/synapse/vendor/substrateinterface/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/substrateinterface/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9508 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/substrateinterface/tests/test_ss58.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.983796 synapse-2.99.0/synapse/vendor/substrateinterface/utils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1064 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/substrateinterface/utils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8241 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/substrateinterface/utils/ss58.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      263 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.983796 synapse-2.99.0/synapse/vendor/xrpl/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      981 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/xrpl/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1269 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/xrpl/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      576 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/xrpl/constants.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.983796 synapse-2.99.0/synapse/vendor/xrpl/core/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      181 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/xrpl/core/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.983796 synapse-2.99.0/synapse/vendor/xrpl/core/addresscodec/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1178 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/xrpl/core/addresscodec/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6526 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/xrpl/core/addresscodec/codec.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      254 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/xrpl/core/addresscodec/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4963 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/xrpl/core/addresscodec/main.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      235 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/xrpl/core/addresscodec/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.983796 synapse-2.99.0/synapse/vendor/xrpl/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/xrpl/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6651 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/xrpl/tests/test_codec.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4299 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/xrpl/tests/test_main.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4221 2022-06-23 22:52:43.000000 synapse-2.99.0/synapse/vendor/xrpl/tests/test_main_test_cases.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-23 22:53:35.935796 synapse-2.99.0/synapse.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2966 2022-06-23 22:53:35.000000 synapse-2.99.0/synapse.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13670 2022-06-23 22:53:35.000000 synapse-2.99.0/synapse.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-23 22:53:35.000000 synapse-2.99.0/synapse.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1070 2022-06-23 22:53:35.000000 synapse-2.99.0/synapse.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2022-06-23 22:53:35.000000 synapse-2.99.0/synapse.egg-info/top_level.txt
```

### Comparing `synapse-2.98.0/LICENSE` & `synapse-2.99.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/PKG-INFO` & `synapse-2.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapse
-Version: 2.98.0
+Version: 2.99.0
 Summary: Synapse Intelligence Analysis Framework
 Home-page: https://github.com/vertexproject/synapse
 Author: The Vertex Project LLC
 Author-email: synapse@vertex.link
 License: Apache License 2.0
 Description: Synapse
         =======
```

### Comparing `synapse-2.98.0/README.rst` & `synapse-2.99.0/README.rst`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/setup.py` & `synapse-2.99.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 import subprocess
 
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 
-VERSION = '2.98.0'
+VERSION = '2.99.0'
 
 class VerifyVersionCommand(install):
     """Custom command to verify that the git tag matches our version"""
     description = 'verify that the git tag matches our version'
 
     def run(self):
         tag = os.getenv('CIRCLE_TAG', '')
```

### Comparing `synapse-2.98.0/synapse/__init__.py` & `synapse-2.99.0/synapse/__init__.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/axon.py` & `synapse-2.99.0/synapse/axon.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/cmds/boss.py` & `synapse-2.99.0/synapse/cmds/boss.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/cmds/cortex.py` & `synapse-2.99.0/synapse/cmds/cortex.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/cmds/cron.py` & `synapse-2.99.0/synapse/cmds/cron.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/cmds/hive.py` & `synapse-2.99.0/synapse/cmds/hive.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/cmds/trigger.py` & `synapse-2.99.0/synapse/cmds/trigger.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/common.py` & `synapse-2.99.0/synapse/common.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/cortex.py` & `synapse-2.99.0/synapse/cortex.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/cryotank.py` & `synapse-2.99.0/synapse/cryotank.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/daemon.py` & `synapse-2.99.0/synapse/daemon.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/data/iana.tlds.mpk` & `synapse-2.99.0/synapse/data/iana.tlds.mpk`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/datamodel.py` & `synapse-2.99.0/synapse/datamodel.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/exc.py` & `synapse-2.99.0/synapse/exc.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/glob.py` & `synapse-2.99.0/synapse/glob.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/agenda.py` & `synapse-2.99.0/synapse/lib/agenda.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/aha.py` & `synapse-2.99.0/synapse/lib/aha.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/ast.py` & `synapse-2.99.0/synapse/lib/ast.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/autodoc.py` & `synapse-2.99.0/synapse/lib/autodoc.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/base.py` & `synapse-2.99.0/synapse/lib/base.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/boss.py` & `synapse-2.99.0/synapse/lib/boss.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/cache.py` & `synapse-2.99.0/synapse/lib/cache.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/cell.py` & `synapse-2.99.0/synapse/lib/cell.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/certdir.py` & `synapse-2.99.0/synapse/lib/certdir.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/chop.py` & `synapse-2.99.0/synapse/lib/chop.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/cli.py` & `synapse-2.99.0/synapse/lib/cli.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/cmd.py` & `synapse-2.99.0/synapse/lib/cmd.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/cmdr.py` & `synapse-2.99.0/synapse/lib/cmdr.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/config.py` & `synapse-2.99.0/synapse/lib/config.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/const.py` & `synapse-2.99.0/synapse/lib/const.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/coro.py` & `synapse-2.99.0/synapse/lib/coro.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/crypto/coin.py` & `synapse-2.99.0/synapse/lib/crypto/coin.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/crypto/ecc.py` & `synapse-2.99.0/synapse/lib/crypto/ecc.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/crypto/tinfoil.py` & `synapse-2.99.0/synapse/lib/crypto/tinfoil.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/datfile.py` & `synapse-2.99.0/synapse/lib/datfile.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/dyndeps.py` & `synapse-2.99.0/synapse/lib/dyndeps.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/encoding.py` & `synapse-2.99.0/synapse/lib/encoding.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/gis.py` & `synapse-2.99.0/synapse/lib/gis.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/grammar.py` & `synapse-2.99.0/synapse/lib/grammar.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/hashitem.py` & `synapse-2.99.0/synapse/lib/hashitem.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/hashset.py` & `synapse-2.99.0/synapse/lib/hashset.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/health.py` & `synapse-2.99.0/synapse/lib/health.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/hive.py` & `synapse-2.99.0/synapse/lib/hive.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/hiveauth.py` & `synapse-2.99.0/synapse/lib/hiveauth.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/httpapi.py` & `synapse-2.99.0/synapse/lib/httpapi.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/interval.py` & `synapse-2.99.0/synapse/lib/interval.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/jsonstor.py` & `synapse-2.99.0/synapse/lib/jsonstor.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/jupyter.py` & `synapse-2.99.0/synapse/lib/jupyter.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/layer.py` & `synapse-2.99.0/synapse/lib/layer.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/link.py` & `synapse-2.99.0/synapse/lib/link.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/lmdbslab.py` & `synapse-2.99.0/synapse/lib/lmdbslab.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/modelrev.py` & `synapse-2.99.0/synapse/lib/modelrev.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/module.py` & `synapse-2.99.0/synapse/lib/module.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/modules.py` & `synapse-2.99.0/synapse/lib/modules.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/msgpack.py` & `synapse-2.99.0/synapse/lib/msgpack.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/multislabseqn.py` & `synapse-2.99.0/synapse/lib/multislabseqn.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/nexus.py` & `synapse-2.99.0/synapse/lib/nexus.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/node.py` & `synapse-2.99.0/synapse/lib/node.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/output.py` & `synapse-2.99.0/synapse/lib/output.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/parser.py` & `synapse-2.99.0/synapse/lib/parser.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/platforms/common.py` & `synapse-2.99.0/synapse/lib/platforms/common.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/platforms/linux.py` & `synapse-2.99.0/synapse/lib/platforms/linux.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     # a memory.max file available.
     # Reference
     # https://www.kernel.org/doc/Documentation/cgroup-v2.txt
     fp = '/sys/fs/cgroup/memory.max'
     if os.path.isfile(fp):
         with open(fp) as f:
             valu = f.read()
-            if valu != 'max':
+            if valu.strip() != 'max':
                 return int(valu)
     # /proc/meminfo is a fallback we can try to use in the event that
     # we find ourselves in a situation where there is not a memory cap.
     # if this happens inside of a container which does not have a maximum
     # memory cap, we could mis-represent the available memory.
     # Reference
     # https://www.kernel.org/doc/Documentation/filesystems/proc.txt
```

### Comparing `synapse-2.98.0/synapse/lib/platforms/windows.py` & `synapse-2.99.0/synapse/lib/platforms/windows.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/provenance.py` & `synapse-2.99.0/synapse/lib/provenance.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/queue.py` & `synapse-2.99.0/synapse/lib/queue.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/ratelimit.py` & `synapse-2.99.0/synapse/lib/ratelimit.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/reflect.py` & `synapse-2.99.0/synapse/lib/reflect.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/rstorm.py` & `synapse-2.99.0/synapse/lib/rstorm.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/scope.py` & `synapse-2.99.0/synapse/lib/scope.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/scrape.py` & `synapse-2.99.0/synapse/lib/scrape.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/share.py` & `synapse-2.99.0/synapse/lib/share.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/slaboffs.py` & `synapse-2.99.0/synapse/lib/slaboffs.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/slabseqn.py` & `synapse-2.99.0/synapse/lib/slabseqn.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/snap.py` & `synapse-2.99.0/synapse/lib/snap.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/spooled.py` & `synapse-2.99.0/synapse/lib/spooled.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/storm.lark` & `synapse-2.99.0/synapse/lib/storm.lark`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/storm.py` & `synapse-2.99.0/synapse/lib/storm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1411,14 +1411,28 @@
                 [ meta:note=* :text=$text :creator=$lib.user.iden :created=now ]
                 return($node)
             }
             init { $note = $addNoteNode($cmdopts.text) }
             [ <(about)+ { yield $note } ]
         ''',
     },
+    {
+        'name': 'uptime',
+        'descr': 'Print the uptime for the Cortex or a connected service.',
+        'cmdargs': (
+            ('name', {'type': 'str', 'nargs': '?',
+                      'help': 'The name, or iden, of the service (if not provided defaults to the Cortex).'}),
+        ),
+        'storm': '''
+            $resp = $lib.cell.uptime(name=$cmdopts.name)
+            $uptime = $lib.model.type(duration).repr($resp.uptime)
+            $starttime = $lib.time.format($resp.starttime, "%Y-%m-%d %H:%M:%S")
+            $lib.print("up {uptime} (since {since})", uptime=$uptime, since=$starttime)
+        ''',
+    },
 )
 
 class DmonManager(s_base.Base):
     '''
     Manager for StormDmon objects.
     '''
     async def __anit__(self, core):
```

### Comparing `synapse-2.98.0/synapse/lib/storm_format.py` & `synapse-2.99.0/synapse/lib/storm_format.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormhttp.py` & `synapse-2.99.0/synapse/lib/stormhttp.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/auth.py` & `synapse-2.99.0/synapse/lib/stormlib/auth.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/backup.py` & `synapse-2.99.0/synapse/lib/stormlib/backup.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/cell.py` & `synapse-2.99.0/synapse/lib/stormlib/cell.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import logging
 
 import synapse.exc as s_exc
+import synapse.lib.const as s_const
 import synapse.lib.stormtypes as s_stormtypes
 
 logger = logging.getLogger(__name__)
 
 
 storm_missing_autoadds = '''
 $absoluteOrder = $lib.view.list(deporder=$lib.true)
@@ -120,26 +121,35 @@
                   'args': (
                       {'name': 'consumers', 'type': 'array', 'default': None,
                        'desc': 'List of Telepath URLs for consumers of the Nexus log.'},
                       {'name': 'timeout', 'type': 'int', 'default': 30,
                        'desc': 'Time (in seconds) to wait for consumers to catch-up before culling.'}
                   ),
                   'returns': {'type': 'int', 'desc': 'The offset that was culled (up to and including).'}}},
+        {'name': 'uptime', 'desc': 'Get update data for the Cortex or a connected Service.',
+         'type': {'type': 'function', '_funcname': '_uptime',
+                  'args': (
+                      {'name': 'name', 'type': 'str', 'default': None,
+                       'desc': 'The name, or iden, of the service to get uptime data for '
+                               '(defaults to the Cortex if not provided).'},
+                  ),
+                  'returns': {'type': 'dict', 'desc': 'A dictionary containing uptime data.', }}},
     )
     _storm_lib_path = ('cell',)
 
     def getObjLocals(self):
         return {
             'getCellInfo': self._getCellInfo,
             'getBackupInfo': self._getBackupInfo,
             'getSystemInfo': self._getSystemInfo,
             'getHealthCheck': self._getHealthCheck,
             'hotFixesApply': self._hotFixesApply,
             'hotFixesCheck': self._hotFixesCheck,
             'trimNexsLog': self._trimNexsLog,
+            'uptime': self._uptime,
         }
 
     async def _hotFixesApply(self):
         if not self.runt.isAdmin():
             mesg = '$lib.cell.stormFixesApply() requires admin privs.'
             raise s_exc.AuthDeny(mesg=mesg)
 
@@ -222,7 +232,26 @@
 
         timeout = await s_stormtypes.toint(timeout, noneok=True)
 
         if consumers is not None:
             consumers = [await s_stormtypes.tostr(turl) async for turl in s_stormtypes.toiter(consumers)]
 
         return await self.runt.snap.core.trimNexsLog(consumers=consumers, timeout=timeout)
+
+    async def _uptime(self, name=None):
+
+        name = await s_stormtypes.tostr(name, noneok=True)
+
+        if name is None:
+            info = await self.runt.snap.core.getSystemInfo()
+        else:
+            ssvc = self.runt.snap.core.getStormSvc(name)
+            if ssvc is None:
+                mesg = f'No service with name/iden: {name}'
+                raise s_exc.NoSuchName(mesg=mesg)
+            await ssvc.proxy.waitready()
+            info = await ssvc.proxy.getSystemInfo()
+
+        return {
+            'starttime': info['cellstarttime'],
+            'uptime': info['celluptime'],
+        }
```

### Comparing `synapse-2.98.0/synapse/lib/stormlib/ethereum.py` & `synapse-2.99.0/synapse/lib/stormlib/ethereum.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/hex.py` & `synapse-2.99.0/synapse/lib/stormlib/hex.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/imap.py` & `synapse-2.99.0/synapse/lib/stormlib/imap.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/infosec.py` & `synapse-2.99.0/synapse/lib/stormlib/infosec.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/ipv6.py` & `synapse-2.99.0/synapse/lib/stormlib/ipv6.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/json.py` & `synapse-2.99.0/synapse/lib/stormlib/json.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/log.py` & `synapse-2.99.0/synapse/lib/stormlib/log.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/macro.py` & `synapse-2.99.0/synapse/lib/stormlib/macro.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/model.py` & `synapse-2.99.0/synapse/lib/stormlib/model.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/modelext.py` & `synapse-2.99.0/synapse/lib/stormlib/modelext.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/notifications.py` & `synapse-2.99.0/synapse/lib/stormlib/notifications.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/oauth.py` & `synapse-2.99.0/synapse/lib/stormlib/oauth.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/project.py` & `synapse-2.99.0/synapse/lib/stormlib/project.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/scrape.py` & `synapse-2.99.0/synapse/lib/stormlib/scrape.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/smtp.py` & `synapse-2.99.0/synapse/lib/stormlib/smtp.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/stix.py` & `synapse-2.99.0/synapse/lib/stormlib/stix.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import logging
 import datetime
 
 import synapse.exc as s_exc
 import synapse.common as s_common
 import synapse.lib.coro as s_coro
 import synapse.lib.node as s_node
+import synapse.lib.msgpack as s_msgpack
 import synapse.lib.stormctrl as s_stormctrl
 import synapse.lib.stormtypes as s_stormtypes
 
 import stix2validator
 
 logger = logging.getLogger(__name__)
 
@@ -566,51 +567,377 @@
             Lifting nodes from a STIX bundle::
 
                 yield $lib.stix($bundle)
         ''',
             'type': {
                 'type': 'function', '_funcname': 'liftBundle',
                 'args': (
-                    {'type': 'dict', 'name': 'bundle', 'desc': 'The stix bundle to lift nodes from.'},
+                    {'type': 'dict', 'name': 'bundle', 'desc': 'The STIX bundle to lift nodes from.'},
                 ),
                 'returns': {'name': 'Yields', 'type': 'storm:node', 'desc': 'Yields nodes'}
             }
         },
     )
     _storm_lib_path = ('stix', )
 
-    def __init__(self, runt, name=()):
-        s_stormtypes.Lib.__init__(self, runt, name)
-
     def getObjLocals(self):
         return {
             'lift': self.liftBundle,
             'validate': self.validateBundle,
         }
 
     async def validateBundle(self, bundle):
         bundle = await s_stormtypes.toprim(bundle)
         return await s_coro.spawn((validateStix, (bundle,), {}))
 
     async def liftBundle(self, bundle):
         bundle = await s_stormtypes.toprim(bundle)
+
         for obj in bundle.get('objects', ()):
             exts = obj.get('extensions')
             if not exts:
                 continue
             synx = exts.get(SYN_STIX_EXTENSION_ID)
             if not synx:  # pragma: no cover
                 continue
             ndef = synx.get('synapse_ndef')
             if not ndef:  # pragma: no cover
                 continue
             node = await self.runt.snap.getNodeByNdef(ndef)
             if node:
                 yield node
 
+stixingest = {
+    'addbundle': True,
+    'bundle': {
+        'storm': '''
+            it:sec:stix:bundle:id=$bundle.id
+            return($node)
+            [ it:sec:stix:bundle=* :id=$bundle.id ]
+            return($node)
+        ''',
+    },
+    'objects': {
+        'intrusion-set': {
+            'storm': '''
+                ($ok, $name) = $lib.trycast(ou:name, $object.name)
+                if $ok {
+
+                    ou:name=$name -> ou:org
+                    { for $alias in $object.aliases { [ :names?+=$alias ] } }
+                    return($node)
+
+                    [ ou:org=* :name=$name ]
+                    { for $alias in $object.aliases { [ :names?+=$alias ] } }
+                    return($node)
+                }
+            ''',
+        },
+        'identity': {
+            'storm': '''
+                switch $object.identity_class {
+                    group: {[ ps:contact=(stix, identity, $object.id) :orgname?=$object.name ]}
+                    organization: {[ ps:contact=(stix, identity, $object.id) :orgname?=$object.name ]}
+                    individual: {[ ps:contact=(stix, identity, $object.id) :name?=$object.name ]}
+                    system: {[ it:host=(stix, identity, $object.id) :name?=$object.name ]}
+                }
+            ''',
+        },
+        'tool': {
+            'storm': '''
+                ($ok, $name) = $lib.trycast(it:prod:softname, $object.name)
+                if $ok {
+                    it:prod:softname=$name -> it:prod:soft
+                    return($node)
+                    [ it:prod:soft=* :name=$name ]
+                    return($node)
+                }
+            ''',
+        },
+        'threat-actor': {
+            'storm': '''
+                [ ps:contact=(stix, threat-actor, $object.id)
+                    :name?=$object.name
+                    :desc?=$object.description
+                    :names?=$object.aliases
+                ]
+                $node.data.set(stix:object, $object)
+                return($node)
+            ''',
+        },
+        'course-of-action': {
+            'storm': '''
+                [ risk:mitigation=(stix, course-of-action, $object.id)
+                    :name?=$object.name
+                    :desc?=$object.description
+                ]
+                $node.data.set(stix:object, $object)
+                return($node)
+            ''',
+        },
+        'campaign': {
+            'storm': '''
+                [ ou:campaign=(stix, campaign, $object.id)
+                    :name?=$object.name
+                    :desc?=$object.description
+                    .seen?=$object.last_seen
+                    .seen?=$object.first_seen
+                ]
+                $node.data.set(stix:object, $object)
+                return($node)
+            ''',
+        },
+        'malware': {
+            'storm': '''
+                ($ok, $name) = $lib.trycast(it:prod:softname, $object.name)
+                if $ok {
+                    it:prod:softname=$name -> it:prod:soft
+                    return($node)
+                    [ it:prod:soft=* :name=$name ]
+                    return($node)
+                }
+            ''',
+        },
+        'indicator': {
+            'storm': '''
+                $guid = $lib.guid(stix, indicator, $object.id)
+                switch $object.pattern_type {
+
+                    yara: {[ it:app:yara:rule=$guid
+                                :name?=$object.name
+                                :text?=$object.pattern
+                    ]}
+
+                    snort: {[ it:app:snort:rule=$guid
+                                :name?=$object.name
+                                :text?=$object.pattern
+                    ]}
+
+                    *: {[ it:sec:stix:indicator=$guid
+                            :name?=$object.name
+                            :pattern?=$object.pattern
+                            :created?=$object.created
+                            :updated?=$object.modified]
+                       | scrape --refs :pattern
+                       }
+                }
+                $node.data.set(stix:object, $object)
+                return($node)
+            ''',
+        },
+        'report': {
+            'storm': '''
+                [ media:news=(stix, report, $object.id)
+                    :title?=$object.name
+                    :summary?=$object.description
+                    :published?=$object.published
+                ]
+                $node.data.set(stix:object, $object)
+                return($node)
+            ''',
+        },
+    },
+    'relationships': (
+
+        {'type': ('campaign', 'attributed-to', 'intrusion-set'), 'storm': '''
+            $n1node.props.org = $n2node
+        '''},
+
+        # this relationship is backwards in the STIX model
+        {'type': ('intrusion-set', 'attributed-to', 'threat-actor'), 'storm': '''
+            $n2node.props.org = $n1node
+        '''},
+
+        {'type': (None, 'uses', None), 'storm': 'yield $n1node [ +(uses)> { yield $n2node } ]'},
+        {'type': (None, 'indicates', None), 'storm': 'yield $n1node [ +(indicates)> { yield $n2node } ]'},
+
+        # nothing to do... they are the same for us...
+        {'type': ('threat-actor', 'attributed-to', 'identity'), 'storm': ''}
+    ),
+}
+
+@s_stormtypes.registry.registerLib
+class LibStixImport(s_stormtypes.Lib):
+
+    _storm_lib_path = ('stix', 'import')
+
+    _storm_locals = (  # type: ignore
+        {
+            'name': 'config', 'desc': '''
+            Return an editable copy of the default STIX ingest config.
+            ''',
+            'type': {
+                'type': 'function', '_funcname': 'config',
+                'returns': {'type': 'dict', 'desc': 'A copy of the default STIX ingest configuration.'},
+            },
+        },
+        {
+            'name': 'ingest', 'desc': '''
+            Import nodes from a STIX bundle.
+            ''',
+            'type': {
+                'type': 'function', '_funcname': 'ingest',
+                'args': (
+                    {'type': 'dict', 'name': 'bundle', 'desc': 'The STIX bundle to ingest.'},
+                    {'type': 'dict', 'name': 'config', 'default': None, 'desc': 'An optional STIX ingest configuration.'},
+                ),
+                'returns': {'name': 'Yields', 'type': 'storm:node', 'desc': 'Yields nodes'}
+            },
+        },
+    )
+
+    def getObjLocals(self):
+        return {
+            'config': self.config,
+            'ingest': self.ingest,
+        }
+
+    async def config(self):
+        return s_msgpack.deepcopy(stixingest, use_list=True)
+
+    async def ingest(self, bundle, config=None):
+
+        if config is None:
+            config = stixingest
+
+        config = await s_stormtypes.toprim(config)
+
+        config.setdefault('bundle', {})
+        config.setdefault('objects', {})
+        config.setdefault('relationships', [])
+
+        rellook = {r['type']: r for r in config.get('relationships', ())}
+
+        nodesbyid = {}
+        relationships = []
+
+        bundlenode = None
+
+        bundleconf = config.get('bundle')
+        if bundleconf is None:
+            bundleconf = {}
+
+        bundlestorm = bundleconf.get('storm')
+        if bundlestorm:
+            bundlenode = await self._callStorm(bundlestorm, {'bundle': bundle})
+
+        self.runt.layerConfirm(('node', 'edge', 'add', 'refs'))
+
+        for obj in bundle.get('objects'):
+
+            objtype = obj.get('type')
+
+            # do these in a second pass...
+            if objtype == 'relationship':
+                relationships.append(obj)
+                continue
+
+            objconf = config['objects'].get(objtype)
+            if objconf is None:
+                await self.runt.snap.warnonce(f'STIX bundle ingest has no object definition for: {objtype}.')
+                continue
+
+            objstorm = objconf.get('storm')
+            if objstorm is None:
+                continue
+
+            try:
+                node = await self._callStorm(objstorm, {'bundle': bundle, 'object': obj})
+                if node is not None:
+                    nodesbyid[obj.get('id')] = node
+            except asyncio.CancelledError: # pragma: no cover
+                raise
+            except Exception as e:
+                await self.runt.snap.warn(f'Error during STIX import callback for {objtype}: {e}')
+
+        for rel in relationships:
+
+            stixn1 = rel.get('source_ref')
+            stixn2 = rel.get('target_ref')
+
+            n1node = nodesbyid.get(stixn1)
+            if n1node is None:
+                await asyncio.sleep(0)
+                continue
+
+            n2node = nodesbyid.get(stixn2)
+            if n2node is None:
+                await asyncio.sleep(0)
+                continue
+
+            reltypes = (
+                (None, rel.get('relationship_type'), None),
+                (None, rel.get('relationship_type'), stixn2.split('--')[0]),
+                (stixn1.split('--')[0], rel.get('relationship_type'), None),
+                (stixn1.split('--')[0], rel.get('relationship_type'), stixn2.split('--')[0]),
+            )
+
+            foundone = False
+            for reltype in reltypes:
+
+                relconf = rellook.get(reltype)
+                if relconf is None:
+                    continue
+
+                relstorm = relconf.get('storm')
+                if relstorm is None: # pragma: no cover
+                    continue
+
+                foundone = True
+
+                try:
+                    node = await self._callStorm(relstorm, {'bundle': bundle, 'n1node': n1node, 'n2node': n2node})
+                    if node is not None:
+                        nodesbyid[rel.get('id')] = node
+                except asyncio.CancelledError: # pragma: no cover
+                    raise
+                except Exception as e:
+                    await self.runt.snap.warn(f'Error during STIX import callback for {reltype}: {e}')
+
+            if not foundone:
+                await self.runt.snap.warnonce(f'STIX bundle ingest has no relationship definition for: {reltype}.')
+
+        # attempt to resolve object_refs
+        for obj in bundle.get('objects'):
+
+            node = nodesbyid.get(obj.get('id'))
+            if node is None:
+                continue
+
+            for refid in obj.get('object_refs', ()):
+                refsnode = nodesbyid.get(refid)
+                if refsnode is None:
+                    continue
+
+                await node.addEdge('refs', refsnode.iden())
+
+        if bundlenode is not None:
+            for node in nodesbyid.values():
+                await bundlenode.addEdge('refs', node.iden())
+                await asyncio.sleep(0)
+            yield bundlenode
+
+        for node in nodesbyid.values():
+            yield node
+
+        if bundlenode:
+            yield bundlenode
+
+    async def _callStorm(self, text, varz):
+
+        query = await self.runt.snap.core.getStormQuery(text)
+        async with self.runt.getSubRuntime(query, opts={'vars': varz}) as runt:
+            try:
+                async for _ in runt.execute():
+                    await asyncio.sleep(0)
+            except s_stormctrl.StormReturn as e:
+                return e.item
+
+        return None
+
 @s_stormtypes.registry.registerLib
 class LibStixExport(s_stormtypes.Lib):
     '''
     A Storm Library for exporting to STIX version 2.1 CS02.
     '''
     _storm_locals = (  # type: ignore
         {
```

### Comparing `synapse-2.98.0/synapse/lib/stormlib/storm.py` & `synapse-2.99.0/synapse/lib/stormlib/storm.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/version.py` & `synapse-2.99.0/synapse/lib/stormlib/version.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/xml.py` & `synapse-2.99.0/synapse/lib/stormlib/xml.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormlib/yaml.py` & `synapse-2.99.0/synapse/lib/stormlib/yaml.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormsvc.py` & `synapse-2.99.0/synapse/lib/stormsvc.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormtypes.py` & `synapse-2.99.0/synapse/lib/stormtypes.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/stormwhois.py` & `synapse-2.99.0/synapse/lib/stormwhois.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/structlog.py` & `synapse-2.99.0/synapse/lib/structlog.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/task.py` & `synapse-2.99.0/synapse/lib/task.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/thishost.py` & `synapse-2.99.0/synapse/lib/thishost.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/time.py` & `synapse-2.99.0/synapse/lib/time.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/trigger.py` & `synapse-2.99.0/synapse/lib/trigger.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/types.py` & `synapse-2.99.0/synapse/lib/types.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/urlhelp.py` & `synapse-2.99.0/synapse/lib/urlhelp.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lib/version.py` & `synapse-2.99.0/synapse/lib/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,10 +219,10 @@
 
     if vers not in spec:
         raise exc(mesg=mesg, valu=valu, verstr=verstr, reqver=reqver)
 
 ##############################################################################
 # The following are touched during the release process by bumpversion.
 # Do not modify these directly.
-version = (2, 98, 0)
+version = (2, 99, 0)
 verstring = '.'.join([str(x) for x in version])
-commit = '3551fbf58113d8443a3173c9b8634b848602e4c9'
+commit = '66e7308e2ed4eb1014f9535304db79b4830c49ff'
```

### Comparing `synapse-2.98.0/synapse/lib/view.py` & `synapse-2.99.0/synapse/lib/view.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lookup/iana.py` & `synapse-2.99.0/synapse/lookup/iana.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lookup/iso3166.py` & `synapse-2.99.0/synapse/lookup/iso3166.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lookup/macho.py` & `synapse-2.99.0/synapse/lookup/macho.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lookup/pe.py` & `synapse-2.99.0/synapse/lookup/pe.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/lookup/phonenum.py` & `synapse-2.99.0/synapse/lookup/phonenum.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/auth.py` & `synapse-2.99.0/synapse/models/auth.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/base.py` & `synapse-2.99.0/synapse/models/base.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/biz.py` & `synapse-2.99.0/synapse/models/biz.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/crypto.py` & `synapse-2.99.0/synapse/models/crypto.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/dns.py` & `synapse-2.99.0/synapse/models/dns.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/economic.py` & `synapse-2.99.0/synapse/models/economic.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/files.py` & `synapse-2.99.0/synapse/models/files.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/geopol.py` & `synapse-2.99.0/synapse/models/geopol.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/geospace.py` & `synapse-2.99.0/synapse/models/geospace.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/gov/cn.py` & `synapse-2.99.0/synapse/models/gov/cn.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/gov/intl.py` & `synapse-2.99.0/synapse/models/gov/intl.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/gov/us.py` & `synapse-2.99.0/synapse/models/gov/us.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/inet.py` & `synapse-2.99.0/synapse/models/inet.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/infotech.py` & `synapse-2.99.0/synapse/models/infotech.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,14 +510,20 @@
                 }),
                 ('it:exec:reg:del', ('guid', {}), {
                     'doc': 'An instance of a host deleting a registry key.',
                 }),
                 ('it:app:yara:rule', ('guid', {}), {
                     'doc': 'A YARA rule unique identifier.',
                 }),
+                ('it:sec:stix:bundle', ('guid', {}), {
+                    'doc': 'A STIX bundle.',
+                }),
+                ('it:sec:stix:indicator', ('guid', {}), {
+                    'doc': 'A STIX indicator pattern.',
+                }),
                 ('it:app:yara:match', ('comp', {'fields': (('rule', 'it:app:yara:rule'), ('file', 'file:bytes'))}), {
                     'doc': 'A YARA rule match to a file.',
                 }),
                 ('it:app:yara:procmatch', ('guid', {}), {
                     'doc': 'An instance of a YARA rule match to a process.',
                 }),
                 ('it:app:snort:rule', ('guid', {}), {
@@ -1792,14 +1798,34 @@
                         'doc': 'The time of the network flow that caused the hit.'}),
                     ('sensor', ('it:host', {}), {
                         'doc': 'The sensor host node that produced the hit.'}),
                     ('version', ('it:semver', {}), {
                         'doc': 'The version of the rule at the time of match.'}),
                 )),
 
+                ('it:sec:stix:bundle', {}, (
+                    ('id', ('str', {}), {
+                        'doc': 'The id field from the STIX bundle.'}),
+                )),
+
+                ('it:sec:stix:indicator', {}, (
+                    ('id', ('str', {}), {
+                        'doc': 'The STIX id field from the indicator pattern.'}),
+                    ('name', ('str', {}), {
+                        'doc': 'The name of the STIX indicator pattern.'}),
+                    ('pattern', ('str', {}), {
+                        'doc': 'The STIX indicator pattern text.'}),
+                    ('created', ('time', {}), {
+                        'doc': 'The time that the indicator pattern was first created.'}),
+                    ('updated', ('time', {}), {
+                        'doc': 'The time that the indicator pattern was last modified.'}),
+                    ('labels', ('array', {'type': 'str', 'uniq': True, 'sorted': True}), {
+                        'doc': 'The label strings embedded in the STIX indicator pattern.'}),
+                )),
+
                 ('it:app:yara:rule', {}, (
                     ('text', ('str', {}), {
                         'doc': 'The YARA rule text.',
                         'disp': {'hint': 'text'},
                     }),
                     ('name', ('str', {}), {
                         'doc': 'The name of the YARA rule.'}),
```

### Comparing `synapse-2.98.0/synapse/models/language.py` & `synapse-2.99.0/synapse/models/language.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/material.py` & `synapse-2.99.0/synapse/models/material.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/media.py` & `synapse-2.99.0/synapse/models/media.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/orgs.py` & `synapse-2.99.0/synapse/models/orgs.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/person.py` & `synapse-2.99.0/synapse/models/person.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,14 +292,17 @@
                     }),
                     ('person', ('ps:person', {}), {
                         'doc': 'The ps:person GUID which owns this contact.',
                     }),
                     ('name', ('ps:name', {}), {
                         'doc': 'The person name listed for the contact.',
                     }),
+                    ('desc', ('str', {}), {
+                        'doc': 'A description of this contact.',
+                    }),
                     ('title', ('str', {'lower': True, 'strip': True}), {
                         'doc': 'The job/org title listed for this contact.',
                     }),
                     ('photo', ('file:bytes', {}), {
                         'doc': 'The photo listed for this contact.',
                     }),
                     ('orgname', ('ou:name', {}), {
```

### Comparing `synapse-2.98.0/synapse/models/proj.py` & `synapse-2.99.0/synapse/models/proj.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/risk.py` & `synapse-2.99.0/synapse/models/risk.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/syn.py` & `synapse-2.99.0/synapse/models/syn.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/telco.py` & `synapse-2.99.0/synapse/models/telco.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/models/transport.py` & `synapse-2.99.0/synapse/models/transport.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/servers/cell.py` & `synapse-2.99.0/synapse/servers/cell.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/servers/stemcell.py` & `synapse-2.99.0/synapse/servers/stemcell.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/telepath.py` & `synapse-2.99.0/synapse/telepath.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/files/__init__.py` & `synapse-2.99.0/synapse/tests/files/__init__.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/files/certdir/cas/ca.crt` & `synapse-2.99.0/synapse/tests/files/certdir/cas/ca.crt`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/files/certdir/cas/ca.key` & `synapse-2.99.0/synapse/tests/files/certdir/cas/ca.key`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/files/certdir/hosts/localhost.crt` & `synapse-2.99.0/synapse/tests/files/certdir/hosts/localhost.crt`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/files/certdir/hosts/localhost.key` & `synapse-2.99.0/synapse/tests/files/certdir/hosts/localhost.key`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/files/certdir/users/root.crt` & `synapse-2.99.0/synapse/tests/files/certdir/users/root.crt`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/files/certdir/users/root.key` & `synapse-2.99.0/synapse/tests/files/certdir/users/root.key`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/files/certdir/users/user.crt` & `synapse-2.99.0/synapse/tests/files/certdir/users/user.crt`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/files/certdir/users/user.key` & `synapse-2.99.0/synapse/tests/files/certdir/users/user.key`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/files/rstorm/httprespmulti.yaml` & `synapse-2.99.0/synapse/tests/files/rstorm/httprespmulti.yaml`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/files/rstorm/testsvc.py` & `synapse-2.99.0/synapse/tests/files/rstorm/testsvc.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/files/stix_export/basic.json` & `synapse-2.99.0/synapse/tests/files/stix_export/basic.json`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/files/stix_export/custom0.json` & `synapse-2.99.0/synapse/tests/files/stix_export/custom0.json`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/files/stix_export/risk0.json` & `synapse-2.99.0/synapse/tests/files/stix_export/risk0.json`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/files/stormpkg/testpkg.yaml` & `synapse-2.99.0/synapse/tests/files/stormpkg/testpkg.yaml`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_axon.py` & `synapse-2.99.0/synapse/tests/test_axon.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_cmds_boss.py` & `synapse-2.99.0/synapse/tests/test_cmds_boss.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_cmds_cortex.py` & `synapse-2.99.0/synapse/tests/test_cmds_cortex.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_cmds_cron.py` & `synapse-2.99.0/synapse/tests/test_cmds_cron.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_cmds_hive.py` & `synapse-2.99.0/synapse/tests/test_cmds_hive.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_cmds_trigger.py` & `synapse-2.99.0/synapse/tests/test_cmds_trigger.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_common.py` & `synapse-2.99.0/synapse/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_cortex.py` & `synapse-2.99.0/synapse/tests/test_cortex.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_cryotank.py` & `synapse-2.99.0/synapse/tests/test_cryotank.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_daemon.py` & `synapse-2.99.0/synapse/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_datamodel.py` & `synapse-2.99.0/synapse/tests/test_datamodel.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_init.py` & `synapse-2.99.0/synapse/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_agenda.py` & `synapse-2.99.0/synapse/tests/test_lib_agenda.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_aha.py` & `synapse-2.99.0/synapse/tests/test_lib_aha.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_ast.py` & `synapse-2.99.0/synapse/tests/test_lib_ast.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_autodoc.py` & `synapse-2.99.0/synapse/tests/test_lib_autodoc.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_base.py` & `synapse-2.99.0/synapse/tests/test_lib_base.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_boss.py` & `synapse-2.99.0/synapse/tests/test_lib_boss.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_cache.py` & `synapse-2.99.0/synapse/tests/test_lib_cache.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_cell.py` & `synapse-2.99.0/synapse/tests/test_lib_cell.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_certdir.py` & `synapse-2.99.0/synapse/tests/test_lib_certdir.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_chop.py` & `synapse-2.99.0/synapse/tests/test_lib_chop.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_cli.py` & `synapse-2.99.0/synapse/tests/test_lib_cli.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_config.py` & `synapse-2.99.0/synapse/tests/test_lib_config.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_const.py` & `synapse-2.99.0/synapse/tests/test_lib_const.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_coro.py` & `synapse-2.99.0/synapse/tests/test_lib_coro.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_crypto_ecc.py` & `synapse-2.99.0/synapse/tests/test_lib_crypto_ecc.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_crypto_tinfoil.py` & `synapse-2.99.0/synapse/tests/test_lib_crypto_tinfoil.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_dyndeps.py` & `synapse-2.99.0/synapse/tests/test_lib_dyndeps.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_encoding.py` & `synapse-2.99.0/synapse/tests/test_lib_encoding.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_gis.py` & `synapse-2.99.0/synapse/tests/test_lib_gis.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_grammar.py` & `synapse-2.99.0/synapse/tests/test_lib_grammar.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_hashitem.py` & `synapse-2.99.0/synapse/tests/test_lib_hashitem.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_hashset.py` & `synapse-2.99.0/synapse/tests/test_lib_hashset.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_health.py` & `synapse-2.99.0/synapse/tests/test_lib_health.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_hive.py` & `synapse-2.99.0/synapse/tests/test_lib_hive.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_hiveauth.py` & `synapse-2.99.0/synapse/tests/test_lib_hiveauth.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_httpapi.py` & `synapse-2.99.0/synapse/tests/test_lib_httpapi.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_interval.py` & `synapse-2.99.0/synapse/tests/test_lib_interval.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_jsonstor.py` & `synapse-2.99.0/synapse/tests/test_lib_jsonstor.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_jupyter.py` & `synapse-2.99.0/synapse/tests/test_lib_jupyter.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_layer.py` & `synapse-2.99.0/synapse/tests/test_lib_layer.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_link.py` & `synapse-2.99.0/synapse/tests/test_lib_link.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_lmdbslab.py` & `synapse-2.99.0/synapse/tests/test_lib_lmdbslab.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_modelrev.py` & `synapse-2.99.0/synapse/tests/test_lib_modelrev.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_module.py` & `synapse-2.99.0/synapse/tests/test_lib_module.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_msgpack.py` & `synapse-2.99.0/synapse/tests/test_lib_msgpack.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_multislabseqn.py` & `synapse-2.99.0/synapse/tests/test_lib_multislabseqn.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_nexus.py` & `synapse-2.99.0/synapse/tests/test_lib_nexus.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_node.py` & `synapse-2.99.0/synapse/tests/test_lib_node.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_output.py` & `synapse-2.99.0/synapse/tests/test_lib_output.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_platforms_linux.py` & `synapse-2.99.0/synapse/tests/test_lib_platforms_linux.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_provenance.py` & `synapse-2.99.0/synapse/tests/test_lib_provenance.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_queue.py` & `synapse-2.99.0/synapse/tests/test_lib_queue.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_reflect.py` & `synapse-2.99.0/synapse/tests/test_lib_reflect.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_rstorm.py` & `synapse-2.99.0/synapse/tests/test_lib_rstorm.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_scope.py` & `synapse-2.99.0/synapse/tests/test_lib_scope.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_scrape.py` & `synapse-2.99.0/synapse/tests/test_lib_scrape.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_slaboffs.py` & `synapse-2.99.0/synapse/tests/test_lib_slaboffs.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_slabseqn.py` & `synapse-2.99.0/synapse/tests/test_lib_slabseqn.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_snap.py` & `synapse-2.99.0/synapse/tests/test_lib_snap.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_spooled.py` & `synapse-2.99.0/synapse/tests/test_lib_spooled.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_storm.py` & `synapse-2.99.0/synapse/tests/test_lib_storm.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormhttp.py` & `synapse-2.99.0/synapse/tests/test_lib_stormhttp.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_backup.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_backup.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_cell.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_cell.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import synapse.exc as s_exc
 
-import synapse.lib.stormlib.cell as s_cell
+import synapse.lib.const as s_const
+import synapse.lib.stormlib.cell as s_stormlib_cell
 
 import synapse.tests.utils as s_test
+import synapse.tests.test_lib_stormsvc as s_t_stormsvc
 
 class StormCellTest(s_test.SynTest):
 
     async def test_stormlib_cell(self):
 
         async with self.getTestCore() as core:
 
@@ -21,17 +23,17 @@
             self.eq(set(ret.keys()), set(tst.keys()))
 
             ret = await core.callStorm('return ( $lib.cell.getHealthCheck() )')
             self.eq(ret, await core.getHealthCheck())
 
             # New cores have stormvar set to the current max version fix
             vers = await core.callStorm('return ( $lib.globals.get($key) )',
-                                        {'vars': {'key': s_cell.runtime_fixes_key}})
+                                        {'vars': {'key': s_stormlib_cell.runtime_fixes_key}})
             self.nn(vers)
-            self.eq(vers, s_cell.getMaxHotFixes())
+            self.eq(vers, s_stormlib_cell.getMaxHotFixes())
 
             user = await core.addUser('bob')
             opts = {'user': user.get('iden')}
 
             with self.raises(s_exc.AuthDeny):
                 await core.callStorm('return ( $lib.cell.getCellInfo() )', opts=opts)
 
@@ -40,14 +42,40 @@
 
             with self.raises(s_exc.AuthDeny):
                 await core.callStorm('return ( $lib.cell.getSystemInfo() )', opts=opts)
 
             with self.raises(s_exc.AuthDeny):
                 await core.callStorm('return ( $lib.cell.getHealthCheck() )', opts=opts)
 
+    async def test_stormlib_cell_uptime(self):
+
+        async with self.getTestCoreProxSvc(s_t_stormsvc.StormvarServiceCell) as (core, prox, svc):
+
+            day = await core.callStorm('return($lib.time.format($lib.time.now(), "%Y-%m-%d"))')
+
+            msgs = await core.stormlist('uptime')
+            self.stormIsInPrint('up 00:00:', msgs)
+            self.stormIsInPrint(f'since {day}', msgs)
+
+            msgs = await core.stormlist('uptime stormvar')
+            self.stormIsInPrint('up 00:00:', msgs)
+            self.stormIsInPrint(f'since {day}', msgs)
+
+            msgs = await core.stormlist('uptime newp')
+            self.stormIsInErr('No service with name/iden: newp', msgs)
+
+            svc.starttime = svc.starttime - (1 * s_const.day + 2 * s_const.hour) / 1000
+            msgs = await core.stormlist('uptime stormvar')
+            self.stormIsInPrint('up 1D 02:00:', msgs)
+            self.stormIsInPrint(day, msgs)
+
+            resp = await core.callStorm('return($lib.cell.uptime())')
+            self.eq(core.startms, resp['starttime'])
+            self.lt(resp['uptime'], s_const.minute)
+
     async def test_stormfix_autoadds(self):
 
         async def get_regression_views(cortex):
             q = '''function get_view(name) {
                         for $view in $lib.view.list() {
                             $p = $view.pack()
                             if ($p.name = $name) {
@@ -165,15 +193,15 @@
             self.none(nodes[0].get('v2_2'))
 
             self.len(0, await core.nodes('it:sec:cpe:v2_2', opts={'view': view0}))
             self.len(0, await core.nodes('it:sec:cpe:v2_2', opts={'view': view1}))
             self.len(0, await core.nodes('it:sec:cpe:v2_2', opts={'view': view2}))
 
             # Set the hotfix valu
-            opts = {'vars': {'key': s_cell.runtime_fixes_key, 'valu': (2, 0, 0)}}
+            opts = {'vars': {'key': s_stormlib_cell.runtime_fixes_key, 'valu': (2, 0, 0)}}
             await core.callStorm('$lib.globals.set($key, $valu)', opts)
 
             # Run all hotfixes.
             msgs = await core.stormlist('$lib.cell.hotFixesApply()')
 
             self.stormIsInPrint('Applying hotfix (3, 0, 0) for [Populate it:sec:cpe:v2_2', msgs)
             self.stormIsInPrint('Applied hotfix (3, 0, 0)', msgs)
```

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_ethereum.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_ethereum.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_imap.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_imap.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_infosec.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_infosec.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_ipv6.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_ipv6.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_json.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_json.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_log.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_log.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_macro.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_macro.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_model.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_model.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_modelext.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_modelext.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_oauth.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_oauth.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_scrape.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_scrape.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_smtp.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_smtp.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_stix.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_stix.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import copy
 import json
 
 import synapse.exc as s_exc
+import synapse.common as s_common
 
 import synapse.lib.stormlib.stix as s_stix
 
 import synapse.tests.utils as s_test
 
 # flake8: noqa: E501
 
-class StormlibModelTest(s_test.SynTest):
+class StormLibStixTest(s_test.SynTest):
 
     def bundeq(self, bund0, bund1):
 
         bund0 = copy.deepcopy(bund0)
         bund1 = copy.deepcopy(bund1)
 
         self._stripStixBundle(bund0)
@@ -284,7 +285,82 @@
             bund = await core.callStorm('''
             init { $bundle = $lib.stix.export.bundle() }
             ou:campaign
             $bundle.add($node)
             fini { return($bundle) }''')
             self.reqValidStix(bund)
             self.bundeq(self.getTestBundle('risk0.json'), bund)
+
+    async def test_stix_import(self):
+        async with self.getTestCore() as core:
+            config = await core.callStorm('return($lib.stix.import.config())')
+            self.nn(config.get('objects'))
+
+            viewiden = await core.callStorm('return($lib.view.get().fork().iden)')
+            stix = s_common.yamlload(self.getTestFilePath('stix_import', 'oasis-example-00.json'))
+            msgs = await core.stormlist('yield $lib.stix.import.ingest($stix)', opts={'view': viewiden, 'vars': {'stix': stix}})
+            self.len(1, await core.nodes('ps:contact:name="adversary bravo"', opts={'view': viewiden}))
+            self.len(1, await core.nodes('it:prod:soft', opts={'view': viewiden}))
+
+            viewiden = await core.callStorm('return($lib.view.get().fork().iden)')
+            stix = s_common.yamlload(self.getTestFilePath('stix_import', 'apt1.json'))
+            msgs = await core.stormlist('yield $lib.stix.import.ingest($stix)', opts={'view': viewiden, 'vars': {'stix': stix}})
+            self.len(34, await core.nodes('media:news -(refs)> *', opts={'view': viewiden}))
+            self.len(1, await core.nodes('it:sec:stix:bundle:id', opts={'view': viewiden}))
+            self.len(3, await core.nodes('it:sec:stix:indicator -(refs)> inet:fqdn', opts={'view': viewiden}))
+
+            stix = s_common.yamlload(self.getTestFilePath('stix_import', 'apt1.json'))
+
+            viewiden = await core.callStorm('return($lib.view.get().fork().iden)')
+            msgs = await core.stormlist('''
+                $config = $lib.stix.import.config()
+                $config.bundle = $lib.null
+                $storm = ${[ it:cmd=$object.name ] return($node)}
+                $config.objects."threat-actor" = ({"storm": $storm})
+                yield $lib.stix.import.ingest($stix, config=$config)
+            ''', opts={'view': viewiden, 'vars': {'stix': stix}})
+            self.len(5, await core.nodes('it:cmd', opts={'view': viewiden}))
+            self.len(0, await core.nodes('it:sec:stix:bundle:id', opts={'view': viewiden}))
+
+            viewiden = await core.callStorm('return($lib.view.get().fork().iden)')
+            msgs = await core.stormlist('''
+                $config = $lib.stix.import.config()
+                $storm00 = ${ $lib.raise(omg, omg) }
+                $config.objects."threat-actor" = ({"storm": $storm00})
+                $config.relationships = ([{
+                    "type": [$lib.null, "indicates", $lib.null],
+                    "storm": $storm00,
+                }])
+                yield $lib.stix.import.ingest($stix, config=$config)
+            ''', opts={'view': viewiden, 'vars': {'stix': stix}})
+            self.stormIsInWarn('Error during STIX import callback for threat-actor:', msgs)
+            self.stormIsInWarn("Error during STIX import callback for (None, 'indicates', None): StormRaise", msgs)
+
+            # NOTE: we mututate the APT1 stix here...
+            stix['objects'].append({
+                'type': 'relationship',
+                'id': 'relationship--6598bf44-1c10-4218-af9f-aaaaaaaaaaaa',
+                'relationship_type': 'frobs',
+                'source_ref': 'threat-actor--6d179234-61fc-40c4-ae86-3d53308d8e65',
+                'target_ref': 'threat-actor--d84cf283-93be-4ca7-890d-76c63eff3636',
+            })
+            stix['objects'].append({
+                'type': 'relationship',
+                'id': 'relationship--6598bf44-1c10-4218-af9f-bbbbbbbbbbbb',
+                'relationship_type': 'gronks',
+                'source_ref': 'threat-actor--6d179234-61fc-40c4-ae86-3d53308d8e65',
+                'target_ref': 'threat-actor--d84cf283-93be-4ca7-890d-76c63eff3636',
+            })
+            viewiden = await core.callStorm('return($lib.view.get().fork().iden)')
+            msgs = await core.stormlist('''
+                $config = $lib.stix.import.config()
+                $storm00 = ${ [ it:cmd=$n1node.props.name ] return($node) }
+                $config.relationships = ([{
+                    "type": [$lib.null, "frobs", $lib.null],
+                    "storm": $storm00,
+                }])
+                yield $lib.stix.import.ingest($stix, config=$config)
+            ''', opts={'view': viewiden, 'vars': {'stix': stix}})
+
+            nodes = [mesg[1] for mesg in msgs if mesg[0] == 'node']
+            self.len(1, [n for n in nodes if n[0][0] == 'it:cmd'])
+            self.stormIsInWarn("STIX bundle ingest has no relationship definition for: ('threat-actor', 'gronks', 'threat-actor')", msgs)
```

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_storm.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_storm.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_xml.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_xml.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormlib_yaml.py` & `synapse-2.99.0/synapse/tests/test_lib_stormlib_yaml.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormsvc.py` & `synapse-2.99.0/synapse/tests/test_lib_stormsvc.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormtypes.py` & `synapse-2.99.0/synapse/tests/test_lib_stormtypes.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_stormwhois.py` & `synapse-2.99.0/synapse/tests/test_lib_stormwhois.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_structlog.py` & `synapse-2.99.0/synapse/tests/test_lib_structlog.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_task.py` & `synapse-2.99.0/synapse/tests/test_lib_task.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_time.py` & `synapse-2.99.0/synapse/tests/test_lib_time.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_trigger.py` & `synapse-2.99.0/synapse/tests/test_lib_trigger.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_types.py` & `synapse-2.99.0/synapse/tests/test_lib_types.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_urlhelp.py` & `synapse-2.99.0/synapse/tests/test_lib_urlhelp.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_version.py` & `synapse-2.99.0/synapse/tests/test_lib_version.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_lib_view.py` & `synapse-2.99.0/synapse/tests/test_lib_view.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_auth.py` & `synapse-2.99.0/synapse/tests/test_model_auth.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_base.py` & `synapse-2.99.0/synapse/tests/test_model_base.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_biz.py` & `synapse-2.99.0/synapse/tests/test_model_biz.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_crypto.py` & `synapse-2.99.0/synapse/tests/test_model_crypto.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_dns.py` & `synapse-2.99.0/synapse/tests/test_model_dns.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_economic.py` & `synapse-2.99.0/synapse/tests/test_model_economic.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_files.py` & `synapse-2.99.0/synapse/tests/test_model_files.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_geopol.py` & `synapse-2.99.0/synapse/tests/test_model_geopol.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_geospace.py` & `synapse-2.99.0/synapse/tests/test_model_geospace.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_gov_cn.py` & `synapse-2.99.0/synapse/tests/test_model_gov_cn.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_gov_intl.py` & `synapse-2.99.0/synapse/tests/test_model_gov_intl.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_gov_us.py` & `synapse-2.99.0/synapse/tests/test_model_gov_us.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_inet.py` & `synapse-2.99.0/synapse/tests/test_model_inet.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_infotech.py` & `synapse-2.99.0/synapse/tests/test_model_infotech.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_language.py` & `synapse-2.99.0/synapse/tests/test_model_language.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_material.py` & `synapse-2.99.0/synapse/tests/test_model_material.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_media.py` & `synapse-2.99.0/synapse/tests/test_model_media.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_orgs.py` & `synapse-2.99.0/synapse/tests/test_model_orgs.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_person.py` & `synapse-2.99.0/synapse/tests/test_model_person.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_proj.py` & `synapse-2.99.0/synapse/tests/test_model_proj.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_risk.py` & `synapse-2.99.0/synapse/tests/test_model_risk.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_syn.py` & `synapse-2.99.0/synapse/tests/test_model_syn.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_telco.py` & `synapse-2.99.0/synapse/tests/test_model_telco.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_model_transport.py` & `synapse-2.99.0/synapse/tests/test_model_transport.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_servers_axon.py` & `synapse-2.99.0/synapse/tests/test_servers_axon.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_servers_cortex.py` & `synapse-2.99.0/synapse/tests/test_servers_cortex.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_servers_cryotank.py` & `synapse-2.99.0/synapse/tests/test_servers_cryotank.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_servers_stemcell.py` & `synapse-2.99.0/synapse/tests/test_servers_stemcell.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_servers_univ.py` & `synapse-2.99.0/synapse/tests/test_servers_univ.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_telepath.py` & `synapse-2.99.0/synapse/tests/test_telepath.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_aha.py` & `synapse-2.99.0/synapse/tests/test_tools_aha.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_autodoc.py` & `synapse-2.99.0/synapse/tests/test_tools_autodoc.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_backup.py` & `synapse-2.99.0/synapse/tests/test_tools_backup.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_cellauth.py` & `synapse-2.99.0/synapse/tests/test_tools_cellauth.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_cryo_cat.py` & `synapse-2.99.0/synapse/tests/test_tools_cryo_cat.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_cryo_list.py` & `synapse-2.99.0/synapse/tests/test_tools_cryo_list.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_csvtool.py` & `synapse-2.99.0/synapse/tests/test_tools_csvtool.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 '''
 
 class CsvToolTest(s_t_utils.SynTest):
 
     def _getOldSynVers(self):
         return (0, 0, 0)
 
-    async def test_csvtool(self):
+    async def test_csvtool_import(self):
 
         async with self.getTestCore() as core:
 
             url = core.getLocalUrl()
 
             dirn = s_common.gendir(core.dirn, 'junk')
 
@@ -68,14 +68,34 @@
             outp.expect('2 nodes')
 
             with mock.patch('synapse.telepath.Proxy._getSynVers', self._getOldSynVers):
                 outp = self.getTestOutp()
                 await s_csvtool.main(argv, outp=outp)
                 outp.expect('Cortex version 0.0.0 is outside of the csvtool supported range')
 
+            view = await core.callStorm('$view = $lib.view.get() $fork=$view.fork() return ( $fork.iden )')
+
+            optspath = s_common.genpath(dirn, 'optsfile.yaml')
+            s_common.yamlsave({'vars': {'hehe': 'haha'}}, optspath)
+
+            q = '''
+            for ($ipv4, $fqdn, $note) in $rows {
+                $note = $lib.str.format('{n} - {h}', n=$note, h=$hehe)
+                [ inet:dns:a?=($fqdn,$ipv4) ]  { | note.add $note }
+            }'''
+            with s_common.genfile(stormpath) as fd:
+                fd.truncate()
+                fd.write(q.encode())
+
+            argv = ['--cortex', url, '--view', view, '--optsfile', optspath, stormpath, csvpath]
+            outp = self.getTestOutp()
+            self.eq(0, await s_csvtool.main(argv, outp=outp))
+            self.len(0, await core.nodes('meta:note'))
+            self.len(2, await core.nodes('meta:note', opts={'view': view}))
+
     async def test_csvtool_missingvals(self):
 
         async with self.getTestCore() as core:
 
             url = core.getLocalUrl()
 
             dirn = s_common.gendir(core.dirn, 'junk')
@@ -187,7 +207,31 @@
                 rows = [row for row in csv.reader(fd)]
                 self.eq(rows, (['20', 'us'], ['30', 'cn'], ['40', '']))
 
             with mock.patch('synapse.telepath.Proxy._getSynVers', self._getOldSynVers):
                 outp = self.getTestOutp()
                 await s_csvtool.main(argv, outp=outp)
                 outp.expect(f'Cortex version 0.0.0 is outside of the csvtool supported range')
+
+            view = await core.callStorm('$view = $lib.view.get() $fork=$view.fork() return ( $fork.iden )')
+            await core.nodes('[test:int=50]', opts={'view': view})
+
+            optspath = s_common.genpath(dirn, 'optsfile.yaml')
+            s_common.yamlsave({'vars': {'hehe': 'haha'}}, optspath)
+
+            q = '''test:int $lib.csv.emit($node, $hehe)'''
+            with s_common.genfile(stormpath) as fd:
+                fd.truncate()
+                fd.write(q.encode())
+
+            argv = ['--cortex', url, '--view', view, '--optsfile', optspath, '--export', stormpath, csvpath]
+            outp = self.getTestOutp()
+            self.eq(0, await s_csvtool.main(argv, outp=outp))
+
+            with open(csvpath, 'r') as fd:
+                rows = [row for row in csv.reader(fd)]
+                self.eq(rows, (['20', 'haha'], ['30', 'haha'], ['40', 'haha'], ['50', 'haha']))
+
+            argv = ['--cortex', url, '--view', 'newp', '--export', stormpath, csvpath]
+            outp = self.getTestOutp()
+            self.eq(-1, await s_csvtool.main(argv, outp=outp))
+            self.true(outp.expect('View is not a guid'))
```

### Comparing `synapse-2.98.0/synapse/tests/test_tools_easycert.py` & `synapse-2.99.0/synapse/tests/test_tools_easycert.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_feed.py` & `synapse-2.99.0/synapse/tests/test_tools_feed.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_genpkg.py` & `synapse-2.99.0/synapse/tests/test_tools_genpkg.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_healthcheck.py` & `synapse-2.99.0/synapse/tests/test_tools_healthcheck.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_hiveload.py` & `synapse-2.99.0/synapse/tests/test_tools_hiveload.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_hivesave.py` & `synapse-2.99.0/synapse/tests/test_tools_hivesave.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_json2mpk.py` & `synapse-2.99.0/synapse/tests/test_tools_json2mpk.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_modrole.py` & `synapse-2.99.0/synapse/tests/test_tools_modrole.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_moduser.py` & `synapse-2.99.0/synapse/tests/test_tools_moduser.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_pullfile.py` & `synapse-2.99.0/synapse/tests/test_tools_pullfile.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_pushfile.py` & `synapse-2.99.0/synapse/tests/test_tools_pushfile.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_rstorm.py` & `synapse-2.99.0/synapse/tests/test_tools_rstorm.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_tools_storm.py` & `synapse-2.99.0/synapse/tests/test_tools_storm.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/test_utils.py` & `synapse-2.99.0/synapse/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tests/utils.py` & `synapse-2.99.0/synapse/tests/utils.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/aha/easycert.py` & `synapse-2.99.0/synapse/tools/aha/easycert.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/aha/enroll.py` & `synapse-2.99.0/synapse/tools/aha/enroll.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/aha/list.py` & `synapse-2.99.0/synapse/tools/aha/list.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/aha/provision/service.py` & `synapse-2.99.0/synapse/tools/aha/provision/service.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/aha/provision/user.py` & `synapse-2.99.0/synapse/tools/aha/provision/user.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/autodoc.py` & `synapse-2.99.0/synapse/tools/autodoc.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/backup.py` & `synapse-2.99.0/synapse/tools/backup.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/cellauth.py` & `synapse-2.99.0/synapse/tools/cellauth.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/cmdr.py` & `synapse-2.99.0/synapse/tools/cmdr.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/cryo/cat.py` & `synapse-2.99.0/synapse/tools/cryo/cat.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/cryo/list.py` & `synapse-2.99.0/synapse/tools/cryo/list.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/csvtool.py` & `synapse-2.99.0/synapse/tools/csvtool.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,24 @@
         opts = pars.parse_args(argv)
     except s_exc.ParserExit as e:
         return e.get('status')
 
     with open(opts.stormfile, 'r', encoding='utf8') as fd:
         text = fd.read()
 
+    stormopts = {}
+    if opts.optsfile:
+        stormopts = s_common.yamlload(opts.optsfile)
+
+    if opts.view:
+        if not s_common.isguid(opts.view):
+            outp.printf(f'View is not a guid {opts.view}')
+            return -1
+        stormopts['view'] = opts.view
+
     if opts.export:
 
         if not opts.cortex:
             outp.printf('--export requires --cortex')
             return -1
 
         if len(opts.csvfiles) != 1:
@@ -50,34 +60,32 @@
                 outp.printf(f'Please use a version of Synapse which supports {valu}; '
                             f'current version is {s_version.verstring}.')
                 return 1
 
             with open(path, 'w') as fd:
 
                 wcsv = csv.writer(fd)
-
                 # prevent streaming nodes by limiting shown events
-                opts = {'show': ('csv:row', 'print', 'warn', 'err')}
-
+                stormopts['show'] = ('csv:row', 'print', 'warn', 'err')
                 count = 0
-                async for name, info in core.storm(text, opts=opts):
+                async for name, info in core.storm(text, opts=stormopts):
 
                     if name == 'csv:row':
                         count += 1
                         wcsv.writerow(info['row'])
                         continue
 
                     if name in ('init', 'fini'):
                         continue
 
                     outp.printf('%s: %r' % (name, info))
 
                 outp.printf(f'exported {count} csv rows.')
 
-        return
+        return 0
 
     def iterrows():
         for path in opts.csvfiles:
 
             with open(path, 'r', encoding='utf8') as fd:
 
                 if opts.csv_header:
@@ -98,20 +106,20 @@
         logfd = s_common.genfile(opts.logfile)
         logfd.seek(0, 2)
 
     async def addCsvData(core):
 
         nodecount = 0
 
+        stormopts['editformat'] = 'splices'
+        vars = stormopts.setdefault('vars', {})
+
         for rows in rowgenr:
 
-            stormopts = {
-                'vars': {'rows': rows},
-                'editformat': 'splices',
-            }
+            vars['rows'] = rows
 
             async for mesg in core.storm(text, opts=stormopts):
 
                 if mesg[0] == 'node':
                     nodecount += 1
 
                 elif mesg[0] == 'err' and not opts.debug:
@@ -206,13 +214,17 @@
     muxp = pars.add_mutually_exclusive_group(required=True)
     muxp.add_argument('--cortex', '-c', type=str,
                       help='The telepath URL for the cortex ( or alias from ~/.syn/aliases ).')
     muxp.add_argument('--test', '-t', default=False, action='store_true',
                       help='Perform a local CSV ingest against a temporary cortex.')
     pars.add_argument('--export', default=False, action='store_true',
                       help='Export CSV data to file from storm using $lib.csv.emit(...) events.')
+    pars.add_argument('--view', default=None, action='store',
+                      help='Optional view to work in.')
+    pars.add_argument('--optsfile', default=None, action='store',
+                      help='Path to an opts file (.yaml) on disk.')
     pars.add_argument('stormfile', help='A Storm script describing how to create nodes from rows.')
     pars.add_argument('csvfiles', nargs='+', help='CSV files to load.')
     return pars
 
 if __name__ == '__main__':  # pragma: no cover
     sys.exit(asyncio.run(s_base.main(main(sys.argv[1:]))))
```

### Comparing `synapse-2.98.0/synapse/tools/easycert.py` & `synapse-2.99.0/synapse/tools/easycert.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/feed.py` & `synapse-2.99.0/synapse/tools/feed.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/genpkg.py` & `synapse-2.99.0/synapse/tools/genpkg.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/healthcheck.py` & `synapse-2.99.0/synapse/tools/healthcheck.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/hive/load.py` & `synapse-2.99.0/synapse/tools/hive/load.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/hive/save.py` & `synapse-2.99.0/synapse/tools/hive/save.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/json2mpk.py` & `synapse-2.99.0/synapse/tools/json2mpk.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/modrole.py` & `synapse-2.99.0/synapse/tools/modrole.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/moduser.py` & `synapse-2.99.0/synapse/tools/moduser.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/promote.py` & `synapse-2.99.0/synapse/tools/promote.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/pullfile.py` & `synapse-2.99.0/synapse/tools/pullfile.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/pushfile.py` & `synapse-2.99.0/synapse/tools/pushfile.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/rstorm.py` & `synapse-2.99.0/synapse/tools/rstorm.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/tools/storm.py` & `synapse-2.99.0/synapse/tools/storm.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/cashaddress/LICENSE` & `synapse-2.99.0/synapse/vendor/cashaddress/LICENSE`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/cashaddress/base58.py` & `synapse-2.99.0/synapse/vendor/cashaddress/base58.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/cashaddress/convert.py` & `synapse-2.99.0/synapse/vendor/cashaddress/convert.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/cashaddress/crypto.py` & `synapse-2.99.0/synapse/vendor/cashaddress/crypto.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/cashaddress/tests/test_cashaddress.py` & `synapse-2.99.0/synapse/vendor/cashaddress/tests/test_cashaddress.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/substrateinterface/LICENSE` & `synapse-2.99.0/synapse/vendor/substrateinterface/LICENSE`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/substrateinterface/__init__.py` & `synapse-2.99.0/synapse/vendor/substrateinterface/__init__.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/substrateinterface/tests/test_ss58.py` & `synapse-2.99.0/synapse/vendor/substrateinterface/tests/test_ss58.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/substrateinterface/utils/__init__.py` & `synapse-2.99.0/synapse/vendor/substrateinterface/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/substrateinterface/utils/ss58.py` & `synapse-2.99.0/synapse/vendor/substrateinterface/utils/ss58.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/xrpl/LICENSE` & `synapse-2.99.0/synapse/vendor/xrpl/LICENSE`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/xrpl/__init__.py` & `synapse-2.99.0/synapse/vendor/xrpl/__init__.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/xrpl/constants.py` & `synapse-2.99.0/synapse/vendor/xrpl/constants.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/xrpl/core/addresscodec/__init__.py` & `synapse-2.99.0/synapse/vendor/xrpl/core/addresscodec/__init__.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/xrpl/core/addresscodec/codec.py` & `synapse-2.99.0/synapse/vendor/xrpl/core/addresscodec/codec.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/xrpl/core/addresscodec/main.py` & `synapse-2.99.0/synapse/vendor/xrpl/core/addresscodec/main.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/xrpl/tests/test_codec.py` & `synapse-2.99.0/synapse/vendor/xrpl/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/xrpl/tests/test_main.py` & `synapse-2.99.0/synapse/vendor/xrpl/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse/vendor/xrpl/tests/test_main_test_cases.py` & `synapse-2.99.0/synapse/vendor/xrpl/tests/test_main_test_cases.py`

 * *Files identical despite different names*

### Comparing `synapse-2.98.0/synapse.egg-info/PKG-INFO` & `synapse-2.99.0/synapse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapse
-Version: 2.98.0
+Version: 2.99.0
 Summary: Synapse Intelligence Analysis Framework
 Home-page: https://github.com/vertexproject/synapse
 Author: The Vertex Project LLC
 Author-email: synapse@vertex.link
 License: Apache License 2.0
 Description: Synapse
         =======
```

### Comparing `synapse-2.98.0/synapse.egg-info/SOURCES.txt` & `synapse-2.99.0/synapse.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -349,14 +349,16 @@
 synapse/tests/files/rstorm/httpresp2.json
 synapse/tests/files/rstorm/httpresp3.json
 synapse/tests/files/rstorm/httprespmulti.yaml
 synapse/tests/files/rstorm/testsvc.py
 synapse/tests/files/stix_export/basic.json
 synapse/tests/files/stix_export/custom0.json
 synapse/tests/files/stix_export/risk0.json
+synapse/tests/files/stix_import/apt1.json
+synapse/tests/files/stix_import/oasis-example-00.json
 synapse/tests/files/stormmod/common
 synapse/tests/files/stormpkg/nocontent.yaml
 synapse/tests/files/stormpkg/nomime.yaml
 synapse/tests/files/stormpkg/nopath.yaml
 synapse/tests/files/stormpkg/nosuchfile.yaml
 synapse/tests/files/stormpkg/notitle.yaml
 synapse/tests/files/stormpkg/testpkg.yaml
```

### Comparing `synapse-2.98.0/synapse.egg-info/requires.txt` & `synapse-2.99.0/synapse.egg-info/requires.txt`

 * *Files identical despite different names*

