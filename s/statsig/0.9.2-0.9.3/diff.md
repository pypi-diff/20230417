# Comparing `tmp/statsig-0.9.2.tar.gz` & `tmp/statsig-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statsig-0.9.2.tar", last modified: Sat Apr 23 00:04:44 2022, max compression
+gzip compressed data, was "statsig-0.9.3.tar", last modified: Tue Apr 26 00:00:25 2022, max compression
```

## Comparing `statsig-0.9.2.tar` & `statsig-0.9.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jiakanwang   (501) staff       (20)        0 2022-04-23 00:04:44.583081 statsig-0.9.2/
--rw-r--r--   0 jiakanwang   (501) staff       (20)      749 2021-11-04 20:34:52.000000 statsig-0.9.2/LICENSE
--rw-r--r--   0 jiakanwang   (501) staff       (20)       17 2021-11-04 20:34:52.000000 statsig-0.9.2/MANIFEST.in
--rw-r--r--   0 jiakanwang   (501) staff       (20)     2114 2022-04-23 00:04:44.582954 statsig-0.9.2/PKG-INFO
--rw-r--r--   0 jiakanwang   (501) staff       (20)     1334 2022-04-20 23:32:56.000000 statsig-0.9.2/README.md
--rw-r--r--   0 jiakanwang   (501) staff       (20)       38 2022-04-23 00:04:44.583124 statsig-0.9.2/setup.cfg
--rw-r--r--   0 jiakanwang   (501) staff       (20)     1286 2022-04-20 23:32:56.000000 statsig-0.9.2/setup.py
-drwxr-xr-x   0 jiakanwang   (501) staff       (20)        0 2022-04-23 00:04:44.582204 statsig-0.9.2/statsig/
--rw-r--r--   0 jiakanwang   (501) staff       (20)      447 2022-04-20 23:32:56.000000 statsig-0.9.2/statsig/__init__.py
--rw-r--r--   0 jiakanwang   (501) staff       (20)     1118 2022-03-02 02:41:13.000000 statsig-0.9.2/statsig/dynamic_config.py
--rw-r--r--   0 jiakanwang   (501) staff       (20)    21364 2022-04-20 23:32:56.000000 statsig-0.9.2/statsig/evaluator.py
--rw-r--r--   0 jiakanwang   (501) staff       (20)     1753 2022-04-20 23:32:56.000000 statsig-0.9.2/statsig/layer.py
--rw-r--r--   0 jiakanwang   (501) staff       (20)     1092 2022-03-22 01:07:36.000000 statsig-0.9.2/statsig/statsig.py
--rw-r--r--   0 jiakanwang   (501) staff       (20)      263 2022-03-02 02:41:13.000000 statsig-0.9.2/statsig/statsig_environment_tier.py
--rw-r--r--   0 jiakanwang   (501) staff       (20)     1576 2022-03-22 01:07:36.000000 statsig-0.9.2/statsig/statsig_event.py
--rw-r--r--   0 jiakanwang   (501) staff       (20)     3988 2022-04-20 23:32:56.000000 statsig-0.9.2/statsig/statsig_logger.py
--rw-r--r--   0 jiakanwang   (501) staff       (20)     2833 2022-04-20 23:32:56.000000 statsig-0.9.2/statsig/statsig_network.py
--rw-r--r--   0 jiakanwang   (501) staff       (20)     1639 2022-04-20 23:32:56.000000 statsig-0.9.2/statsig/statsig_options.py
--rw-r--r--   0 jiakanwang   (501) staff       (20)    12818 2022-04-23 00:04:25.000000 statsig-0.9.2/statsig/statsig_server.py
--rw-r--r--   0 jiakanwang   (501) staff       (20)     2521 2022-04-22 23:19:04.000000 statsig-0.9.2/statsig/statsig_user.py
--rw-r--r--   0 jiakanwang   (501) staff       (20)       22 2022-04-22 23:19:04.000000 statsig-0.9.2/statsig/version.py
-drwxr-xr-x   0 jiakanwang   (501) staff       (20)        0 2022-04-23 00:04:44.582772 statsig-0.9.2/statsig.egg-info/
--rw-r--r--   0 jiakanwang   (501) staff       (20)     2114 2022-04-23 00:04:44.000000 statsig-0.9.2/statsig.egg-info/PKG-INFO
--rw-r--r--   0 jiakanwang   (501) staff       (20)      505 2022-04-23 00:04:44.000000 statsig-0.9.2/statsig.egg-info/SOURCES.txt
--rw-r--r--   0 jiakanwang   (501) staff       (20)        1 2022-04-23 00:04:44.000000 statsig-0.9.2/statsig.egg-info/dependency_links.txt
--rw-r--r--   0 jiakanwang   (501) staff       (20)       95 2022-04-23 00:04:44.000000 statsig-0.9.2/statsig.egg-info/requires.txt
--rw-r--r--   0 jiakanwang   (501) staff       (20)        8 2022-04-23 00:04:44.000000 statsig-0.9.2/statsig.egg-info/top_level.txt
+drwxr-xr-x   0 jiakanwang   (501) staff       (20)        0 2022-04-26 00:00:25.191784 statsig-0.9.3/
+-rw-r--r--   0 jiakanwang   (501) staff       (20)      749 2021-11-04 20:34:52.000000 statsig-0.9.3/LICENSE
+-rw-r--r--   0 jiakanwang   (501) staff       (20)       17 2021-11-04 20:34:52.000000 statsig-0.9.3/MANIFEST.in
+-rw-r--r--   0 jiakanwang   (501) staff       (20)     2114 2022-04-26 00:00:25.191666 statsig-0.9.3/PKG-INFO
+-rw-r--r--   0 jiakanwang   (501) staff       (20)     1334 2022-04-20 23:32:56.000000 statsig-0.9.3/README.md
+-rw-r--r--   0 jiakanwang   (501) staff       (20)       38 2022-04-26 00:00:25.191830 statsig-0.9.3/setup.cfg
+-rw-r--r--   0 jiakanwang   (501) staff       (20)     1286 2022-04-20 23:32:56.000000 statsig-0.9.3/setup.py
+drwxr-xr-x   0 jiakanwang   (501) staff       (20)        0 2022-04-26 00:00:25.190903 statsig-0.9.3/statsig/
+-rw-r--r--   0 jiakanwang   (501) staff       (20)      447 2022-04-20 23:32:56.000000 statsig-0.9.3/statsig/__init__.py
+-rw-r--r--   0 jiakanwang   (501) staff       (20)     1118 2022-03-02 02:41:13.000000 statsig-0.9.3/statsig/dynamic_config.py
+-rw-r--r--   0 jiakanwang   (501) staff       (20)    21336 2022-04-25 23:59:08.000000 statsig-0.9.3/statsig/evaluator.py
+-rw-r--r--   0 jiakanwang   (501) staff       (20)     1753 2022-04-20 23:32:56.000000 statsig-0.9.3/statsig/layer.py
+-rw-r--r--   0 jiakanwang   (501) staff       (20)     1092 2022-03-22 01:07:36.000000 statsig-0.9.3/statsig/statsig.py
+-rw-r--r--   0 jiakanwang   (501) staff       (20)      263 2022-03-02 02:41:13.000000 statsig-0.9.3/statsig/statsig_environment_tier.py
+-rw-r--r--   0 jiakanwang   (501) staff       (20)     1576 2022-03-22 01:07:36.000000 statsig-0.9.3/statsig/statsig_event.py
+-rw-r--r--   0 jiakanwang   (501) staff       (20)     3988 2022-04-20 23:32:56.000000 statsig-0.9.3/statsig/statsig_logger.py
+-rw-r--r--   0 jiakanwang   (501) staff       (20)     2833 2022-04-20 23:32:56.000000 statsig-0.9.3/statsig/statsig_network.py
+-rw-r--r--   0 jiakanwang   (501) staff       (20)     1639 2022-04-20 23:32:56.000000 statsig-0.9.3/statsig/statsig_options.py
+-rw-r--r--   0 jiakanwang   (501) staff       (20)    12818 2022-04-23 00:04:25.000000 statsig-0.9.3/statsig/statsig_server.py
+-rw-r--r--   0 jiakanwang   (501) staff       (20)     2521 2022-04-22 23:19:04.000000 statsig-0.9.3/statsig/statsig_user.py
+-rw-r--r--   0 jiakanwang   (501) staff       (20)       22 2022-04-25 23:54:24.000000 statsig-0.9.3/statsig/version.py
+drwxr-xr-x   0 jiakanwang   (501) staff       (20)        0 2022-04-26 00:00:25.191483 statsig-0.9.3/statsig.egg-info/
+-rw-r--r--   0 jiakanwang   (501) staff       (20)     2114 2022-04-26 00:00:25.000000 statsig-0.9.3/statsig.egg-info/PKG-INFO
+-rw-r--r--   0 jiakanwang   (501) staff       (20)      505 2022-04-26 00:00:25.000000 statsig-0.9.3/statsig.egg-info/SOURCES.txt
+-rw-r--r--   0 jiakanwang   (501) staff       (20)        1 2022-04-26 00:00:25.000000 statsig-0.9.3/statsig.egg-info/dependency_links.txt
+-rw-r--r--   0 jiakanwang   (501) staff       (20)       95 2022-04-26 00:00:25.000000 statsig-0.9.3/statsig.egg-info/requires.txt
+-rw-r--r--   0 jiakanwang   (501) staff       (20)        8 2022-04-26 00:00:25.000000 statsig-0.9.3/statsig.egg-info/top_level.txt
```

### Comparing `statsig-0.9.2/LICENSE` & `statsig-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `statsig-0.9.2/PKG-INFO` & `statsig-0.9.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statsig
-Version: 0.9.2
+Version: 0.9.3
 Summary: Statsig Python Server SDK
 Home-page: https://github.com/statsig-io/python-sdk
 Author: Tore Hanssen, Jiakan Wang
 Author-email: tore@statsig.com, jkw@statsig.com
 License: ISC
 Description: # Statsig Python Server SDK
         [![tests](https://github.com/statsig-io/python-sdk/actions/workflows/test.yml/badge.svg)](https://github.com/statsig-io/python-sdk/actions/workflows/test.yml)
```

### Comparing `statsig-0.9.2/README.md` & `statsig-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `statsig-0.9.2/setup.py` & `statsig-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `statsig-0.9.2/statsig/dynamic_config.py` & `statsig-0.9.3/statsig/dynamic_config.py`

 * *Files identical despite different names*

### Comparing `statsig-0.9.2/statsig/evaluator.py` & `statsig-0.9.3/statsig/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,17 +340,17 @@
                 return _ConfigEvaluation(False, False)
             return _ConfigEvaluation(False, bool(re.match(str_target, str_value)))
         elif op == "eq":
             return _ConfigEvaluation(False, value == target)
         elif op == "neq":
             return _ConfigEvaluation(False, value != target)
         elif op == "before":
-            return self.__compare_dates(value, target, lambda a, b: a.date() < b.date())
+            return self.__compare_dates(value, target, lambda a, b: a < b)
         elif op == "after":
-            return self.__compare_dates(value, target, lambda a, b: a.date() > b.date())
+            return self.__compare_dates(value, target, lambda a, b: a > b)
         elif op == "on":
             return self.__compare_dates(value, target, lambda a, b: a.date() == b.date())
         elif op == "in_segment_list" or op == "not_in_segment_list":
             in_list = self.__check_id_in_list(value, target)
             return _ConfigEvaluation(False, in_list if op == "in_segment_list" else not in_list)
 
         return _ConfigEvaluation(True)
```

### Comparing `statsig-0.9.2/statsig/layer.py` & `statsig-0.9.3/statsig/layer.py`

 * *Files identical despite different names*

### Comparing `statsig-0.9.2/statsig/statsig.py` & `statsig-0.9.3/statsig/statsig.py`

 * *Files identical despite different names*

### Comparing `statsig-0.9.2/statsig/statsig_event.py` & `statsig-0.9.3/statsig/statsig_event.py`

 * *Files identical despite different names*

### Comparing `statsig-0.9.2/statsig/statsig_logger.py` & `statsig-0.9.3/statsig/statsig_logger.py`

 * *Files identical despite different names*

### Comparing `statsig-0.9.2/statsig/statsig_network.py` & `statsig-0.9.3/statsig/statsig_network.py`

 * *Files identical despite different names*

### Comparing `statsig-0.9.2/statsig/statsig_options.py` & `statsig-0.9.3/statsig/statsig_options.py`

 * *Files identical despite different names*

### Comparing `statsig-0.9.2/statsig/statsig_server.py` & `statsig-0.9.3/statsig/statsig_server.py`

 * *Files identical despite different names*

### Comparing `statsig-0.9.2/statsig/statsig_user.py` & `statsig-0.9.3/statsig/statsig_user.py`

 * *Files identical despite different names*

### Comparing `statsig-0.9.2/statsig.egg-info/PKG-INFO` & `statsig-0.9.3/statsig.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statsig
-Version: 0.9.2
+Version: 0.9.3
 Summary: Statsig Python Server SDK
 Home-page: https://github.com/statsig-io/python-sdk
 Author: Tore Hanssen, Jiakan Wang
 Author-email: tore@statsig.com, jkw@statsig.com
 License: ISC
 Description: # Statsig Python Server SDK
         [![tests](https://github.com/statsig-io/python-sdk/actions/workflows/test.yml/badge.svg)](https://github.com/statsig-io/python-sdk/actions/workflows/test.yml)
```

