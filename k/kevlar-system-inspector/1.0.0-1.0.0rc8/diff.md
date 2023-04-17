# Comparing `tmp/kevlar-system-inspector-1.0.0.tar.gz` & `tmp/kevlar-system-inspector-1.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/wrlx-octane/kevlar-inspector/dist/.tmp-7tvbtbh_/kevlar-system-inspector-1.0.0.tar", last modified: Mon Apr 17 20:51:26 2023, max compression
+gzip compressed data, was "/builds/wrlx-octane/kevlar-inspector/dist/.tmp-vfb17x5a/kevlar-system-inspector-1.0.0rc8.tar", last modified: Fri Apr 14 17:39:27 2023, max compression
```

## Comparing `kevlar-system-inspector-1.0.0.tar` & `kevlar-system-inspector-1.0.0rc8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:51:26.000000 kevlar-system-inspector-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3676 2023-04-17 20:51:26.000000 kevlar-system-inspector-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2647 2023-04-17 20:05:10.000000 kevlar-system-inspector-1.0.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:51:26.000000 kevlar-system-inspector-1.0.0/scripts/
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/scripts/kevlar-system-inspector
--rw-rw-rw-   0 root         (0) root         (0)     1351 2023-04-17 20:51:26.000000 kevlar-system-inspector-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:51:26.000000 kevlar-system-inspector-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:51:26.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/
--rw-rw-rw-   0 root         (0) root         (0)     6110 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     6310 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    16848 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/console.py
--rw-rw-rw-   0 root         (0) root         (0)     3713 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6470 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/output.py
--rw-rw-rw-   0 root         (0) root         (0)     8240 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:51:26.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/resources/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1272 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/sysinfo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:51:26.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/templates/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/templates/failures.rst
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/templates/html5-template.txt
--rw-rw-rw-   0 root         (0) root         (0)     3215 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/templates/report.rst
--rw-rw-rw-   0 root         (0) root         (0)    11687 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/templates/starlab.css
--rw-rw-rw-   0 root         (0) root         (0)      330 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/templates/warnings.rst
--rw-rw-rw-   0 root         (0) root         (0)     9440 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/test_allowlisting.py
--rw-rw-rw-   0 root         (0) root         (0)    12968 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/test_kernel_config.py
--rw-rw-rw-   0 root         (0) root         (0)     6077 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/test_kernel_modules.py
--rw-rw-rw-   0 root         (0) root         (0)     2982 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/test_offline_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     4693 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/test_secure_dns.py
--rw-rw-rw-   0 root         (0) root         (0)     2776 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/test_systemd_syscall_filtering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:51:26.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/utils/
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/utils/elf.py
--rw-rw-rw-   0 root         (0) root         (0)     4226 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/utils/kconfig.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/utils/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     3943 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/utils/mount.py
--rw-rw-rw-   0 root         (0) root         (0)     4631 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/utils/systemd.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/utils/workdir.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:51:26.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3676 2023-04-17 20:51:26.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-17 20:51:26.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 20:51:26.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-04-17 20:51:26.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-17 20:51:26.000000 kevlar-system-inspector-1.0.0/src/kevlar_system_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3682 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2650 2023-04-14 17:36:14.000000 kevlar-system-inspector-1.0.0rc8/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/scripts/kevlar-system-inspector
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/
+-rw-rw-rw-   0 root         (0) root         (0)     6110 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6310 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    16848 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/console.py
+-rw-rw-rw-   0 root         (0) root         (0)     3713 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6470 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/output.py
+-rw-rw-rw-   0 root         (0) root         (0)     8240 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/resources/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/sysinfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/failures.rst
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/html5-template.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3215 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/report.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11687 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/starlab.css
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/warnings.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9440 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_allowlisting.py
+-rw-rw-rw-   0 root         (0) root         (0)    12968 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_kernel_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6077 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_kernel_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     2982 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_offline_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     4693 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_secure_dns.py
+-rw-rw-rw-   0 root         (0) root         (0)     2776 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_systemd_syscall_filtering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/elf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4226 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/kconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     3943 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/mount.py
+-rw-rw-rw-   0 root         (0) root         (0)     4631 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/systemd.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/workdir.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-04-14 17:20:49.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3682 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-14 17:39:27.000000 kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector.egg-info/top_level.txt
```

### Comparing `kevlar-system-inspector-1.0.0/LICENSE` & `kevlar-system-inspector-1.0.0rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/PKG-INFO` & `kevlar-system-inspector-1.0.0rc8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevlar-system-inspector
-Version: 1.0.0
+Version: 1.0.0rc8
 Summary: A security scanner for Linux systems
 Home-page: https://www.starlab.io/explore-kevlar-system-inspector
 Author: Star Lab
 Author-email: info@starlab.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -94,8 +94,8 @@
 copied this tarball to your device, you can simply extract and run:
 
 .. code-block:: console
 
    $ tar xf ./kevlar-system-inspector-standalone.tar.gz
    $ sudo ./kevlar-system-inspector-standalone/kevlar-system-inspector
 
-.. _standalone tarball: https://inspector.starlab.io/kevlar-system-inspector-standalone-v1.0.0.tar.gz
+.. _standalone tarball: https://inspector.starlab.io/kevlar-system-inspector-standalone-v1.0.0rc8.tar.gz
```

### Comparing `kevlar-system-inspector-1.0.0/README.rst` & `kevlar-system-inspector-1.0.0rc8/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,8 @@
 copied this tarball to your device, you can simply extract and run:
 
 .. code-block:: console
 
    $ tar xf ./kevlar-system-inspector-standalone.tar.gz
    $ sudo ./kevlar-system-inspector-standalone/kevlar-system-inspector
 
-.. _standalone tarball: https://inspector.starlab.io/kevlar-system-inspector-standalone-v1.0.0.tar.gz
+.. _standalone tarball: https://inspector.starlab.io/kevlar-system-inspector-standalone-v1.0.0rc8.tar.gz
```

### Comparing `kevlar-system-inspector-1.0.0/setup.cfg` & `kevlar-system-inspector-1.0.0rc8/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kevlar-system-inspector
-version = 1.0.0
+version = 1.0.0rc8
 author = Star Lab
 author_email = info@starlab.io
 url = https://www.starlab.io/explore-kevlar-system-inspector
 license = MIT
 license_files = LICENSE
 description = A security scanner for Linux systems
 long_description = file: README.rst
```

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/__init__.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/__init__.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/conftest.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/conftest.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/console.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/console.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/decorators.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/decorators.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/output.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/output.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/report.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/report.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/sysinfo.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/sysinfo.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/templates/failures.rst` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/failures.rst`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/templates/report.rst` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/report.rst`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/templates/starlab.css` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/templates/starlab.css`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/test_allowlisting.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_allowlisting.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/test_kernel_config.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_kernel_config.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/test_kernel_modules.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_kernel_modules.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/test_offline_integrity.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_offline_integrity.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/test_secure_dns.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_secure_dns.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/test_systemd_syscall_filtering.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/test_systemd_syscall_filtering.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/utils/__init__.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/utils/elf.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/elf.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/utils/kconfig.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/kconfig.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/utils/modules.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/modules.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/utils/mount.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/mount.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/utils/systemd.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/systemd.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector/utils/workdir.py` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector/utils/workdir.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector.egg-info/PKG-INFO` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevlar-system-inspector
-Version: 1.0.0
+Version: 1.0.0rc8
 Summary: A security scanner for Linux systems
 Home-page: https://www.starlab.io/explore-kevlar-system-inspector
 Author: Star Lab
 Author-email: info@starlab.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -94,8 +94,8 @@
 copied this tarball to your device, you can simply extract and run:
 
 .. code-block:: console
 
    $ tar xf ./kevlar-system-inspector-standalone.tar.gz
    $ sudo ./kevlar-system-inspector-standalone/kevlar-system-inspector
 
-.. _standalone tarball: https://inspector.starlab.io/kevlar-system-inspector-standalone-v1.0.0.tar.gz
+.. _standalone tarball: https://inspector.starlab.io/kevlar-system-inspector-standalone-v1.0.0rc8.tar.gz
```

### Comparing `kevlar-system-inspector-1.0.0/src/kevlar_system_inspector.egg-info/SOURCES.txt` & `kevlar-system-inspector-1.0.0rc8/src/kevlar_system_inspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

