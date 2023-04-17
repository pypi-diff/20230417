# Comparing `tmp/digicloud-2.5.8.tar.gz` & `tmp/digicloud-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digicloud-2.5.8.tar", last modified: Tue May 10 08:37:21 2022, max compression
+gzip compressed data, was "digicloud-2.5.9.tar", last modified: Sun Jun 12 07:33:34 2022, max compression
```

## Comparing `digicloud-2.5.8.tar` & `digicloud-2.5.9.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-05-10 08:37:21.398012 digicloud-2.5.8/
--rw-rw-r--   0 user      (1000) user      (1000)    11339 2022-05-10 08:35:52.000000 digicloud-2.5.8/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       66 2022-05-10 08:35:52.000000 digicloud-2.5.8/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     1465 2022-05-10 08:37:21.398012 digicloud-2.5.8/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      495 2022-05-10 08:35:52.000000 digicloud-2.5.8/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-05-10 08:37:21.394012 digicloud-2.5.8/digicloud/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      209 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/__main__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-05-10 08:37:21.398012 digicloud-2.5.8/digicloud/cli/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/cli/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      416 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/cli/app.py
--rw-rw-r--   0 user      (1000) user      (1000)     1005 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/cli/formatters.py
--rw-rw-r--   0 user      (1000) user      (1000)     3825 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/cli/parseractions.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-05-10 08:37:21.398012 digicloud-2.5.8/digicloud/commands/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2753 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/access.py
--rw-rw-r--   0 user      (1000) user      (1000)     4703 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/account.py
--rw-rw-r--   0 user      (1000) user      (1000)     2644 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/base.py
--rw-rw-r--   0 user      (1000) user      (1000)     1934 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/config.py
--rw-rw-r--   0 user      (1000) user      (1000)    61785 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/edge.py
--rw-rw-r--   0 user      (1000) user      (1000)     1594 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/explain.py
--rw-rw-r--   0 user      (1000) user      (1000)      805 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/image.py
--rw-rw-r--   0 user      (1000) user      (1000)    25396 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/instance.py
--rw-rw-r--   0 user      (1000) user      (1000)     2371 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/instance_operations.py
--rw-rw-r--   0 user      (1000) user      (1000)     1605 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/instance_type.py
--rw-rw-r--   0 user      (1000) user      (1000)    24100 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/load_balancer.py
--rw-rw-r--   0 user      (1000) user      (1000)     9150 2022-05-10 08:36:21.000000 digicloud-2.5.8/digicloud/commands/namespace.py
--rw-rw-r--   0 user      (1000) user      (1000)     4451 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/network.py
--rw-rw-r--   0 user      (1000) user      (1000)     3077 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/quota.py
--rw-rw-r--   0 user      (1000) user      (1000)     1537 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/region.py
--rw-rw-r--   0 user      (1000) user      (1000)    11017 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/router.py
--rw-rw-r--   0 user      (1000) user      (1000)     6973 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/security.py
--rw-rw-r--   0 user      (1000) user      (1000)     4844 2022-05-10 08:36:21.000000 digicloud-2.5.8/digicloud/commands/snapshot.py
--rw-rw-r--   0 user      (1000) user      (1000)     2973 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/ssh_key.py
--rw-rw-r--   0 user      (1000) user      (1000)     8675 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/subnet.py
--rw-rw-r--   0 user      (1000) user      (1000)     7391 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/volume.py
--rw-rw-r--   0 user      (1000) user      (1000)    13224 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/commands/vpn.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-05-10 08:37:21.398012 digicloud-2.5.8/digicloud/documentations/
--rw-rw-r--   0 user      (1000) user      (1000)     1785 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations/digicloud.md
--rw-rw-r--   0 user      (1000) user      (1000)    11716 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations/edge.md
--rw-rw-r--   0 user      (1000) user      (1000)     2620 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations/firewall.md
--rw-rw-r--   0 user      (1000) user      (1000)     3960 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations/instance.md
--rw-rw-r--   0 user      (1000) user      (1000)     5449 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations/loadbalancer.md
--rw-rw-r--   0 user      (1000) user      (1000)      420 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations/login_required.md
--rw-rw-r--   0 user      (1000) user      (1000)     2196 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations/namespace.md
--rw-rw-r--   0 user      (1000) user      (1000)      929 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations/network.md
--rw-rw-r--   0 user      (1000) user      (1000)     2243 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations/public_ip.md
--rw-rw-r--   0 user      (1000) user      (1000)      932 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations/region.md
--rw-rw-r--   0 user      (1000) user      (1000)     2142 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations/router.md
--rw-rw-r--   0 user      (1000) user      (1000)     1254 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations/snapshot.md
--rw-rw-r--   0 user      (1000) user      (1000)     1842 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations/ssh-key.md
--rw-rw-r--   0 user      (1000) user      (1000)      554 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations/subnet.md
--rw-rw-r--   0 user      (1000) user      (1000)     1476 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations/volume.md
--rw-rw-r--   0 user      (1000) user      (1000)     4891 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations/vpn.md
--rw-rw-r--   0 user      (1000) user      (1000)      705 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/documentations.py
--rw-rw-r--   0 user      (1000) user      (1000)     4408 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/error_handlers.py
--rw-rw-r--   0 user      (1000) user      (1000)     2623 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/formatter.py
--rw-rw-r--   0 user      (1000) user      (1000)     1836 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/main.py
--rw-rw-r--   0 user      (1000) user      (1000)     4090 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/managers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5320 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/middlewares.py
--rw-rw-r--   0 user      (1000) user      (1000)    20680 2022-05-10 08:36:21.000000 digicloud-2.5.8/digicloud/schemas.py
--rw-rw-r--   0 user      (1000) user      (1000)      732 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/sentry.py
--rw-rw-r--   0 user      (1000) user      (1000)     1406 2022-05-10 08:35:52.000000 digicloud-2.5.8/digicloud/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-05-10 08:37:21.398012 digicloud-2.5.8/digicloud.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     1465 2022-05-10 08:37:21.000000 digicloud-2.5.8/digicloud.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1910 2022-05-10 08:37:21.000000 digicloud-2.5.8/digicloud.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-05-10 08:37:21.000000 digicloud-2.5.8/digicloud.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)    11726 2022-05-10 08:37:21.000000 digicloud-2.5.8/digicloud.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-05-10 08:37:21.000000 digicloud-2.5.8/digicloud.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       88 2022-05-10 08:37:21.000000 digicloud-2.5.8/digicloud.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2022-05-10 08:37:21.000000 digicloud-2.5.8/digicloud.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2022-05-10 08:37:21.398012 digicloud-2.5.8/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)    16010 2022-05-10 08:36:21.000000 digicloud-2.5.8/setup.py
+drwxrwxr-x   0 mahyar    (1000) mahyar    (1000)        0 2022-06-12 07:33:34.341476 digicloud-2.5.9/
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)    11339 2021-10-16 11:43:24.000000 digicloud-2.5.9/LICENSE
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)       66 2022-03-09 16:46:12.000000 digicloud-2.5.9/MANIFEST.in
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     1260 2022-06-12 07:33:34.341476 digicloud-2.5.9/PKG-INFO
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)      495 2021-10-16 11:43:24.000000 digicloud-2.5.9/README.md
+drwxrwxr-x   0 mahyar    (1000) mahyar    (1000)        0 2022-06-12 07:33:34.333476 digicloud-2.5.9/digicloud/
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)        0 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/__init__.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)      209 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/__main__.py
+drwxrwxr-x   0 mahyar    (1000) mahyar    (1000)        0 2022-06-12 07:33:34.333476 digicloud-2.5.9/digicloud/cli/
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)        0 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/cli/__init__.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)      416 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/cli/app.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     1005 2022-03-09 10:06:04.000000 digicloud-2.5.9/digicloud/cli/formatters.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     3825 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/cli/parseractions.py
+drwxrwxr-x   0 mahyar    (1000) mahyar    (1000)        0 2022-06-12 07:33:34.337476 digicloud-2.5.9/digicloud/commands/
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)        0 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/commands/__init__.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     2753 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/commands/access.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     4703 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/commands/account.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     2644 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/commands/base.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     1934 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/commands/config.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)    61785 2022-04-16 08:07:32.000000 digicloud-2.5.9/digicloud/commands/edge.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     1594 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/commands/explain.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)      805 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/commands/image.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)    25891 2022-06-12 06:38:21.000000 digicloud-2.5.9/digicloud/commands/instance.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     2371 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/commands/instance_operations.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     1605 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/commands/instance_type.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)    24100 2022-04-16 08:07:49.000000 digicloud-2.5.9/digicloud/commands/load_balancer.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     9150 2022-06-12 06:38:07.000000 digicloud-2.5.9/digicloud/commands/namespace.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     4451 2022-03-09 10:06:04.000000 digicloud-2.5.9/digicloud/commands/network.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     3077 2022-03-09 10:06:04.000000 digicloud-2.5.9/digicloud/commands/quota.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     1537 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/commands/region.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)    11017 2022-03-09 10:06:04.000000 digicloud-2.5.9/digicloud/commands/router.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     6973 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/commands/security.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     4844 2022-06-12 06:38:07.000000 digicloud-2.5.9/digicloud/commands/snapshot.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     2973 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/commands/ssh_key.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     8675 2021-11-22 12:24:29.000000 digicloud-2.5.9/digicloud/commands/subnet.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     7391 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/commands/volume.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)    13224 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/commands/vpn.py
+drwxrwxr-x   0 mahyar    (1000) mahyar    (1000)        0 2022-06-12 07:33:34.341476 digicloud-2.5.9/digicloud/documentations/
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     1785 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/documentations/digicloud.md
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)    11716 2022-04-16 08:07:42.000000 digicloud-2.5.9/digicloud/documentations/edge.md
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     2620 2021-11-22 12:24:29.000000 digicloud-2.5.9/digicloud/documentations/firewall.md
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     4045 2022-06-12 06:38:21.000000 digicloud-2.5.9/digicloud/documentations/instance.md
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     5449 2022-04-16 08:07:49.000000 digicloud-2.5.9/digicloud/documentations/loadbalancer.md
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)      420 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/documentations/login_required.md
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     2196 2022-03-09 10:06:04.000000 digicloud-2.5.9/digicloud/documentations/namespace.md
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)      929 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/documentations/network.md
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     2243 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/documentations/public_ip.md
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)      932 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/documentations/region.md
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     2142 2022-03-09 10:06:04.000000 digicloud-2.5.9/digicloud/documentations/router.md
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     1254 2022-04-16 08:07:24.000000 digicloud-2.5.9/digicloud/documentations/snapshot.md
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     1842 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/documentations/ssh-key.md
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)      554 2021-11-22 12:24:29.000000 digicloud-2.5.9/digicloud/documentations/subnet.md
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     1476 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/documentations/volume.md
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     4891 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/documentations/vpn.md
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)      705 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/documentations.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     4408 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/error_handlers.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     2623 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/formatter.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     1836 2022-02-27 07:50:19.000000 digicloud-2.5.9/digicloud/main.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     4090 2022-03-18 12:50:30.000000 digicloud-2.5.9/digicloud/managers.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     5320 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/middlewares.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)    20680 2022-06-12 06:38:07.000000 digicloud-2.5.9/digicloud/schemas.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)      732 2021-10-16 11:43:24.000000 digicloud-2.5.9/digicloud/sentry.py
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     1406 2022-04-05 08:52:57.000000 digicloud-2.5.9/digicloud/utils.py
+drwxrwxr-x   0 mahyar    (1000) mahyar    (1000)        0 2022-06-12 07:33:34.333476 digicloud-2.5.9/digicloud.egg-info/
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     1260 2022-06-12 07:33:34.000000 digicloud-2.5.9/digicloud.egg-info/PKG-INFO
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)     1910 2022-06-12 07:33:34.000000 digicloud-2.5.9/digicloud.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)        1 2022-06-12 07:33:34.000000 digicloud-2.5.9/digicloud.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)    11726 2022-06-12 07:33:34.000000 digicloud-2.5.9/digicloud.egg-info/entry_points.txt
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)        1 2022-06-12 07:33:34.000000 digicloud-2.5.9/digicloud.egg-info/not-zip-safe
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)       88 2022-06-12 07:33:34.000000 digicloud-2.5.9/digicloud.egg-info/requires.txt
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)       10 2022-06-12 07:33:34.000000 digicloud-2.5.9/digicloud.egg-info/top_level.txt
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)       38 2022-06-12 07:33:34.341476 digicloud-2.5.9/setup.cfg
+-rw-rw-r--   0 mahyar    (1000) mahyar    (1000)    16010 2022-06-12 07:29:55.000000 digicloud-2.5.9/setup.py
```

### Comparing `digicloud-2.5.8/LICENSE` & `digicloud-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/cli/formatters.py` & `digicloud-2.5.9/digicloud/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/cli/parseractions.py` & `digicloud-2.5.9/digicloud/cli/parseractions.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/access.py` & `digicloud-2.5.9/digicloud/commands/access.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/account.py` & `digicloud-2.5.9/digicloud/commands/account.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/base.py` & `digicloud-2.5.9/digicloud/commands/base.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/config.py` & `digicloud-2.5.9/digicloud/commands/config.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/edge.py` & `digicloud-2.5.9/digicloud/commands/edge.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/explain.py` & `digicloud-2.5.9/digicloud/commands/explain.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/image.py` & `digicloud-2.5.9/digicloud/commands/image.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/instance.py` & `digicloud-2.5.9/digicloud/commands/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
     DigiCloud Compute Instance Service.
 """
 from rich.prompt import Confirm
 
 from digicloud import schemas
 from .base import Lister, ShowOne, Command
+from ..cli import parseractions
 from ..error_handlers import CLIError
 from ..utils import is_tty
 
 
 class ListInstance(Lister):
     """List instances."""
     schema = schemas.InstanceList(many=True)
@@ -144,19 +145,21 @@
             '--public-ip',
             required=False,
             metavar='<public_ip>',
             help='Public IP name or ID to use after instance creation'
         )
 
         parser.add_argument(
-            '--additional-volumes',
-            metavar='<additional_volumes>',
+            '--additional-volume',
+            metavar='size=<size>,type=<type>',
+            dest='additional_volumes',
+            action=parseractions.MultiKeyValueAction,
+            required_keys=['size', 'type'],
             default=[],
-            action='append',
-            help='attach additional volume automatically, e.g --additional-volumes 500'
+            help='Create and attach additional volume automatically, e.g --additional-volume size=500,type=SSD'
         )
 
         parser.add_argument(
             '--advanced',
             help='Create a instance with more configuration parameters',
             default=None,
             action='store_true'
@@ -205,17 +208,23 @@
             ),
             (
                 parsed_args.public_ip and parsed_args.count is not None,
                 "--public-ip and --count must not be used together",
             ),
             (
                 parsed_args.additional_volumes and parsed_args.count is not None,
-                "using --additional-volumes and --count together is not supported",
+                "using --additional-volume and --count together is not supported",
+            ),
+            (
+                any([
+                    str(volume['type']).upper() not in ('SSD', 'ULTRA_DISK')
+                    for volume in parsed_args.additional_volumes
+                ]),
+                "additional volume type must be either 'SSD' or 'ULTRA_DISK'"
             ),
-
             (
                 parsed_args.image and parsed_args.snapshot,
                 "--image and --snapshot must not be used together",
             ),
             (
                 parsed_args.image is None and parsed_args.snapshot is None,
                 "one of the --image and --snapshot arguments must be used",
@@ -248,17 +257,17 @@
         if parsed_args.ssh_key:
             payload['ssh_key_name'] = parsed_args.ssh_key
         if parsed_args.firewall:
             payload['security_groups'] = parsed_args.firewall
         if parsed_args.additional_volumes:
             payload['additional_volumes'] = [
                 {
-                    "size": volume_size,
-                    "volume_type": "SSD",
-                } for volume_size in parsed_args.additional_volumes
+                    "size": additional_volume['size'],
+                    "volume_type": additional_volume['type'],
+                } for additional_volume in parsed_args.additional_volumes
             ]
         if parsed_args.with_public_ip:
             payload['has_public_ip'] = parsed_args.with_public_ip
         if parsed_args.public_ip:
             payload['public_ip'] = parsed_args.public_ip
         if parsed_args.description:
             payload['description'] = parsed_args.description
```

### Comparing `digicloud-2.5.8/digicloud/commands/instance_operations.py` & `digicloud-2.5.9/digicloud/commands/instance_operations.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/instance_type.py` & `digicloud-2.5.9/digicloud/commands/instance_type.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/load_balancer.py` & `digicloud-2.5.9/digicloud/commands/load_balancer.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/namespace.py` & `digicloud-2.5.9/digicloud/commands/namespace.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/network.py` & `digicloud-2.5.9/digicloud/commands/network.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/quota.py` & `digicloud-2.5.9/digicloud/commands/quota.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/region.py` & `digicloud-2.5.9/digicloud/commands/region.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/router.py` & `digicloud-2.5.9/digicloud/commands/router.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/security.py` & `digicloud-2.5.9/digicloud/commands/security.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/snapshot.py` & `digicloud-2.5.9/digicloud/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/ssh_key.py` & `digicloud-2.5.9/digicloud/commands/ssh_key.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/subnet.py` & `digicloud-2.5.9/digicloud/commands/subnet.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/volume.py` & `digicloud-2.5.9/digicloud/commands/volume.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/commands/vpn.py` & `digicloud-2.5.9/digicloud/commands/vpn.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/documentations/digicloud.md` & `digicloud-2.5.9/digicloud/documentations/digicloud.md`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/documentations/edge.md` & `digicloud-2.5.9/digicloud/documentations/edge.md`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/documentations/firewall.md` & `digicloud-2.5.9/digicloud/documentations/firewall.md`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/documentations/instance.md` & `digicloud-2.5.9/digicloud/documentations/instance.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,20 +39,21 @@
                         --simple \
                         --instance-type g1.micro \
                         --image Debian_9 \
                         --root-volume-size 50 \
                         --root-volume-type ULTRA_DISK
     or
 
-        # Creating an advanced instance with an additional volume
+        # Creating an advanced instance with two additional volumes
         $ digicloud instance create backup_server
                         --network my_network \
                         --instance-type g1.micro \
                         --image Debian_9
-                        --additional-volume 500
+                        --additional-volume size=64,type=SSD
+                        --additional-volume size=2048,type=ULTRA_DISK
     or
 
         # Creating an advanced (or simple) instance from an existing snapshot 
         $ digicloud instance create backup_server
                         --network my_network \
                         --instance-type g1.micro \
                         --snapshot My_Snapshot
```

### Comparing `digicloud-2.5.8/digicloud/documentations/loadbalancer.md` & `digicloud-2.5.9/digicloud/documentations/loadbalancer.md`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/documentations/namespace.md` & `digicloud-2.5.9/digicloud/documentations/namespace.md`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/documentations/network.md` & `digicloud-2.5.9/digicloud/documentations/network.md`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/documentations/public_ip.md` & `digicloud-2.5.9/digicloud/documentations/public_ip.md`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/documentations/region.md` & `digicloud-2.5.9/digicloud/documentations/region.md`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/documentations/router.md` & `digicloud-2.5.9/digicloud/documentations/router.md`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/documentations/snapshot.md` & `digicloud-2.5.9/digicloud/documentations/snapshot.md`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/documentations/ssh-key.md` & `digicloud-2.5.9/digicloud/documentations/ssh-key.md`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/documentations/subnet.md` & `digicloud-2.5.9/digicloud/documentations/subnet.md`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/documentations/volume.md` & `digicloud-2.5.9/digicloud/documentations/volume.md`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/documentations/vpn.md` & `digicloud-2.5.9/digicloud/documentations/vpn.md`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/documentations.py` & `digicloud-2.5.9/digicloud/documentations.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/error_handlers.py` & `digicloud-2.5.9/digicloud/error_handlers.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/formatter.py` & `digicloud-2.5.9/digicloud/formatter.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/main.py` & `digicloud-2.5.9/digicloud/main.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/managers.py` & `digicloud-2.5.9/digicloud/managers.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/middlewares.py` & `digicloud-2.5.9/digicloud/middlewares.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/schemas.py` & `digicloud-2.5.9/digicloud/schemas.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/sentry.py` & `digicloud-2.5.9/digicloud/sentry.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud/utils.py` & `digicloud-2.5.9/digicloud/utils.py`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud.egg-info/SOURCES.txt` & `digicloud-2.5.9/digicloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/digicloud.egg-info/entry_points.txt` & `digicloud-2.5.9/digicloud.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `digicloud-2.5.8/setup.py` & `digicloud-2.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 try:
     LONG_DESCRIPTION = open('README.md', 'rt').read()
 except IOError:
     LONG_DESCRIPTION = ''
 
 setup(
     name='digicloud',
-    version='2.5.8',
+    version='2.5.9',
     description='DigiCloud CLI',
 
     long_description=LONG_DESCRIPTION,
 
     author='Arash Shams',
     author_email='a.shams@digikala.com',
     url='https://digicloud.ir',
```

