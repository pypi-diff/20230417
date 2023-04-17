# Comparing `tmp/fabrictestbed-extensions-1.4.2rc4.tar.gz` & `tmp/fabrictestbed-extensions-1.4.2rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-extensions-1.4.2rc4.tar", last modified: Tue Apr 11 21:37:27 2023, max compression
+gzip compressed data, was "fabrictestbed-extensions-1.4.2rc5.tar", last modified: Mon Apr 17 16:00:46 2023, max compression
```

## Comparing `fabrictestbed-extensions-1.4.2rc4.tar` & `fabrictestbed-extensions-1.4.2rc5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1025 2023-02-17 18:08:19.627880 fabrictestbed-extensions-1.4.2rc4/.github/workflows/build.yml
--rw-r--r--   0        0        0     1618 2023-04-07 02:35:56.572672 fabrictestbed-extensions-1.4.2rc4/.github/workflows/checks.yml
--rw-r--r--   0        0        0     2402 2023-04-07 02:36:06.076705 fabrictestbed-extensions-1.4.2rc4/.github/workflows/test.yml
--rw-r--r--   0        0        0     1799 2022-11-25 02:08:11.401934 fabrictestbed-extensions-1.4.2rc4/.gitignore
--rw-r--r--   0        0        0      666 2023-02-17 18:08:19.628880 fabrictestbed-extensions-1.4.2rc4/.readthedocs.yaml
--rw-r--r--   0        0        0     2130 2023-04-11 21:36:26.791911 fabrictestbed-extensions-1.4.2rc4/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2022-11-25 02:08:11.402934 fabrictestbed-extensions-1.4.2rc4/LICENSE
--rw-r--r--   0        0        0     4054 2023-04-03 14:05:06.148272 fabrictestbed-extensions-1.4.2rc4/README.md
--rw-r--r--   0        0        0      638 2022-11-25 02:08:11.402934 fabrictestbed-extensions-1.4.2rc4/docs/Makefile
--rw-r--r--   0        0        0      799 2022-11-25 02:08:11.402934 fabrictestbed-extensions-1.4.2rc4/docs/make.bat
--rw-r--r--   0        0        0     1996 2023-01-17 14:22:08.133013 fabrictestbed-extensions-1.4.2rc4/docs/source/conf.py
--rw-r--r--   0        0        0     8869 2023-01-30 21:29:15.591148 fabrictestbed-extensions-1.4.2rc4/docs/source/fablib.rst
--rw-r--r--   0        0        0     4470 2023-04-03 14:05:06.149272 fabrictestbed-extensions-1.4.2rc4/docs/source/index.rst
--rw-r--r--   0        0        0      151 2023-04-11 21:36:26.832911 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/__init__.py
--rw-r--r--   0        0        0        2 2023-01-17 14:22:08.134013 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/editors/__init__.py
--rw-r--r--   0        0        0    18044 2023-02-17 18:08:11.386871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/editors/abc_topology_editor.py
--rw-r--r--   0        0        0     6277 2023-02-17 18:08:11.386871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
--rw-r--r--   0        0        0    68479 2023-02-17 18:08:11.386871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/editors/geo_topology_editor.py
--rw-r--r--   0        0        0        1 2022-11-25 02:08:11.404934 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/__init__.py
--rw-r--r--   0        0        0     4793 2023-01-30 23:39:04.228930 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/abc_fablib.py
--rw-r--r--   0        0        0    20922 2023-04-11 21:29:21.986065 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/component.py
--rw-r--r--   0        0        0    77033 2023-04-11 21:36:26.756911 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/fablib.py
--rw-r--r--   0        0        0     5807 2023-02-17 18:08:11.387871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/facility_port.py
--rw-r--r--   0        0        0    25514 2023-04-11 21:29:21.986065 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/interface.py
--rw-r--r--   0        0        0    37982 2023-04-11 21:29:21.987065 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/network_service.py
--rw-r--r--   0        0        0    94159 2023-04-11 21:29:21.987065 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/node.py
--rw-r--r--   0        0        0    34672 2023-04-11 21:36:26.757911 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/resources.py
--rw-r--r--   0        0        0    72795 2023-04-11 21:29:21.988065 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/slice.py
--rw-r--r--   0        0        0        2 2023-01-17 14:22:08.137013 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/images/__init__.py
--rw-r--r--   0        0        0   199914 2022-11-25 02:08:11.407934 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/images/fabric_logo.png
--rw-r--r--   0        0        0     1316 2022-11-25 02:08:11.407934 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/images/server.png
--rw-r--r--   0        0        0    62250 2022-11-25 02:08:11.408934 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/images/slice_rack.png
--rw-r--r--   0        0        0        2 2023-02-17 18:05:26.140992 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/__init__.py
--rw-r--r--   0        0        0    14765 2023-02-17 18:08:11.388871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/abc_test.py
--rw-r--r--   0        0        0    34231 2023-02-17 18:08:11.389871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/component_tests.py
--rw-r--r--   0        0        0       85 2023-02-17 18:05:26.142992 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/dummy-token.json
--rw-r--r--   0        0        0    13366 2023-02-17 18:05:26.143992 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
--rw-r--r--   0        0        0    10227 2023-02-17 18:08:11.389871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/hello_fabric.py
--rw-r--r--   0        0        0    20659 2023-02-17 18:05:26.144992 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/link_benchmark.py
--rw-r--r--   0        0        0    20919 2023-02-17 18:05:26.145992 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/local_network_benchmark.py
--rw-r--r--   0        0        0    44883 2023-02-17 18:08:11.389871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/network_benchmark_tests.py
--rw-r--r--   0        0        0    10052 2023-02-17 18:08:11.389871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/nvme_benchmark.py
--rw-r--r--   0        0        0     5095 2023-04-03 14:05:06.152272 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/test_basic.py
--rw-r--r--   0        0        0        2 2023-01-17 14:22:08.139013 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/utils/__init__.py
--rw-r--r--   0        0        0     3082 2023-01-30 23:39:04.236930 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/utils/abc_utils.py
--rw-r--r--   0        0        0     3304 2023-01-17 14:22:08.139013 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/utils/node.py
--rw-r--r--   0        0        0     8436 2023-02-17 18:08:11.389871 fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/utils/slice.py
--rw-r--r--   0        0        0     1304 2023-02-17 18:08:19.628880 fabrictestbed-extensions-1.4.2rc4/pyproject.toml
--rwxr-xr-x   0        0        0      122 2022-11-25 02:08:11.409934 fabrictestbed-extensions-1.4.2rc4/sphinx.sh
--rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.4.2rc4/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-04-02 13:36:30.329332 fabrictestbed-extensions-1.4.2rc5/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1618 2023-04-10 21:57:28.666104 fabrictestbed-extensions-1.4.2rc5/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     2402 2023-04-10 21:57:28.666104 fabrictestbed-extensions-1.4.2rc5/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1799 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc5/.gitignore
+-rw-r--r--   0        0        0      666 2023-04-02 13:36:30.329332 fabrictestbed-extensions-1.4.2rc5/.readthedocs.yaml
+-rw-r--r--   0        0        0     2326 2023-04-17 15:58:37.151208 fabrictestbed-extensions-1.4.2rc5/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc5/LICENSE
+-rw-r--r--   0        0        0     4054 2023-04-10 21:57:28.670104 fabrictestbed-extensions-1.4.2rc5/README.md
+-rw-r--r--   0        0        0      638 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc5/docs/Makefile
+-rw-r--r--   0        0        0      799 2022-06-27 17:36:02.824097 fabrictestbed-extensions-1.4.2rc5/docs/make.bat
+-rw-r--r--   0        0        0     1996 2023-01-20 23:07:58.270662 fabrictestbed-extensions-1.4.2rc5/docs/source/conf.py
+-rw-r--r--   0        0        0     8869 2023-02-17 15:17:40.022255 fabrictestbed-extensions-1.4.2rc5/docs/source/fablib.rst
+-rw-r--r--   0        0        0     4470 2023-04-10 21:57:28.670104 fabrictestbed-extensions-1.4.2rc5/docs/source/index.rst
+-rw-r--r--   0        0        0      151 2023-04-17 15:58:37.151208 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/__init__.py
+-rw-r--r--   0        0        0        2 2023-01-20 23:07:58.270662 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/editors/__init__.py
+-rw-r--r--   0        0        0    18044 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/editors/abc_topology_editor.py
+-rw-r--r--   0        0        0     6277 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
+-rw-r--r--   0        0        0    68479 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/editors/geo_topology_editor.py
+-rw-r--r--   0        0        0        1 2023-02-17 19:04:16.623066 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/__init__.py
+-rw-r--r--   0        0        0     4793 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/abc_fablib.py
+-rw-r--r--   0        0        0    20922 2023-04-10 21:57:48.074249 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/component.py
+-rw-r--r--   0        0        0    76799 2023-04-17 15:58:37.151208 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/fablib.py
+-rw-r--r--   0        0        0     5807 2023-04-02 14:43:57.308548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/facility_port.py
+-rw-r--r--   0        0        0    25679 2023-04-17 15:58:37.155208 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/interface.py
+-rw-r--r--   0        0        0    38588 2023-04-17 15:50:56.020260 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/network_service.py
+-rw-r--r--   0        0        0    94720 2023-04-17 15:58:37.155208 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/node.py
+-rw-r--r--   0        0        0    34672 2023-04-10 21:57:48.078249 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/resources.py
+-rw-r--r--   0        0        0    81254 2023-04-17 15:58:37.159208 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/slice.py
+-rw-r--r--   0        0        0        2 2023-01-20 23:07:58.278662 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/images/__init__.py
+-rw-r--r--   0        0        0   199914 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/images/fabric_logo.png
+-rw-r--r--   0        0        0     1316 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/images/server.png
+-rw-r--r--   0        0        0    62250 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/images/slice_rack.png
+-rw-r--r--   0        0        0        2 2023-01-20 23:07:58.278662 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/__init__.py
+-rw-r--r--   0        0        0    14765 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/abc_test.py
+-rw-r--r--   0        0        0    34231 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/component_tests.py
+-rw-r--r--   0        0        0       85 2023-04-02 13:36:30.333332 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/dummy-token.json
+-rw-r--r--   0        0        0    13366 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
+-rw-r--r--   0        0        0    10227 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/hello_fabric.py
+-rw-r--r--   0        0        0    20659 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/link_benchmark.py
+-rw-r--r--   0        0        0    20919 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/local_network_benchmark.py
+-rw-r--r--   0        0        0    44883 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/network_benchmark_tests.py
+-rw-r--r--   0        0        0    10052 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/nvme_benchmark.py
+-rw-r--r--   0        0        0     5095 2023-04-10 21:57:28.682104 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/test_basic.py
+-rw-r--r--   0        0        0        2 2023-01-20 23:07:58.282662 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/utils/__init__.py
+-rw-r--r--   0        0        0     3082 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/utils/abc_utils.py
+-rw-r--r--   0        0        0     3304 2023-01-20 23:07:58.282662 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/utils/node.py
+-rw-r--r--   0        0        0     8436 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/utils/slice.py
+-rw-r--r--   0        0        0     1304 2023-04-02 14:43:57.312548 fabrictestbed-extensions-1.4.2rc5/pyproject.toml
+-rwxr-xr-x   0        0        0      122 2022-06-27 17:36:02.832097 fabrictestbed-extensions-1.4.2rc5/sphinx.sh
+-rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.4.2rc5/PKG-INFO
```

### Comparing `fabrictestbed-extensions-1.4.2rc4/.github/workflows/build.yml` & `fabrictestbed-extensions-1.4.2rc5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/.github/workflows/checks.yml` & `fabrictestbed-extensions-1.4.2rc5/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/.github/workflows/test.yml` & `fabrictestbed-extensions-1.4.2rc5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/.gitignore` & `fabrictestbed-extensions-1.4.2rc5/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/.readthedocs.yaml` & `fabrictestbed-extensions-1.4.2rc5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/CHANGELOG.md` & `fabrictestbed-extensions-1.4.2rc5/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Change Log
+# Change Log 
 
 This is the changelog file for FABRIC testbed extensions.  All notable
 changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
@@ -20,23 +20,27 @@
 - Userdata support.
 - Automatically assigning IPs, depending on mode.
 - Support for post-boot configuration.  Files or directories can be
   uploaded post-boot, and commands can be submitted to be run
   post-boot.
 - A way to define layer-2 networks.
 - A way to query link and facility port information
+- Added function to make IP address of node publicly routable with external networking. `make_ip_publicly_routable`
+- Streamlined polling after a submit to reduce load on the control framework
 
 ### Changed
 
 - Fablib now uses pyproject.toml for specifying packaging metadata
   instead of setup.py and friends (issue
   [#74](https://github.com/fabric-testbed/fabrictestbed-extensions/issues/74)).
 - Make configure_nvme() more generic (PR
   [#126](https://github.com/fabric-testbed/fabrictestbed-extensions/pull/126)).
 
+
+
 ### Fixed
 
 - Fixed an issue with auto network configuration executing twice
 - Fablib will now fail early when required configuration is missing
   (issue
   [#69](https://github.com/fabric-testbed/fabrictestbed-extensions/issues/69)).
 - A workaround for Debian/Ubuntu nmcli transition.
```

### Comparing `fabrictestbed-extensions-1.4.2rc4/LICENSE` & `fabrictestbed-extensions-1.4.2rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/README.md` & `fabrictestbed-extensions-1.4.2rc5/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/docs/Makefile` & `fabrictestbed-extensions-1.4.2rc5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/docs/make.bat` & `fabrictestbed-extensions-1.4.2rc5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/docs/source/conf.py` & `fabrictestbed-extensions-1.4.2rc5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/docs/source/fablib.rst` & `fabrictestbed-extensions-1.4.2rc5/docs/source/fablib.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/docs/source/index.rst` & `fabrictestbed-extensions-1.4.2rc5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/editors/abc_topology_editor.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/editors/abc_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/editors/cytoscape_topology_editor.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/editors/cytoscape_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/editors/geo_topology_editor.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/editors/geo_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/abc_fablib.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/abc_fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/component.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/component.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/fablib.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/fablib.py`

 * *Files 0% similar despite different names*

```diff
@@ -2101,20 +2101,23 @@
         table,
         headers=None,
         title="",
         title_font_size="1.25em",
         output=None,
         quiet=False,
     ):
+        if len(table) == 0:
+            return None
+
         if headers is not None:
             printable_table = pd.DataFrame(table, columns=headers)
         else:
             printable_table = pd.DataFrame(table)
 
-            # Table config (maybe some of this is unnecessary?
+        # Table config (maybe some of this is unnecessary?
         # df.style.set_properties(**{'background-color': 'black',
         #                   'color': 'green'})
 
         properties = {  # 'background-color': f'{FablibManager.FABRIC_LIGHT}',
             "text-align": "left",
             "border": f"1px {FablibManager.FABRIC_BLACK} solid !important",
         }
@@ -2177,18 +2180,14 @@
                         ("color", f"{FablibManager.FABRIC_BLACK}"),
                     ],
                 )
             ],
             overwrite=False,
         )
 
-        # printable_table = printable_table.set_table_styles([dict(selector='.level0',
-        #                                                         props=[('border', '1px black solid !important')])],
-        #                                                   overwrite=False)
-
         if not quiet:
             display(printable_table)
 
         return printable_table
 
     def list_table_json(self, data, quiet=False):
         json_str = json.dumps(data, indent=4)
```

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/facility_port.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/facility_port.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/interface.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -808,15 +808,20 @@
         if "mode" not in fablib_data:
             self.set_mode("config")
             fablib_data = self.get_fablib_data()
 
         return fablib_data["mode"]
 
     def config(self):
-        fablib_data = self.get_fablib_data()
+        network = self.get_network()
+        if not network:
+            logging.info(
+                f"interface {self.get_name()} not connected to network, skipping config."
+            )
+            return
 
         fablib_data = self.get_fablib_data()
         if "configured" in fablib_data and bool(fablib_data["configured"]):
             logging.debug(
                 f"interface {self.get_name()} already configured, skipping config."
             )
             return
```

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/network_service.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/network_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,24 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from fabrictestbed_extensions.fablib.slice import Slice
     from fabrictestbed_extensions.fablib.interface import Interface
     from fabric_cf.orchestrator.swagger_client import Sliver as OrchestratorSliver
 
-from fabrictestbed.slice_editor import ServiceType, NetworkService as FimNetworkService
+from fabrictestbed.slice_editor import (
+    ServiceType,
+    Labels,
+    Flags,
+    NetworkService as FimNetworkService,
+)
 from fim.slivers.network_service import ServiceType, NSLayer
 
 from fabrictestbed.slice_editor import UserData
+from fabric_cf.orchestrator.orchestrator_proxy import Status
 
 from ipaddress import IPv4Address, IPv6Address, IPv4Network, IPv6Network
 import ipaddress
 import json
 
 
 class NetworkService:
@@ -1051,14 +1057,26 @@
 
     def free_ip(self, addr: IPv4Address or IPv6Address):
         allocated_ips = self.get_allocated_ips()
         if addr in allocated_ips:
             allocated_ips.remove(addr)
         self.set_allocated_ips(allocated_ips)
 
+    def make_ip_publicly_routable(self, ipv6: list[str] = None, ipv4: list[str] = None):
+        labels = self.fim_network_service.labels
+        if labels is None:
+            labels = Labels()
+        if self.fim_network_service.type == ServiceType.FABNetv4Ext:
+            labels = Labels.update(labels, ipv4=ipv4)
+
+        elif self.fim_network_service.type == ServiceType.FABNetv6Ext:
+            labels = Labels.update(labels, ipv6=ipv6)
+
+        self.fim_network_service.set_properties(labels=labels)
+
     def set_gateway(self, gateway: IPv4Address or IPv6Address):
         fablib_data = self.get_fablib_data()
         fablib_data["subnet"]["gateway"] = str(gateway)
         self.set_fablib_data(fablib_data)
 
     def init_fablib_data(self):
         fablib_data = {"instantiated": "False", "mode": "manual"}
```

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/node.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -2572,31 +2572,44 @@
                 subnet = self.get_slice().get_network(name=str(net_name)).get_subnet()
 
             # print(f"subnet: {subnet} ({type(subnet)}, next_hop: {next_hop} ({type(next_hop)}")
 
             self.ip_route_add(subnet=ipaddress.ip_network(subnet), gateway=next_hop)
 
     def run_post_boot_tasks(self, log_dir: str = "."):
+        logging.debug(f"run_post_boot_tasks: {self.get_name()}")
         fablib_data = self.get_fablib_data()
         if "post_boot_tasks" in fablib_data:
             commands = fablib_data["post_boot_tasks"]
         else:
             commands = []
 
+        logging.debug(f"run_post_boot_tasks: commands: {commands}")
+
         for command in commands:
+            logging.debug(f"run_post_boot_tasks: command: {command}")
+
             if command[0] == "execute":
                 self.execute(
                     self.render_template(command[1]),
                     quiet=True,
                     output_file=f"{log_dir}/{self.get_name()}.log",
                 )
             elif command[0] == "upload_file":
-                self.upload_file(command[1], command[2])
+                logging.debug(f"run_post_boot_tasks: upload_file: {command}")
+
+                rtnval = self.upload_file(command[1], command[2])
+                logging.debug(f"run_post_boot_tasks: upload_file rtnval: {rtnval}")
+
             elif command[0] == "upload_directory":
-                self.upload_directory(command[1], command[2])
+                logging.debug(f"run_post_boot_tasks: upload_directory: {command}")
+
+                rtnval = self.upload_directory(command[1], command[2])
+                logging.debug(f"run_post_boot_tasks: upload_directory rtnval: {rtnval}")
+
             else:
                 logging.error(f"Invalid post boot command: {command}")
 
     def run_post_update_commands(self, log_dir: str = "."):
         fablib_data = self.get_fablib_data()
         if "post_update_commands" in fablib_data:
             commands = fablib_data["post_update_commands"]
```

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/resources.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/resources.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/fablib/slice.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/fablib/slice.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from concurrent.futures import ThreadPoolExecutor
 
 import pandas as pd
 import json
 
 from typing import TYPE_CHECKING
 
+from IPython.core.display_functions import display
 from fabrictestbed_extensions.fablib.facility_port import FacilityPort
 
 if TYPE_CHECKING:
     from fabric_cf.orchestrator.swagger_client import (
         Slice as OrchestratorSlice,
         Sliver as OrchestratorSliver,
     )
@@ -77,14 +78,19 @@
         self.slice_id = None
         self.topology = None
         self.slivers = []
         self.fablib_manager = fablib_manager
 
         self.slice_key = fablib_manager.get_default_slice_key()
 
+        self.update_topology_count = 0
+        self.update_slivers_count = 0
+        self.update_slice_count = 0
+        self.update_count = 0
+
     def get_fablib_manager(self):
         return self.fablib_manager
 
     def __str__(self):
         """
         Creates a tabulated string describing the properties of the slice.
 
@@ -533,15 +539,18 @@
         Not recommended for most users.  See Slice.update() method.
 
         Updates this slice manager slice to store the most up-to-date
         slice manager slice
 
         :raises Exception: if slice manager slice no longer exists
         """
-        logging.info(f"update_slice: {self.get_name()}")
+        self.update_slice_count += 1
+        logging.info(
+            f"update_slice: {self.get_name()}, count: {self.update_slice_count}"
+        )
 
         if self.fablib_manager.get_log_level() == logging.DEBUG:
             start = time.time()
 
         return_status, slices = self.fablib_manager.get_slice_manager().slices(
             excludes=[], slice_id=self.slice_id, name=self.slice_name
         )
@@ -565,15 +574,18 @@
         """
         Not recommended for most users.  See Slice.update() method.
 
         Updates the fabric slice topology with the slice manager slice's topology
 
         :raises Exception: if topology could not be gotten from slice manager
         """
-        logging.info(f"update_topology: {self.get_name()}")
+        self.update_topology_count += 1
+        logging.info(
+            f"update_topology: {self.get_name()}, count: {self.update_topology_count}"
+        )
 
         # Update topology
         if self.sm_slice.model is not None and self.sm_slice.model != "":
             self.topology = ExperimentTopology()
             self.topology.load(graph_string=self.sm_slice.model)
             return
 
@@ -595,15 +607,18 @@
         """
         Not recommended for most users.  See Slice.update() method.
 
         Updates the slivers with the current slice manager.
 
         :raises Exception: if topology could not be gotten from slice manager
         """
-        logging.debug(f"update_slivers: {self.get_name()}")
+        self.update_slivers_count += 1
+        logging.debug(
+            f"update_slivers: {self.get_name()}, count: {self.update_slivers_count}"
+        )
 
         if self.sm_slice is None:
             return
         status, slivers = self.fablib_manager.get_slice_manager().slivers(
             slice_object=self.sm_slice
         )
         if status == Status.OK:
@@ -625,15 +640,16 @@
 
     def update(self):
         """
         (re)Query the FABRIC services for updated information about this slice.
 
         :raises Exception: if updating topology fails
         """
-        logging.info(f"update : {self.get_name()}")
+        self.update_count += 1
+        logging.info(f"update : {self.get_name()}, count: {self.update_count}")
 
         try:
             self.update_slice()
         except Exception as e:
             logging.warning(f"slice.update_slice failed: {e}")
 
         try:
@@ -1603,22 +1619,32 @@
 
         """
         try:
             return "IPv4" if type(ip_address(IP)) is IPv4Address else "IPv6"
         except ValueError:
             return "Invalid"
 
-    def isReady(self):
+    def isReady(self, update=False):
         if not self.isStable():
+            logging.debug(
+                f"isReady: {self.get_name()} not stable ({self.get_state()}), returning false"
+            )
             return False
 
+        if update:
+            self.update()
+
         for node in self.get_nodes():
-            if node.get_reservation_state() == "Ticketed":
+            if (
+                node.get_reservation_state() == "Ticketed"
+                or not node.get_reservation_state()
+                or node.get_reservation_state() == "None"
+            ):
                 logging.warning(
-                    f"slice not ready: node {node.get_name()} status: {node.get_status()}"
+                    f"slice not ready: node {node.get_name()} status: {node.get_reservation_state()}"
                 )
                 return False
 
             if (
                 node.get_reservation_state() == "Active"
                 and node.get_management_ip() == None
             ):
@@ -1644,15 +1670,15 @@
                         return False
                 except Exception as e:
                     logging.warning(f"slice not ready: net {net.get_name()}, {e}")
                     return False
 
         return True
 
-    def wait_jupyter(self, timeout: int = 1800, interval: int = 10):
+    def wait_jupyter(self, timeout: int = 1800, interval: int = 30, verbose=False):
         """
         Waits for the slice to be in a stable and displays jupyter compliant tables of the slice progress.
 
         :param timeout: how many seconds to wait on the slice
         :type timeout: int
         :param interval: how often in seconds to check on slice state
         :type interval: int
@@ -1660,57 +1686,121 @@
         :return: the stable slice on the slice manager
         :rtype: SMSlice
         """
 
         from IPython.display import clear_output
         import time
 
+        logging.debug(f"wait_jupyter: slice {self.get_name()}")
+
         start = time.time()
 
         if len(self.get_interfaces()) > 0:
             hasNetworks = True
         else:
             hasNetworks = False
 
         count = 0
         # while not self.isStable():
-        while not self.isReady():
+        # while not self.isReady():
+        while True:
             if time.time() > start + timeout:
                 raise Exception(f"Timeout {timeout} sec exceeded in Jupyter wait")
 
             time.sleep(interval)
-            self.update()
+            stable = False
+            self.update_slice()
+            self.update_slivers()
+            if self.isStable():
+                stable = True
+                self.update()
+                if len(self.get_interfaces()) > 0:
+                    hasNetworks = True
+                else:
+                    hasNetworks = False
+                if self.isReady():
+                    break
+            else:
+                if verbose:
+                    self.update()
+                    if len(self.get_interfaces()) > 0:
+                        hasNetworks = True
+                    else:
+                        hasNetworks = False
+                else:
+                    self.update_slice()
 
             slice_show_table = self.show(colors=True, quiet=True)
-            node_table = self.list_nodes(colors=True, quiet=True)
-            if hasNetworks:
-                network_table = self.list_networks(colors=True, quiet=True)
+            sliver_table = self.list_slivers(colors=True, quiet=True)
+
+            logging.debug(f"sliver_table: {sliver_table}")
+            if stable or verbose:
+                node_table = self.list_nodes(colors=True, quiet=True)
+                if hasNetworks:
+                    network_table = self.list_networks(colors=True, quiet=True)
 
             time_string = f"{time.time() - start:.0f} sec"
 
             # Clear screen
             clear_output(wait=True)
 
             print(f"\nRetry: {count}, Time: {time_string}")
+            logging.debug(
+                f"{self.get_name()}, update_count: {self.update_count}, update_topology_count: {self.update_topology_count}, update_slivers_count: {self.update_slivers_count},  update_slice_count: {self.update_slice_count}"
+            )
+
+            if stable:
+                if slice_show_table:
+                    display(slice_show_table)
+                if node_table:
+                    display(node_table)
+                if hasNetworks and network_table:
+                    display(network_table)
 
-            display(slice_show_table)
-            display(node_table)
-            if hasNetworks:
-                display(network_table)
+            else:
+                if slice_show_table:
+                    display(slice_show_table)
+                if sliver_table:
+                    display(sliver_table)
+                if verbose:
+                    if node_table:
+                        display(node_table)
+                    if hasNetworks and network_table:
+                        display(network_table)
 
             count += 1
 
+        # self.update()
+
+        # if len(self.get_interfaces()) > 0:
+        #    hasNetworks = True
+        # else:
+        #    hasNetworks = False
+
+        slice_show_table = self.show(colors=True, quiet=True)
+        node_table = self.list_nodes(colors=True, quiet=True)
+        if hasNetworks:
+            network_table = self.list_networks(colors=True, quiet=True)
+
+        clear_output(wait=True)
+
+        display(slice_show_table)
+        display(node_table)
+        if hasNetworks and network_table:
+            display(network_table)
+
         print(f"\nTime to stable {time.time() - start:.0f} seconds")
 
         print("Running post_boot_config ... ")
         self.post_boot_config()
         print(f"Time to post boot config {time.time() - start:.0f} seconds")
 
         # Last update to get final data for display
-        self.update()
+        # no longer needed because post_boot_config does this
+        # self.update()
 
         slice_show_table = self.show(colors=True, quiet=True)
         node_table = self.list_nodes(colors=True, quiet=True)
         if hasNetworks:
             network_table = self.list_networks(colors=True, quiet=True)
 
         time_string = f"{time.time() - start:.0f} sec"
@@ -1785,63 +1875,68 @@
                 slice_graph=slice_graph,
                 ssh_key=self.get_slice_public_key(),
             )
             if return_status == Status.OK:
                 logging.info(
                     f"Submit request success: return_status {return_status}, slice_reservations: {slice_reservations}"
                 )
+                logging.debug(f"slice_reservations: {slice_reservations}")
+                logging.debug(f"slice_id: {slice_reservations[0].slice_id}")
+                self.slice_id = slice_reservations[0].slice_id
             else:
                 logging.error(
                     f"Submit request error: return_status {return_status}, slice_reservations: {slice_reservations}"
                 )
                 raise Exception(
                     f"Submit request error: return_status {return_status}, slice_reservations: {slice_reservations}"
                 )
 
-            self.slice_id = slice_reservations[0].slice_id
-
         if return_status != Status.OK:
             raise Exception(
                 "Failed to submit slice: {}, {}".format(
                     return_status, slice_reservations
                 )
             )
 
-        logging.debug(f"slice_reservations: {slice_reservations}")
+        # logging.debug(f"slice_reservations: {slice_reservations}")
         # logging.debug(f"slice_id: {slice_reservations[0].slice_id}")
         # self.slice_id = slice_reservations[0].slice_id
 
-        time.sleep(1)
-        self.update()
+        # time.sleep(1)
+        # self.update()
 
-        if not wait:
-            return self.slice_id
+        # if not wait:
+        #    return self.slice_id
 
         if (
             progress
             and wait_jupyter == "text"
             and self.fablib_manager.is_jupyter_notebook()
         ):
             self.wait_jupyter(timeout=wait_timeout, interval=wait_interval)
             return self.slice_id
 
-        if wait:
+        elif wait:
+            self.update()
+
             self.wait()
 
             if wait_ssh:
                 self.wait_ssh(
                     timeout=wait_timeout, interval=wait_interval, progress=progress
                 )
 
             if progress:
                 print("Running post boot config ... ", end="")
 
-            self.update()
             if post_boot_config:
                 self.post_boot_config()
+        else:
+            self.update()
+            return self.slice_id
 
         if progress:
             print("Done!")
 
         return self.slice_id
 
     def list_networks(
@@ -1911,25 +2006,27 @@
         def state_color(val):
             if val == "Active":
                 color = f"{self.get_fablib_manager().SUCCESS_LIGHT_COLOR}"
             elif val == "Ticketed":
                 color = f"{self.get_fablib_manager().IN_PROGRESS_LIGHT_COLOR}"
             elif val == "ActiveTicketed":
                 color = f"{self.get_fablib_manager().IN_PROGRESS_LIGHT_COLOR}"
-            elif val == "Closed":
-                color = f"{self.get_fablib_manager().IN_PROGRESS_LIGHT_COLOR}"
+            elif val == "Failed":
+                color = f"{self.get_fablib_manager().ERROR_LIGHT_COLOR}"
             else:
                 color = ""
             # return 'color: %s' % color
             return "background-color: %s" % color
 
         table = []
         for network in self.get_networks():
             table.append(network.toDict())
 
+        table = sorted(table, key=lambda x: (x["name"]))
+
         if pretty_names:
             pretty_names_dict = NetworkService.get_pretty_name_dict()
         else:
             pretty_names_dict = {}
 
         logging.debug(f"network service: pretty_names_dict = {pretty_names_dict}")
 
@@ -1939,25 +2036,166 @@
             title="Networks",
             output=output,
             quiet=True,
             filter_function=filter_function,
             pretty_names_dict=pretty_names_dict,
         )
 
-        if colors:
+        if table and colors:
             if pretty_names:
                 # table = table.apply(highlight, axis=1)
                 table = table.applymap(state_color, subset=pd.IndexSlice[:, ["State"]])
                 table = table.applymap(error_color, subset=pd.IndexSlice[:, ["Error"]])
             else:
                 # table = table.apply(highlight, axis=1)
                 table = table.applymap(state_color, subset=pd.IndexSlice[:, ["state"]])
                 table = table.applymap(error_color, subset=pd.IndexSlice[:, ["error"]])
 
-        if not quiet:
+        if table and not quiet:
+            display(table)
+
+        return table
+
+    def list_slivers(
+        self,
+        output=None,
+        fields=None,
+        colors=False,
+        quiet=False,
+        filter_function=None,
+        pretty_names=True,
+    ):
+        """
+        Lists all the slivers in the slice.
+
+        There are several output options: "text", "pandas", and "json" that determine the format of the
+        output that is returned and (optionally) displayed/printed.
+
+        output:  'text': string formatted with tabular
+                  'pandas': pandas dataframe
+                  'json': string in json format
+
+        fields: json output will include all available fields/columns.
+
+        Example: fields=['Name','State']
+
+        filter_function:  A lambda function to filter data by field values.
+
+        Example: filter_function=lambda s: s['State'] == 'Active'
+
+        :param output: output format
+        :type output: str
+        :param fields: list of fields (table columns) to show
+        :type fields: List[str]
+        :param quiet: True to specify printing/display
+        :type quiet: bool
+        :param filter_function: lambda function
+        :type filter_function: lambda
+        :param colors: True to add colors to the table when possible
+        :type colors: bool
+        :return: table in format specified by output parameter
+        :rtype: Object
+        """
+
+        def error_color(val):
+            # if 'Failure' in val:
+            if val != "" and not "TicketReviewPolicy" in val:
+                color = f"{self.get_fablib_manager().ERROR_LIGHT_COLOR}"
+            else:
+                color = ""
+            # return 'color: %s' % color
+
+            return "background-color: %s" % color
+
+        def highlight(x):
+            if x.State == "Ticketed":
+                return [
+                    f"background-color: {self.get_fablib_manager().IN_PROGRESS_LIGHT_COLOR}"
+                ] * (len(fields))
+            elif x.State == "None":
+                return ["opacity: 50%"] * (len(fields))
+            else:
+                return ["background-color: "] * (len(fields))
+
+        def state_color(val):
+            if val == "Active":
+                color = f"{self.get_fablib_manager().SUCCESS_LIGHT_COLOR}"
+            elif val == "Ticketed" or val == "Nascent" or val == "ActiveTicketed":
+                color = f"{self.get_fablib_manager().IN_PROGRESS_LIGHT_COLOR}"
+            else:
+                color = ""
+            # return 'color: %s' % color
+            return "background-color: %s" % color
+
+        table = []
+        for sliver in self.get_slivers():
+            try:
+                import json
+
+                reservation_info = json.loads(sliver.sliver["ReservationInfo"])
+                error = reservation_info["error_message"]
+            except:
+                error = ""
+
+            if sliver.sliver_type == "NetworkServiceSliver":
+                type = "network"
+            elif sliver.sliver_type == "NodeSliver":
+                type = "node"
+            else:
+                type = sliver.sliver_type
+
+            table.append(
+                {
+                    "id": sliver.sliver_id,
+                    "name": sliver.sliver["Name"],
+                    "type": type,
+                    "state": sliver.state,
+                    "error": error,
+                }
+            )
+
+            logging.debug(sliver)
+        table = sorted(table, key=lambda x: ([-ord(c) for c in x["type"]], x["name"]))
+
+        logging.debug(f"table: {table}")
+
+        if pretty_names:
+            pretty_names_dict = {
+                "name": "Name",
+                "id": "ID",
+                "type": "Type",
+                "state": "State",
+                "error": "Error",
+            }
+        else:
+            pretty_names_dict = {}
+
+        logging.debug(f"pretty_names_dict = {pretty_names_dict}")
+
+        table = self.get_fablib_manager().list_table(
+            table,
+            fields=fields,
+            title="Slivers",
+            output=output,
+            quiet=True,
+            filter_function=filter_function,
+            pretty_names_dict=pretty_names_dict,
+        )
+
+        if table and colors:
+            if pretty_names:
+                # table = table.apply(highlight, axis=1)
+                table = table.applymap(state_color, subset=pd.IndexSlice[:, ["State"]])
+                table = table.applymap(error_color, subset=pd.IndexSlice[:, ["Error"]])
+            else:
+                # table = table.apply(highlight, axis=1)
+                table = table.applymap(state_color, subset=pd.IndexSlice[:, ["state"]])
+                table = table.applymap(error_color, subset=pd.IndexSlice[:, ["error"]])
+
+        if table and not quiet:
             display(table)
 
         return table
 
     def list_nodes(
         self,
         output=None,
@@ -2029,14 +2267,16 @@
             # return 'color: %s' % color
             return "background-color: %s" % color
 
         table = []
         for node in self.get_nodes():
             table.append(node.toDict())
 
+        table = sorted(table, key=lambda x: (x["name"]))
+
         # if fields == None:
         #    fields = ["ID", "Name", "Site", "Host",
         #              "Cores", "RAM", "Disk", "Image",
         #              "Username", "Management IP", "State", "Error"]
 
         if pretty_names:
             pretty_names_dict = Node.get_pretty_name_dict()
@@ -2051,24 +2291,24 @@
             title="Nodes",
             output=output,
             quiet=True,
             filter_function=filter_function,
             pretty_names_dict=pretty_names_dict,
         )
 
-        if colors:
+        if table and colors:
             if pretty_names:
                 # table = table.apply(highlight, axis=1)
                 table = table.applymap(state_color, subset=pd.IndexSlice[:, ["State"]])
                 table = table.applymap(error_color, subset=pd.IndexSlice[:, ["Error"]])
             else:
                 # table = table.apply(highlight, axis=1)
                 table = table.applymap(state_color, subset=pd.IndexSlice[:, ["state"]])
                 table = table.applymap(error_color, subset=pd.IndexSlice[:, ["error"]])
-        if not quiet:
+        if table and not quiet:
             display(table)
 
         return table
 
     def modify(
         self,
         wait: int = True,
@@ -2112,43 +2352,47 @@
             raise Exception(
                 "Failed to submit modify slice: {}, {}".format(
                     return_status, slice_reservations
                 )
             )
 
         logging.debug(f"slice_reservations: {slice_reservations}")
-        logging.debug(f"slice_id: {slice_reservations[0].slice_id}")
-        self.slice_id = slice_reservations[0].slice_id
+        # logging.debug(f"slice_id: {slice_reservations[0].slice_id}")
+        # self.slice_id = slice_reservations[0].slice_id
 
-        time.sleep(1)
-        self.update()
+        # time.sleep(1)
+        # self.update()
 
         if (
             progress
             and wait_jupyter == "text"
             and self.fablib_manager.is_jupyter_notebook()
         ):
             self.wait_jupyter(timeout=wait_timeout, interval=wait_interval)
             return self.slice_id
 
-        if wait:
+        elif wait:
             self.wait_ssh(
                 timeout=wait_timeout, interval=wait_interval, progress=progress
             )
 
             if progress:
                 print("Running post boot config ... ", end="")
 
             self.update()
             if post_boot_config:
                 self.post_boot_config()
+        else:
+            self.update()
 
         if progress:
             print("Done!")
 
+        return self.slice_id
+
     def modify_accept(self):
         """
         Submits an accept to accept the last modify slice request to FABRIC.
         """
         # Request slice from Orchestrator
         return_status, topology = self.fablib_manager.get_slice_manager().modify_accept(
             slice_id=self.slice_id
```

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/images/fabric_logo.png` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/images/fabric_logo.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/images/server.png` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/images/server.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/images/slice_rack.png` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/images/slice_rack.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/abc_test.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/abc_test.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/component_tests.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/component_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/hello_fabric.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/hello_fabric.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/link_benchmark.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/link_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/local_network_benchmark.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/local_network_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/network_benchmark_tests.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/network_benchmark_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/nvme_benchmark.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/nvme_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/tests/test_basic.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/utils/abc_utils.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/utils/abc_utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/utils/node.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/utils/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/fabrictestbed_extensions/utils/slice.py` & `fabrictestbed-extensions-1.4.2rc5/fabrictestbed_extensions/utils/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/pyproject.toml` & `fabrictestbed-extensions-1.4.2rc5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.4.2rc4/PKG-INFO` & `fabrictestbed-extensions-1.4.2rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-extensions
-Version: 1.4.2rc4
+Version: 1.4.2rc5
 Summary: FABRIC Python Client Library and CLI Extensions
 Author-email: Paul Ruth <pruth@renci.org>, Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

