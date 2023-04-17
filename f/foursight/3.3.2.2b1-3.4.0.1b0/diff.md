# Comparing `tmp/foursight-3.3.2.2b1.tar.gz` & `tmp/foursight-3.4.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight-3.3.2.2b1.tar", max compression
+gzip compressed data, was "foursight-3.4.0.1b0.tar", max compression
```

## Comparing `foursight-3.3.2.2b1.tar` & `foursight-3.4.0.1b0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1083 2022-09-07 10:59:14.705392 foursight-3.3.2.2b1/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-01-19 14:12:17.947754 foursight-3.3.2.2b1/chalicelib_fourfront/__init__.py
--rw-r--r--   0        0        0     1055 2023-01-19 14:12:17.950010 foursight-3.3.2.2b1/chalicelib_fourfront/app_utils.py
--rw-r--r--   0        0        0     5405 2023-01-19 14:12:17.952115 foursight-3.3.2.2b1/chalicelib_fourfront/check_schedules.py
--rw-r--r--   0        0        0    53878 2023-02-27 17:05:51.839220 foursight-3.3.2.2b1/chalicelib_fourfront/check_setup.json
--rw-r--r--   0        0        0    53878 2022-12-28 10:57:56.906089 foursight-3.3.2.2b1/chalicelib_fourfront/check_setup.json-20221228
--rw-r--r--   0        0        0    54449 2023-01-06 03:27:49.344020 foursight-3.3.2.2b1/chalicelib_fourfront/check_setup.json-debug
--rw-r--r--   0        0        0      249 2023-01-19 14:12:17.956201 foursight-3.3.2.2b1/chalicelib_fourfront/checks/__init__.py
--rw-r--r--   0        0        0    59585 2023-01-19 14:12:17.959883 foursight-3.3.2.2b1/chalicelib_fourfront/checks/audit_checks.py
--rw-r--r--   0        0        0    37766 2023-01-19 14:12:17.963001 foursight-3.3.2.2b1/chalicelib_fourfront/checks/badge_checks.py
--rw-r--r--   0        0        0    11548 2023-01-19 14:12:17.965655 foursight-3.3.2.2b1/chalicelib_fourfront/checks/deployment_checks.py
--rw-r--r--   0        0        0     2939 2023-01-25 11:36:46.617974 foursight-3.3.2.2b1/chalicelib_fourfront/checks/ecs_checks.py
--rw-r--r--   0        0        0     3914 2023-01-19 14:12:17.970674 foursight-3.3.2.2b1/chalicelib_fourfront/checks/es_checks.py
--rw-r--r--   0        0        0    14578 2023-01-19 14:12:17.974522 foursight-3.3.2.2b1/chalicelib_fourfront/checks/header_checks.py
--rw-r--r--   0        0        0      262 2023-01-19 14:12:17.974848 foursight-3.3.2.2b1/chalicelib_fourfront/checks/helpers/confchecks.py
--rw-r--r--   0        0        0    44428 2023-01-19 14:12:17.975418 foursight-3.3.2.2b1/chalicelib_fourfront/checks/helpers/google_utils.py
--rw-r--r--   0        0        0    95229 2023-01-19 14:12:17.978748 foursight-3.3.2.2b1/chalicelib_fourfront/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0    17372 2023-01-19 14:12:17.979325 foursight-3.3.2.2b1/chalicelib_fourfront/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     3686 2023-01-19 14:12:17.979607 foursight-3.3.2.2b1/chalicelib_fourfront/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0    97361 2023-01-19 14:12:17.983575 foursight-3.3.2.2b1/chalicelib_fourfront/checks/higlass_checks.py
--rw-r--r--   0        0        0    32926 2023-01-19 14:12:17.989004 foursight-3.3.2.2b1/chalicelib_fourfront/checks/release_updates_checks.py
--rw-r--r--   0        0        0    45202 2023-01-19 14:12:17.990151 foursight-3.3.2.2b1/chalicelib_fourfront/checks/system_checks.py
--rw-r--r--   0        0        0    45238 2023-01-06 03:27:33.359253 foursight-3.3.2.2b1/chalicelib_fourfront/checks/system_checks.py-debug
--rw-r--r--   0        0        0     2325 2022-11-23 00:12:24.017150 foursight-3.3.2.2b1/chalicelib_fourfront/checks/test_checks.py-backup-for-delete-20221128
--rw-r--r--   0        0        0   127978 2023-01-26 16:17:00.941264 foursight-3.3.2.2b1/chalicelib_fourfront/checks/wfr_checks.py
--rw-r--r--   0        0        0    43470 2023-01-19 14:12:18.009971 foursight-3.3.2.2b1/chalicelib_fourfront/checks/wfr_encode_checks.py
--rw-r--r--   0        0        0   137820 2023-01-25 11:33:59.675086 foursight-3.3.2.2b1/chalicelib_fourfront/checks/wrangler_checks.py
--rw-r--r--   0        0        0      621 2023-01-19 14:12:18.017415 foursight-3.3.2.2b1/chalicelib_fourfront/package.py
--rw-r--r--   0        0        0      316 2023-01-19 14:12:18.019943 foursight-3.3.2.2b1/chalicelib_fourfront/vars.py
--rw-r--r--   0        0        0     8580 2022-11-04 15:36:09.144135 foursight-3.3.2.2b1/chalicelib_fourfront/x
--rw-r--r--   0        0        0     8506 2022-11-04 15:36:19.535078 foursight-3.3.2.2b1/chalicelib_fourfront/xx
--rw-r--r--   0        0        0     1206 2023-03-17 03:04:47.531794 foursight-3.3.2.2b1/pyproject.toml
--rw-r--r--   0        0        0     1434 1970-01-01 00:00:00.000000 foursight-3.3.2.2b1/setup.py
--rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 foursight-3.3.2.2b1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-07 10:59:14.705392 foursight-3.4.0.1b0/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-01-19 14:12:17.947754 foursight-3.4.0.1b0/chalicelib_fourfront/__init__.py
+-rw-r--r--   0        0        0     1055 2023-03-29 20:27:15.171164 foursight-3.4.0.1b0/chalicelib_fourfront/app_utils.py
+-rw-r--r--   0        0        0     5405 2023-01-19 14:12:17.952115 foursight-3.4.0.1b0/chalicelib_fourfront/check_schedules.py
+-rw-r--r--   0        0        0    53878 2023-02-27 17:05:51.839220 foursight-3.4.0.1b0/chalicelib_fourfront/check_setup.json
+-rw-r--r--   0        0        0    53878 2022-12-28 10:57:56.906089 foursight-3.4.0.1b0/chalicelib_fourfront/check_setup.json-20221228
+-rw-r--r--   0        0        0    54449 2023-01-06 03:27:49.344020 foursight-3.4.0.1b0/chalicelib_fourfront/check_setup.json-debug
+-rw-r--r--   0        0        0      249 2023-01-19 14:12:17.956201 foursight-3.4.0.1b0/chalicelib_fourfront/checks/__init__.py
+-rw-r--r--   0        0        0    59585 2023-01-19 14:12:17.959883 foursight-3.4.0.1b0/chalicelib_fourfront/checks/audit_checks.py
+-rw-r--r--   0        0        0    37766 2023-01-19 14:12:17.963001 foursight-3.4.0.1b0/chalicelib_fourfront/checks/badge_checks.py
+-rw-r--r--   0        0        0    11548 2023-01-19 14:12:17.965655 foursight-3.4.0.1b0/chalicelib_fourfront/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2939 2023-01-25 11:36:46.617974 foursight-3.4.0.1b0/chalicelib_fourfront/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3914 2023-01-19 14:12:17.970674 foursight-3.4.0.1b0/chalicelib_fourfront/checks/es_checks.py
+-rw-r--r--   0        0        0    14578 2023-01-19 14:12:17.974522 foursight-3.4.0.1b0/chalicelib_fourfront/checks/header_checks.py
+-rw-r--r--   0        0        0      262 2023-01-19 14:12:17.974848 foursight-3.4.0.1b0/chalicelib_fourfront/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0    44428 2023-01-19 14:12:17.975418 foursight-3.4.0.1b0/chalicelib_fourfront/checks/helpers/google_utils.py
+-rw-r--r--   0        0        0    95229 2023-01-19 14:12:17.978748 foursight-3.4.0.1b0/chalicelib_fourfront/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0    17372 2023-01-19 14:12:17.979325 foursight-3.4.0.1b0/chalicelib_fourfront/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     3686 2023-01-19 14:12:17.979607 foursight-3.4.0.1b0/chalicelib_fourfront/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0    97361 2023-01-19 14:12:17.983575 foursight-3.4.0.1b0/chalicelib_fourfront/checks/higlass_checks.py
+-rw-r--r--   0        0        0    32926 2023-01-19 14:12:17.989004 foursight-3.4.0.1b0/chalicelib_fourfront/checks/release_updates_checks.py
+-rw-r--r--   0        0        0    45202 2023-01-19 14:12:17.990151 foursight-3.4.0.1b0/chalicelib_fourfront/checks/system_checks.py
+-rw-r--r--   0        0        0    45238 2023-01-06 03:27:33.359253 foursight-3.4.0.1b0/chalicelib_fourfront/checks/system_checks.py-debug
+-rw-r--r--   0        0        0     2325 2022-11-23 00:12:24.017150 foursight-3.4.0.1b0/chalicelib_fourfront/checks/test_checks.py-backup-for-delete-20221128
+-rw-r--r--   0        0        0   127978 2023-01-26 16:17:00.941264 foursight-3.4.0.1b0/chalicelib_fourfront/checks/wfr_checks.py
+-rw-r--r--   0        0        0    43470 2023-01-19 14:12:18.009971 foursight-3.4.0.1b0/chalicelib_fourfront/checks/wfr_encode_checks.py
+-rw-r--r--   0        0        0   137820 2023-01-25 11:33:59.675086 foursight-3.4.0.1b0/chalicelib_fourfront/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      621 2023-03-29 20:27:15.171432 foursight-3.4.0.1b0/chalicelib_fourfront/package.py
+-rw-r--r--   0        0        0      316 2023-03-29 19:16:47.518681 foursight-3.4.0.1b0/chalicelib_fourfront/vars.py
+-rw-r--r--   0        0        0     8580 2022-11-04 15:36:09.144135 foursight-3.4.0.1b0/chalicelib_fourfront/x
+-rw-r--r--   0        0        0     8506 2022-11-04 15:36:19.535078 foursight-3.4.0.1b0/chalicelib_fourfront/xx
+-rw-r--r--   0        0        0     1233 2023-04-17 12:08:29.735226 foursight-3.4.0.1b0/pyproject.toml
+-rw-r--r--   0        0        0     1444 1970-01-01 00:00:00.000000 foursight-3.4.0.1b0/setup.py
+-rw-r--r--   0        0        0     1090 1970-01-01 00:00:00.000000 foursight-3.4.0.1b0/PKG-INFO
```

### Comparing `foursight-3.3.2.2b1/LICENSE.txt` & `foursight-3.4.0.1b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/app_utils.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/check_schedules.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/check_setup.json` & `foursight-3.4.0.1b0/chalicelib_fourfront/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/check_setup.json-20221228` & `foursight-3.4.0.1b0/chalicelib_fourfront/check_setup.json-20221228`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/check_setup.json-debug` & `foursight-3.4.0.1b0/chalicelib_fourfront/check_setup.json-debug`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/audit_checks.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/badge_checks.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/badge_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/deployment_checks.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/ecs_checks.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/es_checks.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/header_checks.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/header_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/helpers/google_utils.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/helpers/google_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/helpers/wfr_utils.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/helpers/wfrset_utils.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/helpers/wrangler_utils.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/higlass_checks.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/higlass_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/release_updates_checks.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/release_updates_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/system_checks.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/system_checks.py-debug` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/system_checks.py-debug`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/test_checks.py-backup-for-delete-20221128` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/test_checks.py-backup-for-delete-20221128`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/wfr_checks.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/wfr_encode_checks.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/wfr_encode_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/checks/wrangler_checks.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/package.py` & `foursight-3.4.0.1b0/chalicelib_fourfront/package.py`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/x` & `foursight-3.4.0.1b0/chalicelib_fourfront/x`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/chalicelib_fourfront/xx` & `foursight-3.4.0.1b0/chalicelib_fourfront/xx`

 * *Files identical despite different names*

### Comparing `foursight-3.3.2.2b1/pyproject.toml` & `foursight-3.4.0.1b0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "foursight"
-version = "3.3.2.2b1"
+version = "3.4.0.1b0"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_fourfront" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.10"
-dcicutils = "^6.8.0"
+dcicutils = "7.2.0.1b0"
 click = "^7.1.2"
-PyJWT = "2.5.0"
+PyJWT = "^2.5.0"
 Jinja2 = "2.10.1"
 MarkupSafe = "1.1.1"
 google-api-python-client = "^1.7.4"
 geocoder = "1.38.1"
 elasticsearch = "^7.13.4"
 elasticsearch-dsl = "^7.0.0"
 gitpython = "^3.1.2"
 pytz = "^2020.1"
-tibanna_ff = ">=0.22.5"
+#tibanna_ff = ">=0.22.5"
+tibanna-ff = "^1.4.0"
 ## adding foursight-core
 # use below for deployment
-foursight-core = "3.3.2.2b1"
+foursight-core = "4.1.0.1b0"
 # use below for tests but not for deployment
 # foursight-core = { git = "https://github.com/4dn-dcic/foursight-core.git", branch="master" }
 pytest = "5.1.2"
 gspread = ">=3.6.0"
 oauth2client = ">=4.1.3"
 pandas = ">=1.1.4"
```

### Comparing `foursight-3.3.2.2b1/setup.py` & `foursight-3.4.0.1b0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,39 +8,39 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Jinja2==2.10.1',
  'MarkupSafe==1.1.1',
- 'PyJWT==2.5.0',
+ 'PyJWT>=2.5.0,<3.0.0',
  'click>=7.1.2,<8.0.0',
- 'dcicutils>=6.8.0,<7.0.0',
+ 'dcicutils==7.2.0.1b0',
  'elasticsearch-dsl>=7.0.0,<8.0.0',
  'elasticsearch>=7.13.4,<8.0.0',
- 'foursight-core==3.3.2.2b1',
+ 'foursight-core==4.1.0.1b0',
  'geocoder==1.38.1',
  'gitpython>=3.1.2,<4.0.0',
  'google-api-python-client>=1.7.4,<2.0.0',
  'gspread>=3.6.0',
  'oauth2client>=4.1.3',
  'pandas>=1.1.4',
  'pytest==5.1.2',
  'pytz>=2020.1,<2021.0',
- 'tibanna_ff>=0.22.5']
+ 'tibanna-ff>=1.4.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['decrypt-accounts-file = '
                      'foursight_core.scripts.decrypt_accounts_file:main',
                      'encrypt-accounts-file = '
                      'foursight_core.scripts.encrypt_accounts_file:main']}
 
 setup_kwargs = {
     'name': 'foursight',
-    'version': '3.3.2.2b1',
+    'version': '3.4.0.1b0',
     'description': 'Serverless Chalice Application for Monitoring',
     'long_description': 'None',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `foursight-3.3.2.2b1/PKG-INFO` & `foursight-3.4.0.1b0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: foursight
-Version: 3.3.2.2b1
+Version: 3.4.0.1b0
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (==2.10.1)
 Requires-Dist: MarkupSafe (==1.1.1)
-Requires-Dist: PyJWT (==2.5.0)
+Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
-Requires-Dist: dcicutils (>=6.8.0,<7.0.0)
+Requires-Dist: dcicutils (==7.2.0.1b0)
 Requires-Dist: elasticsearch (>=7.13.4,<8.0.0)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
-Requires-Dist: foursight-core (==3.3.2.2b1)
+Requires-Dist: foursight-core (==4.1.0.1b0)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.7.4,<2.0.0)
 Requires-Dist: gspread (>=3.6.0)
 Requires-Dist: oauth2client (>=4.1.3)
 Requires-Dist: pandas (>=1.1.4)
 Requires-Dist: pytest (==5.1.2)
 Requires-Dist: pytz (>=2020.1,<2021.0)
-Requires-Dist: tibanna_ff (>=0.22.5)
+Requires-Dist: tibanna-ff (>=1.4.0,<2.0.0)
```

