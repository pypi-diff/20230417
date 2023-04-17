# Comparing `tmp/python-scripttease-6.8.2.tar.gz` & `tmp/python-scripttease-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-scripttease-6.8.2.tar", last modified: Tue Jan 26 17:11:04 2021, max compression
+gzip compressed data, was "dist/python-scripttease-7.0.0.tar", last modified: Mon Apr 17 17:40:24 2023, max compression
```

## Comparing `python-scripttease-6.8.2.tar` & `python-scripttease-7.0.0.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2021-01-26 17:11:04.652541 python-scripttease-6.8.2/
--rw-r--r--   0 shawn      (501) staff       (20)       87 2019-04-26 18:33:34.000000 python-scripttease-6.8.2/DESCRIPTION.txt
--rw-r--r--   0 shawn      (501) staff       (20)     1519 2019-04-26 17:53:38.000000 python-scripttease-6.8.2/LICENSE.txt
--rw-r--r--   0 shawn      (501) staff       (20)      204 2020-09-02 16:16:51.000000 python-scripttease-6.8.2/MANIFEST.in
--rw-r--r--   0 shawn      (501) staff       (20)     1382 2021-01-26 17:11:04.651871 python-scripttease-6.8.2/PKG-INFO
--rw-r--r--   0 shawn      (501) staff       (20)        5 2021-01-26 17:09:57.000000 python-scripttease-6.8.2/VERSION.txt
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2021-01-26 17:11:04.630961 python-scripttease-6.8.2/python_scripttease.egg-info/
--rw-r--r--   0 shawn      (501) staff       (20)     1382 2021-01-26 17:11:04.000000 python-scripttease-6.8.2/python_scripttease.egg-info/PKG-INFO
--rw-r--r--   0 shawn      (501) staff       (20)     1202 2021-01-26 17:11:04.000000 python-scripttease-6.8.2/python_scripttease.egg-info/SOURCES.txt
--rw-r--r--   0 shawn      (501) staff       (20)        1 2021-01-26 17:11:04.000000 python-scripttease-6.8.2/python_scripttease.egg-info/dependency_links.txt
--rw-r--r--   0 shawn      (501) staff       (20)       57 2021-01-26 17:11:04.000000 python-scripttease-6.8.2/python_scripttease.egg-info/entry_points.txt
--rw-r--r--   0 shawn      (501) staff       (20)        1 2021-01-26 17:11:04.000000 python-scripttease-6.8.2/python_scripttease.egg-info/not-zip-safe
--rw-r--r--   0 shawn      (501) staff       (20)       33 2021-01-26 17:11:04.000000 python-scripttease-6.8.2/python_scripttease.egg-info/requires.txt
--rw-r--r--   0 shawn      (501) staff       (20)       12 2021-01-26 17:11:04.000000 python-scripttease-6.8.2/python_scripttease.egg-info/top_level.txt
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2021-01-26 17:11:04.634733 python-scripttease-6.8.2/scripttease/
--rw-r--r--   0 shawn      (501) staff       (20)        0 2020-07-16 18:21:17.000000 python-scripttease-6.8.2/scripttease/__init__.py
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2021-01-26 17:11:04.636654 python-scripttease-6.8.2/scripttease/cli/
--rw-r--r--   0 shawn      (501) staff       (20)     5387 2020-09-17 15:03:03.000000 python-scripttease-6.8.2/scripttease/cli/__init__.py
--rw-r--r--   0 shawn      (501) staff       (20)     2851 2020-09-06 16:12:02.000000 python-scripttease-6.8.2/scripttease/cli/initialize.py
--rw-r--r--   0 shawn      (501) staff       (20)     3870 2020-09-06 15:12:06.000000 python-scripttease-6.8.2/scripttease/cli/subcommands.py
--rw-r--r--   0 shawn      (501) staff       (20)       29 2020-09-06 15:16:54.000000 python-scripttease-6.8.2/scripttease/constants.py
--rw-r--r--   0 shawn      (501) staff       (20)     2302 2020-09-06 15:49:30.000000 python-scripttease-6.8.2/scripttease/factory.py
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2021-01-26 17:11:04.638066 python-scripttease-6.8.2/scripttease/library/
--rw-r--r--   0 shawn      (501) staff       (20)        0 2020-07-16 18:22:49.000000 python-scripttease-6.8.2/scripttease/library/__init__.py
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2021-01-26 17:11:04.640729 python-scripttease-6.8.2/scripttease/library/commands/
--rw-r--r--   0 shawn      (501) staff       (20)      114 2020-07-22 22:31:00.000000 python-scripttease-6.8.2/scripttease/library/commands/__init__.py
--rw-r--r--   0 shawn      (501) staff       (20)     9067 2021-01-26 16:59:49.000000 python-scripttease-6.8.2/scripttease/library/commands/base.py
--rw-r--r--   0 shawn      (501) staff       (20)     6726 2020-09-06 15:12:40.000000 python-scripttease-6.8.2/scripttease/library/commands/templates.py
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2021-01-26 17:11:04.647445 python-scripttease-6.8.2/scripttease/library/overlays/
--rw-r--r--   0 shawn      (501) staff       (20)        0 2020-07-20 22:05:01.000000 python-scripttease-6.8.2/scripttease/library/overlays/__init__.py
--rw-r--r--   0 shawn      (501) staff       (20)     7252 2020-09-17 14:58:21.000000 python-scripttease-6.8.2/scripttease/library/overlays/centos.py
--rw-r--r--   0 shawn      (501) staff       (20)     3862 2020-09-24 20:03:35.000000 python-scripttease-6.8.2/scripttease/library/overlays/common.py
--rw-r--r--   0 shawn      (501) staff       (20)     5736 2020-08-08 15:32:51.000000 python-scripttease-6.8.2/scripttease/library/overlays/django.py
--rw-r--r--   0 shawn      (501) staff       (20)     9209 2020-09-17 14:50:38.000000 python-scripttease-6.8.2/scripttease/library/overlays/mysql.py
--rw-r--r--   0 shawn      (501) staff       (20)     8233 2020-09-22 20:28:26.000000 python-scripttease-6.8.2/scripttease/library/overlays/pgsql.py
--rw-r--r--   0 shawn      (501) staff       (20)    21145 2020-09-24 20:09:38.000000 python-scripttease-6.8.2/scripttease/library/overlays/posix.py
--rw-r--r--   0 shawn      (501) staff       (20)     8739 2020-09-17 14:58:41.000000 python-scripttease-6.8.2/scripttease/library/overlays/ubuntu.py
--rw-r--r--   0 shawn      (501) staff       (20)     1881 2020-07-21 23:21:02.000000 python-scripttease-6.8.2/scripttease/library/scripts.py
-drwxr-xr-x   0 shawn      (501) staff       (20)        0 2021-01-26 17:11:04.651282 python-scripttease-6.8.2/scripttease/parsers/
--rw-r--r--   0 shawn      (501) staff       (20)       98 2020-07-21 22:15:37.000000 python-scripttease-6.8.2/scripttease/parsers/__init__.py
--rw-r--r--   0 shawn      (501) staff       (20)     1805 2020-09-06 15:15:31.000000 python-scripttease-6.8.2/scripttease/parsers/base.py
--rw-r--r--   0 shawn      (501) staff       (20)     6087 2020-12-16 22:41:14.000000 python-scripttease-6.8.2/scripttease/parsers/ini.py
--rw-r--r--   0 shawn      (501) staff       (20)     8469 2021-01-26 17:07:06.000000 python-scripttease-6.8.2/scripttease/parsers/utils.py
--rw-r--r--   0 shawn      (501) staff       (20)        0 2020-07-16 18:24:34.000000 python-scripttease-6.8.2/scripttease/parsers/yaml.py
--rw-r--r--   0 shawn      (501) staff       (20)      120 2020-09-06 15:17:03.000000 python-scripttease-6.8.2/scripttease/variables.py
--rw-r--r--   0 shawn      (501) staff       (20)       68 2021-01-26 17:09:57.000000 python-scripttease-6.8.2/scripttease/version.py
--rw-r--r--   0 shawn      (501) staff       (20)       38 2021-01-26 17:11:04.652721 python-scripttease-6.8.2/setup.cfg
--rw-r--r--   0 shawn      (501) staff       (20)     1942 2020-10-06 21:53:40.000000 python-scripttease-6.8.2/setup.py
+drwxr-xr-x   0 shawn      (501) staff       (20)        0 2023-04-17 17:40:24.646536 python-scripttease-7.0.0/
+-rw-r--r--   0 shawn      (501) staff       (20)       87 2019-04-26 18:33:34.000000 python-scripttease-7.0.0/DESCRIPTION.txt
+-rw-r--r--   0 shawn      (501) staff       (20)     1516 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/LICENSE.txt
+-rw-r--r--   0 shawn      (501) staff       (20)      204 2020-09-02 16:16:51.000000 python-scripttease-7.0.0/MANIFEST.in
+-rw-r--r--   0 shawn      (501) staff       (20)     1478 2023-04-17 17:40:24.646216 python-scripttease-7.0.0/PKG-INFO
+-rw-r--r--   0 shawn      (501) staff       (20)        5 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/VERSION.txt
+drwxr-xr-x   0 shawn      (501) staff       (20)        0 2023-04-17 17:40:24.635827 python-scripttease-7.0.0/python_scripttease.egg-info/
+-rw-r--r--   0 shawn      (501) staff       (20)     1478 2023-04-17 17:40:24.000000 python-scripttease-7.0.0/python_scripttease.egg-info/PKG-INFO
+-rw-r--r--   0 shawn      (501) staff       (20)     1164 2023-04-17 17:40:24.000000 python-scripttease-7.0.0/python_scripttease.egg-info/SOURCES.txt
+-rw-r--r--   0 shawn      (501) staff       (20)        1 2023-04-17 17:40:24.000000 python-scripttease-7.0.0/python_scripttease.egg-info/dependency_links.txt
+-rw-r--r--   0 shawn      (501) staff       (20)       56 2023-04-17 17:40:24.000000 python-scripttease-7.0.0/python_scripttease.egg-info/entry_points.txt
+-rw-r--r--   0 shawn      (501) staff       (20)        1 2023-04-17 17:40:24.000000 python-scripttease-7.0.0/python_scripttease.egg-info/not-zip-safe
+-rw-r--r--   0 shawn      (501) staff       (20)       67 2023-04-17 17:40:24.000000 python-scripttease-7.0.0/python_scripttease.egg-info/requires.txt
+-rw-r--r--   0 shawn      (501) staff       (20)       12 2023-04-17 17:40:24.000000 python-scripttease-7.0.0/python_scripttease.egg-info/top_level.txt
+drwxr-xr-x   0 shawn      (501) staff       (20)        0 2023-04-17 17:40:24.638343 python-scripttease-7.0.0/scripttease/
+-rw-r--r--   0 shawn      (501) staff       (20)        0 2020-07-16 18:21:17.000000 python-scripttease-7.0.0/scripttease/__init__.py
+drwxr-xr-x   0 shawn      (501) staff       (20)        0 2023-04-17 17:40:24.639500 python-scripttease-7.0.0/scripttease/cli/
+-rw-r--r--   0 shawn      (501) staff       (20)     3573 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/cli/__init__.py
+-rw-r--r--   0 shawn      (501) staff       (20)     9590 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/cli/initialize.py
+-rw-r--r--   0 shawn      (501) staff       (20)     5349 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/cli/subcommands.py
+-rw-r--r--   0 shawn      (501) staff       (20)      314 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/constants.py
+-rw-r--r--   0 shawn      (501) staff       (20)       84 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/exceptions.py
+drwxr-xr-x   0 shawn      (501) staff       (20)        0 2023-04-17 17:40:24.640584 python-scripttease-7.0.0/scripttease/lib/
+-rw-r--r--   0 shawn      (501) staff       (20)        0 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/lib/__init__.py
+drwxr-xr-x   0 shawn      (501) staff       (20)        0 2023-04-17 17:40:24.643846 python-scripttease-7.0.0/scripttease/lib/commands/
+-rw-r--r--   0 shawn      (501) staff       (20)        0 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/lib/commands/__init__.py
+-rw-r--r--   0 shawn      (501) staff       (20)    24600 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/base.py
+-rw-r--r--   0 shawn      (501) staff       (20)     7431 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/centos.py
+-rw-r--r--   0 shawn      (501) staff       (20)     5186 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/django.py
+-rw-r--r--   0 shawn      (501) staff       (20)     3263 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/messages.py
+-rw-r--r--   0 shawn      (501) staff       (20)     7386 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/mysql.py
+-rw-r--r--   0 shawn      (501) staff       (20)     8705 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/pgsql.py
+-rw-r--r--   0 shawn      (501) staff       (20)      281 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/php.py
+-rw-r--r--   0 shawn      (501) staff       (20)    19570 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/posix.py
+-rw-r--r--   0 shawn      (501) staff       (20)     2046 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/python.py
+-rw-r--r--   0 shawn      (501) staff       (20)     9009 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/commands/ubuntu.py
+-rw-r--r--   0 shawn      (501) staff       (20)     2028 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/lib/contexts.py
+-rw-r--r--   0 shawn      (501) staff       (20)     4425 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/factories.py
+drwxr-xr-x   0 shawn      (501) staff       (20)        0 2023-04-17 17:40:24.645422 python-scripttease-7.0.0/scripttease/lib/loaders/
+-rw-r--r--   0 shawn      (501) staff       (20)      177 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/lib/loaders/__init__.py
+-rw-r--r--   0 shawn      (501) staff       (20)     7511 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/loaders/base.py
+-rw-r--r--   0 shawn      (501) staff       (20)     2919 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/scripttease/lib/loaders/ini.py
+-rw-r--r--   0 shawn      (501) staff       (20)     2176 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/lib/loaders/yaml.py
+-rw-r--r--   0 shawn      (501) staff       (20)      213 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/variables.py
+-rw-r--r--   0 shawn      (501) staff       (20)       68 2023-04-04 14:50:40.000000 python-scripttease-7.0.0/scripttease/version.py
+-rw-r--r--   0 shawn      (501) staff       (20)       38 2023-04-17 17:40:24.646642 python-scripttease-7.0.0/setup.cfg
+-rw-r--r--   0 shawn      (501) staff       (20)     2005 2023-04-17 17:40:07.000000 python-scripttease-7.0.0/setup.py
```

### Comparing `python-scripttease-6.8.2/LICENSE.txt` & `python-scripttease-7.0.0/LICENSE.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 are permitted provided that the following conditions are met:
 
     * Redistributions of source code must retain the above copyright notice,
       this list of conditions and the following disclaimer.
     * Redistributions in binary form must reproduce the above copyright notice,
       this list of conditions and the following disclaimer in the documentation
       and/or other materials provided with the distribution.
-    * Neither the name of Pleasant Tents, LLC nor the names of its contributors
+    * Neither the name of copyright holder nor the names of its contributors
       may be used to endorse or promote products derived from this software
       without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
 "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
 LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
 A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR
```

### Comparing `python-scripttease-6.8.2/PKG-INFO` & `python-scripttease-7.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Metadata-Version: 2.1
 Name: python-scripttease
-Version: 6.8.2
+Version: 7.0.0
 Summary: A collection of classes and commands for automated command line scripting using Python.
 Home-page: https://develmaycare.com/products/python/scripttease/
 Author: Shawn Davis
 Author-email: shawn@develmaycare.com
 License: UNKNOWN
-Download-URL: https://github.com/develmaycare/python-scripttease
-Project-URL: Documentation, https://docs.develmaycare.com/en/python-scripttease/latest/
-Project-URL: Source, https://github.com/develmaycare/python-scripttease
-Project-URL: Tracker, https://github.com/develmaycare/python-scripttease/issues/
+Download-URL: https://gittraction.com/diff6/python-scripttease
+Project-URL: Documentation, https://docs.diff6.com/en/python-scripttease/latest/
+Project-URL: Source, https://gittraction.com/diff6/python-scripttease
+Project-URL: Tracker, https://gittraction.com/diff6/python-scripttease/issues
 Description: # Python Script Tease
         
         ![](https://img.shields.io/badge/status-active-green.svg)
-        ![](https://img.shields.io/badge/stage-development-blue.svg)
+        ![](https://img.shields.io/badge/stage-stable-green.svg)
         ![](https://img.shields.io/badge/coverage-100%25-green.svg)
         
         A collection of classes and commands for automated command line scripting using Python.
+        
+        ## Install
+        
+        ```bash
+        pip install python-scripttease;
+        ```
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `python-scripttease-6.8.2/python_scripttease.egg-info/PKG-INFO` & `python-scripttease-7.0.0/python_scripttease.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Metadata-Version: 2.1
 Name: python-scripttease
-Version: 6.8.2
+Version: 7.0.0
 Summary: A collection of classes and commands for automated command line scripting using Python.
 Home-page: https://develmaycare.com/products/python/scripttease/
 Author: Shawn Davis
 Author-email: shawn@develmaycare.com
 License: UNKNOWN
-Download-URL: https://github.com/develmaycare/python-scripttease
-Project-URL: Documentation, https://docs.develmaycare.com/en/python-scripttease/latest/
-Project-URL: Source, https://github.com/develmaycare/python-scripttease
-Project-URL: Tracker, https://github.com/develmaycare/python-scripttease/issues/
+Download-URL: https://gittraction.com/diff6/python-scripttease
+Project-URL: Documentation, https://docs.diff6.com/en/python-scripttease/latest/
+Project-URL: Source, https://gittraction.com/diff6/python-scripttease
+Project-URL: Tracker, https://gittraction.com/diff6/python-scripttease/issues
 Description: # Python Script Tease
         
         ![](https://img.shields.io/badge/status-active-green.svg)
-        ![](https://img.shields.io/badge/stage-development-blue.svg)
+        ![](https://img.shields.io/badge/stage-stable-green.svg)
         ![](https://img.shields.io/badge/coverage-100%25-green.svg)
         
         A collection of classes and commands for automated command line scripting using Python.
+        
+        ## Install
+        
+        ```bash
+        pip install python-scripttease;
+        ```
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `python-scripttease-6.8.2/python_scripttease.egg-info/SOURCES.txt` & `python-scripttease-7.0.0/python_scripttease.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 python_scripttease.egg-info/dependency_links.txt
 python_scripttease.egg-info/entry_points.txt
 python_scripttease.egg-info/not-zip-safe
 python_scripttease.egg-info/requires.txt
 python_scripttease.egg-info/top_level.txt
 scripttease/__init__.py
 scripttease/constants.py
-scripttease/factory.py
+scripttease/exceptions.py
 scripttease/variables.py
 scripttease/version.py
 scripttease/cli/__init__.py
 scripttease/cli/initialize.py
 scripttease/cli/subcommands.py
-scripttease/library/__init__.py
-scripttease/library/scripts.py
-scripttease/library/commands/__init__.py
-scripttease/library/commands/base.py
-scripttease/library/commands/templates.py
-scripttease/library/overlays/__init__.py
-scripttease/library/overlays/centos.py
-scripttease/library/overlays/common.py
-scripttease/library/overlays/django.py
-scripttease/library/overlays/mysql.py
-scripttease/library/overlays/pgsql.py
-scripttease/library/overlays/posix.py
-scripttease/library/overlays/ubuntu.py
-scripttease/parsers/__init__.py
-scripttease/parsers/base.py
-scripttease/parsers/ini.py
-scripttease/parsers/utils.py
-scripttease/parsers/yaml.py
+scripttease/lib/__init__.py
+scripttease/lib/contexts.py
+scripttease/lib/factories.py
+scripttease/lib/commands/__init__.py
+scripttease/lib/commands/base.py
+scripttease/lib/commands/centos.py
+scripttease/lib/commands/django.py
+scripttease/lib/commands/messages.py
+scripttease/lib/commands/mysql.py
+scripttease/lib/commands/pgsql.py
+scripttease/lib/commands/php.py
+scripttease/lib/commands/posix.py
+scripttease/lib/commands/python.py
+scripttease/lib/commands/ubuntu.py
+scripttease/lib/loaders/__init__.py
+scripttease/lib/loaders/base.py
+scripttease/lib/loaders/ini.py
+scripttease/lib/loaders/yaml.py
```

### Comparing `python-scripttease-6.8.2/scripttease/library/overlays/centos.py` & `python-scripttease-7.0.0/scripttease/lib/commands/centos.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,53 @@
 # Imports
 
 from commonkit import split_csv
-from ..commands import Command, Template
-from .common import COMMON_MAPPINGS
+from .base import Command
 from .django import DJANGO_MAPPINGS
+from .messages import MESSAGE_MAPPINGS
 from .mysql import MYSQL_MAPPINGS
 from .pgsql import PGSQL_MAPPINGS
-from .posix import POSIX_MAPPINGS, Function
+from .php import PHP_MAPPINGS
+from .posix import POSIX_MAPPINGS
+from .python import PYTHON_MAPPINGS
 
 # Exports
 
 __all__ = (
-    "MAPPINGS",
+    "CENTOS_MAPPINGS",
     "apache",
     "apache_reload",
     "apache_restart",
     "apache_start",
     "apache_stop",
     "apache_test",
-    "command_exists",
     "service_reload",
     "service_restart",
     "service_start",
     "service_stop",
     "system",
     "system_install",
     "system_reboot",
     "system_update",
     "system_upgrade",
     "system_uninstall",
-    "template",
     "user",
-    "Function",
 )
 
-
-def command_exists(name):
-    """Indicates whether a given command exists in this overaly.
-
-    :param name: The name of the command.
-    :type name: str
-
-    :rtype: bool
-
-    """
-    return name in MAPPINGS
+# Functions
 
 
 def apache(op, **kwargs):
     """Execute an Apache-related command.
 
-    - op (str): The operation to perform; reload, restart, start, stop, test.
+    :param op: The operation to perform; ``reload``, ``restart``, ``start``, ``stop``, ``test``.
+    :type op: str
 
     """
+    # See https://unix.stackexchange.com/questions/258854/disable-and-enable-modules-in-apache-centos7
     if op == "reload":
         return apache_reload(**kwargs)
     elif op == "restart":
         return apache_restart(**kwargs)
     elif op == "start":
         return apache_start(**kwargs)
     elif op == "stop":
@@ -64,171 +55,183 @@
     elif op == "test":
         return apache_test(**kwargs)
     else:
         raise NameError("Unrecognized or unsupported apache operation: %s" % op)
 
 
 def apache_reload(**kwargs):
+    """Reload the apache service."""
     kwargs.setdefault("comment", "reload apache")
     kwargs.setdefault("register", "apache_reloaded")
 
     return Command("apachectl –k reload", **kwargs)
 
 
 def apache_restart(**kwargs):
+    """Restart the apache service."""
     kwargs.setdefault("comment", "restart apache")
     kwargs.setdefault("register", "apache_restarted")
 
     return Command("apachectl –k restart", **kwargs)
 
 
 def apache_start(**kwargs):
+    """Start the apache service."""
     kwargs.setdefault("comment", "start apache")
     kwargs.setdefault("register", "apache_started")
 
     return Command("apachectl –k start", **kwargs)
 
 
 def apache_stop(**kwargs):
+    """Stop the apache service."""
     kwargs.setdefault("comment", "stop apache")
 
     return Command("apachectl –k stop", **kwargs)
 
 
 def apache_test(**kwargs):
+    """Run a configuration test on apache."""
     kwargs.setdefault("comment", "check apache configuration")
     kwargs.setdefault("register", "apache_checks_out")
 
     return Command("apachectl configtest", **kwargs)
 
 
-def service_reload(name, **kwargs):
+def service_reload(service, **kwargs):
     """Reload a service.
 
-    - name (str): The service name.
+    :param service: The service name.
+    :type service: str
 
     """
-    kwargs.setdefault("comment", "reload %s service" % name)
-    kwargs.setdefault("register", "%s_reloaded" % name)
+    kwargs.setdefault("comment", "reload %s service" % service)
+    kwargs.setdefault("register", "%s_reloaded" % service)
 
-    return Command("systemctl reload %s" % name, **kwargs)
+    return Command("systemctl reload %s" % service, **kwargs)
 
 
-def service_restart(name, **kwargs):
+def service_restart(service, **kwargs):
     """Restart a service.
 
-    - name (str): The service name.
+    :param service: The service name.
+    :type service: str
 
     """
-    kwargs.setdefault("comment", "restart %s service" % name)
-    kwargs.setdefault("register", "%s_restarted" % name)
+    kwargs.setdefault("comment", "restart %s service" % service)
+    kwargs.setdefault("register", "%s_restarted" % service)
 
-    return Command("ssystemctl restart %s" % name, **kwargs)
+    return Command("ssystemctl restart %s" % service, **kwargs)
 
 
-def service_start(name, **kwargs):
+def service_start(service, **kwargs):
     """Start a service.
 
-    - name (str): The service name.
+    :param service: The service name.
+    :type service: str
 
     """
-    kwargs.setdefault("comment", "start %s service" % name)
-    kwargs.setdefault("register", "%s_started" % name)
+    kwargs.setdefault("comment", "start %s service" % service)
+    kwargs.setdefault("register", "%s_started" % service)
 
-    return Command("systemctl start %s" % name, **kwargs)
+    return Command("systemctl start %s" % service, **kwargs)
 
 
-def service_stop(name, **kwargs):
+def service_stop(service, **kwargs):
     """Stop a service.
 
-    - name (str): The service name.
+    :param service: The service name.
+    :type service: str
 
     """
-    kwargs.setdefault("comment", "stop %s service" % name)
-    kwargs.setdefault("register", "%s_stopped" % name)
+    kwargs.setdefault("comment", "stop %s service" % service)
+    kwargs.setdefault("register", "%s_stopped" % service)
 
-    return Command("systemctl stop %s" % name, **kwargs)
+    return Command("systemctl stop %s" % service, **kwargs)
 
 
 def system(op, **kwargs):
     """Perform a system operation.
 
-    - op (str): The operation to perform; reboot, update, upgrade.
+    :param op: The operation to perform; ``reboot``, ``update``, ``upgrade``.
+    :type op: str
 
     """
     if op == "reboot":
         return system_reboot(**kwargs)
     elif op == "update":
         return system_update(**kwargs)
     elif op == "upgrade":
         return system_upgrade(**kwargs)
     else:
         raise NameError("Unrecognized or unsupported system operation: %s" % op)
 
 
-def system_install(name, **kwargs):
+def system_install(package, **kwargs):
     """Install a system-level package.
 
-    - name (str): The name of the package to install.
+    :param package: The name of the package to install.
+    :type package: str
 
     """
-    kwargs.setdefault("comment", "install system package %s" % name)
+    kwargs.setdefault("comment", "install system package %s" % package)
 
-    return Command("yum install -y %s" % name, **kwargs)
+    return Command("yum install -y %s" % package, **kwargs)
 
 
 def system_reboot(**kwargs):
+    """Reboot the system."""
     kwargs.setdefault("comment", "reboot the system")
 
     return Command("reboot", **kwargs)
 
 
-def system_uninstall(name, **kwargs):
+def system_uninstall(package, **kwargs):
     """Uninstall a system-level package.
 
-    - name (str): The name of the package to uninstall.
+    :param package: The name of the package to remove.
+    :type package: str
 
     """
-    kwargs.setdefault("comment", "remove system package %s" % name)
+    kwargs.setdefault("comment", "remove system package %s" % package)
 
-    return Command("yum remove -y %s" % name, **kwargs)
+    return Command("yum remove -y %s" % package, **kwargs)
 
 
 def system_update(**kwargs):
+    """Update the system's package info."""
     kwargs.setdefault("comment", "update system package info")
 
     return Command("yum check-update", **kwargs)
 
 
 def system_upgrade(**kwargs):
+    """updated the system."""
     kwargs.setdefault("comment", "upgrade the system")
 
     return Command("yum update -y", **kwargs)
 
 
-def template(source, target, backup=True, parser=None, **kwargs):
-    """Create a file from a template.
+def user(name, groups=None, home=None, op="add", password=None, **kwargs):
+    """Create or remove a user.
 
-    - source (str): The path to the template file.
-    - target (str): The path to where the new file should be created.
-    - backup (bool): Indicates whether a backup should be made if the target file already exists.
-    - parser (str): The parser to use ``jinja`` (the default) or ``simple``.
+    :param name: The username.
+    :type name: str
 
-    """
-    return Template(source, target, backup=backup, parser=parser, **kwargs)
+    :param groups: A list of groups to which the user should belong.
+    :type groups: list | str
 
+    :param home: The path to the user's home directory.
+    :type home: str
 
-def user(name, groups=None, home=None, op="add", password=None, **kwargs):
-    """Create or remove a user.
+    :param op: The operation to perform; ``add`` or ``remove``.
+    :type op:
 
-    - name (str): The user name.
-    - groups (str | list): A list of groups to which the user should belong.
-    - home (str): The path to the user's home directory.
-    - op (str); The operation to perform; ``add`` or ``remove``.
-    - password (str): The user's password. (NOT IMPLEMENTED)
+    :param password: The user's password. (NOT IMPLEMENTED)
+    :type password: str
 
     """
     if op == "add":
         kwargs.setdefault("comment", "create a user named %s" % name)
 
         commands = list()
 
@@ -244,38 +247,39 @@
 
         if type(groups) in [list, tuple]:
             for group in groups:
                 commands.append(Command("gpasswd -a %s %s" % (name, group), **kwargs))
 
         a = list()
         for c in commands:
-            a.append(c.get_statement(suppress_comment=True))
+            a.append(c.get_statement(include_comment=True))
 
         return Command("\n".join(a), **kwargs)
     elif op == "remove":
         kwargs.setdefault("comment", "remove a user named %s" % name)
         return Command("userdel -r %s" % name, **kwargs)
     else:
         raise NameError("Unsupported or unrecognized operation: %s" % op)
 
 
-MAPPINGS = {
+CENTOS_MAPPINGS = {
     'apache': apache,
     'install': system_install,
     'reboot': system_reboot,
     'reload': service_reload,
     'restart': service_restart,
     'start': service_start,
     'stop': service_stop,
     'system': system,
-    'template': template,
     'update': system_update,
     'uninstall': system_uninstall,
     'upgrade': system_upgrade,
     'user': user,
 }
 
-MAPPINGS.update(COMMON_MAPPINGS)
-MAPPINGS.update(DJANGO_MAPPINGS)
-MAPPINGS.update(MYSQL_MAPPINGS)
-MAPPINGS.update(PGSQL_MAPPINGS)
-MAPPINGS.update(POSIX_MAPPINGS)
+CENTOS_MAPPINGS.update(DJANGO_MAPPINGS)
+CENTOS_MAPPINGS.update(MESSAGE_MAPPINGS)
+CENTOS_MAPPINGS.update(MYSQL_MAPPINGS)
+CENTOS_MAPPINGS.update(PHP_MAPPINGS)
+CENTOS_MAPPINGS.update(PGSQL_MAPPINGS)
+CENTOS_MAPPINGS.update(POSIX_MAPPINGS)
+CENTOS_MAPPINGS.update(PYTHON_MAPPINGS)
```

### Comparing `python-scripttease-6.8.2/scripttease/library/overlays/django.py` & `python-scripttease-7.0.0/scripttease/lib/commands/django.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,188 +1,167 @@
-# Imports
+from ...constants import EXCLUDED_KWARGS
+from .base import Command
 
-import os
-from ..commands import Command
 
-# Exports
+def django(management_command, *args, excluded_kwargs=None, **kwargs):
+    """Common function for assembling Django management commands.
 
-__all__ = (
-    "DJANGO_MAPPINGS",
-    "django",
-    "django_check",
-    "django_collect_static",
-    "django_dumpdata",
-    "django_loaddata",
-    "django_migrate",
-)
+    :param management_command: The name of the management command.
+    :type management_command: str
 
-# Functions
+    :param excluded_kwargs: A dictionary of kwargs that should be excluded from the management command parameters.
+    :param excluded_kwargs: dict
 
+    :rtype: scripttease.lib.commands.base.Command
 
-def _django(name, *args, venv=None, **kwargs):
-    """Process a django-based command.
+    If provided, args are passed directly to the command as positional parameters.
 
-    :param name: The name of the management command.
-    :type name: str
+    Any provided kwargs are converted to long form parameters. For example, database="alternative_db" becomes
+    ``--database="alternative_db"``.
 
-    :param venv: The virtual environment to use.
-    :type venv: str
+    A kwarg with a ``True`` value becomes a long form parameter with no value. For example, natural_foreign=True becomes
+    ``--natural-foreign``.
 
-    args and kwargs are used to instantiate the command instance.
-
-    This exists because we need ``django()`` to serve as an interface for any management command.
+    Finally, any kwarg that is not a string is passed without quotes. For example, testing=1 becomes ``--testing=1``.
 
     """
+    # The excluded parameters (filtered below) may vary based on implementation. We do, however, need a default.
+    excluded_kwargs = excluded_kwargs or EXCLUDED_KWARGS
+
+    venv = kwargs.pop("venv", None)
     if venv is not None:
         kwargs['prefix'] = "source %s/bin/activate" % venv
 
-    kwargs.setdefault("comment", "run %s django management command" % name)
-
-    # Base parameters need to be captured, because all others are assumed to be switches for the management command.
-    _kwargs = {
-        'comment': kwargs.pop("comment", None),
-        'condition': kwargs.pop("condition", None),
-        'cd': kwargs.pop("cd", None),
-        'environments': kwargs.pop("environments", None),
-        'function': kwargs.pop("function", None),
-        # 'local': kwargs.pop("local", False),
-        'prefix': kwargs.pop("prefix", None),
-        'register': kwargs.pop("register", None),
-        'shell': kwargs.pop("shell", "/bin/bash"),
-        'stop': kwargs.pop("stop", False),
-        'sudo': kwargs.pop('sudo', False),
-        'tags': kwargs.pop("tags", None),
-    }
+    # Django's management commands can have a number of options. We need to filter out internal parameters so that these
+    # are not used as options for the management command.
+    _kwargs = dict()
+    for key in excluded_kwargs:
+        if key in kwargs:
+            _kwargs[key] = kwargs.pop(key)
 
-    statement = list()
-    statement.append("./manage.py %s" % name)
+    if 'comment' not in _kwargs:
+        _kwargs['comment'] = "run %s django management command" % management_command
 
-    # Remaining kwargs are assumed to be switches.
+    a = list()
+    a.append("./manage.py %s" % management_command)
     for key, value in kwargs.items():
         key = key.replace("_", "-")
-        if type(value) is bool:
-            if value is True:
-                statement.append("--%s" % key)
+        if type(value) is bool and value is True:
+            a.append("--%s" % key)
+        elif type(value) is str:
+            a.append('--%s="%s"' % (key, value))
         else:
-            statement.append("--%s=%s" % (key, value))
+            a.append('--%s=%s' % (key, value))
 
-    if len(args) > 0:
-        statement.append(" ".join(args))
+    _args = list(args)
+    if len(_args) > 0:
+        a.append(" ".join(_args))
 
-    return Command(" ".join(statement), **_kwargs)
+    statement = " ".join(a)
 
+    return Command(statement, **_kwargs)
 
-def django(name, *args, venv=None, **kwargs):
-    """Run any Django management command.
 
-    - name (str): The name of the management command.
-    - venv (str): The of the virtual environment to use.
-
-    args are passed as positional arguments, while kwargs are given as switches.
+def django_check(**kwargs):
+    """Run Django checks."""
+    kwargs.setdefault("comment", "run django checks")
+    kwargs.setdefault("register", "django_checks_out")
+    return django("check", **kwargs)
 
-    """
-    if name == "check":
-        return django_check(venv=venv, **kwargs)
-    elif name in ("collectstatic", "static"):
-        return django_collect_static(venv=venv, **kwargs)
-    elif name == "migrate":
-        return django_migrate(venv=venv, **kwargs)
-    else:
-        return _django(name, *args, venv=venv, **kwargs)
 
+def django_createsuperuser(username, email=None, **kwargs):
+    """Create a superuser account.
 
-def django_check(venv=None, **kwargs):
-    """Run the Django check command.
+    :param username: The name for the user account.
+    :type username: str
 
-    - venv (str): The of the virtual environment to use.
+    :param email: The user's email address. Optional, but recommended because the account must be created without a
+                  password.
+    :type email: str
 
     """
-    kwargs.setdefault("comment", "run django checks")
-    kwargs.setdefault("register", "django_checks_out")
+    kwargs.setdefault("comment", "create the %s superuser" % username)
+    kwargs['username'] = username
+    kwargs['noinput'] = True
 
-    return _django("check", venv=venv, **kwargs)
+    if email is not None:
+        kwargs['email'] = email
 
+    return django("createsuperuser", **kwargs)
 
-def django_collect_static(venv=None, **kwargs):
-    """Collect static files.
 
-    - venv (str): The of the virtual environment to use.
+def django_dump(target, path=None, **kwargs):
+    """Dump data fixtures.
 
-    """
-    kwargs.setdefault("comment", "collect static files")
+    :param target: The app name or ``app.ModelName``.
+    :type target: str
 
-    return _django("collectstatic", venv=venv, **kwargs)
+    :param path: The path to the fixture file.
+    :type path: str
 
+    """
+    kwargs.setdefault("comment", "dump app/model data for %s" % target)
+    kwargs.setdefault("format", "json")
+    kwargs.setdefault("indent", 4)
 
-def django_dumpdata(app_name, base_path="local", file_name="initial", indent=4, natural_foreign=False,
-                    natural_primary=False, path=None, venv=None, **kwargs):
-    """Dump data from the database.
-
-    - app_name (str): The name (app label) of the app. ``app_label.ModelName`` may also be given.
-    - base_path (str): The path under which apps are located in source.
-    - file_name (str): The file name to which the data will be dumped.
-    - indent (int): Indentation of the exported fixtures.
-    - natural_foreign (bool): Use the natural foreign parameter.
-    - natural_primary (bool): Use the natural primary parameter.
-    - path (str): The path to the data file.
-    - venv (str): The of the virtual environment to use.
+    app = target
+    file_name = "%s/initial.%s" % (app, kwargs['format'])
+    if "." in target:
+        app, model = target.split(".")
+        file_name = "%s/%s.%s" % (app, model.lower(), kwargs['format'])
 
-    """
-    kwargs.setdefault("comment", "export fixtures for %s" % app_name)
+    if path is None:
+        path = "../fixtures/%s" % file_name
 
-    output_format = kwargs.pop("format", "json")
+    return django("dumpdata", target, "> %s" % path, **kwargs)
 
-    _path = path or os.path.join(base_path, app_name, "fixtures", "%s.%s" % (file_name, output_format))
 
-    return _django(
-        "dumpdata",
-        app_name,
-        "> %s" % _path,
-        format=output_format,
-        indent=indent,
-        natural_foreign=natural_foreign,
-        natural_primary=natural_primary,
-        venv=venv,
-        **kwargs
-    )
-
-
-def django_loaddata(app_name, base_path="local", file_name="initial", path=None, venv=None, **kwargs):
-    """Load data into the database.
-
-    - app_name (str): The name (app label) of the app. ``app_label.ModelName`` may also be given.
-    - base_path (str): The path under which apps are located in source.
-    - file_name (str): The file name to which the data will be dumped.
-    - path (str): The path to the data file.
-    - venv (str): The of the virtual environment to use.
+def django_load(target, path=None, **kwargs):
+    """Load data fixtures.
 
-    """
-    kwargs.setdefault("comment", "load fixtures for %s" % app_name)
+    :param target: The app name or ``app.ModelName``.
+    :type target: str
 
-    output_format = kwargs.pop("format", "json")
+    :param path: The path to the fixture file.
+    :type path: str
 
-    _path = path or os.path.join(base_path, app_name, "fixtures", "%s.%s" % (file_name, output_format))
+    """
+    kwargs.setdefault("comment", "load app/model data from %s" % target)
+    input_format = kwargs.pop("format", "json")
 
-    return _django("loaddata", _path, venv=venv, **kwargs)
+    app = target
+    file_name = "%s/initial.%s" % (app, input_format)
+    if "." in target:
+        app, model = target.split(".")
+        file_name = "%s/%s.%s" % (app, model.lower(), input_format)
 
+    if path is None:
+        path = "../fixtures/%s" % file_name
 
-def django_migrate(venv=None, **kwargs):
-    """Apply database migrations.
+    return django("loaddata", path, **kwargs)
 
-    - venv (str): The of the virtual environment to use.
 
-    """
-    kwargs.setdefault("comment", "run django database migrations")
+def django_migrate(**kwargs):
+    """Apply database migrations."""
+    kwargs.setdefault("comment", "apply database migrations")
+    return django("migrate", **kwargs)
 
-    return _django("migrate", venv=venv, **kwargs)
 
-# Mapping
+def django_static(**kwargs):
+    """Collect static files."""
+    kwargs.setdefault("comment", "collect static files")
+    kwargs.setdefault("noinput", True)
+    return django("collectstatic", **kwargs)
 
 
 DJANGO_MAPPINGS = {
     'django': django,
     'django.check': django_check,
-    'django.collect_static': django_collect_static,
-    'django.dumpdata': django_dumpdata,
-    'django.loaddata': django_loaddata,
+    'django.collectstatic': django_static,
+    'django.createsuperuser': django_createsuperuser,
+    'django.dump': django_dump,
+    'django.dumpdata': django_dump,
+    'django.load': django_load,
+    'django.loaddata': django_load,
     'django.migrate': django_migrate,
+    'django.static': django_static,
 }
```

### Comparing `python-scripttease-6.8.2/scripttease/library/overlays/posix.py` & `python-scripttease-7.0.0/scripttease/lib/commands/posix.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,52 @@
-# Imports
-
-from commonkit import indent, split_csv
 import os
-from ..commands import Command
+from .base import Command, MultipleCommands, Prompt
+
+
+def append(path, content=None, **kwargs):
+    """Append content to a file.
+
+    :param path: The path to the file.
+    :type path: str
 
-# Exports
+    :param content: The content to be appended.
+    :type content: str
 
-__all__ = (
-    "POSIX_MAPPINGS",
-    "archive",
-    "certbot",
-    "dialog",
-    "echo",
-    "extract",
-    "file_append",
-    "file_copy",
-    "file_write",
-    "mkdir",
-    "move",
-    "perms",
-    "prompt",
-    "remove",
-    "rename",
-    "rsync",
-    "scopy",
-    "sed",
-    "symlink",
-    "touch",
-    "wait",
-    "Function",
-    "Prompt",
-)
+    """
+    kwargs.setdefault("comment", "append to %s" % path)
 
-# Functions
+    statement = 'echo "%s" >> %s' % (content or "", path)
+
+    return Command(statement, **kwargs)
 
 
 def archive(from_path, absolute=False, exclude=None, file_name="archive.tgz", strip=None, to_path=".", view=False,
             **kwargs):
     """Create a file archive.
 
-    - from_path (str): The path that should be archived.
-    - absolute (bool): Set to ``True`` to preserve the leading slash.
-    - exclude (str): A pattern to be excluded from the archive.
-    - strip (int): Remove the specified number of leading elements from the path.
-    - to_path (str): Where the archive should be created. This should *not* include the file name.
-    - view (bool): View the output of the command as it happens.
+    :param from_path: The path that should be archived.
+    :type from_path: str
+
+    :param absolute: Set to ``True`` to preserve the leading slash.
+    :type absolute: bool
+
+    :param exclude: A pattern to be excluded from the archive.
+    :type exclude: str
+
+    :param file_name: The name of the archive file.
+    :type file_name: str
+
+    :param strip: Remove the specified number of leading elements from the path.
+    :type strip: int
+
+    :param to_path: Where the archive should be created. This should *not* include the file name.
+    :type to_path: str
+
+    :param view: View the output of the command as it happens.
+    :type view: bool
 
     """
     tokens = ["tar"]
     switches = ["-cz"]
 
     if absolute:
         switches.append("P")
@@ -60,296 +58,351 @@
 
     if exclude:
         tokens.append("--exclude %s" % exclude)
 
     if strip:
         tokens.append("--strip-components %s" % strip)
 
-    to_path = os.path.join(to_path, file_name)
+    to_path = "%s/%s" % (to_path, file_name)
     tokens.append('-f %s %s' % (to_path, from_path))
 
     name = " ".join(tokens)
 
     return Command(name, **kwargs)
 
 
 def certbot(domain_name, email=None, webroot=None, **kwargs):
     """Get new SSL certificate from Let's Encrypt.
 
-    - domain_name (str): The domain name for which the SSL certificate is requested.
-    - email (str): The email address of the requester sent to the certificate authority. Required.
-    - webroot (str): The directory where the challenge file will be created.
+    :param domain_name: The domain name for which the SSL certificate is requested.
+    :type domain_name: str
+
+    :param email: The email address of the requester sent to the certificate authority. Required.
+    :type email: str
+
+    :param webroot: The directory where the challenge file will be created.
+    :type webroot: str
 
     """
     _email = email or os.environ.get("SCRIPTTEASE_CERTBOT_EMAIL", None)
     _webroot = webroot or os.path.join("/var", "www", "domains", domain_name.replace(".", "_"), "www")
 
     if not _email:
         raise ValueError("Email is required for certbot command.")
 
     template = "certbot certonly --agree-tos --email %(email)s -n --webroot -w %(webroot)s -d %(domain_name)s"
-    name = template % {
+    statement = template % {
         'domain_name': domain_name,
         'email': _email,
         'webroot': _webroot,
     }
 
-    return Command(name, **kwargs)
+    return Command(statement, **kwargs)
 
 
-def dialog(message, height=15, title="Message", width=100, **kwargs):
-    """Display a dialog message.
+def copy(from_path, to_path, overwrite=False, recursive=False, **kwargs):
+    """Copy a file or directory.
+
+    :param from_path: The file or directory to be copied.
+    :type from_path: str
+
+    :param to_path: The location to which the file or directory should be copied.
+    :type to_path: str
 
-    - message (str): The message to be displayed.
-    - height (int): The height of the dialog.
-    - title (str): The title of the dialog.
-    - width (int): The width of the dialog.
+    :param overwrite: Indicates files and directories should be overwritten if they exist.
+    :type overwrite: bool
+
+    :param recursive: Copy sub-directories.
+    :type recursive: bool
 
     """
-    kwargs.setdefault("comment", "display a dialog message")
+    kwargs.setdefault("comment", "copy %s to %s" % (from_path, to_path))
 
     a = list()
-    a.append('dialog --clear --backtitle "%s"' % title)
-    a.append('--msgbox "%s" %s %s; clear;' % (message, height, width))
+    a.append("cp")
 
-    return Command(" ".join(a), **kwargs)
+    if not overwrite:
+        a.append("-n")
 
+    if recursive:
+        a.append("-R")
 
-def echo(message, **kwargs):
-    """Echo a message.
+    a.append(from_path)
+    a.append(to_path)
 
-    - message (str): The message to be printed to screen.
+    return Command(" ".join(a), **kwargs)
 
-    """
-    kwargs.setdefault("comment", "print message to screen")
 
-    return Command('echo "%s"' % message, **kwargs)
+def directory(path, group=None, mode=None, owner=None, recursive=False, **kwargs):
+    """Create a directory.
 
+    :param path: The path to be created.
+    :type path: str
 
-def extract(from_path, absolute=False, exclude=None, strip=None, to_path=None, view=False, **kwargs):
-    """Extract a file archive.
+    :param mode: The access permissions of the new directory.
+    :type mode: int | str
 
-    - from_path (str): The path that should be archived.
-    - absolute (bool): Set to ``True`` to preserve the leading slash.
-    - exclude (str): A pattern to be excluded from the archive.
-    - strip (int): Remove the specified number of leading elements from the path.
-    - to_path (str): Where the archive should be extracted. This should *not* include the file name.
-    - view (bool): View the output of the command as it happens.
+    :param recursive: Create all directories along the path.
+    :type recursive: bool
 
     """
-    _to_path = to_path or "./"
+    comment = kwargs.pop("comment", "create directory %s" % path)
 
-    tokens = ["tar"]
-    switches = ["-xz"]
+    statement = ["mkdir"]
+    if mode is not None:
+        statement.append("-m %s" % mode)
 
-    if absolute:
-        switches.append("P")
+    if recursive:
+        statement.append("-p")
 
-    if view:
-        switches.append("v")
+    statement.append(path)
 
-    tokens.append("".join(switches))
+    mkdir = Command(" ".join(statement), comment=comment, **kwargs)
 
-    if exclude:
-        tokens.append("--exclude %s" % exclude)
+    chgrp = None
+    if group:
+        if recursive:
+            chgrp = Command("chgrp -R %s %s" % (group, path), comment="set %s group on %s" % (group, path), **kwargs)
+        else:
+            chgrp = Command("chgrp %s %s" % (group, path), comment="set %s group on %s" % (group, path), **kwargs)
 
-    if strip:
-        tokens.append("--strip-components %s" % strip)
+    chown = None
+    if owner:
+        if recursive:
+            chown = Command("chown -R %s %s" % (owner, path), comment="set %s owner on %s" % (owner, path), **kwargs)
+        else:
+            chown = Command("chown %s %s" % (owner, path), comment="set %s owner on %s" % (owner, path), **kwargs)
 
-    tokens.append('-f %s %s' % (from_path, _to_path))
+    commands = list()
+    commands.append(mkdir)
+    if chgrp is not None:
+        commands.append(chgrp)
 
-    name = " ".join(tokens)
+    if chown is not None:
+        commands.append(chown)
 
-    return Command(name, **kwargs)
+    if len(commands) == 1:
+        return commands[0]
 
+    return MultipleCommands(commands, comment=comment)
 
-def file_append(path, content=None, **kwargs):
-    """Append content to a file.
 
-    - path (str): The path to the file.
-    - content (str): The content to be appended.
+def extract(from_path, absolute=False, exclude=None, strip=None, to_path=None, view=False, **kwargs):
+    """Extract a file archive.
 
-    """
-    kwargs.setdefault("comment", "append to %s" % path)
+    :param from_path: The path to be extracted.
+    :type from_path: str
 
-    statement = 'echo "%s" >> %s' % (content or "", path)
+    :param absolute: Set to ``True`` to preserve the leading slash.
+    :type absolute: bool
 
-    return Command(statement, **kwargs)
+    :param exclude: A pattern to be excluded from the extraction.
+    :type exclude: str
 
+    :param strip: Remove the specified number of leading elements from the path.
+    :type strip: int
 
-def file_copy(from_path, to_path, overwrite=False, recursive=False, **kwargs):
-    """Copy a file or directory.
+    :param to_path: Where the extraction should occur.
+    :type to_path: str
 
-    - from_path (str): The file or directory to be copied.
-    - to_path (str): The location to which the file or directory should be copied.
-    - overwrite (bool): Indicates files and directories should be overwritten if they exist.
-    - recursive (bool): Copy sub-directories.
+    :param view: View the output of the command as it happens.
+    :type view: bool
 
     """
-    kwargs.setdefault("comment", "copy %s to %s" % (from_path, to_path))
-
-    a = list()
-    a.append("cp")
-
-    if not overwrite:
-        a.append("-n")
+    _to_path = to_path or "./"
 
-    if recursive:
-        a.append("-R")
+    tokens = ["tar"]
+    switches = ["-xz"]
 
-    a.append(from_path)
-    a.append(to_path)
+    if absolute:
+        switches.append("P")
 
-    return Command(" ".join(a), **kwargs)
+    if view:
+        switches.append("v")
 
+    tokens.append("".join(switches))
 
-def file_write(path, content=None, **kwargs):
-    """Write to a file.
+    if exclude:
+        tokens.append("--exclude %s" % exclude)
 
-    - path (str): The file to be written.
-    - content (str): The content to be written. Note: If omitted, this command is equivalent to ``touch``.
+    if strip:
+        tokens.append("--strip-components %s" % strip)
 
-    """
-    _content = content or ""
+    tokens.append('-f %s %s' % (from_path, _to_path))
 
-    kwargs.setdefault("comment", "write to %s" % path)
+    statement = " ".join(tokens)
 
-    a = list()
+    return Command(statement, **kwargs)
 
-    if len(_content.split("\n")) > 1:
-        a.append("cat > %s << EOF" % path)
-        a.append(_content)
-        a.append("EOF")
-    else:
-        a.append('echo "%s" > %s' % (_content, path))
 
-    return Command(" ".join(a), **kwargs)
+def link(source, force=False, target=None, **kwargs):
+    """Create a symlink.
 
+    :param source: The source of the link.
+    :type source: str
 
-def mkdir(path, mode=None, recursive=True, **kwargs):
-    """Create a directory.
+    :param force: Force the creation of the link.
+    :type force: bool
 
-    - path (str): The path to be created.
-    - mode (int | str): The access permissions of the new directory.
-    - recursive (bool): Create all directories along the path.
+    :param target: The name or path of the target. Defaults to the base name of the source path.
+    :type target: str
 
     """
-    kwargs.setdefault("comment", "create directory %s" % path)
+    _target = target or os.path.basename(source)
 
-    statement = ["mkdir"]
-    if mode is not None:
-        statement.append("-m %s" % mode)
+    kwargs.setdefault("comment", "link to %s" % source)
 
-    if recursive:
-        statement.append("-p")
+    statement = ["ln -s"]
 
-    statement.append(path)
+    if force:
+        statement.append("-f")
+
+    statement.append(source)
+    statement.append(_target)
 
     return Command(" ".join(statement), **kwargs)
 
 
 def move(from_path, to_path, **kwargs):
     """Move a file or directory.
-    
-    - from_path (str): The current path.
-    - to_path (str): The new path.
-    
+
+    :param from_path: The current path.
+    :type from_path: str
+
+    :param to_path: The new path.
+    :type to_path: str
+
     """
     kwargs.setdefault("comment", "move %s to %s" % (from_path, to_path))
     statement = "mv %s %s" % (from_path, to_path)
 
     return Command(statement, **kwargs)
 
 
 def perms(path, group=None, mode=None, owner=None, recursive=False, **kwargs):
     """Set permissions on a file or directory.
 
-    - path (str): The path to be changed.
-    - group (str): The name of the group to be applied.
-    - mode (int | str): The access permissions of the file or directory.
-    - owner (str): The name of the user to be applied.
-    - recursive: Create all directories along the path.
+    :param path: The path to be changed.
+    :type path: str
 
-    """
-    commands = list()
+    :param group: The name of the group to be applied.
+    :type group: str
 
-    kwargs['comment'] = "set permissions on %s" % path
+    :param mode: The access permissions of the file or directory.
+    :type mode: int | str
 
+    :param owner: The name of the user to be applied.
+    :type owner: str
+
+    :param recursive: Update all files and directories along the path.
+    :type recursive: bool
+
+    """
+    comment = kwargs.pop("comment", "set permissions on %s" % path)
+
+    chgrp = None
     if group is not None:
-        statement = ["chgrp"]
+        a = ["chgrp"]
 
         if recursive:
-            statement.append("-R")
+            a.append("-R")
 
-        statement.append(group)
-        statement.append(path)
+        a.append(group)
+        a.append(path)
 
-        commands.append(Command(" ".join(statement), **kwargs))
+        chgrp = Command(" ".join(a), comment="set %s group on %s" % (group, path), **kwargs)
 
-    if owner is not None:
-        statement = ["chown"]
+    chmod = None
+    if mode is not None:
+        a = ["chmod"]
 
         if recursive:
-            statement.append("-R")
+            a.append("-R")
 
-        statement.append(owner)
-        statement.append(path)
+        a.append(str(mode))
+        a.append(path)
 
-        commands.append(Command(" ".join(statement), **kwargs))
+        chmod = Command(" ".join(a), comment="set %s mode on %s" % (mode, path), **kwargs)
 
-    if mode is not None:
-        statement = ["chmod"]
+    chown = None
+    if owner is not None:
+        a = ["chown"]
 
         if recursive:
-            statement.append("-R")
+            a.append("-R")
 
-        statement.append(str(mode))
-        statement.append(path)
+        a.append(owner)
+        a.append(path)
 
-        commands.append(Command(" ".join(statement), **kwargs))
+        chown = Command(" ".join(a), comment="set %s owner on %s" % (owner, path), **kwargs)
 
-    kwargs.setdefault("comment", "set permissions on %s" % path)
+    commands = list()
+    if chgrp is not None:
+        commands.append(chgrp)
 
-    a = list()
-    for c in commands:
-        a.append(c.get_statement(suppress_comment=True))
+    if chmod is not None:
+        commands.append(chmod)
 
-    return Command("\n".join(a), **kwargs)
+    if chown is not None:
+        commands.append(chown)
 
+    if len(commands) == 1:
+        return commands[0]
 
-def prompt(name, back_title="Input", choices=None, default=None, fancy=False, help_text=None, label=None, **kwargs):
+    return MultipleCommands(commands, comment=comment, **kwargs)
+
+
+def prompt(name, back_title="Input", choices=None, default=None, dialog=False, help_text=None, label=None, **kwargs):
     """Prompt the user for input.
 
-    - name (str): The programmatic name of the input.
-    - back_title (str): The back title used with the dialog command.
-    - choices (str | list): A list of valid choices.
-    - default: The default value.
-    - fancy (bool): Use a dialog command for the prompt.
-    - help_text (str): The text to display with the dialog command.
-    - label (str): The label for the input.
+    :param name: The programmatic name of the input.
+    :type name: str
+
+    :param back_title: The back title used with the dialog command.
+    :type back_title: str
+
+    :param choices: A list of valid choices.
+    :type choices: list | str
+
+    :param default: The default value.
+    :type default: str
+
+    :param dialog: Use a dialog command for the prompt.
+    :type dialog: bool
+
+    :param help_text: The text to display with the dialog command.
+    :type help_text: str
+
+    :param label: The label for the input.
+    :type label: str
 
     """
     return Prompt(
         name,
         back_title=back_title,
         choices=choices,
         default=default,
-        fancy=fancy,
+        dialog=dialog,
         help_text=help_text,
         label=label,
         **kwargs
     )
 
 
 def remove(path, force=False, recursive=False, **kwargs):
     """Remove a file or directory.
 
-    - path (str): The path to be removed.
-    - force (bool): Force the removal.
-    - recursive (bool): Remove all directories along the path.
+    :param path: The path to be removed.
+    :type path: str
+
+    :param force: Force the removal.
+    :type force: bool
+
+    :param recursive: Remove all directories along the path.
+    :type recursive: bool
 
     """
     kwargs.setdefault("comment", "remove %s" % path)
 
     statement = ["rm"]
 
     if force:
@@ -359,39 +412,96 @@
         statement.append("-r")
 
     statement.append(path)
 
     return Command(" ".join(statement), **kwargs)
 
 
-def rename(from_name, to_name, **kwargs):
-    """Rename a file or directory.
+def replace(path, backup=".b", delimiter="/", find=None, sub=None, **kwargs):
+    """Find and replace text in a file.
+
+    :param path: The path to the file to be edited.
+    :type path: str
+
+    :param backup: The backup file extension to use.
+    :type backup: str
+
+    :param delimiter: The pattern delimiter.
+    :type delimiter: str
 
-    - from_name (str): The name (or path) of the existing file.
-    - to_name (str): The name (or path) of the new file.
+    :param find: The old text. Required.
+    :param find: str
+
+    :param sub: The new text. Required.
+    :type sub: str
 
     """
-    kwargs.setdefault("comment", "rename %s" % from_name)
-    return move(from_name, to_name, **kwargs)
+
+    kwargs.setdefault("comment", "find and replace in %s" % path)
+
+    context = {
+        'backup': backup,
+        'delimiter': delimiter,
+        'path': path,
+        'pattern': find,
+        'replace': sub,
+    }
+
+    template = "sed -i %(backup)s 's%(delimiter)s%(pattern)s%(delimiter)s%(replace)s%(delimiter)sg' %(path)s"
+
+    statement = template % context
+
+    return Command(statement, **kwargs)
+
+
+def run(statement, **kwargs):
+    """Run any command.
+
+    :param statement: The statement to be executed.
+    :type statement: str
+
+    """
+    kwargs.setdefault("comment", "run statement")
+
+    return Command(statement, **kwargs)
 
 
 def rsync(source, target, delete=False, exclude=None, host=None, key_file=None, links=True, port=22,
           recursive=True, user=None, **kwargs):
     """Synchronize a directory structure.
 
-    - source (str): The source directory.
-    - target (str): The target directory.
-    - delete (bool): Indicates target files that exist in source but not in target should be removed.
-    - exclude (str): The path to an exclude file.
-    - host (str): The host name or IP address. This causes the command to run over SSH.
-    - key_file (str): The privacy SSH key (path) for remote connections. User expansion is automatically applied.
-    - links (bool): Include symlinks in the sync.
-    - port (int): The SSH port to use for remote connections.
-    - recursive (bool): Indicates source contents should be recursively synchronized.
-    - user (str): The user name to use for remote connections.
+    :param source: The source directory.
+    :type source: str
+
+    :param target: The target directory.
+    :type target: str
+
+    :param delete: Indicates target files that exist in source but not in target should be removed.
+    :type delete: bool
+
+    :param exclude: The path to an exclude file.
+    :type exclude: str
+
+    :param host: The host name or IP address.
+    :type host: str
+
+    :param key_file: The privacy SSH key (path) for remote connections. User expansion is automatically applied.
+    :type key_file: str
+
+    :param links: Include symlinks in the sync.
+    :type links: bool
+
+    :param port: The SSH port to use for remote connections.
+    :type port: int
+
+    :param recursive: Indicates source contents should be recursively synchronized.
+    :type recursive: bool
+
+    :param user: The username to use for remote connections.
+    :type user: str
 
     """
     # - guess: When ``True``, the ``host``, ``key_file``, and ``user`` will be guessed based on the base name of
     #               the source path.
     # :type guess: bool
     # if guess:
     #     host = host or os.path.basename(source).replace("_", ".")
@@ -403,17 +513,26 @@
     #     user = user
 
     kwargs.setdefault("comment", "sync %s with %s" % (source, target))
 
     # rsync -e "ssh -i $(SSH_KEY) -p $(SSH_PORT)" -P -rvzc --delete
     # $(OUTPUTH_PATH) $(SSH_USER)@$(SSH_HOST):$(UPLOAD_PATH) --cvs-exclude;
 
+    # ansible:
+    # /usr/bin/rsync --delay-updates -F --compress --delete-after --copy-links --archive --rsh='/usr/bin/ssh -S none -
+    # i /home/shawn/.ssh/sharedservices_group -o Port=4894 -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null'
+    # --rsync-path='sudo -u root rsync'
+    # --exclude-from=/home/shawn/Work/app_sharedservices_group/deploy/roles/project/rsync.txt
+    # --out-format='<<CHANGED>>%i %n%L'
+
     tokens = list()
     tokens.append("rsync")
-    tokens.append("--cvs-exclude")
+    # BUG: Providing rsync --cvs-exclude was causing directories named "tags" to be omitted.
+    # tokens.append("--cvs-exclude")
+    tokens.append("--exclude=.git")
     tokens.append("--checksum")
     tokens.append("--compress")
 
     if links:
         tokens.append("--copy-links")
 
     if delete:
@@ -445,20 +564,31 @@
 
     return Command(statement, **kwargs)
 
 
 def scopy(from_path, to_path, host=None, key_file=None, port=22, user=None, **kwargs):
     """Copy a file or directory to a remote server.
 
-    - from_path (str): The source directory.
-    - to_path (str): The target directory.
-    - host (str): The host name or IP address. Required.
-    - key_file (str): The privacy SSH key (path) for remote connections. User expansion is automatically applied.
-    - port (int): The SSH port to use for remote connections.
-    - user (str): The user name to use for remote connections.
+    :param from_path: The source of the copy.
+    :type from_path: str
+
+    :param to_path: The remote target of the copy.
+    :type to_path: str
+
+    :param host: The host name or IP address. Required.
+    :type host: str
+
+    :param key_file: The privacy SSH key (path) for remote connections. User expansion is automatically applied.
+    :type key_file: str
+
+    :param port: The SSH port to use for remote connections.
+    :type port: int
+
+    :param user: The username to use for remote connections.
+    :type user: str
 
     """
     kwargs.setdefault("comment", "copy %s to remote %s" % (from_path, to_path))
 
     # TODO: What to do to force local versus remote commands?
     # kwargs['local'] = True
 
@@ -478,280 +608,147 @@
         statement.append("%s:%s" % (host, to_path))
     else:
         raise ValueError("Host is a required keyword argument.")
 
     return Command(" ".join(statement), **kwargs)
 
 
-def sed(path, backup=".b", delimiter="/", find=None, replace=None, **kwargs):
-    """Find and replace text in a file.
+def sync(source, target, delete=False, exclude=None, links=True, recursive=True, **kwargs):
+    """Synchronize a local directory structure.
 
-    - path (str): The path to the file to be edited.
-    - backup (str): The backup file extension to use.
-    - delimiter (str): The pattern delimiter.
-    - find (str): The old text. Required.
-    - replace (str): The new text. Required.
+    :param source: The source directory.
+    :type source: str
 
-    """
+    :param target: The target directory.
+    :type target: str
 
-    kwargs.setdefault("comment", "find and replace in %s" % path)
+    :param delete: Indicates target files that exist in source but not in target should be removed.
+    :type delete: bool
 
-    context = {
-        'backup': backup,
-        'delimiter': delimiter,
-        'path': path,
-        'pattern': find,
-        'replace': replace,
-    }
+    :param exclude: The path to an exclude file.
+    :type exclude: str
 
-    template = "sed -i %(backup)s 's%(delimiter)s%(pattern)s%(delimiter)s%(replace)s%(delimiter)sg' %(path)s"
+    :param links: Include symlinks in the sync.
+    :type links: bool
 
-    statement = template % context
+    :param recursive: Indicates source contents should be recursively synchronized.
+    :type recursive: bool
 
-    return Command(statement, **kwargs)
+    """
+    # - guess: When ``True``, the ``host``, ``key_file``, and ``user`` will be guessed based on the base name of
+    #               the source path.
+    # :type guess: bool
+    # if guess:
+    #     host = host or os.path.basename(source).replace("_", ".")
+    #     key_file = key_file or os.path.expanduser(os.path.join("~/.ssh", os.path.basename(source)))
+    #     user = user or os.path.basename(source)
+    # else:
+    #     host = host
+    #     key_file = key_file
+    #     user = user
 
+    kwargs.setdefault("comment", "sync %s with %s" % (source, target))
 
-def symlink(source, force=False, target=None, **kwargs):
-    """Create a symlink.
+    # rsync -e "ssh -i $(SSH_KEY) -p $(SSH_PORT)" -P -rvzc --delete
+    # $(OUTPUTH_PATH) $(SSH_USER)@$(SSH_HOST):$(UPLOAD_PATH) --cvs-exclude;
 
-    - source (str): The source of the link.
-    - force (bool): Force the creation of the link.
-    - target (str): The name or path of the target. Defaults to the base name of the source path.
+    tokens = list()
+    tokens.append("rsync")
+    tokens.append("--cvs-exclude")
+    tokens.append("--checksum")
+    tokens.append("--compress")
 
-    """
-    _target = target or os.path.basename(source)
+    if links:
+        tokens.append("--copy-links")
 
-    kwargs.setdefault("comment", "link to %s" % source)
+    if delete:
+        tokens.append("--delete")
 
-    statement = ["ln -s"]
+    if exclude is not None:
+        tokens.append("--exclude-from=%s" % exclude)
 
-    if force:
-        statement.append("-f")
+    # --partial and --progress
+    tokens.append("-P")
 
-    statement.append(source)
-    statement.append(_target)
+    if recursive:
+        tokens.append("--recursive")
 
-    return Command(" ".join(statement), **kwargs)
+    tokens.append(source)
+    tokens.append(target)
+
+    statement = " ".join(tokens)
+
+    return Command(statement, **kwargs)
 
 
 def touch(path, **kwargs):
     """Touch a file or directory.
 
-    - path (str): The file or directory to touch.
+    :param path: The file or directory to touch.
+    :type path: str
 
     """
     kwargs.setdefault("comment", "touch %s" % path)
 
     return Command("touch %s" % path, **kwargs)
 
 
 def wait(seconds, **kwargs):
     """Pause execution for a number of seconds.
 
-    - seconds (int): The number of seconds to wait.
+    :param seconds: The number of seconds to wait.
+    :type seconds: int
 
     """
     kwargs.setdefault("comment", "pause for %s seconds" % seconds)
 
     return Command("sleep %s" % seconds, **kwargs)
 
-# Classes
-
-
-class Function(object):
-    """A function that may be used to organize related commands to be called together."""
-
-    def __init__(self, name, commands=None, comment=None):
-        """Initialize a function.
-
-        :param name: The name of the function.
-        :type name: str
-
-        :param commands: The command instances to be included in the function's output.
-        :type commands: list
-
-        :param comment: A comment regarding the function.
-        :type comment: str
-
-        """
-        self.commands = commands or list()
-        self.comment = comment
-        self.name = name
-
-    def to_string(self):
-        """Export the function as a string.
-
-        :rtype: str
-
-        """
-        a = list()
-
-        if self.comment is not None:
-            a.append("# %s" % self.comment)
-
-        a.append("function %s()" % self.name)
-        a.append("{")
-        for command in self.commands:
-            a.append(indent(command.get_statement(cd=True)))
-            a.append("")
-
-        a.append("}")
-
-        return "\n".join(a)
-
-
-class Prompt(Command):
-    """Prompt the user for input."""
-
-    def __init__(self, name, back_title="Input", choices=None, default=None, fancy=False, help_text=None, label=None,
-                 **kwargs):
-        """Initialize a prompt for user input.
-
-        :param name: The variable name.
-        :type name: str
-
-        :param back_title: The back title of the input. Used only when ``dialog`` is enabled.
-        :type back_title: str
-
-        :param choices: Valid choices for the variable. May be given as a list of strings or a comma separated string.
-        :type choices: list[str] | str
-
-        :param default: The default value of the variable.
 
-        :param fancy: Indicates the dialog command should be used.
-        :type fancy: bool
-
-        :param help_text: Additional text to display. Only use when ``fancy`` is ``True``.
-        :type help_text: str
-
-        :param label: The label of the prompt.
-
-        """
-        self.back_title = back_title
-        self.default = default
-        self.dialog_enabled = fancy
-        self.help_text = help_text
-        self.label = label or name.replace("_", " ").title()
-        self.variable_name = name
-
-        if type(choices) in (list, tuple):
-            self.choices = choices
-        elif type(choices) is str:
-            self.choices = split_csv(choices, smart=False)
-            # for i in choices.split(","):
-            #     self.choices.append(i.strip())
-        else:
-            self.choices = None
-
-        kwargs.setdefault("comment", "prompt user for %s input" % name)
-
-        super().__init__(name, **kwargs)
-
-    def get_statement(self, cd=False, suppress_comment=False):
-        """Get the statement using dialog or read."""
-        if self.dialog_enabled:
-            return self._get_dialog_statement()
-
-        return self._get_read_statement()
-
-    def _get_dialog_statement(self):
-        """Get the dialog statement."""
-        a = list()
-
-        a.append('dialog --clear --backtitle "%s" --title "%s"' % (self.back_title, self.label))
-
-        if self.choices is not None:
-            a.append('--menu "%s" 15 40 %s' % (self.help_text or "Select", len(self.choices)))
-            count = 1
-            for choice in self.choices:
-                a.append('"%s" %s' % (choice, count))
-                count += 1
-
-            a.append('2>/tmp/input.txt')
-        else:
-            if self.help_text is not None:
-                a.append('--inputbox "%s"' % self.help_text)
-            else:
-                a.append('--inputbox ""')
-
-            a.append('8 60 2>/tmp/input.txt')
-
-        b = list()
-
-        b.append('touch /tmp/input.txt')
-        b.append(" ".join(a))
-
-        b.append('%s=$(</tmp/input.txt)' % self.variable_name)
-        b.append('clear')
-        b.append('rm /tmp/input.txt')
-
-        if self.default is not None:
-            b.append('if [[ -z "$%s" ]]; then %s="%s"; fi;' % (self.variable_name, self.variable_name, self.default))
-
-        # b.append('echo "$%s"' % self.name)
-
-        return "\n".join(b)
-
-    def _get_read_statement(self):
-        """Get the standard read statement."""
-        a = list()
-
-        if self.choices is not None:
-            a.append('echo "%s "' % self.label)
-
-            options = list()
-            for choice in self.choices:
-                options.append('"%s"' % choice)
-
-            a.append('options=(%s)' % " ".join(options))
-            a.append('select opt in "${options[@]}"')
-            a.append('do')
-            a.append('    case $opt in')
+def write(path, content=None, **kwargs):
+    """Write to a file.
 
-            for choice in self.choices:
-                a.append('        "%s") %s=$opt; break;;' % (choice, self.variable_name))
+    :param path: The file to be written.
+    :type path: str
 
-            # a.append('        %s) %s=$opt;;' % ("|".join(self.choices), self.name))
-            a.append('        *) echo "invalid choice";;')
-            a.append('    esac')
-            a.append('done')
+    :param content: The content to be written. Note: If omitted, this command is equivalent to ``touch``.
+    :type content: str
 
-            # a.append("read %s" % self.name)
-        else:
-            a.append('echo -n "%s "' % self.label)
-            a.append("read %s" % self.variable_name)
+    """
+    _content = content or ""
 
-        if self.default is not None:
-            a.append('if [[ -z "$%s" ]]; then %s="%s"; fi;' % (self.variable_name, self.variable_name, self.default))
+    kwargs.setdefault("comment", "write to %s" % path)
 
-        # a.append('echo "$%s"' % self.name)
+    a = list()
 
-        return "\n".join(a)
+    if len(_content.split("\n")) > 1:
+        a.append("cat > %s << EOF" % path)
+        a.append(_content)
+        a.append("EOF")
+    else:
+        a.append('echo "%s" > %s' % (_content, path))
 
-# Mappings
+    return Command(" ".join(a), **kwargs)
 
 
 POSIX_MAPPINGS = {
-    'append': file_append,
+    'append': append,
     'archive': archive,
     'certbot': certbot,
-    'copy': file_copy,
-    'dialog': dialog,
-    'echo': echo,
+    'copy': copy,
+    'dir': directory,
     'extract': extract,
-    'func': Function,
-    # 'function': Function,
-    'mkdir': mkdir,
+    'link': link,
     'move': move,
     'perms': perms,
     'prompt': prompt,
     'remove': remove,
-    'rename': rename,
+    'replace': replace,
+    'run': run,
     'rsync': rsync,
     'scopy': scopy,
-    'sed': sed,
     'ssl': certbot,
-    'symlink': symlink,
+    'sync': sync,
     'touch': touch,
     'wait': wait,
-    'write': file_write,
+    'write': write,
 }
```

### Comparing `python-scripttease-6.8.2/scripttease/library/overlays/ubuntu.py` & `python-scripttease-7.0.0/scripttease/lib/commands/ubuntu.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,55 @@
 # Imports
 
 from commonkit import split_csv
-from ..commands import Command, Template
-from .common import COMMON_MAPPINGS
+from .base import Command
 from .django import DJANGO_MAPPINGS
+from .messages import MESSAGE_MAPPINGS
 from .mysql import MYSQL_MAPPINGS
 from .pgsql import PGSQL_MAPPINGS
-from .posix import POSIX_MAPPINGS, Function
+from .php import PHP_MAPPINGS
+from .posix import POSIX_MAPPINGS
+from .python import PYTHON_MAPPINGS
 
 # Exports
 
 __all__ = (
-    "MAPPINGS",
+    "UBUNTU_MAPPINGS",
     "apache",
     "apache_disable_module",
     "apache_disable_site",
     "apache_enable_module",
     "apache_enable_site",
     "apache_reload",
     "apache_restart",
     "apache_start",
     "apache_stop",
     "apache_test",
-    "command_exists",
     "service_reload",
     "service_restart",
     "service_start",
     "service_stop",
     "system",
     "system_install",
     "system_reboot",
     "system_update",
     "system_upgrade",
     "system_uninstall",
-    "template",
+    # "template",
     "user",
-    "Function",
 )
 
-
-def command_exists(name):
-    """Indicates whether a given command exists in this overaly.
-
-    :param name: The name of the command.
-    :type name: str
-
-    :rtype: bool
-
-    """
-    return name in MAPPINGS
+# Functions
 
 
 def apache(op, **kwargs):
     """Execute an Apache-related command.
 
-    - op (str): The operation to perform; reload, restart, start, stop, test.
+    :param op: The operation to perform; ``reload``, ``restart``, ``start``, ``stop``, ``test``.
+    :type op: str
 
     """
     if op == "reload":
         return apache_reload(**kwargs)
     elif op == "restart":
         return apache_restart(**kwargs)
     elif op == "start":
@@ -67,215 +58,232 @@
         return apache_stop(**kwargs)
     elif op == "test":
         return apache_test(**kwargs)
     else:
         raise NameError("Unrecognized or unsupported apache operation: %s" % op)
 
 
-def apache_disable_module(name, **kwargs):
+def apache_disable_module(module, **kwargs):
     """Disable an Apache module.
 
-    - name (str): The module name.
+    :param module: The name of the module.
+    :type module: str
 
     """
-    kwargs.setdefault("comment", "disable %s apache module" % name)
+    kwargs.setdefault("comment", "disable %s apache module" % module)
 
-    return Command("a2dismod %s" % name, **kwargs)
+    return Command("a2dismod %s" % module, **kwargs)
 
 
-def apache_disable_site(name, **kwargs):
+def apache_disable_site(site, **kwargs):
     """Disable an Apache site.
 
-    - name (str): The domain name.
+    :param site: The site/domain name.
+    :type site: str
 
     """
-    kwargs.setdefault("comment", "disable %s apache site" % name)
+    kwargs.setdefault("comment", "disable %s apache site" % site)
 
-    return Command("a2dissite %s" % name, **kwargs)
+    return Command("a2dissite %s" % site, **kwargs)
 
 
-def apache_enable_module(name, **kwargs):
+def apache_enable_module(module, **kwargs):
     """Enable an Apache module.
 
-    - name (str): The module name.
+    :param module: The name of the module.
+    :type module: str
 
     """
-    kwargs.setdefault("comment", "enable %s apache module" % name)
+    kwargs.setdefault("comment", "enable %s apache module" % module)
 
-    return Command("a2enmod %s" % name, **kwargs)
+    return Command("a2enmod %s" % module, **kwargs)
 
 
-def apache_enable_site(name, **kwargs):
+def apache_enable_site(site, **kwargs):
     """Enable an Apache site.
 
+    :param site: The site/domain name.
+    :type site: str
 
     """
-    kwargs.setdefault("comment", "enable %s apache module" % name)
+    kwargs.setdefault("comment", "enable %s apache module" % site)
 
-    return Command("a2ensite %s" % name, **kwargs)
+    return Command("a2ensite %s" % site, **kwargs)
 
 
 def apache_reload(**kwargs):
+    """Reload the apache service."""
     kwargs.setdefault("comment", "reload apache")
     kwargs.setdefault("register", "apache_reloaded")
 
     return Command("service apache2 reload", **kwargs)
 
 
 def apache_restart(**kwargs):
+    """Restart the apache service."""
     kwargs.setdefault("comment", "restart apache")
     kwargs.setdefault("register", "apache_restarted")
 
     return Command("service apache2 restart", **kwargs)
 
 
 def apache_start(**kwargs):
+    """Start the apache service."""
     kwargs.setdefault("comment", "start apache")
     kwargs.setdefault("register", "apache_started")
 
     return Command("service apache2 start", **kwargs)
 
 
 def apache_stop(**kwargs):
+    """Stop the apache service."""
     kwargs.setdefault("comment", "stop apache")
 
     return Command("service apache2 stop", **kwargs)
 
 
 def apache_test(**kwargs):
+    """Run a configuration test on apache."""
     kwargs.setdefault("comment", "check apache configuration")
     kwargs.setdefault("register", "apache_checks_out")
 
     return Command("apachectl configtest", **kwargs)
 
 
-def service_reload(name, **kwargs):
+def service_reload(service, **kwargs):
     """Reload a service.
 
-    - name (str): The service name.
+    :param service: The service name.
+    :type service: str
 
     """
-    kwargs.setdefault("comment", "reload %s service" % name)
-    kwargs.setdefault("register", "%s_reloaded" % name)
+    kwargs.setdefault("comment", "reload %s service" % service)
+    kwargs.setdefault("register", "%s_reloaded" % service)
 
-    return Command("service %s reload" % name, **kwargs)
+    return Command("service %s reload" % service, **kwargs)
 
 
-def service_restart(name, **kwargs):
+def service_restart(service, **kwargs):
     """Restart a service.
 
-    - name (str): The service name.
+    :param service: The service name.
+    :type service: str
 
     """
-    kwargs.setdefault("comment", "restart %s service" % name)
-    kwargs.setdefault("register", "%s_restarted" % name)
+    kwargs.setdefault("comment", "restart %s service" % service)
+    kwargs.setdefault("register", "%s_restarted" % service)
 
-    return Command("service %s restart" % name, **kwargs)
+    return Command("service %s restart" % service, **kwargs)
 
 
-def service_start(name, **kwargs):
+def service_start(service, **kwargs):
     """Start a service.
 
-    - name (str): The service name.
+    :param service: The service name.
+    :type service: str
 
     """
-    kwargs.setdefault("comment", "start %s service" % name)
-    kwargs.setdefault("register", "%s_started" % name)
+    kwargs.setdefault("comment", "start %s service" % service)
+    kwargs.setdefault("register", "%s_started" % service)
 
-    return Command("service %s start" % name, **kwargs)
+    return Command("service %s start" % service, **kwargs)
 
 
-def service_stop(name, **kwargs):
+def service_stop(service, **kwargs):
     """Stop a service.
 
-    - name (str): The service name.
+    :param service: The service name.
+    :type service: str
 
     """
-    kwargs.setdefault("comment", "stop %s service" % name)
-    kwargs.setdefault("register", "%s_stopped" % name)
+    kwargs.setdefault("comment", "stop %s service" % service)
+    kwargs.setdefault("register", "%s_stopped" % service)
 
-    return Command("service %s stop" % name, **kwargs)
+    return Command("service %s stop" % service, **kwargs)
 
 
 def system(op, **kwargs):
     """Perform a system operation.
 
-    - op (str): The operation to perform; reboot, update, upgrade.
+    :param op: The operation to perform; ``reboot``, ``update``, ``upgrade``.
+    :type op: str
 
     """
     if op == "reboot":
         return system_reboot(**kwargs)
     elif op == "update":
         return system_update(**kwargs)
     elif op == "upgrade":
         return system_upgrade(**kwargs)
     else:
         raise NameError("Unrecognized or unsupported system operation: %s" % op)
 
 
-def system_install(name, **kwargs):
+def system_install(package, **kwargs):
     """Install a system-level package.
 
-    - name (str): The name of the package to install.
+    :param package: The name of the package to install.
+    :type package: str
 
     """
-    kwargs.setdefault("comment", "install system package %s" % name)
+    kwargs.setdefault("comment", "install system package %s" % package)
 
-    return Command("apt-get install -y %s" % name, **kwargs)
+    return Command("apt install -y %s" % package, **kwargs)
 
 
 def system_reboot(**kwargs):
+    """Reboot the system."""
     kwargs.setdefault("comment", "reboot the system")
 
     return Command("reboot", **kwargs)
 
 
-def system_uninstall(name, **kwargs):
+def system_uninstall(package, **kwargs):
     """Uninstall a system-level package.
 
-    - name (str): The name of the package to uninstall.
+    :param package: The name of the package to remove.
+    :type package: str
 
     """
-    kwargs.setdefault("comment", "remove system package %s" % name)
+    kwargs.setdefault("comment", "remove system package %s" % package)
 
-    return Command("apt-get uninstall -y %s" % name, **kwargs)
+    return Command("apt uninstall -y %s" % package, **kwargs)
 
 
 def system_update(**kwargs):
+    """Update the system's package info."""
     kwargs.setdefault("comment", "update system package info")
 
-    return Command("apt-get update -y", **kwargs)
+    return Command("apt update -y", **kwargs)
 
 
 def system_upgrade(**kwargs):
+    """updated the system."""
     kwargs.setdefault("comment", "upgrade the system")
 
-    return Command("apt-get upgrade -y", **kwargs)
+    return Command("apt upgrade -y", **kwargs)
 
 
-def template(source, target, backup=True, parser=None, **kwargs):
-    """Create a file from a template.
+def user(name, groups=None, home=None, op="add", password=None, **kwargs):
+    """Create or remove a user.
 
-    - source (str): The path to the template file.
-    - target (str): The path to where the new file should be created.
-    - backup (bool): Indicates whether a backup should be made if the target file already exists.
-    - parser (str): The parser to use ``jinja`` (the default) or ``simple``.
+    :param name: The username.
+    :type name: str
 
-    """
-    return Template(source, target, backup=backup, parser=parser, **kwargs)
+    :param groups: A list of groups to which the user should belong.
+    :type groups: list | str
 
+    :param home: The path to the user's home directory.
+    :type home: str
 
-def user(name, groups=None, home=None, op="add", password=None, **kwargs):
-    """Create or remove a user.
+    :param op: The operation to perform; ``add`` or ``remove``.
+    :type op:
 
-    - name (str): The user name.
-    - groups (str | list): A list of groups to which the user should belong.
-    - home (str): The path to the user's home directory.
-    - op (str); The operation to perform; ``add`` or ``remove``.
-    - password (str): The user's password. (NOT IMPLEMENTED)
+    :param password: The user's password. (NOT IMPLEMENTED)
+    :type password: str
 
     """
     if op == "add":
         kwargs.setdefault("comment", "create a user named %s" % name)
 
         commands = list()
 
@@ -292,25 +300,25 @@
 
         if type(groups) in [list, tuple]:
             for group in groups:
                 commands.append(Command("adduser %s %s" % (name, group), **kwargs))
 
         a = list()
         for c in commands:
-            a.append(c.get_statement(suppress_comment=True))
+            a.append(c.get_statement(include_comment=True))
 
-        return Command("\n".join(a), **kwargs)
+        return Command("\n".join(a), name="user_add", **kwargs)
     elif op == "remove":
         kwargs.setdefault("comment", "remove a user named %s" % name)
-        return Command("deluser %s" % name, **kwargs)
+        return Command("deluser %s" % name, name="user_remove", **kwargs)
     else:
         raise NameError("Unsupported or unrecognized operation: %s" % op)
 
 
-MAPPINGS = {
+UBUNTU_MAPPINGS = {
     'apache': apache,
     'apache.disable_module': apache_disable_module,
     'apache.disable_site': apache_disable_site,
     'apache.enable_module': apache_enable_module,
     'apache.enable_site': apache_enable_site,
     'apache.reload': apache_reload,
     'apache.restart': apache_restart,
@@ -320,19 +328,20 @@
     'install': system_install,
     'reboot': system_reboot,
     'reload': service_reload,
     'restart': service_restart,
     'start': service_start,
     'stop': service_stop,
     'system': system,
-    'template': template,
     'update': system_update,
     'uninstall': system_uninstall,
     'upgrade': system_upgrade,
     'user': user,
 }
 
-MAPPINGS.update(COMMON_MAPPINGS)
-MAPPINGS.update(DJANGO_MAPPINGS)
-MAPPINGS.update(MYSQL_MAPPINGS)
-MAPPINGS.update(PGSQL_MAPPINGS)
-MAPPINGS.update(POSIX_MAPPINGS)
+UBUNTU_MAPPINGS.update(DJANGO_MAPPINGS)
+UBUNTU_MAPPINGS.update(MESSAGE_MAPPINGS)
+UBUNTU_MAPPINGS.update(MYSQL_MAPPINGS)
+UBUNTU_MAPPINGS.update(PGSQL_MAPPINGS)
+UBUNTU_MAPPINGS.update(PHP_MAPPINGS)
+UBUNTU_MAPPINGS.update(POSIX_MAPPINGS)
+UBUNTU_MAPPINGS.update(PYTHON_MAPPINGS)
```

### Comparing `python-scripttease-6.8.2/setup.py` & `python-scripttease-7.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,26 +16,30 @@
     version=read_file("VERSION.txt"),
     description=read_file("DESCRIPTION.txt"),
     long_description=read_file("README.markdown"),
     long_description_content_type="text/markdown",
     author='Shawn Davis',
     author_email='shawn@develmaycare.com',
     url='https://develmaycare.com/products/python/scripttease/',
-    download_url='https://github.com/develmaycare/python-scripttease',
+    download_url='https://gittraction.com/diff6/python-scripttease',
     project_urls={
-        'Documentation': "https://docs.develmaycare.com/en/python-scripttease/latest/",
-        'Source': "https://github.com/develmaycare/python-scripttease",
-        'Tracker': "https://github.com/develmaycare/python-scripttease/issues/"
+        'Documentation': "https://docs.diff6.com/en/python-scripttease/latest/",
+        'Source': "https://gittraction.com/diff6/python-scripttease",
+        'Tracker': "https://gittraction.com/diff6/python-scripttease/issues"
     },
     packages=find_packages(exclude=["tests", "tests.*"]),
     include_package_data=True,
     install_requires=[
+        "colorama",
         "jinja2",
+        "Markdown",
         "pygments",
         "python-commonkit",
+        "pyyaml",
+        "tabulate",
     ],
     # dependency_links=[
     #     "https://github.com/develmaycare/superpython",
     # ],
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Environment :: Console',
@@ -50,11 +54,11 @@
     tests_require=[
         "coverage",
         "pytest",
     ],
     test_suite='runtests.runtests',
     entry_points={
       'console_scripts': [
-          'tease = script_tease.cli:main_command',
+          'tease = scripttease.cli:main_command',
       ],
     },
 )
```

