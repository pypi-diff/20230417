# Comparing `tmp/provider-switch-0.0.8.tar.gz` & `tmp/provider-switch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "provider-switch-0.0.8.tar", last modified: Tue Dec 20 07:29:04 2022, max compression
+gzip compressed data, was "provider-switch-0.0.9.tar", last modified: Tue Dec 20 07:36:09 2022, max compression
```

## Comparing `provider-switch-0.0.8.tar` & `provider-switch-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 tainguyenthanh   (501) staff       (20)        0 2022-12-20 07:29:04.254319 provider-switch-0.0.8/
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)     1057 2022-12-05 23:00:46.000000 provider-switch-0.0.8/LICENSE.txt
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)      407 2022-12-20 07:29:04.253807 provider-switch-0.0.8/PKG-INFO
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)       76 2022-12-07 09:30:15.000000 provider-switch-0.0.8/README.md
-drwxr-xr-x   0 tainguyenthanh   (501) staff       (20)        0 2022-12-20 07:29:04.243866 provider-switch-0.0.8/provider_switch/
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)      103 2022-12-06 06:44:36.000000 provider-switch-0.0.8/provider_switch/__init__.py
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)     1474 2022-12-06 02:17:54.000000 provider-switch-0.0.8/provider_switch/exceptions.py
-drwxr-xr-x   0 tainguyenthanh   (501) staff       (20)        0 2022-12-20 07:29:04.248880 provider-switch-0.0.8/provider_switch/helpers/
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)        0 2022-12-06 06:40:20.000000 provider-switch-0.0.8/provider_switch/helpers/__init__.py
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)     1042 2022-12-06 02:17:54.000000 provider-switch-0.0.8/provider_switch/helpers/common_helper.py
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)     2139 2022-12-06 02:17:54.000000 provider-switch-0.0.8/provider_switch/helpers/dotdictify.py
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)     3139 2022-12-20 07:12:35.000000 provider-switch-0.0.8/provider_switch/helpers/mapping_data.py
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)      867 2022-12-06 02:59:04.000000 provider-switch-0.0.8/provider_switch/helpers/response_helper.py
-drwxr-xr-x   0 tainguyenthanh   (501) staff       (20)        0 2022-12-20 07:29:04.250826 provider-switch-0.0.8/provider_switch/models/
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)        0 2022-12-06 02:49:00.000000 provider-switch-0.0.8/provider_switch/models/__init__.py
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)     5891 2022-12-20 07:28:46.000000 provider-switch-0.0.8/provider_switch/models/provider_model.py
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)     5200 2022-12-07 08:44:11.000000 provider-switch-0.0.8/provider_switch/provider_collection.py
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)     9271 2022-12-20 07:11:21.000000 provider-switch-0.0.8/provider_switch/provider_switch_handler.py
-drwxr-xr-x   0 tainguyenthanh   (501) staff       (20)        0 2022-12-20 07:29:04.251914 provider-switch-0.0.8/provider_switch/ssm/
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)        0 2022-12-06 06:39:41.000000 provider-switch-0.0.8/provider_switch/ssm/__init__.py
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)     2540 2022-12-07 08:44:56.000000 provider-switch-0.0.8/provider_switch/ssm/ssm_client.py
-drwxr-xr-x   0 tainguyenthanh   (501) staff       (20)        0 2022-12-20 07:29:04.253151 provider-switch-0.0.8/provider_switch/utils/
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)        0 2022-12-06 06:39:55.000000 provider-switch-0.0.8/provider_switch/utils/__init__.py
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)     1446 2022-12-06 02:26:10.000000 provider-switch-0.0.8/provider_switch/utils/common.py
-drwxr-xr-x   0 tainguyenthanh   (501) staff       (20)        0 2022-12-20 07:29:04.246296 provider-switch-0.0.8/provider_switch.egg-info/
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)      407 2022-12-20 07:29:04.000000 provider-switch-0.0.8/provider_switch.egg-info/PKG-INFO
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)      785 2022-12-20 07:29:04.000000 provider-switch-0.0.8/provider_switch.egg-info/SOURCES.txt
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)        1 2022-12-20 07:29:04.000000 provider-switch-0.0.8/provider_switch.egg-info/dependency_links.txt
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)        6 2022-12-20 07:29:04.000000 provider-switch-0.0.8/provider_switch.egg-info/requires.txt
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)       16 2022-12-20 07:29:04.000000 provider-switch-0.0.8/provider_switch.egg-info/top_level.txt
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)      116 2022-12-05 09:22:31.000000 provider-switch-0.0.8/pyproject.toml
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)       38 2022-12-20 07:29:04.254491 provider-switch-0.0.8/setup.cfg
--rw-r--r--   0 tainguyenthanh   (501) staff       (20)      723 2022-12-20 07:28:59.000000 provider-switch-0.0.8/setup.py
+drwxr-xr-x   0 tainguyenthanh   (501) staff       (20)        0 2022-12-20 07:36:09.836638 provider-switch-0.0.9/
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)     1057 2022-12-05 23:00:46.000000 provider-switch-0.0.9/LICENSE.txt
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)      407 2022-12-20 07:36:09.836126 provider-switch-0.0.9/PKG-INFO
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)       76 2022-12-07 09:30:15.000000 provider-switch-0.0.9/README.md
+drwxr-xr-x   0 tainguyenthanh   (501) staff       (20)        0 2022-12-20 07:36:09.823023 provider-switch-0.0.9/provider_switch/
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)      103 2022-12-06 06:44:36.000000 provider-switch-0.0.9/provider_switch/__init__.py
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)     1474 2022-12-06 02:17:54.000000 provider-switch-0.0.9/provider_switch/exceptions.py
+drwxr-xr-x   0 tainguyenthanh   (501) staff       (20)        0 2022-12-20 07:36:09.829263 provider-switch-0.0.9/provider_switch/helpers/
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)        0 2022-12-06 06:40:20.000000 provider-switch-0.0.9/provider_switch/helpers/__init__.py
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)     1042 2022-12-06 02:17:54.000000 provider-switch-0.0.9/provider_switch/helpers/common_helper.py
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)     2139 2022-12-06 02:17:54.000000 provider-switch-0.0.9/provider_switch/helpers/dotdictify.py
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)     3139 2022-12-20 07:12:35.000000 provider-switch-0.0.9/provider_switch/helpers/mapping_data.py
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)      867 2022-12-06 02:59:04.000000 provider-switch-0.0.9/provider_switch/helpers/response_helper.py
+drwxr-xr-x   0 tainguyenthanh   (501) staff       (20)        0 2022-12-20 07:36:09.830726 provider-switch-0.0.9/provider_switch/models/
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)        0 2022-12-06 02:49:00.000000 provider-switch-0.0.9/provider_switch/models/__init__.py
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)     5891 2022-12-20 07:35:37.000000 provider-switch-0.0.9/provider_switch/models/provider_model.py
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)     5200 2022-12-07 08:44:11.000000 provider-switch-0.0.9/provider_switch/provider_collection.py
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)     9271 2022-12-20 07:11:21.000000 provider-switch-0.0.9/provider_switch/provider_switch_handler.py
+drwxr-xr-x   0 tainguyenthanh   (501) staff       (20)        0 2022-12-20 07:36:09.832133 provider-switch-0.0.9/provider_switch/ssm/
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)        0 2022-12-06 06:39:41.000000 provider-switch-0.0.9/provider_switch/ssm/__init__.py
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)     2540 2022-12-07 08:44:56.000000 provider-switch-0.0.9/provider_switch/ssm/ssm_client.py
+drwxr-xr-x   0 tainguyenthanh   (501) staff       (20)        0 2022-12-20 07:36:09.833534 provider-switch-0.0.9/provider_switch/utils/
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)        0 2022-12-06 06:39:55.000000 provider-switch-0.0.9/provider_switch/utils/__init__.py
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)     1446 2022-12-06 02:26:10.000000 provider-switch-0.0.9/provider_switch/utils/common.py
+drwxr-xr-x   0 tainguyenthanh   (501) staff       (20)        0 2022-12-20 07:36:09.825837 provider-switch-0.0.9/provider_switch.egg-info/
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)      407 2022-12-20 07:36:09.000000 provider-switch-0.0.9/provider_switch.egg-info/PKG-INFO
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)      785 2022-12-20 07:36:09.000000 provider-switch-0.0.9/provider_switch.egg-info/SOURCES.txt
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)        1 2022-12-20 07:36:09.000000 provider-switch-0.0.9/provider_switch.egg-info/dependency_links.txt
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)        6 2022-12-20 07:36:09.000000 provider-switch-0.0.9/provider_switch.egg-info/requires.txt
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)       16 2022-12-20 07:36:09.000000 provider-switch-0.0.9/provider_switch.egg-info/top_level.txt
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)      116 2022-12-05 09:22:31.000000 provider-switch-0.0.9/pyproject.toml
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)       38 2022-12-20 07:36:09.836794 provider-switch-0.0.9/setup.cfg
+-rw-r--r--   0 tainguyenthanh   (501) staff       (20)      723 2022-12-20 07:36:07.000000 provider-switch-0.0.9/setup.py
```

### Comparing `provider-switch-0.0.8/LICENSE.txt` & `provider-switch-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `provider-switch-0.0.8/provider_switch/exceptions.py` & `provider-switch-0.0.9/provider_switch/exceptions.py`

 * *Files identical despite different names*

### Comparing `provider-switch-0.0.8/provider_switch/helpers/common_helper.py` & `provider-switch-0.0.9/provider_switch/helpers/common_helper.py`

 * *Files identical despite different names*

### Comparing `provider-switch-0.0.8/provider_switch/helpers/dotdictify.py` & `provider-switch-0.0.9/provider_switch/helpers/dotdictify.py`

 * *Files identical despite different names*

### Comparing `provider-switch-0.0.8/provider_switch/helpers/mapping_data.py` & `provider-switch-0.0.9/provider_switch/helpers/mapping_data.py`

 * *Files identical despite different names*

### Comparing `provider-switch-0.0.8/provider_switch/helpers/response_helper.py` & `provider-switch-0.0.9/provider_switch/helpers/response_helper.py`

 * *Files identical despite different names*

### Comparing `provider-switch-0.0.8/provider_switch/models/provider_model.py` & `provider-switch-0.0.9/provider_switch/models/provider_model.py`

 * *Files identical despite different names*

### Comparing `provider-switch-0.0.8/provider_switch/provider_collection.py` & `provider-switch-0.0.9/provider_switch/provider_collection.py`

 * *Files identical despite different names*

### Comparing `provider-switch-0.0.8/provider_switch/provider_switch_handler.py` & `provider-switch-0.0.9/provider_switch/provider_switch_handler.py`

 * *Files identical despite different names*

### Comparing `provider-switch-0.0.8/provider_switch/ssm/ssm_client.py` & `provider-switch-0.0.9/provider_switch/ssm/ssm_client.py`

 * *Files identical despite different names*

### Comparing `provider-switch-0.0.8/provider_switch/utils/common.py` & `provider-switch-0.0.9/provider_switch/utils/common.py`

 * *Files identical despite different names*

### Comparing `provider-switch-0.0.8/provider_switch.egg-info/SOURCES.txt` & `provider-switch-0.0.9/provider_switch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `provider-switch-0.0.8/setup.py` & `provider-switch-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='provider-switch',
-    version='0.0.8',
+    version='0.0.9',
     description='provider-switch',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Tai Nguyen',
     author_email='tai.nguyen@hiip.asia',
```

