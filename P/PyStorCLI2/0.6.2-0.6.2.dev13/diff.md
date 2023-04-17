# Comparing `tmp/PyStorCLI2-0.6.2.tar.gz` & `tmp/PyStorCLI2-0.6.2.dev13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyStorCLI2-0.6.2.tar", last modified: Mon Apr 17 14:51:13 2023, max compression
+gzip compressed data, was "PyStorCLI2-0.6.2.dev13.tar", last modified: Mon Apr 17 14:47:41 2023, max compression
```

## Comparing `PyStorCLI2-0.6.2.tar` & `PyStorCLI2-0.6.2.dev13.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.832631 PyStorCLI2-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.812631 PyStorCLI2-0.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.816631 PyStorCLI2-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.816631 PyStorCLI2-0.6.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-17 14:51:13.832631 PyStorCLI2-0.6.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.816631 PyStorCLI2-0.6.2/PyStorCLI2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-17 14:51:13.000000 PyStorCLI2-0.6.2/PyStorCLI2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-17 14:51:13.000000 PyStorCLI2-0.6.2/PyStorCLI2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:51:13.000000 PyStorCLI2-0.6.2/PyStorCLI2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-17 14:51:13.000000 PyStorCLI2-0.6.2/PyStorCLI2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-17 14:51:13.000000 PyStorCLI2-0.6.2/PyStorCLI2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 14:51:13.000000 PyStorCLI2-0.6.2/PyStorCLI2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.820631 PyStorCLI2-0.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-17 14:50:46.000000 PyStorCLI2-0.6.2/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (123)   857298 2023-04-17 14:50:46.000000 PyStorCLI2-0.6.2/docs/pystorcli2.html
--rw-r--r--   0 runner    (1001) docker     (123)   371378 2023-04-17 14:50:46.000000 PyStorCLI2-0.6.2/docs/search.js
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.820631 PyStorCLI2-0.6.2/pystorcli/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli/cachevault.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli/cmdRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli/storcli.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 14:51:13.000000 PyStorCLI2-0.6.2/pystorcli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.820631 PyStorCLI2-0.6.2/pystorcli2/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.820631 PyStorCLI2-0.6.2/pystorcli2/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5262 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/bin/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/cachevault.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/cmdRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.824631 PyStorCLI2-0.6.2/pystorcli2/controller/
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/controller/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.824631 PyStorCLI2-0.6.2/pystorcli2/drive/
--rw-r--r--   0 runner    (1001) docker     (123)    18691 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/drive/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/drive/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.824631 PyStorCLI2-0.6.2/pystorcli2/enclosure/
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/enclosure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/storcli.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-17 14:51:13.000000 PyStorCLI2-0.6.2/pystorcli2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.824631 PyStorCLI2-0.6.2/pystorcli2/virtualdrive/
--rw-r--r--   0 runner    (1001) docker     (123)    23271 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/virtualdrive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/virtualdrive/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/virtualdrive/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli2/virtualdrive/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.824631 PyStorCLI2-0.6.2/pystorcli_mirror/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/pystorcli_mirror/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:51:13.832631 PyStorCLI2-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.824631 PyStorCLI2-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/baseTest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.816631 PyStorCLI2-0.6.2/tests/datatest/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.816631 PyStorCLI2-0.6.2/tests/datatest/controllerSet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.824631 PyStorCLI2-0.6.2/tests/datatest/controllerSet/test00/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/controllerSet/test00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/controllerSet/test00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.824631 PyStorCLI2-0.6.2/tests/datatest/controllerSet/test01/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/controllerSet/test01/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/controllerSet/test01/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.824631 PyStorCLI2-0.6.2/tests/datatest/controllerSet/test02/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/controllerSet/test02/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/controllerSet/test02/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.824631 PyStorCLI2-0.6.2/tests/datatest/namedSet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.828631 PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid0_00/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid0_00/__c0_add_vd_r0_name=create_vd_raid0_drives=35_12-13_strip=512_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid0_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid0_00/__c0_v1_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid0_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid0_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.828631 PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid1_00/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid1_00/__c0_add_vd_r1_name=create_vd_raid1_drives=35_12-13_strip=512_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid1_00/__c0_add_vd_r1_name=create_vd_raid1_drives=35_12-13_strip=512_PDperArray=2_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid1_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid1_00/__c0_v1_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid1_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid1_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.828631 PyStorCLI2-0.6.2/tests/datatest/namedSet/delete_vd_00/
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/delete_vd_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/delete_vd_00/__c0_v1_del_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/delete_vd_00/__c0_v1_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/delete_vd_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/delete_vd_00/device.json
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.828631 PyStorCLI2-0.6.2/tests/datatest/namedSet/set_state_offline_00/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_set_offline_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/set_state_offline_00/__c0_e35_sall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/set_state_offline_00/__c0_e35_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/set_state_offline_00/__c0_eall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/set_state_offline_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/set_state_offline_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/set_state_offline_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.832631 PyStorCLI2-0.6.2/tests/datatest/namedSet/show_events_00/
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/show_events_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/show_events_00/__c0_show_events_file=_root_raid_events.log_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/show_events_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/show_events_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.832631 PyStorCLI2-0.6.2/tests/datatest/namedSet/spindown_disk_00/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_spindown_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/spindown_disk_00/__c0_e35_sall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/spindown_disk_00/__c0_e35_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/spindown_disk_00/__c0_eall_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/spindown_disk_00/__c0_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/spindown_disk_00/_show_J.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/namedSet/spindown_disk_00/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.816631 PyStorCLI2-0.6.2/tests/datatest/storcliSet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:51:13.832631 PyStorCLI2-0.6.2/tests/datatest/storcliSet/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/datatest/storcliSet/dummy/device.json
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/storclifile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/test_controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-17 14:50:30.000000 PyStorCLI2-0.6.2/tests/test_storcli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.708275 PyStorCLI2-0.6.2.dev13/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.692275 PyStorCLI2-0.6.2.dev13/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.696275 PyStorCLI2-0.6.2.dev13/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.696275 PyStorCLI2-0.6.2.dev13/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-17 14:47:41.708275 PyStorCLI2-0.6.2.dev13/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.696275 PyStorCLI2-0.6.2.dev13/PyStorCLI2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-17 14:47:41.000000 PyStorCLI2-0.6.2.dev13/PyStorCLI2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-17 14:47:41.000000 PyStorCLI2-0.6.2.dev13/PyStorCLI2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 14:47:41.000000 PyStorCLI2-0.6.2.dev13/PyStorCLI2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-17 14:47:41.000000 PyStorCLI2-0.6.2.dev13/PyStorCLI2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-17 14:47:41.000000 PyStorCLI2-0.6.2.dev13/PyStorCLI2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 14:47:41.000000 PyStorCLI2-0.6.2.dev13/PyStorCLI2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.696275 PyStorCLI2-0.6.2.dev13/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-17 14:47:16.000000 PyStorCLI2-0.6.2.dev13/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)   857304 2023-04-17 14:47:16.000000 PyStorCLI2-0.6.2.dev13/docs/pystorcli2.html
+-rw-r--r--   0 runner    (1001) docker     (123)   371378 2023-04-17 14:47:16.000000 PyStorCLI2-0.6.2.dev13/docs/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.700275 PyStorCLI2-0.6.2.dev13/pystorcli/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli/cachevault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli/cmdRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli/storcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-17 14:47:41.000000 PyStorCLI2-0.6.2.dev13/pystorcli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.700275 PyStorCLI2-0.6.2.dev13/pystorcli2/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.700275 PyStorCLI2-0.6.2.dev13/pystorcli2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5262 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/bin/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/cachevault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/cmdRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.700275 PyStorCLI2-0.6.2.dev13/pystorcli2/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/controller/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.700275 PyStorCLI2-0.6.2.dev13/pystorcli2/drive/
+-rw-r--r--   0 runner    (1001) docker     (123)    18691 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/drive/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/drive/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.700275 PyStorCLI2-0.6.2.dev13/pystorcli2/enclosure/
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/enclosure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/storcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-17 14:47:41.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.700275 PyStorCLI2-0.6.2.dev13/pystorcli2/virtualdrive/
+-rw-r--r--   0 runner    (1001) docker     (123)    23271 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/virtualdrive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/virtualdrive/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/virtualdrive/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli2/virtualdrive/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.700275 PyStorCLI2-0.6.2.dev13/pystorcli_mirror/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/pystorcli_mirror/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 14:47:41.708275 PyStorCLI2-0.6.2.dev13/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.700275 PyStorCLI2-0.6.2.dev13/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/baseTest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.692275 PyStorCLI2-0.6.2.dev13/tests/datatest/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.692275 PyStorCLI2-0.6.2.dev13/tests/datatest/controllerSet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.700275 PyStorCLI2-0.6.2.dev13/tests/datatest/controllerSet/test00/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/controllerSet/test00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/controllerSet/test00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.700275 PyStorCLI2-0.6.2.dev13/tests/datatest/controllerSet/test01/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/controllerSet/test01/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/controllerSet/test01/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.704275 PyStorCLI2-0.6.2.dev13/tests/datatest/controllerSet/test02/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/controllerSet/test02/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/controllerSet/test02/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.704275 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.704275 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid0_00/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid0_00/__c0_add_vd_r0_name=create_vd_raid0_drives=35_12-13_strip=512_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid0_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid0_00/__c0_v1_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid0_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid0_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.704275 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid1_00/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid1_00/__c0_add_vd_r1_name=create_vd_raid1_drives=35_12-13_strip=512_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid1_00/__c0_add_vd_r1_name=create_vd_raid1_drives=35_12-13_strip=512_PDperArray=2_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid1_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid1_00/__c0_v1_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid1_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid1_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.704275 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/delete_vd_00/
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/delete_vd_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/delete_vd_00/__c0_v1_del_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/delete_vd_00/__c0_v1_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/delete_vd_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/delete_vd_00/device.json
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.704275 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/set_state_offline_00/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_set_offline_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/set_state_offline_00/__c0_e35_sall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/set_state_offline_00/__c0_e35_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/set_state_offline_00/__c0_eall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/set_state_offline_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/set_state_offline_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/set_state_offline_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.704275 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/show_events_00/
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/show_events_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/show_events_00/__c0_show_events_file=_root_raid_events.log_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/show_events_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/show_events_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.708275 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/spindown_disk_00/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_spindown_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/spindown_disk_00/__c0_e35_sall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/spindown_disk_00/__c0_e35_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/spindown_disk_00/__c0_eall_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/spindown_disk_00/__c0_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/spindown_disk_00/_show_J.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/spindown_disk_00/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.692275 PyStorCLI2-0.6.2.dev13/tests/datatest/storcliSet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 14:47:41.708275 PyStorCLI2-0.6.2.dev13/tests/datatest/storcliSet/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/datatest/storcliSet/dummy/device.json
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/storclifile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/test_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-17 14:47:02.000000 PyStorCLI2-0.6.2.dev13/tests/test_storcli.py
```

### Comparing `PyStorCLI2-0.6.2/.github/workflows/check.yml` & `PyStorCLI2-0.6.2.dev13/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/.github/workflows/publish-to-pypi.yml` & `PyStorCLI2-0.6.2.dev13/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/CHANGELOG.md` & `PyStorCLI2-0.6.2.dev13/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/LICENSE` & `PyStorCLI2-0.6.2.dev13/LICENSE`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/PKG-INFO` & `PyStorCLI2-0.6.2.dev13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStorCLI2
-Version: 0.6.2
+Version: 0.6.2.dev13
 Summary: StorCLI module wrapper 2
 Author-email: Rafael Leira <rafael.leira@naudit.es>, Martin Dojcak <martin.dojcak@lablabs.io>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Naudit/pystorcli2
 Keywords: storcli,wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `PyStorCLI2-0.6.2/PyStorCLI2.egg-info/PKG-INFO` & `PyStorCLI2-0.6.2.dev13/PyStorCLI2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStorCLI2
-Version: 0.6.2
+Version: 0.6.2.dev13
 Summary: StorCLI module wrapper 2
 Author-email: Rafael Leira <rafael.leira@naudit.es>, Martin Dojcak <martin.dojcak@lablabs.io>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/Naudit/pystorcli2
 Keywords: storcli,wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `PyStorCLI2-0.6.2/PyStorCLI2.egg-info/SOURCES.txt` & `PyStorCLI2-0.6.2.dev13/PyStorCLI2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/README.md` & `PyStorCLI2-0.6.2.dev13/README.md`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/docs/pystorcli2.html` & `PyStorCLI2-0.6.2.dev13/docs/pystorcli2.html`

 * *Files 0% similar despite different names*

```diff
@@ -607,15 +607,15 @@
 </span></pre></div>
 
 
             </section>
                 <section id="__version__">
                     <div class="attr variable">
             <span class="name">__version__</span>        =
-<span class="default_value">&#39;0.6.2&#39;</span>
+<span class="default_value">&#39;0.6.2.dev13&#39;</span>
 
         
     </div>
     <a class="headerlink" href="#__version__"></a>
```

#### html2text {}

```diff
@@ -194,15 +194,15 @@
 14from .drive import DriveState, Drive, Drives
 15from .virtualdrive import VirtualDrive, VirtualDrives
 16
 17__all__ = ['__version__', 'StorCLI', 'Controller', 'Controllers',
 18           'Enclosure', 'Enclosures', 'DriveState', 'Drive', 'Drives',
 'VirtualDrive', 'VirtualDrives']
 
-__version__ = '0.6.2'
+__version__ = '0.6.2.dev13'
    ⁰
 class StorCLI: View Source
 _28class StorCLI(object):
 _29    """StorCLI command line wrapper
 _30
 _31    Instance of this class is storcli command line wrapper
 _32
```

### Comparing `PyStorCLI2-0.6.2/docs/search.js` & `PyStorCLI2-0.6.2.dev13/docs/search.js`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pyproject.toml` & `PyStorCLI2-0.6.2.dev13/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli/__init__.py` & `PyStorCLI2-0.6.2.dev13/pystorcli/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli/cachevault.py` & `PyStorCLI2-0.6.2.dev13/pystorcli/cachevault.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli/cmdRunner.py` & `PyStorCLI2-0.6.2.dev13/pystorcli/cmdRunner.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli/common.py` & `PyStorCLI2-0.6.2.dev13/pystorcli/common.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli/exc.py` & `PyStorCLI2-0.6.2.dev13/pystorcli/exc.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli/storcli.py` & `PyStorCLI2-0.6.2.dev13/pystorcli/storcli.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/__init__.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/bin/metrics.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/bin/metrics.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/cachevault.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/cachevault.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/cmdRunner.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/cmdRunner.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/common.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/common.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/controller/__init__.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/controller/metrics.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/controller/metrics.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/drive/__init__.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/drive/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/drive/metrics.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/drive/metrics.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/drive/state.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/drive/state.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/enclosure/__init__.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/enclosure/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/exc.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/exc.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/storcli.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/storcli.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/virtualdrive/__init__.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/virtualdrive/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/virtualdrive/access.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/virtualdrive/access.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/virtualdrive/metrics.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/virtualdrive/metrics.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli2/virtualdrive/state.py` & `PyStorCLI2-0.6.2.dev13/pystorcli2/virtualdrive/state.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/pystorcli_mirror/__init__.py` & `PyStorCLI2-0.6.2.dev13/pystorcli_mirror/__init__.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/baseTest.py` & `PyStorCLI2-0.6.2.dev13/tests/baseTest.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/controllerSet/test01/_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/controllerSet/test01/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/controllerSet/test02/_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/controllerSet/test02/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid0_00/__c0_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid0_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid0_00/__c0_v1_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid0_00/__c0_v1_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid0_00/_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid0_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid1_00/__c0_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid1_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid1_00/__c0_v1_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid1_00/__c0_v1_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/create_vd_raid1_00/_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/create_vd_raid1_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/delete_vd_00/__c0_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/delete_vd_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/delete_vd_00/__c0_v1_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/delete_vd_00/__c0_v1_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/delete_vd_00/_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/delete_vd_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/set_state_offline_00/__c0_e35_s12_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/set_state_offline_00/__c0_e35_sall_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/set_state_offline_00/__c0_e35_sall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/set_state_offline_00/__c0_e35_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/set_state_offline_00/__c0_e35_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/set_state_offline_00/__c0_eall_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/set_state_offline_00/__c0_eall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/set_state_offline_00/__c0_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/set_state_offline_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/set_state_offline_00/_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/set_state_offline_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/show_events_00/__c0_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/show_events_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/show_events_00/_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/show_events_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/spindown_disk_00/__c0_e35_s12_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/spindown_disk_00/__c0_e35_sall_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/spindown_disk_00/__c0_e35_sall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/spindown_disk_00/__c0_e35_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/spindown_disk_00/__c0_e35_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/spindown_disk_00/__c0_eall_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/spindown_disk_00/__c0_eall_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/spindown_disk_00/__c0_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/spindown_disk_00/__c0_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/datatest/namedSet/spindown_disk_00/_show_J.json` & `PyStorCLI2-0.6.2.dev13/tests/datatest/namedSet/spindown_disk_00/_show_J.json`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/exceptions.py` & `PyStorCLI2-0.6.2.dev13/tests/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/storclifile.py` & `PyStorCLI2-0.6.2.dev13/tests/storclifile.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/test_common.py` & `PyStorCLI2-0.6.2.dev13/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/test_controllers.py` & `PyStorCLI2-0.6.2.dev13/tests/test_controllers.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/test_operations.py` & `PyStorCLI2-0.6.2.dev13/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `PyStorCLI2-0.6.2/tests/test_storcli.py` & `PyStorCLI2-0.6.2.dev13/tests/test_storcli.py`

 * *Files identical despite different names*

