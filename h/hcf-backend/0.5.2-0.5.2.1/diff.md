# Comparing `tmp/hcf-backend-0.5.2.tar.gz` & `tmp/hcf-backend-0.5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcf-backend-0.5.2.tar", last modified: Thu Apr 13 17:20:10 2023, max compression
+gzip compressed data, was "hcf-backend-0.5.2.1.tar", last modified: Mon Apr 17 02:31:52 2023, max compression
```

## Comparing `hcf-backend-0.5.2.tar` & `hcf-backend-0.5.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-13 17:20:10.827791 hcf-backend-0.5.2/
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)     1478 2019-01-31 18:02:16.000000 hcf-backend-0.5.2/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2686 2023-04-13 17:20:10.827791 hcf-backend-0.5.2/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2067 2023-04-11 20:57:08.000000 hcf-backend-0.5.2/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-13 17:20:10.823791 hcf-backend-0.5.2/hcf_backend/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       46 2023-04-13 16:15:44.000000 hcf-backend-0.5.2/hcf_backend/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    14039 2023-04-13 16:11:52.000000 hcf-backend-0.5.2/hcf_backend/backend.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4529 2023-04-13 17:18:18.000000 hcf-backend-0.5.2/hcf_backend/manager.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-13 17:20:10.823791 hcf-backend-0.5.2/hcf_backend/utils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1566 2023-04-11 21:18:45.000000 hcf-backend-0.5.2/hcf_backend/utils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3896 2023-04-11 21:07:29.000000 hcf-backend-0.5.2/hcf_backend/utils/crawlmanager.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    13380 2023-04-13 16:12:38.000000 hcf-backend-0.5.2/hcf_backend/utils/hcfpal.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-13 17:20:10.823791 hcf-backend-0.5.2/hcf_backend.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2686 2023-04-13 17:20:10.000000 hcf-backend-0.5.2/hcf_backend.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      377 2023-04-13 17:20:10.000000 hcf-backend-0.5.2/hcf_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-04-13 17:20:10.000000 hcf-backend-0.5.2/hcf_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      107 2023-04-13 17:20:10.000000 hcf-backend-0.5.2/hcf_backend.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       12 2023-04-13 17:20:10.000000 hcf-backend-0.5.2/hcf_backend.egg-info/top_level.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2021-07-13 00:16:34.000000 hcf-backend-0.5.2/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-04-13 17:20:10.827791 hcf-backend-0.5.2/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1012 2023-04-13 16:15:32.000000 hcf-backend-0.5.2/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-17 02:31:52.522353 hcf-backend-0.5.2.1/
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)     1478 2019-01-31 18:02:16.000000 hcf-backend-0.5.2.1/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2688 2023-04-17 02:31:52.522353 hcf-backend-0.5.2.1/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2067 2023-04-11 20:57:08.000000 hcf-backend-0.5.2.1/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-17 02:31:52.518352 hcf-backend-0.5.2.1/hcf_backend/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       48 2023-04-17 02:30:13.000000 hcf-backend-0.5.2.1/hcf_backend/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    14039 2023-04-13 16:11:52.000000 hcf-backend-0.5.2.1/hcf_backend/backend.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4529 2023-04-13 17:18:18.000000 hcf-backend-0.5.2.1/hcf_backend/manager.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-17 02:31:52.522353 hcf-backend-0.5.2.1/hcf_backend/utils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1566 2023-04-11 21:18:45.000000 hcf-backend-0.5.2.1/hcf_backend/utils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4003 2023-04-17 02:24:22.000000 hcf-backend-0.5.2.1/hcf_backend/utils/crawlmanager.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    13380 2023-04-13 16:12:38.000000 hcf-backend-0.5.2.1/hcf_backend/utils/hcfpal.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-17 02:31:52.518352 hcf-backend-0.5.2.1/hcf_backend.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2688 2023-04-17 02:31:52.000000 hcf-backend-0.5.2.1/hcf_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      377 2023-04-17 02:31:52.000000 hcf-backend-0.5.2.1/hcf_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-04-17 02:31:52.000000 hcf-backend-0.5.2.1/hcf_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      107 2023-04-17 02:31:52.000000 hcf-backend-0.5.2.1/hcf_backend.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       12 2023-04-17 02:31:52.000000 hcf-backend-0.5.2.1/hcf_backend.egg-info/top_level.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2021-07-13 00:16:34.000000 hcf-backend-0.5.2.1/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-04-17 02:31:52.522353 hcf-backend-0.5.2.1/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1014 2023-04-17 02:30:02.000000 hcf-backend-0.5.2.1/setup.py
```

### Comparing `hcf-backend-0.5.2/LICENSE` & `hcf-backend-0.5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2/PKG-INFO` & `hcf-backend-0.5.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcf-backend
-Version: 0.5.2
+Version: 0.5.2.1
 Summary: ScrapyCloud HubStorage frontier backend for Frontera
 Home-page: https://github.com/scrapinghub/hcf-backend
 Maintainer: Scrapinghub
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hcf-backend-0.5.2/README.md` & `hcf-backend-0.5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2/hcf_backend/backend.py` & `hcf-backend-0.5.2.1/hcf_backend/backend.py`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2/hcf_backend/manager.py` & `hcf-backend-0.5.2.1/hcf_backend/manager.py`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2/hcf_backend/utils/__init__.py` & `hcf-backend-0.5.2.1/hcf_backend/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2/hcf_backend/utils/crawlmanager.py` & `hcf-backend-0.5.2.1/hcf_backend/utils/crawlmanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,17 +88,19 @@
                         "HCF_CONSUMER_FRONTIER": self.args.frontier,
                     }
                 )
                 frontera_settings_json = json.dumps(frontera_settings)
                 logger.info(
                     f"Will schedule spider job with frontera settings {frontera_settings_json}"
                 )
-                jobkey = self.schedule_spider(
-                    self.args.spider,
-                    frontera_settings_json=frontera_settings_json,
+                jobkey = self.schedule_spider_with_jobargs(
+                    job_args_override={
+                        "spider_args": {"frontera_settings_json": frontera_settings_json},
+                    },
+                    spider=self.args.spider,
                 )
                 logger.info(
                     f"Scheduled job {jobkey} with frontera settings {frontera_settings_json}"
                 )
             return True
         return bool(running_jobs)
```

### Comparing `hcf-backend-0.5.2/hcf_backend/utils/hcfpal.py` & `hcf-backend-0.5.2.1/hcf_backend/utils/hcfpal.py`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2/hcf_backend.egg-info/PKG-INFO` & `hcf-backend-0.5.2.1/hcf_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcf-backend
-Version: 0.5.2
+Version: 0.5.2.1
 Summary: ScrapyCloud HubStorage frontier backend for Frontera
 Home-page: https://github.com/scrapinghub/hcf-backend
 Maintainer: Scrapinghub
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hcf-backend-0.5.2/setup.py` & `hcf-backend-0.5.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name="hcf-backend",
-    version="0.5.2",
+    version="0.5.2.1",
     description="ScrapyCloud HubStorage frontier backend for Frontera",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="BSD",
     url="https://github.com/scrapinghub/hcf-backend",
     maintainer="Scrapinghub",
     packages=find_packages(),
```

