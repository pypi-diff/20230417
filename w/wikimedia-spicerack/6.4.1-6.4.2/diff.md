# Comparing `tmp/wikimedia-spicerack-6.4.1.tar.gz` & `tmp/wikimedia-spicerack-6.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikimedia-spicerack-6.4.1.tar", last modified: Thu Mar 30 15:30:57 2023, max compression
+gzip compressed data, was "wikimedia-spicerack-6.4.2.tar", last modified: Mon Apr 17 16:46:52 2023, max compression
```

## Comparing `wikimedia-spicerack-6.4.1.tar` & `wikimedia-spicerack-6.4.2.tar`

### file list

```diff
@@ -1,275 +1,275 @@
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.952962 wikimedia-spicerack-6.4.1/
--rw-r--r--   0 riccardo   (501) staff       (20)       45 2018-08-06 08:05:22.000000 wikimedia-spicerack-6.4.1/.coveragerc
--rw-r--r--   0 riccardo   (501) staff       (20)       84 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.1/.git-blame-ignore-revs
--rw-r--r--   0 riccardo   (501) staff       (20)      292 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.1/.gitignore
--rw-r--r--   0 riccardo   (501) staff       (20)       96 2018-08-06 08:05:22.000000 wikimedia-spicerack-6.4.1/.gitreview
--rw-r--r--   0 riccardo   (501) staff       (20)      668 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/.mailmap
--rw-r--r--   0 riccardo   (501) staff       (20)      207 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/.wmfconfig
--rw-r--r--   0 riccardo   (501) staff       (20)   103601 2023-03-30 15:21:09.000000 wikimedia-spicerack-6.4.1/CHANGELOG.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      271 2018-08-06 08:05:22.000000 wikimedia-spicerack-6.4.1/COPYRIGHT
--rw-r--r--   0 riccardo   (501) staff       (20)    34686 2018-08-06 08:05:22.000000 wikimedia-spicerack-6.4.1/LICENSE
--rw-r--r--   0 riccardo   (501) staff       (20)     1691 2023-03-30 15:30:57.953278 wikimedia-spicerack-6.4.1/PKG-INFO
--rw-r--r--   0 riccardo   (501) staff       (20)      443 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.1/README.rst
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.011715 wikimedia-spicerack-6.4.1/doc/
--rw-r--r--   0 riccardo   (501) staff       (20)      611 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/doc/Makefile
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.016093 wikimedia-spicerack-6.4.1/doc/examples/
--rw-r--r--   0 riccardo   (501) staff       (20)     1801 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/doc/examples/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.049446 wikimedia-spicerack-6.4.1/doc/source/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.051432 wikimedia-spicerack-6.4.1/doc/source/_static/
--rw-r--r--   0 riccardo   (501) staff       (20)      369 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/doc/source/_static/theme_overrides.css
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.215861 wikimedia-spicerack-6.4.1/doc/source/api/
--rw-r--r--   0 riccardo   (501) staff       (20)     1051 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/doc/source/api/index.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      101 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.administrative.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.alerting.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.alertmanager.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       39 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.apt.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.confctl.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.constants.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.cookbook.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.debmonitor.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      112 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.decorators.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.dhcp.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.dnsdisc.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       93 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.elasticsearch_cluster.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.exceptions.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.ganeti.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.icinga.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       63 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.interactive.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.ipmi.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       43 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.k8s.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       46 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.kafka.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.mediawiki.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       45 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.mysql.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       66 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.mysql_legacy.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.netbox.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.peeringdb.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.puppet.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.redfish.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       69 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.redis_cluster.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.remote.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.reposync.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.service.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       81 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.toolforge.etcdctl.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.toolforge.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.1/doc/source/api/spicerack.typing.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     6670 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/doc/source/conf.py
--rw-r--r--   0 riccardo   (501) staff       (20)      831 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/doc/source/configuration.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.1/doc/source/cookbook.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     2722 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/doc/source/development.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       44 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/doc/source/docutils.conf
--rw-r--r--   0 riccardo   (501) staff       (20)      384 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.1/doc/source/index.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     1227 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/doc/source/installation.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     9468 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/doc/source/introduction.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       62 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/doc/source/release.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/prospector.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      258 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/pyproject.toml
--rw-r--r--   0 riccardo   (501) staff       (20)      565 2023-03-30 15:30:57.965709 wikimedia-spicerack-6.4.1/setup.cfg
--rwxr-xr-x   0 riccardo   (501) staff       (20)     3281 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.1/setup.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.345818 wikimedia-spicerack-6.4.1/spicerack/
--rw-r--r--   0 riccardo   (501) staff       (20)    27361 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.1/spicerack/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)    17795 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/_cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3900 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/_log.py
--rw-r--r--   0 riccardo   (501) staff       (20)    18780 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/_menu.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1442 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/_module_api.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3478 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/administrative.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2769 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/alerting.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12766 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/alertmanager.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5853 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/apt.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8072 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/confctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)      262 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/constants.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5988 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2141 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/debmonitor.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3869 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/decorators.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10442 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/dhcp.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12124 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.1/spicerack/dnsdisc.py
--rw-r--r--   0 riccardo   (501) staff       (20)    30520 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/elasticsearch_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)      550 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/exceptions.py
--rw-r--r--   0 riccardo   (501) staff       (20)    13849 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/ganeti.py
--rw-r--r--   0 riccardo   (501) staff       (20)    27163 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/icinga.py
--rw-r--r--   0 riccardo   (501) staff       (20)      848 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/interactive.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10263 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/ipmi.py
--rw-r--r--   0 riccardo   (501) staff       (20)    18466 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/k8s.py
--rw-r--r--   0 riccardo   (501) staff       (20)    15061 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/kafka.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14797 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/mediawiki.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3329 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/mysql.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14945 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/mysql_legacy.py
--rw-r--r--   0 riccardo   (501) staff       (20)    13278 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/netbox.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5157 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/peeringdb.py
--rw-r--r--   0 riccardo   (501) staff       (20)    20891 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.1/spicerack/puppet.py
--rw-r--r--   0 riccardo   (501) staff       (20)        0 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/py.typed
--rw-r--r--   0 riccardo   (501) staff       (20)    36793 2023-03-30 15:21:09.000000 wikimedia-spicerack-6.4.1/spicerack/redfish.py
--rw-r--r--   0 riccardo   (501) staff       (20)     6421 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/redis_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)    27921 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.1/spicerack/remote.py
--rw-r--r--   0 riccardo   (501) staff       (20)     7111 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/reposync.py
--rw-r--r--   0 riccardo   (501) staff       (20)    23056 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.1/spicerack/service.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.369618 wikimedia-spicerack-6.4.1/spicerack/tests/
--rw-r--r--   0 riccardo   (501) staff       (20)      871 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/__init__.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.383545 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.398264 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/confctl/
--rw-r--r--   0 riccardo   (501) staff       (20)       33 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/confctl/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      698 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/confctl/schema.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.403396 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/config/
--rw-r--r--   0 riccardo   (501) staff       (20)       59 2020-10-23 11:19:20.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/config/valid.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       79 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      219 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/config_bad_external_modules.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       44 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/config_empty_base_dirs.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      216 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/config_external_modules.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      126 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/config_multiple_base_dirs.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      113 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/config_wrong_overrides.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:56.935060 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.413952 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/
--rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/__do_not_add_init_py_file_here__
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.438284 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/
--rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      953 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)      648 2023-01-11 10:33:35.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py
--rw-r--r--   0 riccardo   (501) staff       (20)      299 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/get_runner_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py
--rw-r--r--   0 riccardo   (501) staff       (20)      787 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py
--rw-r--r--   0 riccardo   (501) staff       (20)      743 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      632 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py
--rw-r--r--   0 riccardo   (501) staff       (20)      638 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      697 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py
--rw-r--r--   0 riccardo   (501) staff       (20)      438 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/cookbook.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.449854 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group1/
--rw-r--r--   0 riccardo   (501) staff       (20)       49 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group1/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group1/cookbook1.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.462775 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group2/
--rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group2/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      523 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.465429 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/
--rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/cookbook3.py
--rw-r--r--   0 riccardo   (501) staff       (20)      114 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group2/zcookbook4.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.525749 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/
--rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      267 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/argparse_ok.py
--rw-r--r--   0 riccardo   (501) staff       (20)      368 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/argument_parser_raise_system_exit.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.527299 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/
--rw-r--r--   0 riccardo   (501) staff       (20)       46 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      259 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      274 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise_system_exit_str.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.530944 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/
--rw-r--r--   0 riccardo   (501) staff       (20)       70 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      148 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/skipped.py
--rw-r--r--   0 riccardo   (501) staff       (20)      186 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_syntax.py
--rw-r--r--   0 riccardo   (501) staff       (20)      162 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/keyboard_interrupt.py
--rw-r--r--   0 riccardo   (501) staff       (20)       44 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/missing_run_function.py
--rw-r--r--   0 riccardo   (501) staff       (20)      144 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/non_zero_exit.py
--rw-r--r--   0 riccardo   (501) staff       (20)      173 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_exception.py
--rw-r--r--   0 riccardo   (501) staff       (20)      154 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_0.py
--rw-r--r--   0 riccardo   (501) staff       (20)      164 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_9.py
--rw-r--r--   0 riccardo   (501) staff       (20)      170 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_str.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.534730 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/
--rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/cookbook4.py
--rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py
--rw-r--r--   0 riccardo   (501) staff       (20)      276 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/root.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.536314 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/debmonitor/
--rw-r--r--   0 riccardo   (501) staff       (20)      109 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/debmonitor/config.ini
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.542353 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/discovery/
--rw-r--r--   0 riccardo   (501) staff       (20)       80 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/discovery/authdns.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.548258 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/elasticsearch/
--rw-r--r--   0 riccardo   (501) staff       (20)       84 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/elasticsearch/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:56.942288 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/external_cookbook/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.561122 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/external_cookbook/cookbooks/
--rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/external_cookbook/cookbooks/__do_not_add_init_py_file_here__
--rw-r--r--   0 riccardo   (501) staff       (20)      456 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/external_cookbook/cookbooks/external_cookbook.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.564788 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      141 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/cookbook1.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.566754 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/external_modules/
--rw-r--r--   0 riccardo   (501) staff       (20)       32 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/external_modules/__init__.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.575333 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/external_modules/spicerack_ext/
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/external_modules/spicerack_ext/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      396 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/external_modules/spicerack_ext/cool_feature.py
--rw-r--r--   0 riccardo   (501) staff       (20)      695 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/external_modules/spicerack_extender.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.635059 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/ganeti/
--rw-r--r--   0 riccardo   (501) staff       (20)       96 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/ganeti/404.json
--rw-r--r--   0 riccardo   (501) staff       (20)       26 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/ganeti/bogus.json
--rw-r--r--   0 riccardo   (501) staff       (20)       53 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/ganeti/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)     8697 2020-11-03 18:42:40.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/ganeti/info.json
--rw-r--r--   0 riccardo   (501) staff       (20)     3398 2020-11-03 18:42:40.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/ganeti/instance.json
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.687368 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/
--rw-r--r--   0 riccardo   (501) staff       (20)      194 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_downtimed.json
--rw-r--r--   0 riccardo   (501) staff       (20)        4 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_invalid.json
--rw-r--r--   0 riccardo   (501) staff       (20)      214 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_missing.json
--rw-r--r--   0 riccardo   (501) staff       (20)      195 2022-06-06 10:26:19.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_valid.json
--rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json
--rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json
--rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json
--rw-r--r--   0 riccardo   (501) staff       (20)      196 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_with_empty_failed_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      768 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_with_failed_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      188 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_with_no_matching_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_with_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.692404 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/kafka/
--rw-r--r--   0 riccardo   (501) staff       (20)      347 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/kafka/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.695259 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/netbox/
--rw-r--r--   0 riccardo   (501) staff       (20)       82 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/netbox/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.698204 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/peeringdb/
--rw-r--r--   0 riccardo   (501) staff       (20)    11449 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/peeringdb/asn.json
--rw-r--r--   0 riccardo   (501) staff       (20)      797 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/peeringdb/ixlan.json
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.699528 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/phabricator/
--rw-r--r--   0 riccardo   (501) staff       (20)      100 2020-10-23 11:21:26.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/phabricator/valid.conf
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.700853 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/redis_cluster/
--rw-r--r--   0 riccardo   (501) staff       (20)      229 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/redis_cluster/cluster.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.707487 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/remote/
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/remote/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/remote/config_installer.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.713255 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/reposync/
--rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/reposync/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.720174 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/service/
--rw-r--r--   0 riccardo   (501) staff       (20)     3250 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/service/service.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)     2580 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/sphinx_checker.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.890285 wikimedia-spicerack-6.4.1/spicerack/tests/unit/
--rw-r--r--   0 riccardo   (501) staff       (20)       40 2018-08-25 07:06:49.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)    28172 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test__cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4574 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test__log.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2553 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_administrative.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3508 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_alerting.py
--rw-r--r--   0 riccardo   (501) staff       (20)    13229 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_alertmanager.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1957 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_apt.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8651 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_confctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_debmonitor.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5416 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_decorators.py
--rw-r--r--   0 riccardo   (501) staff       (20)    18840 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_dhcp.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12139 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_dnsdisc.py
--rw-r--r--   0 riccardo   (501) staff       (20)    42981 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_elasticsearch_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)    15541 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_ganeti.py
--rw-r--r--   0 riccardo   (501) staff       (20)    39132 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_icinga.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14385 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_init.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1186 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_interactive.py
--rw-r--r--   0 riccardo   (501) staff       (20)    20462 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_ipmi.py
--rw-r--r--   0 riccardo   (501) staff       (20)    24006 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_k8s.py
--rw-r--r--   0 riccardo   (501) staff       (20)     9470 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_kafka.py
--rw-r--r--   0 riccardo   (501) staff       (20)    11536 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_mediawiki.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3323 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_mysql.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10535 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_mysql_legacy.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14999 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_netbox.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4588 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_peeringdb.py
--rw-r--r--   0 riccardo   (501) staff       (20)    34515 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_puppet.py
--rw-r--r--   0 riccardo   (501) staff       (20)    44515 2023-03-30 15:21:09.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_redfish.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4275 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_redis_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)    22477 2023-03-28 16:38:16.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_remote.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5618 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_reposync.py
--rw-r--r--   0 riccardo   (501) staff       (20)    16842 2023-03-28 16:38:16.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_service.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.898352 wikimedia-spicerack-6.4.1/spicerack/tests/unit/toolforge/
--rw-r--r--   0 riccardo   (501) staff       (20)    28976 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/tests/unit/toolforge/test_etcdctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3639 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/tests/vulture_whitelist.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.905943 wikimedia-spicerack-6.4.1/spicerack/toolforge/
--rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.1/spicerack/toolforge/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)     9529 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/toolforge/etcdctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)      299 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.1/spicerack/typing.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2374 2023-03-28 16:38:16.000000 wikimedia-spicerack-6.4.1/tox.ini
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.916590 wikimedia-spicerack-6.4.1/utils/
--rwxr-xr-x   0 riccardo   (501) staff       (20)     1174 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/utils/check-style.sh
--rwxr-xr-x   0 riccardo   (501) staff       (20)      452 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.1/utils/format-code.sh
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-03-30 15:30:57.952230 wikimedia-spicerack-6.4.1/wikimedia_spicerack.egg-info/
--rw-r--r--   0 riccardo   (501) staff       (20)     1691 2023-03-30 15:30:56.000000 wikimedia-spicerack-6.4.1/wikimedia_spicerack.egg-info/PKG-INFO
--rw-r--r--   0 riccardo   (501) staff       (20)     9703 2023-03-30 15:30:56.000000 wikimedia-spicerack-6.4.1/wikimedia_spicerack.egg-info/SOURCES.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-03-30 15:30:56.000000 wikimedia-spicerack-6.4.1/wikimedia_spicerack.egg-info/dependency_links.txt
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-30 15:30:56.000000 wikimedia-spicerack-6.4.1/wikimedia_spicerack.egg-info/entry_points.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-03-30 15:30:56.000000 wikimedia-spicerack-6.4.1/wikimedia_spicerack.egg-info/not-zip-safe
--rw-r--r--   0 riccardo   (501) staff       (20)      647 2023-03-30 15:30:56.000000 wikimedia-spicerack-6.4.1/wikimedia_spicerack.egg-info/requires.txt
--rw-r--r--   0 riccardo   (501) staff       (20)       10 2023-03-30 15:30:56.000000 wikimedia-spicerack-6.4.1/wikimedia_spicerack.egg-info/top_level.txt
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:52.518626 wikimedia-spicerack-6.4.2/
+-rw-r--r--   0 riccardo   (501) staff       (20)       45 2018-08-06 08:05:22.000000 wikimedia-spicerack-6.4.2/.coveragerc
+-rw-r--r--   0 riccardo   (501) staff       (20)       84 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/.git-blame-ignore-revs
+-rw-r--r--   0 riccardo   (501) staff       (20)      292 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/.gitignore
+-rw-r--r--   0 riccardo   (501) staff       (20)       96 2018-08-06 08:05:22.000000 wikimedia-spicerack-6.4.2/.gitreview
+-rw-r--r--   0 riccardo   (501) staff       (20)      668 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/.mailmap
+-rw-r--r--   0 riccardo   (501) staff       (20)      207 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/.wmfconfig
+-rw-r--r--   0 riccardo   (501) staff       (20)   104056 2023-04-17 16:31:29.000000 wikimedia-spicerack-6.4.2/CHANGELOG.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      271 2018-08-06 08:05:22.000000 wikimedia-spicerack-6.4.2/COPYRIGHT
+-rw-r--r--   0 riccardo   (501) staff       (20)    34686 2018-08-06 08:05:22.000000 wikimedia-spicerack-6.4.2/LICENSE
+-rw-r--r--   0 riccardo   (501) staff       (20)     1691 2023-04-17 16:46:52.519043 wikimedia-spicerack-6.4.2/PKG-INFO
+-rw-r--r--   0 riccardo   (501) staff       (20)      443 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/README.rst
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:49.255108 wikimedia-spicerack-6.4.2/doc/
+-rw-r--r--   0 riccardo   (501) staff       (20)      611 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/doc/Makefile
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:49.256811 wikimedia-spicerack-6.4.2/doc/examples/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1801 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/examples/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:49.332229 wikimedia-spicerack-6.4.2/doc/source/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:49.334326 wikimedia-spicerack-6.4.2/doc/source/_static/
+-rw-r--r--   0 riccardo   (501) staff       (20)      369 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/doc/source/_static/theme_overrides.css
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:49.795046 wikimedia-spicerack-6.4.2/doc/source/api/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1051 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/doc/source/api/index.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      101 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.administrative.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.alerting.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.alertmanager.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       39 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.apt.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.confctl.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.constants.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.cookbook.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.debmonitor.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      112 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.decorators.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.dhcp.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.dnsdisc.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       93 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.elasticsearch_cluster.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.exceptions.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.ganeti.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.icinga.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       63 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.interactive.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.ipmi.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       43 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.k8s.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       46 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.kafka.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.mediawiki.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       45 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.mysql.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       66 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.mysql_legacy.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.netbox.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.peeringdb.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.puppet.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.redfish.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       69 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.redis_cluster.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.remote.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.reposync.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.service.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       81 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.toolforge.etcdctl.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.toolforge.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/doc/source/api/spicerack.typing.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     6670 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/doc/source/conf.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      831 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/doc/source/configuration.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/doc/source/cookbook.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     2722 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/development.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       44 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/doc/source/docutils.conf
+-rw-r--r--   0 riccardo   (501) staff       (20)      384 2022-02-08 17:32:11.000000 wikimedia-spicerack-6.4.2/doc/source/index.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     1227 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/doc/source/installation.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     9468 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/doc/source/introduction.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       62 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/doc/source/release.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/prospector.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      258 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/pyproject.toml
+-rw-r--r--   0 riccardo   (501) staff       (20)      565 2023-04-17 16:46:52.624861 wikimedia-spicerack-6.4.2/setup.cfg
+-rwxr-xr-x   0 riccardo   (501) staff       (20)     3281 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/setup.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.379719 wikimedia-spicerack-6.4.2/spicerack/
+-rw-r--r--   0 riccardo   (501) staff       (20)    27361 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/spicerack/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    17795 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/_cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3900 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/_log.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    18780 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/_menu.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1442 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/_module_api.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3478 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/administrative.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2769 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/alerting.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12766 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/alertmanager.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5853 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/apt.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8072 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/confctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      262 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/constants.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5988 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2141 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/debmonitor.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3869 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/decorators.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    10442 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/dhcp.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12124 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/spicerack/dnsdisc.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    30520 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/elasticsearch_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      550 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/exceptions.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    13849 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/ganeti.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    27163 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/icinga.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      848 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/interactive.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    10263 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/ipmi.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    18466 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/k8s.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14951 2023-04-17 16:31:29.000000 wikimedia-spicerack-6.4.2/spicerack/kafka.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14797 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/mediawiki.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3329 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/mysql.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14945 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/mysql_legacy.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    13278 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/netbox.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5157 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/peeringdb.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    20891 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/spicerack/puppet.py
+-rw-r--r--   0 riccardo   (501) staff       (20)        0 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/py.typed
+-rw-r--r--   0 riccardo   (501) staff       (20)    36793 2023-03-30 15:21:09.000000 wikimedia-spicerack-6.4.2/spicerack/redfish.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     6421 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/redis_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    27921 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/spicerack/remote.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     7111 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/reposync.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    23081 2023-04-17 16:31:29.000000 wikimedia-spicerack-6.4.2/spicerack/service.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.386947 wikimedia-spicerack-6.4.2/spicerack/tests/
+-rw-r--r--   0 riccardo   (501) staff       (20)      871 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/__init__.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.562800 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.566876 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/confctl/
+-rw-r--r--   0 riccardo   (501) staff       (20)       33 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/confctl/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      698 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/confctl/schema.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.569476 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/config/
+-rw-r--r--   0 riccardo   (501) staff       (20)       59 2020-10-23 11:19:20.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/config/valid.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       79 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      219 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/config_bad_external_modules.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       44 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/config_empty_base_dirs.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      216 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/config_external_modules.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      126 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/config_multiple_base_dirs.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      113 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/config_wrong_overrides.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:48.993912 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.622925 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/
+-rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/__do_not_add_init_py_file_here__
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.803489 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/
+-rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      953 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      648 2023-01-11 10:33:35.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      299 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/get_runner_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      787 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      743 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      632 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      638 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      697 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      438 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/cookbook.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.828194 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group1/
+-rw-r--r--   0 riccardo   (501) staff       (20)       49 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group1/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group1/cookbook1.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.899697 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group2/
+-rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group2/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      523 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:50.919420 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/
+-rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/cookbook3.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      114 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group2/zcookbook4.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.159012 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/
+-rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      267 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/argparse_ok.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      368 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/argument_parser_raise_system_exit.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.164216 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/
+-rw-r--r--   0 riccardo   (501) staff       (20)       46 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      259 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      274 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise_system_exit_str.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.255261 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/
+-rw-r--r--   0 riccardo   (501) staff       (20)       70 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      148 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/skipped.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      186 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_syntax.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      162 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/keyboard_interrupt.py
+-rw-r--r--   0 riccardo   (501) staff       (20)       44 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/missing_run_function.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      144 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/non_zero_exit.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      173 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_exception.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      154 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_0.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      164 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_9.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      170 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_str.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.259270 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/
+-rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/cookbook4.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      276 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/root.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.263743 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/debmonitor/
+-rw-r--r--   0 riccardo   (501) staff       (20)      109 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/debmonitor/config.ini
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.266512 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/discovery/
+-rw-r--r--   0 riccardo   (501) staff       (20)       80 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/discovery/authdns.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.267939 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/elasticsearch/
+-rw-r--r--   0 riccardo   (501) staff       (20)       84 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/elasticsearch/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:49.000014 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_cookbook/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.271368 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_cookbook/cookbooks/
+-rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_cookbook/cookbooks/__do_not_add_init_py_file_here__
+-rw-r--r--   0 riccardo   (501) staff       (20)      456 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_cookbook/cookbooks/external_cookbook.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.297131 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      141 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/cookbook1.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.377228 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_modules/
+-rw-r--r--   0 riccardo   (501) staff       (20)       32 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_modules/__init__.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.386252 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_modules/spicerack_ext/
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_modules/spicerack_ext/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      396 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_modules/spicerack_ext/cool_feature.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      695 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_modules/spicerack_extender.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.410001 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/ganeti/
+-rw-r--r--   0 riccardo   (501) staff       (20)       96 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/ganeti/404.json
+-rw-r--r--   0 riccardo   (501) staff       (20)       26 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/ganeti/bogus.json
+-rw-r--r--   0 riccardo   (501) staff       (20)       53 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/ganeti/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)     8697 2020-11-03 18:42:40.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/ganeti/info.json
+-rw-r--r--   0 riccardo   (501) staff       (20)     3398 2020-11-03 18:42:40.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/ganeti/instance.json
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.671811 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/
+-rw-r--r--   0 riccardo   (501) staff       (20)      194 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_downtimed.json
+-rw-r--r--   0 riccardo   (501) staff       (20)        4 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_invalid.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      214 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_missing.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      195 2022-06-06 10:26:19.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_valid.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      196 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_empty_failed_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      768 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_failed_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      188 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_no_matching_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.749223 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/kafka/
+-rw-r--r--   0 riccardo   (501) staff       (20)      347 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/kafka/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.758503 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/netbox/
+-rw-r--r--   0 riccardo   (501) staff       (20)       82 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/netbox/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.804776 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/peeringdb/
+-rw-r--r--   0 riccardo   (501) staff       (20)    11449 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/peeringdb/asn.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      797 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/peeringdb/ixlan.json
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.807678 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/phabricator/
+-rw-r--r--   0 riccardo   (501) staff       (20)      100 2020-10-23 11:21:26.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/phabricator/valid.conf
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.810737 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/redis_cluster/
+-rw-r--r--   0 riccardo   (501) staff       (20)      229 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/redis_cluster/cluster.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.815176 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/remote/
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/remote/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/remote/config_installer.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.817549 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/reposync/
+-rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/reposync/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:51.838797 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/service/
+-rw-r--r--   0 riccardo   (501) staff       (20)     3273 2023-04-17 16:31:29.000000 wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/service/service.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)     2580 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/sphinx_checker.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:52.378280 wikimedia-spicerack-6.4.2/spicerack/tests/unit/
+-rw-r--r--   0 riccardo   (501) staff       (20)       40 2018-08-25 07:06:49.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    28172 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test__cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4574 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test__log.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2553 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_administrative.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3508 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_alerting.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    13229 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_alertmanager.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1957 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_apt.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8651 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_confctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_debmonitor.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5416 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_decorators.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    18840 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_dhcp.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12139 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_dnsdisc.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    42981 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_elasticsearch_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    15541 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_ganeti.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    39132 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_icinga.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14385 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_init.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1186 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_interactive.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    20462 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_ipmi.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    24006 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_k8s.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     9470 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_kafka.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    11536 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_mediawiki.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3323 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_mysql.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    10535 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_mysql_legacy.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14999 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_netbox.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4588 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_peeringdb.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    34515 2023-03-28 16:38:15.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_puppet.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    44515 2023-03-30 15:21:09.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_redfish.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4275 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_redis_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    22477 2023-03-28 16:38:16.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_remote.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5618 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_reposync.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    16842 2023-03-28 16:38:16.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_service.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:52.380167 wikimedia-spicerack-6.4.2/spicerack/tests/unit/toolforge/
+-rw-r--r--   0 riccardo   (501) staff       (20)    28976 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/tests/unit/toolforge/test_etcdctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3676 2023-04-17 16:31:29.000000 wikimedia-spicerack-6.4.2/spicerack/tests/vulture_whitelist.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:52.433410 wikimedia-spicerack-6.4.2/spicerack/toolforge/
+-rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-6.4.2/spicerack/toolforge/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     9529 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/toolforge/etcdctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      299 2023-03-15 15:44:38.000000 wikimedia-spicerack-6.4.2/spicerack/typing.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2374 2023-03-28 16:38:16.000000 wikimedia-spicerack-6.4.2/tox.ini
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:52.440156 wikimedia-spicerack-6.4.2/utils/
+-rwxr-xr-x   0 riccardo   (501) staff       (20)     1174 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/utils/check-style.sh
+-rwxr-xr-x   0 riccardo   (501) staff       (20)      452 2023-03-14 11:49:21.000000 wikimedia-spicerack-6.4.2/utils/format-code.sh
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-17 16:46:52.517573 wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1691 2023-04-17 16:46:48.000000 wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/PKG-INFO
+-rw-r--r--   0 riccardo   (501) staff       (20)     9703 2023-04-17 16:46:48.000000 wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/SOURCES.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-04-17 16:46:48.000000 wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/dependency_links.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-04-17 16:46:48.000000 wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/entry_points.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-04-17 16:46:48.000000 wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/not-zip-safe
+-rw-r--r--   0 riccardo   (501) staff       (20)      647 2023-04-17 16:46:48.000000 wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/requires.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)       10 2023-04-17 16:46:48.000000 wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/top_level.txt
```

### Comparing `wikimedia-spicerack-6.4.1/.mailmap` & `wikimedia-spicerack-6.4.2/.mailmap`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/CHANGELOG.rst` & `wikimedia-spicerack-6.4.2/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 Spicerack Changelog
 -------------------
 
+`v6.4.2`_ (2023-04-17)
+^^^^^^^^^^^^^^^^^^^^^^
+
+Minor improvements
+""""""""""""""""""
+
+* kafka: remove setting to avoid checking the hostname in TLS certs as all clusters in production are now running
+  with PKI TLS certs that have the hostname in their CN.
+
+Bug fixes
+"""""""""
+
+* service: add ``httpbb_dir`` field that was added to the Puppet service catalog.
+
 `v6.4.1`_ (2023-03-30)
 ^^^^^^^^^^^^^^^^^^^^^^
 
 Bug fixes
 """""""""
 
 * redfish: update log entries location for Dell and make it compatible with different iDRAC versions.
@@ -2535,7 +2549,8 @@
 .. _`v6.1.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.1.0
 .. _`v6.2.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.2.0
 .. _`v6.2.1`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.2.1
 .. _`v6.2.2`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.2.2
 .. _`v6.3.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.3.0
 .. _`v6.4.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.4.0
 .. _`v6.4.1`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.4.1
+.. _`v6.4.2`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.4.2
```

### Comparing `wikimedia-spicerack-6.4.1/LICENSE` & `wikimedia-spicerack-6.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/PKG-INFO` & `wikimedia-spicerack-6.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikimedia-spicerack
-Version: 6.4.1
+Version: 6.4.2
 Summary: Automation framework for the WMF production infrastructure
 Home-page: https://github.com/wikimedia/operations-software-spicerack
 Author: Riccardo Coccioli
 Author-email: rcoccioli@wikimedia.org
 License: GPLv3+
 Keywords: wmf,automation,orchestration
 Platform: GNU/Linux
```

### Comparing `wikimedia-spicerack-6.4.1/doc/Makefile` & `wikimedia-spicerack-6.4.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/doc/examples/config.yaml` & `wikimedia-spicerack-6.4.2/doc/examples/config.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/doc/source/api/index.rst` & `wikimedia-spicerack-6.4.2/doc/source/api/index.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/doc/source/conf.py` & `wikimedia-spicerack-6.4.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/doc/source/configuration.rst` & `wikimedia-spicerack-6.4.2/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/doc/source/development.rst` & `wikimedia-spicerack-6.4.2/doc/source/development.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/doc/source/installation.rst` & `wikimedia-spicerack-6.4.2/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/doc/source/introduction.rst` & `wikimedia-spicerack-6.4.2/doc/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/prospector.yaml` & `wikimedia-spicerack-6.4.2/prospector.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/setup.cfg` & `wikimedia-spicerack-6.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/setup.py` & `wikimedia-spicerack-6.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/__init__.py` & `wikimedia-spicerack-6.4.2/spicerack/__init__.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/_cookbook.py` & `wikimedia-spicerack-6.4.2/spicerack/_cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/_log.py` & `wikimedia-spicerack-6.4.2/spicerack/_log.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/_menu.py` & `wikimedia-spicerack-6.4.2/spicerack/_menu.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/_module_api.py` & `wikimedia-spicerack-6.4.2/spicerack/_module_api.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/administrative.py` & `wikimedia-spicerack-6.4.2/spicerack/administrative.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/alerting.py` & `wikimedia-spicerack-6.4.2/spicerack/alerting.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/alertmanager.py` & `wikimedia-spicerack-6.4.2/spicerack/alertmanager.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/apt.py` & `wikimedia-spicerack-6.4.2/spicerack/apt.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/confctl.py` & `wikimedia-spicerack-6.4.2/spicerack/confctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/cookbook.py` & `wikimedia-spicerack-6.4.2/spicerack/cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/debmonitor.py` & `wikimedia-spicerack-6.4.2/spicerack/debmonitor.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/decorators.py` & `wikimedia-spicerack-6.4.2/spicerack/decorators.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/dhcp.py` & `wikimedia-spicerack-6.4.2/spicerack/dhcp.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/dnsdisc.py` & `wikimedia-spicerack-6.4.2/spicerack/dnsdisc.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/elasticsearch_cluster.py` & `wikimedia-spicerack-6.4.2/spicerack/elasticsearch_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/exceptions.py` & `wikimedia-spicerack-6.4.2/spicerack/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/ganeti.py` & `wikimedia-spicerack-6.4.2/spicerack/ganeti.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/icinga.py` & `wikimedia-spicerack-6.4.2/spicerack/icinga.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/interactive.py` & `wikimedia-spicerack-6.4.2/spicerack/interactive.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/ipmi.py` & `wikimedia-spicerack-6.4.2/spicerack/ipmi.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/k8s.py` & `wikimedia-spicerack-6.4.2/spicerack/k8s.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/kafka.py` & `wikimedia-spicerack-6.4.2/spicerack/kafka.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
             kafka_config: complete, available in Puppet, kafka definition.
             dry_run: enable dry run mode.
 
         """
         self._dry_run = dry_run
         self._site = consumer_definition.site
         context = ssl.create_default_context()
-        context.check_hostname = False  # TODO can be changed after https://phabricator.wikimedia.org/T291905
         crt_location = "/etc/ssl/certs/ca-certificates.crt"
         context.load_verify_locations(crt_location)
 
         logger.debug(
             "Creating kafka client (kafka consumer with site prefix) with SSL context (check_hostname: %s, "
             "verify_mode: %s) for cluster and site: %s, %s",
             context.check_hostname,
```

### Comparing `wikimedia-spicerack-6.4.1/spicerack/mediawiki.py` & `wikimedia-spicerack-6.4.2/spicerack/mediawiki.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/mysql.py` & `wikimedia-spicerack-6.4.2/spicerack/mysql.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/mysql_legacy.py` & `wikimedia-spicerack-6.4.2/spicerack/mysql_legacy.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/netbox.py` & `wikimedia-spicerack-6.4.2/spicerack/netbox.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/peeringdb.py` & `wikimedia-spicerack-6.4.2/spicerack/peeringdb.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/puppet.py` & `wikimedia-spicerack-6.4.2/spicerack/puppet.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/redfish.py` & `wikimedia-spicerack-6.4.2/spicerack/redfish.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/redis_cluster.py` & `wikimedia-spicerack-6.4.2/spicerack/redis_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/remote.py` & `wikimedia-spicerack-6.4.2/spicerack/remote.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/reposync.py` & `wikimedia-spicerack-6.4.2/spicerack/reposync.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/service.py` & `wikimedia-spicerack-6.4.2/spicerack/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,14 +417,15 @@
     port: int
     sites: list[str]
     state: str
     _dry_run: bool
     _alertmanager: AlertmanagerHosts
     aliases: list[str] = field(default_factory=list)
     discovery: Optional[ServiceDiscovery] = None
+    httpbb_dir: str = ""
     lvs: Optional[ServiceLVS] = None
     monitoring: Optional[ServiceMonitoring] = None
     page: bool = True  # Default value in Puppet.
     probes: list[dict] = field(default_factory=list)
     public_aliases: list[str] = field(default_factory=list)
     public_endpoint: str = ""
     role: str = ""
```

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/__init__.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/confctl/schema.yaml` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/confctl/schema.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/external_modules/spicerack_extender.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/external_modules/spicerack_extender.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/ganeti/info.json` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/ganeti/info.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/ganeti/instance.json` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/ganeti/instance.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_with_failed_services.json` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_failed_services.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_with_services.json` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_services.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/peeringdb/asn.json` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/peeringdb/asn.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/peeringdb/ixlan.json` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/peeringdb/ixlan.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/fixtures/service/service.yaml` & `wikimedia-spicerack-6.4.2/spicerack/tests/fixtures/service/service.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 service2:
   encryption: true
   role: "service2"
   public_endpoint: "service2"
   public_aliases:
     - "service2-alias"
   port: 443
+  httpbb_dir: service2
   description: service2 description
   probes:
     - type: http
       host: service2.wikimedia.org
   sites:
     - codfw
     - eqiad
```

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/sphinx_checker.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/sphinx_checker.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test__cookbook.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test__cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test__log.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test__log.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_administrative.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_administrative.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_alerting.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_alerting.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_alertmanager.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_alertmanager.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_apt.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_apt.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_confctl.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_confctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_debmonitor.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_debmonitor.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_decorators.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_dhcp.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_dhcp.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_dnsdisc.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_dnsdisc.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_elasticsearch_cluster.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_elasticsearch_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_ganeti.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_ganeti.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_icinga.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_icinga.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_init.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_init.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_interactive.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_interactive.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_ipmi.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_ipmi.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_k8s.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_k8s.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_kafka.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_kafka.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_mediawiki.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_mediawiki.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_mysql.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_mysql.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_mysql_legacy.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_mysql_legacy.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_netbox.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_netbox.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_peeringdb.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_peeringdb.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_puppet.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_puppet.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_redfish.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_redfish.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_redis_cluster.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_redis_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_remote.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_remote.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_reposync.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_reposync.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/test_service.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/test_service.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/unit/toolforge/test_etcdctl.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/unit/toolforge/test_etcdctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/spicerack/tests/vulture_whitelist.py` & `wikimedia-spicerack-6.4.2/spicerack/tests/vulture_whitelist.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 
 # Needed because of https://github.com/jendrikseipp/vulture/issues/264
 whitelist_service = Whitelist()
 whitelist_service.Service.aliases
 whitelist_service.Service.bgp
 whitelist_service.Service.depool_threshold
 whitelist_service.Service.encryption
+whitelist_service.Service.httpbb_dir
 whitelist_service.Service.lvs
 whitelist_service.Service.lvs_class
 whitelist_service.Service.monitors
 whitelist_service.Service.name
 whitelist_service.Service.page
 whitelist_service.Service.probes
 whitelist_service.Service.protocol
```

### Comparing `wikimedia-spicerack-6.4.1/spicerack/toolforge/etcdctl.py` & `wikimedia-spicerack-6.4.2/spicerack/toolforge/etcdctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/tox.ini` & `wikimedia-spicerack-6.4.2/tox.ini`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/utils/check-style.sh` & `wikimedia-spicerack-6.4.2/utils/check-style.sh`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/wikimedia_spicerack.egg-info/PKG-INFO` & `wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikimedia-spicerack
-Version: 6.4.1
+Version: 6.4.2
 Summary: Automation framework for the WMF production infrastructure
 Home-page: https://github.com/wikimedia/operations-software-spicerack
 Author: Riccardo Coccioli
 Author-email: rcoccioli@wikimedia.org
 License: GPLv3+
 Keywords: wmf,automation,orchestration
 Platform: GNU/Linux
```

### Comparing `wikimedia-spicerack-6.4.1/wikimedia_spicerack.egg-info/SOURCES.txt` & `wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-6.4.1/wikimedia_spicerack.egg-info/requires.txt` & `wikimedia-spicerack-6.4.2/wikimedia_spicerack.egg-info/requires.txt`

 * *Files identical despite different names*

