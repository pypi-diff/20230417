# Comparing `tmp/hcs-cli-0.1.28.tar.gz` & `tmp/hcs-cli-0.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.28.tar", last modified: Tue Apr 11 23:24:51 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.29.tar", last modified: Mon Apr 17 21:14:58 2023, max compression
```

## Comparing `hcs-cli-0.1.28.tar` & `hcs-cli-0.1.29.tar`

### file list

```diff
@@ -1,128 +1,129 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.274489 hcs-cli-0.1.28/
--rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.28/.gitignore
--rw-r--r--   0 nanw       (501) staff       (20)       82 2023-04-07 18:36:38.000000 hcs-cli-0.1.28/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)      701 2023-04-08 01:22:34.000000 hcs-cli-0.1.28/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-11 23:24:51.274052 hcs-cli-0.1.28/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     1486 2023-04-11 01:01:20.000000 hcs-cli-0.1.28/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.168485 hcs-cli-0.1.28/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-11 23:24:50.000000 hcs-cli-0.1.28/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     2782 2023-04-11 23:24:51.000000 hcs-cli-0.1.28/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-04-11 23:24:50.000000 hcs-cli-0.1.28/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-04-11 23:24:50.000000 hcs-cli-0.1.28/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      142 2023-04-11 23:24:50.000000 hcs-cli-0.1.28/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-04-11 23:24:50.000000 hcs-cli-0.1.28/hcs_cli.egg-info/top_level.txt
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.148573 hcs-cli-0.1.28/payload/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.169422 hcs-cli-0.1.28/payload/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-11 00:40:07.000000 hcs-cli-0.1.28/payload/lcm/zero.json
--rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-07 16:11:06.000000 hcs-cli-0.1.28/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      142 2023-04-08 01:21:33.000000 hcs-cli-0.1.28/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-04-11 23:24:51.275841 hcs-cli-0.1.28/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)      544 2023-04-11 23:24:25.000000 hcs-cli-0.1.28/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.171269 hcs-cli-0.1.28/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:50.000000 hcs-cli-0.1.28/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:42.000000 hcs-cli-0.1.28/tests/conftest.py
--rw-r--r--   0 nanw       (501) staff       (20)     2425 2023-04-08 01:06:36.000000 hcs-cli-0.1.28/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.172366 hcs-cli-0.1.28/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:35.000000 hcs-cli-0.1.28/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.172941 hcs-cli-0.1.28/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:38.000000 hcs-cli-0.1.28/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.176741 hcs-cli-0.1.28/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:39.000000 hcs-cli-0.1.28/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.178339 hcs-cli-0.1.28/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:41.000000 hcs-cli-0.1.28/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 21:57:30.000000 hcs-cli-0.1.28/tests/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)      290 2023-04-08 01:06:36.000000 hcs-cli-0.1.28/tests/vhcs/cli/cmds/test_auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     1343 2023-04-08 01:06:36.000000 hcs-cli-0.1.28/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-08 01:16:54.000000 hcs-cli-0.1.28/tests/vhcs/cli/cmds/test_profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.178900 hcs-cli-0.1.28/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.28/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.179920 hcs-cli-0.1.28/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.181564 hcs-cli-0.1.28/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.182082 hcs-cli-0.1.28/vhcs/cli/cmds/admin/
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-10 16:58:33.000000 hcs-cli-0.1.28/vhcs/cli/cmds/admin/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.184833 hcs-cli-0.1.28/vhcs/cli/cmds/admin/edge/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:21:00.000000 hcs-cli-0.1.28/vhcs/cli/cmds/admin/edge/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      343 2023-04-10 19:16:01.000000 hcs-cli-0.1.28/vhcs/cli/cmds/admin/edge/get.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-10 16:21:00.000000 hcs-cli-0.1.28/vhcs/cli/cmds/admin/edge/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.188605 hcs-cli-0.1.28/vhcs/cli/cmds/admin/template/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:20:13.000000 hcs-cli-0.1.28/vhcs/cli/cmds/admin/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      351 2023-04-10 19:13:27.000000 hcs-cli-0.1.28/vhcs/cli/cmds/admin/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1393 2023-04-10 17:45:24.000000 hcs-cli-0.1.28/vhcs/cli/cmds/admin/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)      375 2023-04-07 18:22:47.000000 hcs-cli-0.1.28/vhcs/cli/cmds/auth.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.191659 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.195104 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      196 2023-04-07 18:26:01.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      187 2023-04-07 18:26:21.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      380 2023-04-11 01:00:36.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.201698 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1289 2023-04-11 00:52:05.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)      474 2023-04-11 00:46:01.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      235 2023-04-11 23:21:14.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      962 2023-04-10 19:04:36.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1693 2023-04-10 21:48:05.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:18:56.000000 hcs-cli-0.1.28/vhcs/cli/cmds/lcm/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.208136 hcs-cli-0.1.28/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.28/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-07 18:26:57.000000 hcs-cli-0.1.28/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      297 2023-04-07 18:27:02.000000 hcs-cli-0.1.28/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      163 2023-04-07 18:27:20.000000 hcs-cli-0.1.28/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-04-06 22:12:04.000000 hcs-cli-0.1.28/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:21:03.000000 hcs-cli-0.1.28/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.211043 hcs-cli-0.1.28/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3644 2023-04-08 01:06:36.000000 hcs-cli-0.1.28/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      332 2023-04-07 18:23:32.000000 hcs-cli-0.1.28/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.215986 hcs-cli-0.1.28/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-06 17:42:33.000000 hcs-cli-0.1.28/vhcs/cli/cmds/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      662 2023-04-07 18:27:15.000000 hcs-cli-0.1.28/vhcs/cli/cmds/vmhub/redeem-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      567 2023-04-07 18:27:38.000000 hcs-cli-0.1.28/vhcs/cli/cmds/vmhub/request-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      110 2023-04-07 18:22:14.000000 hcs-cli-0.1.28/vhcs/cli/cmds/vmhub/test.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2397 2023-04-11 23:19:57.000000 hcs-cli-0.1.28/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.218441 hcs-cli-0.1.28/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.239035 hcs-cli-0.1.28/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-10 18:35:40.000000 hcs-cli-0.1.28/vhcs/common/ctxp/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.244025 hcs-cli-0.1.28/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1419 2023-04-07 23:54:52.000000 hcs-cli-0.1.28/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     1817 2023-04-08 01:12:13.000000 hcs-cli-0.1.28/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     4139 2023-04-11 23:07:45.000000 hcs-cli-0.1.28/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/common/ctxp/cli_state.py
--rw-r--r--   0 nanw       (501) staff       (20)      337 2023-04-07 00:28:47.000000 hcs-cli-0.1.28/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-07 00:28:55.000000 hcs-cli-0.1.28/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     5680 2023-04-07 00:18:58.000000 hcs-cli-0.1.28/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)      548 2023-04-07 16:49:23.000000 hcs-cli-0.1.28/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     2128 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     3695 2023-04-08 01:06:36.000000 hcs-cli-0.1.28/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     2157 2023-04-11 23:18:54.000000 hcs-cli-0.1.28/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2633 2023-04-07 00:29:18.000000 hcs-cli-0.1.28/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     4246 2023-04-07 00:37:01.000000 hcs-cli-0.1.28/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.252591 hcs-cli-0.1.28/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)       54 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2504 2023-04-07 00:18:58.000000 hcs-cli-0.1.28/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     3601 2023-04-07 00:18:58.000000 hcs-cli-0.1.28/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     3866 2023-04-10 22:09:28.000000 hcs-cli-0.1.28/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      549 2023-04-07 19:17:10.000000 hcs-cli-0.1.28/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      370 2023-04-10 18:29:50.000000 hcs-cli-0.1.28/vhcs/common/sglib/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.255216 hcs-cli-0.1.28/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7327 2023-04-06 17:22:27.000000 hcs-cli-0.1.28/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.264113 hcs-cli-0.1.28/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      986 2023-04-10 16:58:33.000000 hcs-cli-0.1.28/vhcs/service/_util.py
--rw-r--r--   0 nanw       (501) staff       (20)      822 2023-04-10 19:16:10.000000 hcs-cli-0.1.28/vhcs/service/admin.py
--rw-r--r--   0 nanw       (501) staff       (20)     3199 2023-04-11 01:04:04.000000 hcs-cli-0.1.28/vhcs/service/lcm.py
--rw-r--r--   0 nanw       (501) staff       (20)      610 2023-04-07 21:33:14.000000 hcs-cli-0.1.28/vhcs/service/pki.py
--rw-r--r--   0 nanw       (501) staff       (20)      929 2023-04-07 19:31:02.000000 hcs-cli-0.1.28/vhcs/service/vmhub.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-11 23:24:51.272030 hcs-cli-0.1.28/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/util/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2160 2023-04-10 21:32:09.000000 hcs-cli-0.1.28/vhcs/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     4699 2023-04-06 02:05:21.000000 hcs-cli-0.1.28/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1127 2023-04-10 19:16:42.000000 hcs-cli-0.1.28/vhcs/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)      832 2023-04-07 19:01:08.000000 hcs-cli-0.1.28/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.214221 hcs-cli-0.1.29/
+-rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.29/.gitignore
+-rw-r--r--   0 nanw       (501) staff       (20)       82 2023-04-07 18:36:38.000000 hcs-cli-0.1.29/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)      729 2023-04-17 20:42:14.000000 hcs-cli-0.1.29/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-17 21:14:58.213666 hcs-cli-0.1.29/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     1486 2023-04-11 01:01:20.000000 hcs-cli-0.1.29/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.104380 hcs-cli-0.1.29/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-17 21:14:57.000000 hcs-cli-0.1.29/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     2804 2023-04-17 21:14:58.000000 hcs-cli-0.1.29/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-04-17 21:14:57.000000 hcs-cli-0.1.29/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-04-17 21:14:57.000000 hcs-cli-0.1.29/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      168 2023-04-17 21:14:57.000000 hcs-cli-0.1.29/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-04-17 21:14:57.000000 hcs-cli-0.1.29/hcs_cli.egg-info/top_level.txt
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.076564 hcs-cli-0.1.29/payload/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.105369 hcs-cli-0.1.29/payload/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-11 00:40:07.000000 hcs-cli-0.1.29/payload/lcm/zero.json
+-rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-07 16:11:06.000000 hcs-cli-0.1.29/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      168 2023-04-17 20:59:09.000000 hcs-cli-0.1.29/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-04-17 21:14:58.214354 hcs-cli-0.1.29/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)      545 2023-04-17 21:14:53.000000 hcs-cli-0.1.29/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.107544 hcs-cli-0.1.29/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:50.000000 hcs-cli-0.1.29/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:42.000000 hcs-cli-0.1.29/tests/conftest.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2425 2023-04-08 01:06:36.000000 hcs-cli-0.1.29/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.108685 hcs-cli-0.1.29/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:35.000000 hcs-cli-0.1.29/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.109779 hcs-cli-0.1.29/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:38.000000 hcs-cli-0.1.29/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.114317 hcs-cli-0.1.29/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:39.000000 hcs-cli-0.1.29/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.116570 hcs-cli-0.1.29/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:41.000000 hcs-cli-0.1.29/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 21:57:30.000000 hcs-cli-0.1.29/tests/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)      290 2023-04-08 01:06:36.000000 hcs-cli-0.1.29/tests/vhcs/cli/cmds/test_auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1343 2023-04-08 01:06:36.000000 hcs-cli-0.1.29/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-08 01:16:54.000000 hcs-cli-0.1.29/tests/vhcs/cli/cmds/test_profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.117448 hcs-cli-0.1.29/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.29/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.119222 hcs-cli-0.1.29/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.123858 hcs-cli-0.1.29/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.124966 hcs-cli-0.1.29/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-10 16:58:33.000000 hcs-cli-0.1.29/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.129598 hcs-cli-0.1.29/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:21:00.000000 hcs-cli-0.1.29/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      341 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-10 16:21:00.000000 hcs-cli-0.1.29/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.135816 hcs-cli-0.1.29/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:20:13.000000 hcs-cli-0.1.29/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      349 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1235 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/cli/cmds/admin/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)      375 2023-04-07 18:22:47.000000 hcs-cli-0.1.29/vhcs/cli/cmds/auth.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.140051 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.144993 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      196 2023-04-07 18:26:01.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      187 2023-04-07 18:26:21.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      382 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.153213 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1257 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)      474 2023-04-11 00:46:01.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      235 2023-04-11 23:21:14.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      957 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:18:56.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.160779 hcs-cli-0.1.29/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.29/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-07 18:26:57.000000 hcs-cli-0.1.29/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      297 2023-04-07 18:27:02.000000 hcs-cli-0.1.29/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      163 2023-04-07 18:27:20.000000 hcs-cli-0.1.29/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-04-06 22:12:04.000000 hcs-cli-0.1.29/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:21:03.000000 hcs-cli-0.1.29/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.163422 hcs-cli-0.1.29/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3840 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      171 2023-04-17 21:14:07.000000 hcs-cli-0.1.29/vhcs/cli/cmds/test.py
+-rw-r--r--   0 nanw       (501) staff       (20)      332 2023-04-07 18:23:32.000000 hcs-cli-0.1.29/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.170119 hcs-cli-0.1.29/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-06 17:42:33.000000 hcs-cli-0.1.29/vhcs/cli/cmds/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      662 2023-04-07 18:27:15.000000 hcs-cli-0.1.29/vhcs/cli/cmds/vmhub/redeem-otp.py
+-rw-r--r--   0 nanw       (501) staff       (20)      567 2023-04-07 18:27:38.000000 hcs-cli-0.1.29/vhcs/cli/cmds/vmhub/request-otp.py
+-rw-r--r--   0 nanw       (501) staff       (20)      110 2023-04-07 18:22:14.000000 hcs-cli-0.1.29/vhcs/cli/cmds/vmhub/test.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2413 2023-04-17 21:01:02.000000 hcs-cli-0.1.29/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.172582 hcs-cli-0.1.29/vhcs/common/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/common/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.186532 hcs-cli-0.1.29/vhcs/common/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/common/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-10 18:35:40.000000 hcs-cli-0.1.29/vhcs/common/ctxp/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.190881 hcs-cli-0.1.29/vhcs/common/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/common/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1419 2023-04-07 23:54:52.000000 hcs-cli-0.1.29/vhcs/common/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1819 2023-04-17 21:08:13.000000 hcs-cli-0.1.29/vhcs/common/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4139 2023-04-11 23:07:45.000000 hcs-cli-0.1.29/vhcs/common/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/common/ctxp/cli_state.py
+-rw-r--r--   0 nanw       (501) staff       (20)      337 2023-04-07 00:28:47.000000 hcs-cli-0.1.29/vhcs/common/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-07 00:28:55.000000 hcs-cli-0.1.29/vhcs/common/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5680 2023-04-07 00:18:58.000000 hcs-cli-0.1.29/vhcs/common/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)      548 2023-04-07 16:49:23.000000 hcs-cli-0.1.29/vhcs/common/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2128 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/common/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3954 2023-04-17 21:10:37.000000 hcs-cli-0.1.29/vhcs/common/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2157 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/common/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2633 2023-04-07 00:29:18.000000 hcs-cli-0.1.29/vhcs/common/ctxp/var_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4246 2023-04-07 00:37:01.000000 hcs-cli-0.1.29/vhcs/common/logger.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.198389 hcs-cli-0.1.29/vhcs/common/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)       54 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/common/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2504 2023-04-07 00:18:58.000000 hcs-cli-0.1.29/vhcs/common/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3601 2023-04-07 00:18:58.000000 hcs-cli-0.1.29/vhcs/common/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3853 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/common/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      549 2023-04-07 19:17:10.000000 hcs-cli-0.1.29/vhcs/common/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      370 2023-04-10 18:29:50.000000 hcs-cli-0.1.29/vhcs/common/sglib/util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.201035 hcs-cli-0.1.29/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7327 2023-04-06 17:22:27.000000 hcs-cli-0.1.29/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.207460 hcs-cli-0.1.29/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      985 2023-04-17 21:09:33.000000 hcs-cli-0.1.29/vhcs/service/_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)      823 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/service/admin.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3194 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/service/lcm.py
+-rw-r--r--   0 nanw       (501) staff       (20)      610 2023-04-07 21:33:14.000000 hcs-cli-0.1.29/vhcs/service/pki.py
+-rw-r--r--   0 nanw       (501) staff       (20)      929 2023-04-07 19:31:02.000000 hcs-cli-0.1.29/vhcs/service/vmhub.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.212862 hcs-cli-0.1.29/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/util/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2159 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4699 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1127 2023-04-10 19:16:42.000000 hcs-cli-0.1.29/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)      832 2023-04-07 19:01:08.000000 hcs-cli-0.1.29/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.28/.gitignore` & `hcs-cli-0.1.29/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/Makefile` & `hcs-cli-0.1.29/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 lint:
 	python3 -m black .	
 
 build:
 	export SCM_REV=$(shell git rev-parse --short HEAD); \
 	python3 setup.py sdist bdist_wheel
 
+update:
+	pipreqs . --force
+
 buildrelease:
 	python3 setup.py sdist bdist_wheel
 
 uninstall:
 	pip3 uninstall -y hcs-cli
 
 devinstall:
```

### Comparing `hcs-cli-0.1.28/PKG-INFO` & `hcs-cli-0.1.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.28
+Version: 0.1.29
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/nanw1103/hcs-cli
 Project-URL: Bug Tracker, https://github.com/nanw1103/hcs-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/nanw1103/hcs-cli
 Project-URL: changelog, https://github.com/nanw1103/hcs-cli/blob/master/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.28/README.md` & `hcs-cli-0.1.29/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/hcs_cli.egg-info/PKG-INFO` & `hcs-cli-0.1.29/hcs_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.28
+Version: 0.1.29
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/nanw1103/hcs-cli
 Project-URL: Bug Tracker, https://github.com/nanw1103/hcs-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/nanw1103/hcs-cli
 Project-URL: changelog, https://github.com/nanw1103/hcs-cli/blob/master/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.28/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.29/hcs_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 tests/vhcs/cli/cmds/pki/__init__.py
 tests/vhcs/cli/cmds/pki/get_root_ca.py
 vhcs/__init__.py
 vhcs/cli/__init__.py
 vhcs/cli/main.py
 vhcs/cli/cmds/__init__.py
 vhcs/cli/cmds/auth.py
+vhcs/cli/cmds/test.py
 vhcs/cli/cmds/upgrade.py
 vhcs/cli/cmds/admin/__init__.py
 vhcs/cli/cmds/admin/edge/__init__.py
 vhcs/cli/cmds/admin/edge/get.py
 vhcs/cli/cmds/admin/edge/list.py
 vhcs/cli/cmds/admin/template/__init__.py
 vhcs/cli/cmds/admin/template/get.py
```

### Comparing `hcs-cli-0.1.28/payload/lcm/zero.json` & `hcs-cli-0.1.29/payload/lcm/zero.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/pyproject.toml` & `hcs-cli-0.1.29/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/setup.py` & `hcs-cli-0.1.29/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from setuptools_scm import get_version
 import os
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-VERSION = "0.1.28"
+VERSION = "0.1.29"
+
 
 def get_version():
     version = VERSION
     local_version = os.environ.get("SCM_REV")
     if local_version:
         version += "+" + local_version
     return version
```

### Comparing `hcs-cli-0.1.28/tests/test_utils.py` & `hcs-cli-0.1.29/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.29/tests/vhcs/cli/cmds/test_context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/tests/vhcs/cli/cmds/test_profile.py` & `hcs-cli-0.1.29/tests/vhcs/cli/cmds/test_profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/cli/cmds/admin/template/list.py` & `hcs-cli-0.1.29/vhcs/cli/cmds/admin/template/list.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,26 +4,33 @@
 
 
 @click.command()
 @click.option("--limit", "-l", type=int, required=False, default=20, help="Optionally, specify cloud provider type.")
 @option_org_id
 @click.option("--brokerable-only", type=bool, required=False, default=False)
 @click.option("--expanded", type=bool, required=False, default=False)
-@click.option("--reported-search", type=str, required=False, help="Search expression for selection of template reported properties")
+@click.option(
+    "--reported-search",
+    type=str,
+    required=False,
+    help="Search expression for selection of template reported properties",
+)
 @click.option("--template-search", type=str, required=False, help="Search expression for selection of templates")
-@click.option("--sort", type=str, required=False, help="Ascending/Descending. Format is property,{asc|desc} and default is ascending")
-def list(limit: int, 
-         org: str, 
-         brokerable_only: bool,
-         expanded: bool,
-         reported_search: str,
-         template_search: str,
-         sort: str
-         ):
+@click.option(
+    "--sort",
+    type=str,
+    required=False,
+    help="Ascending/Descending. Format is property,{asc|desc} and default is ascending",
+)
+def list(
+    limit: int, org: str, brokerable_only: bool, expanded: bool, reported_search: str, template_search: str, sort: str
+):
     """List templates"""
-    return admin.template.list(limit, 
-                               org_id = get_org_id(org),
-                               borkerable_only = brokerable_only,
-                               expanded = expanded,
-                               reported_search = reported_search,
-                               template_search = template_search,
-                               sort = sort)
+    return admin.template.list(
+        limit,
+        org_id=get_org_id(org),
+        borkerable_only=brokerable_only,
+        expanded=expanded,
+        reported_search=reported_search,
+        template_search=template_search,
+        sort=sort,
+    )
```

### Comparing `hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/create.py` & `hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/create.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,32 +24,30 @@
         payload = file.read()
 
     try:
         template = json.loads(payload)
     except Exception as e:
         msg = "Invalid template: " + str(e)
         return msg, 1
-    
-    template['id'] = _rand_id(16)
+
+    template["id"] = _rand_id(16)
     org_id = get_org_id(org)
-    template['orgId'] = org_id
+    template["orgId"] = org_id
 
     provider = _create_zerocloud_provider(org_id)
-    template['provider']['providerAccessId'] = provider['id']
+    template["provider"]["providerAccessId"] = provider["id"]
 
     ret = lcm.template.create(template)
 
     if id_only:
         return ret.get("id")
     return ret
 
+
 def _rand_id(n: int):
-    return ''.join(random.choices("abcdefghijkmnpqrstuvwxyz23456789", k=n))
+    return "".join(random.choices("abcdefghijkmnpqrstuvwxyz23456789", k=n))
+
 
 def _create_zerocloud_provider(org_id: str):
-    data = {
-        "name": "nanw-test-" + _rand_id(4),
-        "orgId": org_id,
-        "type": "ZEROCLOUD"
-    }
+    data = {"name": "nanw-test-" + _rand_id(4), "orgId": org_id, "type": "ZEROCLOUD"}
 
     return lcm.provider.create(data)
```

### Comparing `hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/list.py` & `hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import click
 from vhcs.service import lcm
 from vhcs.common.sglib.util import option_org_id, get_org_id
 from vhcs.common.ctxp.util import option_id_only
 
+
 @click.command("list")
 @click.option("--limit", "-l", type=int, required=False, default=20, help="Optionally, specify cloud provider type.")
 @option_org_id
 @option_id_only
 @click.option("--type", "-t", type=str, required=False, help="Optionally, specify cloud provider type.")
 @click.option("--name", "-n", type=str, required=False, help="Optionally, specify name pattern to find.")
 def list_templates(limit: int, org: str, id_only: bool, type: str, name: str):
     """List templates"""
     if org == "all":
         ret = lcm.template.list(limit, name=name, type=type)
     else:
         ret = lcm.template.list(limit, org_id=get_org_id(org), name=name, type=type)
 
     if id_only:
+
         def _get_id_only(t):
             return t.get("id")
+
         return list(map(_get_id_only, ret))
-        
+
     return ret
```

### Comparing `hcs-cli-0.1.28/vhcs/cli/cmds/lcm/template/wait.py` & `hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/wait.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 import click
 from vhcs.service import lcm
 from vhcs.util import duration
 
 
 @click.command()
 @click.argument("id", type=str, required=True)
-@click.option("--status", "-s", 
-              type=click.Choice(["READY", "ERROR", "DELETING", "EXPANDING", "SHRINKING", "CUSTOMIZING", "MAINTENANCE"]), 
-              required=False, 
-              default="READY",
-              help="The target status to wait for.")
-@click.option("--timeout", "-t", type=str, required=False, default="1m",
-              help="Timeout. Examples: '2m', '30s', '1h30m'")
+@click.option(
+    "--status",
+    "-s",
+    type=click.Choice(["READY", "ERROR", "DELETING", "EXPANDING", "SHRINKING", "CUSTOMIZING", "MAINTENANCE"]),
+    required=False,
+    default="READY",
+    help="The target status to wait for.",
+)
+@click.option("--timeout", "-t", type=str, required=False, default="1m", help="Timeout. Examples: '2m', '30s', '1h30m'")
 @click.option(
     "--fail-fast/--fail-timeout-only",
     "-f",
     type=bool,
     default=True,
     required=False,
     help="Stop waiting if the template reached to non-expected terminal states, e.g. waiting for ERROR but template is READY, or waiting for READY and template is ERROR.",
 )
-@click.option("--silent/--return-template", type=bool, required=False, default=True,
-              help="Slient mode will has no output on success. Otherwise the full template is returned")
+@click.option(
+    "--silent/--return-template",
+    type=bool,
+    required=False,
+    default=True,
+    help="Slient mode will has no output on success. Otherwise the full template is returned",
+)
 def wait(id: str, status: str, timeout: str, fail_fast: bool, silent: bool):
     """Wait for a template to transit to specific status. If the template"""
 
     timeout_seconds = duration.to_seconds(timeout)
     expected_status = status.upper().split(",")
     exclude_status = []
     if fail_fast:
```

### Comparing `hcs-cli-0.1.28/vhcs/cli/cmds/pki/delete_org_cert.py` & `hcs-cli-0.1.29/vhcs/cli/cmds/pki/delete_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/cli/cmds/pki/sign_resource_cert.py` & `hcs-cli-0.1.29/vhcs/cli/cmds/pki/sign_resource_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/cli/cmds/profile/init.py` & `hcs-cli-0.1.29/vhcs/cli/cmds/profile/init.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,20 +71,24 @@
 def init(name: str, recreate_defaults: bool, property: list):
     """Init profile interactively"""
 
     _create_default_profiles(recreate_defaults)
     _create_nightly_profile(recreate_defaults)
 
     print()
-    print("Preparing profile: " + name)
-    doc = _copy_profile("nightly")
+    if profile.exists(name):
+        print("Updating existing profile: " + name)
+        doc = profile.get(name)
+    else:
+        print("Preparing profile: " + name)
+        doc = _copy_profile("nightly")
 
     hcs_url = doc.hcs.url
     doc.hcs.url = click.prompt("HCS URL", type=str, show_default=True, default=hcs_url)
-    region_url = doc.hcs.regions[0].url
+    region_url = doc.hcs.regions[0].url or ""
     region_url = click.prompt("HCS region URL", type=str, show_default=True, default=region_url)
     doc.hcs.regions[0].url = region_url
     doc.csp.url = _get_csp_url(doc.hcs.url)
 
     while True:
         default_val = doc.csp.apiToken or ""
         csp_api_token = click.prompt("CSP API Token", type=str, default=default_val, show_default=True)
@@ -105,8 +109,9 @@
             if csp_client_key:
                 doc.csp.clientId = csp_client_id
                 doc.csp.clientKey = csp_client_key
                 break
         break
 
     profile.create(name, doc)
+    print("Profile created as " + profile.file(name))
     return profile.current()
```

### Comparing `hcs-cli-0.1.28/vhcs/cli/cmds/vmhub/redeem-otp.py` & `hcs-cli-0.1.29/vhcs/cli/cmds/vmhub/redeem-otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/cli/cmds/vmhub/request-otp.py` & `hcs-cli-0.1.29/vhcs/cli/cmds/vmhub/request-otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/cli/main.py` & `hcs-cli-0.1.29/vhcs/cli/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,32 +21,35 @@
 
 logger.setup()
 logging.getLogger("charset_normalizer").setLevel(logging.WARN)
 logging.getLogger("csp").setLevel(logging.INFO)
 logging.getLogger("context").setLevel(logging.WARN)
 logging.getLogger("init").setLevel(logging.WARN)
 logging.getLogger("profile").setLevel(logging.WARN)
+logging.getLogger("httpx").setLevel(logging.WARN)
 # -----------------------------------------------------------
 
 
 @click.group()
 @click.version_option(package_name="hcs-cli")
 @option_verbose
 @option_output
 @option_field
 @click.option("--profile", "-p", type=str, required=False, help="Specify the profile to use. Optional.")
 @click.option("--upgrade-check/--no-upgrade-check", default=True, help="Check new version of HCS CLI.")
 @click.option("--telemetry/--no-telemetry", default=True, help="Send telemetry")
 def cli(**kwargs):
 
-    if kwargs.get('upgrade_check'):
+    upgrade_check = kwargs.get("upgrade_check")
+    if upgrade_check:
         from vhcs.util.versions import check_upgrade
+
         check_upgrade()
-        
-    profile = kwargs.get('profile')
+
+    profile = kwargs.get("profile")
     if profile:
         ctxp.profile._active_profile_name = profile
 
 
 # @cli.result_callback()
 # def _process_result(result, **kwargs):
 #     print("_process_result", result, kwargs)
@@ -58,22 +61,19 @@
         commands_dir = path.join(_module_dir, "cli/cmds")
         config_path = path.join(_module_dir, "config")
         ctxp.init(cli_name="hcs", main_cli=cli, commands_dir=commands_dir, config_path=config_path)
     except ctxp.CtxpException as e:
         ctxp.panic(e)
     except httpx.HTTPStatusError as e:
         import traceback
+
         traceback.print_exc()
         try:
             err = json.loads(e.response.text)
         except:
-            err = {
-                "message": str(e),
-                "response": e.response.text,
-                "resource": str(e.request.url)
-            }
+            err = {"message": str(e), "response": e.response.text, "resource": str(e.request.url)}
         text = json.dumps(err, indent=4)
         ctxp.panic(text)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hcs-cli-0.1.28/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.29/vhcs/common/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/common/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.29/vhcs/common/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/common/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.29/vhcs/common/ctxp/built_in_cmds/profile.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     if name:
         data = ctxp.profile.get(name)
     else:
         data = ctxp.profile.current()
 
     if data == None:
         ctxp.panic(
-            "Profile not set. Use 'hcs profile use <profile-name>' to choose one, or 'hcs profile init' to crate"
+            "Profile not set. Use 'hcs profile use <profile-name>' to choose one, or 'hcs profile init' to create."
         )
     return data
 
 
 @profile.command()
 @click.argument("name")
 def delete(name: str):
```

### Comparing `hcs-cli-0.1.28/vhcs/common/ctxp/cli_processor.py` & `hcs-cli-0.1.29/vhcs/common/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/common/ctxp/context.py` & `hcs-cli-0.1.29/vhcs/common/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.29/vhcs/common/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/common/ctxp/init.py` & `hcs-cli-0.1.29/vhcs/common/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/common/ctxp/jsondot.py` & `hcs-cli-0.1.29/vhcs/common/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/common/ctxp/profile.py` & `hcs-cli-0.1.29/vhcs/common/ctxp/profile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .util import CtxpException
+from .util import CtxpException, panic
 from .jsondot import dotdict
 from .fstore import fstore
 
 
 _store: fstore = None
 _active_profile_name: str = None
 _plain: dotdict = None
@@ -26,22 +26,27 @@
 
 
 def create(name: str, data: dict) -> None:
     _store.save(name, data)
     use(name)
 
 
-def current(reload: bool = False) -> dict:
+def current(reload: bool = False, exit_on_failure = True) -> dict:
     """Get content of the current active profile"""
     profile_name = name()
     if not profile_name:
         raise CtxpException("Profile not specified")
     data = get(profile_name, reload)
     global _plain
     _plain = None
+
+    if data is None and exit_on_failure:
+        panic(
+            "Profile not set. Use 'hcs profile list' to list and 'hcs profile use <profile-name>' to choose one, or use 'hcs profile init' to create a profile."
+        )
     return data
 
 
 def name() -> str:
     """Get the current active profile name"""
 
     global _active_profile_name
```

### Comparing `hcs-cli-0.1.28/vhcs/common/ctxp/util.py` & `hcs-cli-0.1.29/vhcs/common/ctxp/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,30 +16,32 @@
 
         if output == "json":
             text = json.dumps(data, indent=4)
         elif output == "json-compact":
             text = json.dumps(data)
         elif output == "yaml":
             import vhcs.common.ctxp as ctxp
+
             text = yaml.dump(ctxp.jsondot.plain(data))
         elif output == "text":
             if isinstance(data, list):
                 text = ""
                 for i in data:
                     line = i if type(i) is str else json.dumps(i)
                     text += line + "\n"
             elif isinstance(data, dict):
                 text = json.dumps(data, indent=4)
             else:
                 text = json.dumps(data, indent=4)
         else:
             raise Exception(f"Unexpected output format: {output}")
-    
+
     print(text, end="")
 
+
 def _filter_fields(obj: any, fields: str):
     if not fields:
         return obj
     parts = fields.split(",")
 
     def _filter_obj(o):
         if not isinstance(o, dict):
@@ -49,14 +51,15 @@
                 del o[k]
         return o
 
     if isinstance(obj, list):
         return list(map(_filter_obj, obj))
     return _filter_obj(obj)
 
+
 def panic(reason: any = None, code: int = 1):
     print(reason, file=sys.stderr)
     sys.exit(code)
 
 
 option_verbose = click.option(
     "-v",
@@ -83,9 +86,9 @@
 )
 
 option_id_only = click.option(
     "--id-only/--full-object",
     type=bool,
     default=False,
     required=False,
-    help="Output only the object, instead of the full data object"
+    help="Output only the object, instead of the full data object",
 )
```

### Comparing `hcs-cli-0.1.28/vhcs/common/ctxp/var_template.py` & `hcs-cli-0.1.29/vhcs/common/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/common/logger.py` & `hcs-cli-0.1.29/vhcs/common/logger.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/common/sglib/auth.py` & `hcs-cli-0.1.29/vhcs/common/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/common/sglib/csp.py` & `hcs-cli-0.1.29/vhcs/common/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/common/sglib/ez_client.py` & `hcs-cli-0.1.29/vhcs/common/sglib/ez_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 log = logging.getLogger(__name__)
 
 log_http_details = False
 
 
 def _raise_on_4xx_5xx(response: httpx.Response):
-    
+
     if not response.is_success:
         response.read()
         if len(response.text) > 0:
             text = _try_formatting_json(response.text)
             log.debug(text)
 
     response.raise_for_status()
@@ -76,14 +76,15 @@
         resp = func()
         return _parse_resp(resp)
     except httpx.HTTPStatusError as e:
         if e.response.status_code == 404:
             return None
         raise
 
+
 class EzClient:
     def __init__(self, base_url: str, get_auth: callable = None) -> None:
         event_hooks = {"response": [_raise_on_4xx_5xx]}
         event_hooks["request"] = [_log_request]
         event_hooks["response"].insert(0, _log_response)
 
         self._client = httpx.Client(base_url=base_url, timeout=30, event_hooks=event_hooks)
@@ -110,15 +111,14 @@
             if e.response.status_code == 404 and raise_on_404:
                 raise e
 
     def patch(self, url: str, json: dict):
         self.login()
         resp = self._client.patch(url, json=json)
         return _parse_resp(resp)
-        
 
     def delete(self, url: str, raise_on_404: bool = False):
         self.login()
         try:
             return self._client.delete(url)
         except httpx.HTTPStatusError as e:
             if not raise_on_404 and e.response.status_code == 404:
@@ -130,8 +130,7 @@
         return _parse_resp(resp)
 
     def close(self):
         self._client.close()
 
     def dump_response(self, response: HTTPResponse):
         log.info("response text: " + response.text())
-
```

### Comparing `hcs-cli-0.1.28/vhcs/common/sglib/hcs_client.py` & `hcs-cli-0.1.29/vhcs/common/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.29/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/service/_util.py` & `hcs-cli-0.1.29/vhcs/service/_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from vhcs.common.ctxp import profile, panic
 from vhcs.common.sglib import hcs_client
 
-
 def hdc_service_client(service_name: str):
     url = profile.current().hcs.url
     if not url.endswith("/"):
         url += "/"
     url += service_name
     return hcs_client(url)
```

### Comparing `hcs-cli-0.1.28/vhcs/service/admin.py` & `hcs-cli-0.1.29/vhcs/service/admin.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         return _client.get(url)
 
     @staticmethod
     def list(limit: int = 10, **kwargs):
         def _get_page(query_string):
             url = "/v2/templates?" + query_string
             return _client.get(url)
+
         return PageRequest(_get_page, limit, **kwargs).get()
 
 
 class edge:
     @staticmethod
     def get(id: str, **kwargs):
         url = with_query(f"/v2/edge-deployments/{id}", **kwargs)
```

### Comparing `hcs-cli-0.1.28/vhcs/service/lcm.py` & `hcs-cli-0.1.29/vhcs/service/lcm.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,29 +16,30 @@
     def list(limit: int = 20, name: str = None, **kwargs):
         def _get_page(query_string):
             url = "/v1/templates?" + query_string
             return _client.get(url)
 
         ret = PageRequest(_get_page, limit, **kwargs).get()
         if name:
-            #filter_fn = lambda t : t.name.find(name) >= 0
+            # filter_fn = lambda t : t.name.find(name) >= 0
             def filter_fn(t):
                 return t.name.find(name) >= 0
+
             ret = list(filter(filter_fn, ret))
         return ret
 
     @staticmethod
     def delete(id: str, org_id: str, force: bool):
         resp = _client.delete(f"/v1/templates/{id}?org_id={org_id}&force={force}")
         return _convert_resp(resp)
 
     @staticmethod
     def create(template: dict):
         url = "/v1/templates"
-        url += "/" + template['providerType'].lower()
+        url += "/" + template["providerType"].lower()
         return _client.post(url=url, json=template)
 
     @staticmethod
     def wait(
         id: str,
         expected_status: list,
         timeout_seconds: int,
@@ -89,23 +90,24 @@
         return PageRequest(_get_page, limit, **kwargs).get()
 
     @staticmethod
     def delete(id: str):
         resp = _client.delete(f"/v1/providers/{id}")
         return _convert_resp(resp)
 
-
     @staticmethod
     def create(data: dict):
-        url = "/v1/providers/" + data['type'].lower()
+        url = "/v1/providers/" + data["type"].lower()
         return _client.post(url, json=data)
 
+
 def _convert_resp(resp):
     if resp:
         resp.read()
         try:
             json.loads(resp.text)
         except:
             return resp.text
-        
+
+
 def test():
     print("test")
```

### Comparing `hcs-cli-0.1.28/vhcs/service/pki.py` & `hcs-cli-0.1.29/vhcs/service/pki.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/service/vmhub.py` & `hcs-cli-0.1.29/vhcs/service/vmhub.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/util/duration.py` & `hcs-cli-0.1.29/vhcs/util/duration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import re
 
 PATTERN = re.compile("^(([0-9]+)D)?(([0-9]+)H)?(([0-9]+)M)?(([0-9]+)S)?$")
 
 
 # Examples
 
@@ -30,36 +29,38 @@
     if m:
         total_seconds += int(m) * 60
     if s:
         total_seconds += int(s)
 
     return total_seconds
 
+
 def to_duration(seconds: int) -> str:
     ONE_MINUTE = 60
     ONE_HOUR = ONE_MINUTE * 60
     ONE_DAY = ONE_HOUR * 24
     days = int(seconds / ONE_DAY)
     seconds %= ONE_DAY
     hours = int(seconds / ONE_HOUR)
     seconds %= ONE_HOUR
     minutes = int(seconds / ONE_MINUTE)
     seconds %= ONE_MINUTE
 
-    ret = ''
+    ret = ""
     if days > 0:
-        ret += f'{days}D'
+        ret += f"{days}D"
     if hours > 0:
-        ret += f'{hours}H'
+        ret += f"{hours}H"
     if minutes > 0:
-        ret += f'{minutes}M'
+        ret += f"{minutes}M"
     if seconds > 0:
-        ret += f'{seconds}S'
+        ret += f"{seconds}S"
     return ret
 
+
 def _test():
     data = {
         "14S": 14,
         "13M": 13 * 60,
         "12H": 12 * 3600,
         "11D": 11 * 24 * 3600,
         "13M14S": 13 * 60 + 14,
@@ -68,18 +69,18 @@
         "12H13M": 12 * 3600 + 13 * 60,
         "11D13M": 11 * 24 * 3600 + 13 * 60,
         "11D12H": 11 * 24 * 3600 + 12 * 3600,
         "11D12H13M": 11 * 24 * 3600 + 12 * 3600 + 13 * 60,
         "11D12H14S": 11 * 24 * 3600 + 12 * 3600 + 14,
         "11D13M14S": 11 * 24 * 3600 + 13 * 60 + 14,
         "12H13M14S": 12 * 3600 + 13 * 60 + 14,
-        "11D12H13M14S": 11 * 24 * 3600 + 12 * 3600 + 13 * 60 + 14
+        "11D12H13M14S": 11 * 24 * 3600 + 12 * 3600 + 13 * 60 + 14,
     }
     for k in data.keys():
         v = data[k]
-        assert to_seconds(k) == v, f'to_seconds failed: k={k},v={v},got={to_seconds(k)}'
-        assert to_duration(v) == k, f'to_duration failed: k={k},v={v},got={to_duration(v)}'
+        assert to_seconds(k) == v, f"to_seconds failed: k={k},v={v},got={to_seconds(k)}"
+        assert to_duration(v) == k, f"to_duration failed: k={k},v={v},got={to_duration(v)}"
     print("PASS")
-    
+
 
 if __name__ == "__main__":
-    _test()
+    _test()
```

### Comparing `hcs-cli-0.1.28/vhcs/util/pki_util.py` & `hcs-cli-0.1.29/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/util/query_util.py` & `hcs-cli-0.1.29/vhcs/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.28/vhcs/util/versions.py` & `hcs-cli-0.1.29/vhcs/util/versions.py`

 * *Files identical despite different names*

