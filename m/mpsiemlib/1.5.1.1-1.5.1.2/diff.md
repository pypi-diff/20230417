# Comparing `tmp/mpsiemlib-1.5.1.1.tar.gz` & `tmp/mpsiemlib-1.5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpsiemlib-1.5.1.1.tar", last modified: Mon Apr 17 21:28:14 2023, max compression
+gzip compressed data, was "mpsiemlib-1.5.1.2.tar", last modified: Mon Apr 17 21:37:52 2023, max compression
```

## Comparing `mpsiemlib-1.5.1.1.tar` & `mpsiemlib-1.5.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 21:28:14.788036 mpsiemlib-1.5.1.1/
--rw-rw-rw-   0        0        0    35823 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/LICENSE
--rw-rw-rw-   0        0        0      240 2023-04-17 21:28:14.787036 mpsiemlib-1.5.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2002 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/README.md
--rw-rw-rw-   0        0        0     2132 2023-04-17 21:18:01.000000 mpsiemlib-1.5.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-17 21:28:14.746036 mpsiemlib-1.5.1.1/mpsiemlib/
--rw-rw-rw-   0        0        0      282 2023-04-17 21:26:31.000000 mpsiemlib-1.5.1.1/mpsiemlib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:28:14.762045 mpsiemlib-1.5.1.1/mpsiemlib/common/
--rw-rw-rw-   0        0        0     3979 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/common/BaseFunctions.py
--rw-rw-rw-   0        0        0     5716 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/common/Interfaces.py
--rw-rw-rw-   0        0        0    17673 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/common/MPSIEMAuth.py
--rw-rw-rw-   0        0        0      685 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:28:14.765036 mpsiemlib-1.5.1.1/mpsiemlib/helpers/
--rw-rw-rw-   0        0        0     2304 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/helpers/__init__.py
--rw-rw-rw-   0        0        0    40858 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/helpers/content_helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:28:14.785036 mpsiemlib-1.5.1.1/mpsiemlib/modules/
--rw-rw-rw-   0        0        0    40168 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/modules/Assets.py
--rw-rw-rw-   0        0        0    20163 2023-04-14 14:01:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/modules/Events.py
--rw-rw-rw-   0        0        0     7344 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/modules/EventsAPI.py
--rw-rw-rw-   0        0        0     4876 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/modules/Filters.py
--rw-rw-rw-   0        0        0     7139 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/modules/HealthMonitor.py
--rw-rw-rw-   0        0        0    16421 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/modules/Incidents.py
--rw-rw-rw-   0        0        0    83645 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/modules/KnowledgeBase.py
--rw-rw-rw-   0        0        0     8631 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/modules/SourceMonitor.py
--rw-rw-rw-   0        0        0    18784 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/modules/Tables.py
--rw-rw-rw-   0        0        0    19999 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/modules/Tasks.py
--rw-rw-rw-   0        0        0    27285 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/modules/UsersAndRoles.py
--rw-rw-rw-   0        0        0     2206 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.1/mpsiemlib/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:28:14.756036 mpsiemlib-1.5.1.1/mpsiemlib.egg-info/
--rw-rw-rw-   0        0        0      240 2023-04-17 21:28:14.000000 mpsiemlib-1.5.1.1/mpsiemlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      819 2023-04-17 21:28:14.000000 mpsiemlib-1.5.1.1/mpsiemlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 21:28:14.000000 mpsiemlib-1.5.1.1/mpsiemlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 20:15:01.000000 mpsiemlib-1.5.1.1/mpsiemlib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       43 2023-04-17 21:28:14.000000 mpsiemlib-1.5.1.1/mpsiemlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-17 21:28:14.000000 mpsiemlib-1.5.1.1/mpsiemlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 21:28:14.788036 mpsiemlib-1.5.1.1/setup.cfg
--rw-rw-rw-   0        0        0      554 2023-04-17 20:20:08.000000 mpsiemlib-1.5.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:37:52.720280 mpsiemlib-1.5.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3740 2023-04-17 21:37:52.720280 mpsiemlib-1.5.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2002 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/README.md
+-rw-rw-rw-   0        0        0     2132 2023-04-17 21:18:01.000000 mpsiemlib-1.5.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-17 21:37:52.681281 mpsiemlib-1.5.1.2/mpsiemlib/
+-rw-rw-rw-   0        0        0      282 2023-04-17 21:37:49.000000 mpsiemlib-1.5.1.2/mpsiemlib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:37:52.697281 mpsiemlib-1.5.1.2/mpsiemlib/common/
+-rw-rw-rw-   0        0        0     3979 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/common/BaseFunctions.py
+-rw-rw-rw-   0        0        0     5716 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/common/Interfaces.py
+-rw-rw-rw-   0        0        0    17673 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/common/MPSIEMAuth.py
+-rw-rw-rw-   0        0        0      685 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:37:52.700281 mpsiemlib-1.5.1.2/mpsiemlib/helpers/
+-rw-rw-rw-   0        0        0     2304 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/helpers/__init__.py
+-rw-rw-rw-   0        0        0    40858 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/helpers/content_helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:37:52.718281 mpsiemlib-1.5.1.2/mpsiemlib/modules/
+-rw-rw-rw-   0        0        0    40168 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/modules/Assets.py
+-rw-rw-rw-   0        0        0    20163 2023-04-14 14:01:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/modules/Events.py
+-rw-rw-rw-   0        0        0     7344 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/modules/EventsAPI.py
+-rw-rw-rw-   0        0        0     4876 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/modules/Filters.py
+-rw-rw-rw-   0        0        0     7139 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/modules/HealthMonitor.py
+-rw-rw-rw-   0        0        0    16421 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/modules/Incidents.py
+-rw-rw-rw-   0        0        0    83645 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/modules/KnowledgeBase.py
+-rw-rw-rw-   0        0        0     8631 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/modules/SourceMonitor.py
+-rw-rw-rw-   0        0        0    18784 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/modules/Tables.py
+-rw-rw-rw-   0        0        0    19999 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/modules/Tasks.py
+-rw-rw-rw-   0        0        0    27285 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/modules/UsersAndRoles.py
+-rw-rw-rw-   0        0        0     2206 2023-04-14 13:51:06.000000 mpsiemlib-1.5.1.2/mpsiemlib/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 21:37:52.692280 mpsiemlib-1.5.1.2/mpsiemlib.egg-info/
+-rw-rw-rw-   0        0        0     3740 2023-04-17 21:37:52.000000 mpsiemlib-1.5.1.2/mpsiemlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      819 2023-04-17 21:37:52.000000 mpsiemlib-1.5.1.2/mpsiemlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 21:37:52.000000 mpsiemlib-1.5.1.2/mpsiemlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 20:15:01.000000 mpsiemlib-1.5.1.2/mpsiemlib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       43 2023-04-17 21:37:52.000000 mpsiemlib-1.5.1.2/mpsiemlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-17 21:37:52.000000 mpsiemlib-1.5.1.2/mpsiemlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 21:37:52.720280 mpsiemlib-1.5.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      768 2023-04-17 21:32:14.000000 mpsiemlib-1.5.1.2/setup.py
```

### Comparing `mpsiemlib-1.5.1.1/LICENSE` & `mpsiemlib-1.5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/README.md` & `mpsiemlib-1.5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/README.rst` & `mpsiemlib-1.5.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/common/BaseFunctions.py` & `mpsiemlib-1.5.1.2/mpsiemlib/common/BaseFunctions.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/common/Interfaces.py` & `mpsiemlib-1.5.1.2/mpsiemlib/common/Interfaces.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/common/MPSIEMAuth.py` & `mpsiemlib-1.5.1.2/mpsiemlib/common/MPSIEMAuth.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/common/__init__.py` & `mpsiemlib-1.5.1.2/mpsiemlib/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/helpers/__init__.py` & `mpsiemlib-1.5.1.2/mpsiemlib/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/helpers/content_helpers.py` & `mpsiemlib-1.5.1.2/mpsiemlib/helpers/content_helpers.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/modules/Assets.py` & `mpsiemlib-1.5.1.2/mpsiemlib/modules/Assets.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/modules/Events.py` & `mpsiemlib-1.5.1.2/mpsiemlib/modules/Events.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/modules/EventsAPI.py` & `mpsiemlib-1.5.1.2/mpsiemlib/modules/EventsAPI.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/modules/Filters.py` & `mpsiemlib-1.5.1.2/mpsiemlib/modules/Filters.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/modules/HealthMonitor.py` & `mpsiemlib-1.5.1.2/mpsiemlib/modules/HealthMonitor.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/modules/Incidents.py` & `mpsiemlib-1.5.1.2/mpsiemlib/modules/Incidents.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/modules/KnowledgeBase.py` & `mpsiemlib-1.5.1.2/mpsiemlib/modules/KnowledgeBase.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/modules/SourceMonitor.py` & `mpsiemlib-1.5.1.2/mpsiemlib/modules/SourceMonitor.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/modules/Tables.py` & `mpsiemlib-1.5.1.2/mpsiemlib/modules/Tables.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/modules/Tasks.py` & `mpsiemlib-1.5.1.2/mpsiemlib/modules/Tasks.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/modules/UsersAndRoles.py` & `mpsiemlib-1.5.1.2/mpsiemlib/modules/UsersAndRoles.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib/modules/__init__.py` & `mpsiemlib-1.5.1.2/mpsiemlib/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `mpsiemlib-1.5.1.1/mpsiemlib.egg-info/SOURCES.txt` & `mpsiemlib-1.5.1.2/mpsiemlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

