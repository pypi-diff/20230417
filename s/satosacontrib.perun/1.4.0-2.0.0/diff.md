# Comparing `tmp/satosacontrib.perun-1.4.0.tar.gz` & `tmp/satosacontrib.perun-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satosacontrib.perun-1.4.0.tar", last modified: Fri Mar 10 10:16:46 2023, max compression
+gzip compressed data, was "satosacontrib.perun-2.0.0.tar", last modified: Mon Apr 17 14:27:54 2023, max compression
```

## Comparing `satosacontrib.perun-1.4.0.tar` & `satosacontrib.perun-2.0.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 10:16:46.322574 satosacontrib.perun-1.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      246 2023-03-10 10:16:46.322574 satosacontrib.perun-1.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 10:16:46.230572 satosacontrib.perun-1.4.0/satosacontrib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 10:16:46.234572 satosacontrib.perun-1.4.0/satosacontrib/perun/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 10:16:46.314574 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/
--rw-rw-rw-   0 root         (0) root         (0)     1134 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     5297 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/context_attributes_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3840 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/is_eligible_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2200 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     1200 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     5667 2023-03-09 15:28:42.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/perun_attributes_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)    11614 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/perun_ensure_member.py
--rw-rw-rw-   0 root         (0) root         (0)    11333 2023-03-09 15:28:42.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/perun_entitlement.py
--rw-rw-rw-   0 root         (0) root         (0)     2857 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/perun_identity_beta_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     4811 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/perun_user_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)    24571 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/sp_authorization_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)    11223 2023-03-09 15:28:42.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/update_user_ext_source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 10:16:46.318574 satosacontrib.perun-1.4.0/satosacontrib/perun/utils/
--rw-rw-rw-   0 root         (0) root         (0)     2042 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/utils/ConfigStore.py
--rw-rw-rw-   0 root         (0) root         (0)     4435 2023-03-10 08:39:44.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/utils/CurlConnector.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2023-03-09 15:28:42.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/utils/CurlConnectorInterface.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/utils/PerunConstants.py
--rw-rw-rw-   0 root         (0) root         (0)     4339 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/utils/Utils.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/satosacontrib/perun/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 10:16:46.230572 satosacontrib.perun-1.4.0/satosacontrib.perun.egg-info/
--rw-r--r--   0 root         (0) root         (0)      246 2023-03-10 10:16:46.000000 satosacontrib.perun-1.4.0/satosacontrib.perun.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1975 2023-03-10 10:16:46.000000 satosacontrib.perun-1.4.0/satosacontrib.perun.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-10 10:16:46.000000 satosacontrib.perun-1.4.0/satosacontrib.perun.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      179 2023-03-10 10:16:46.000000 satosacontrib.perun-1.4.0/satosacontrib.perun.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-03-10 10:16:46.000000 satosacontrib.perun-1.4.0/satosacontrib.perun.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-03-10 10:16:46.322574 satosacontrib.perun-1.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      600 2023-03-10 09:07:03.000000 satosacontrib.perun-1.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 10:16:46.322574 satosacontrib.perun-1.4.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/tests/test_auth_event_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     7500 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/tests/test_is_eligible_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2012 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/tests/test_microservice_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     3972 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/tests/test_perun_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    15103 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/tests/test_perun_ensure_member.py
--rw-rw-rw-   0 root         (0) root         (0)     7143 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/tests/test_perun_entitlement.py
--rw-rw-rw-   0 root         (0) root         (0)     5403 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/tests/test_perun_user_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)    36337 2023-03-09 15:28:42.000000 satosacontrib.perun-1.4.0/tests/test_sp_authorization_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     7233 2023-03-02 18:50:54.000000 satosacontrib.perun-1.4.0/tests/test_update_ues.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:27:53.998046 satosacontrib.perun-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      246 2023-04-17 14:27:53.998046 satosacontrib.perun-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:27:53.438033 satosacontrib.perun-2.0.0/satosacontrib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/satosacontrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:27:53.438033 satosacontrib.perun-2.0.0/satosacontrib/perun/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:27:53.502034 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/
+-rw-rw-rw-   0 root         (0) root         (0)      588 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     5297 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/context_attributes_microservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:27:53.574036 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/idm/
+-rw-rw-rw-   0 root         (0) root         (0)      387 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/idm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5927 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/idm/attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11822 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/idm/ensure_member.py
+-rw-rw-rw-   0 root         (0) root         (0)    11583 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/idm/entitlement.py
+-rw-rw-rw-   0 root         (0) root         (0)     4831 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/idm/perun_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    24791 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/idm/sp_authorization.py
+-rw-rw-rw-   0 root         (0) root         (0)    11491 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py
+-rw-rw-rw-   0 root         (0) root         (0)     3840 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/is_eligible_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2200 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1200 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:27:53.778041 satosacontrib.perun-2.0.0/satosacontrib/perun/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     2042 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/utils/ConfigStore.py
+-rw-rw-rw-   0 root         (0) root         (0)     4435 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/utils/CurlConnector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/utils/CurlConnectorInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/utils/PerunConstants.py
+-rw-rw-rw-   0 root         (0) root         (0)     6364 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/utils/Utils.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/satosacontrib/perun/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:27:53.438033 satosacontrib.perun-2.0.0/satosacontrib.perun.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      246 2023-04-17 14:27:53.000000 satosacontrib.perun-2.0.0/satosacontrib.perun.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-04-17 14:27:53.000000 satosacontrib.perun-2.0.0/satosacontrib.perun.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 14:27:53.000000 satosacontrib.perun-2.0.0/satosacontrib.perun.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      179 2023-04-17 14:27:53.000000 satosacontrib.perun-2.0.0/satosacontrib.perun.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-17 14:27:53.000000 satosacontrib.perun-2.0.0/satosacontrib.perun.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-17 14:27:53.998046 satosacontrib.perun-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      600 2023-04-17 14:15:59.000000 satosacontrib.perun-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:27:53.998046 satosacontrib.perun-2.0.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/tests/test_auth_event_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     7500 2023-04-03 10:53:57.000000 satosacontrib.perun-2.0.0/tests/test_is_eligible_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2531 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/tests/test_microservice_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     3981 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/tests/test_perun_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    14517 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/tests/test_perun_ensure_member.py
+-rw-rw-rw-   0 root         (0) root         (0)     7117 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/tests/test_perun_entitlement.py
+-rw-rw-rw-   0 root         (0) root         (0)     5672 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/tests/test_perun_user_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)    36568 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/tests/test_sp_authorization_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     7291 2023-04-17 11:35:57.000000 satosacontrib.perun-2.0.0/tests/test_update_ues.py
```

### Comparing `satosacontrib.perun-1.4.0/LICENSE` & `satosacontrib.perun-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/context_attributes_microservice.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/context_attributes_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/is_eligible_microservice.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/is_eligible_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/perun_attributes_microservice.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/idm/attributes.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,17 +6,18 @@
     AdaptersManagerNotExistsException,
 )
 from satosa.exception import SATOSAError
 from satosa.context import Context
 from satosa.internal import InternalData
 
 from satosacontrib.perun.utils.ConfigStore import ConfigStore
+from satosacontrib.perun.utils.Utils import Utils
 
 
-class PerunAttributes(ResponseMicroService):
+class Attributes(ResponseMicroService):
 
     """
     This Satosa microservice fetches user attributes by its names listed
     as keys of attrMap config property and set them as Attributes
     values to keys specified as attrMap values. Old values of
     Attributes are replaced.
 
@@ -32,15 +33,15 @@
         self.MODE_FULL = "FULL"
         self.MODE_PARTIAL = "PARTIAL"
 
         self.__global_cfg = ConfigStore.get_global_cfg(config["global_cfg_path"])
         self.__attr_map_cfg = ConfigStore.get_attributes_map(
             self.__global_cfg["attrs_cfg_path"]
         )
-
+        self.__allowed_requesters = self.__global_cfg.get("allowed_requesters", {})
         self.__adapters_manager = AdaptersManager(
             self.__global_cfg["adapters_manager"], self.__attr_map_cfg
         )
 
         if not config["mode"]:
             config["mode"] = self.MODE_FULL
 
@@ -55,15 +56,16 @@
         """
         This is where the micro service should modify the request / response.
         Subclasses must call this method (or in another way make sure the
         next callable is called).
         @param context: The current context
         @param data: Data to be modified
         """
-
+        if not Utils.allow_by_requester(context, data, self.__allowed_requesters):
+            return super().process(context, data)
         user_id = data.attributes.get(
             self.__global_cfg["perun_user_id_attribute"]
         )  # noqa
         if not user_id:
             raise SATOSAError(
                 self.__class__.__name__ + f"Missing mandatory attribute "
                 f"'{self.__global_cfg['perun_user_id_attribute']}' "
```

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/perun_ensure_member.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/idm/ensure_member.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,37 +8,38 @@
 from satosa.micro_services.base import ResponseMicroService
 from satosa.exception import SATOSAError
 from satosa.response import Redirect
 from satosacontrib.perun.utils.ConfigStore import ConfigStore
 from satosacontrib.perun.utils.Utils import Utils
 
 
-class PerunEnsureMember(ResponseMicroService):
+class EnsureMember(ResponseMicroService):
     """
     This Satosa microservice checks member status
     of the user and calls registration if needed
     """
 
     def __init__(self, config, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        self.LOG_PREFIX = "perun:PerunEnsureMember: "
+        self.LOG_PREFIX = "perun:EnsureMember: "
         self.REGISTER_URL = "register_url"
         self.VO_SHORT_NAME = "vo_short_name"
         self.GROUP_NAME = "group_name"
         self.CALLBACK_PARAMETER_NAME = "callback_parameter_name"
         self.PARAM_REGISTRATION_URL = "registration_url"
 
         self.__logger = Logger.get_logger(self.__class__.__name__)
 
         self.__config = config
         self.__global_cfg = ConfigStore.get_global_cfg(config["global_cfg_path"])
         self.__attr_map_cfg = ConfigStore.get_attributes_map(
             self.__global_cfg["attrs_cfg_path"]
         )
+        self.__allowed_requesters = self.__global_cfg.get("allowed_requesters", {})
         self.__adapters_manager = AdaptersManager(
             self.__global_cfg["adapters_manager"], self.__attr_map_cfg
         )
 
         self.__signing_cfg = self.__global_cfg["jwk"]
 
         if (
@@ -91,14 +92,17 @@
         """
         This is where the micro service should modify the request / response.
         Subclasses must call this method (or in another way make sure the
         next callable is called).
         @param context: The current context
         @param data: Data to be modified
         """
+
+        if not Utils.allow_by_requester(context, data, self.__allowed_requesters):
+            return super().process(context, data)
         user_id = data.attributes.get(
             self.__global_cfg["perun_user_id_attribute"]
         )  # noqa
         if not user_id:
             raise SATOSAError(
                 self.LOG_PREFIX + f"Missing mandatory attribute "
                 f"'{self.__global_cfg['perun_user_id_attribute']}' "  # noqa
```

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/perun_entitlement.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/idm/entitlement.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 from perun.connector.adapters.AdaptersManager import AdaptersManager
 from satosa.exception import SATOSAError
 from re import sub
 from natsort import natsorted
 from urllib.parse import quote
 
 from satosacontrib.perun.utils.ConfigStore import ConfigStore
+from satosacontrib.perun.utils.Utils import Utils
 
 
 def encode_entitlement(group_name):
     return quote(group_name, safe="!$'()*,;&=@:+")
 
 
 def encode_name(name):
     return quote(name, safe="!'()*")
 
 
-class PerunEntitlement(ResponseMicroService):
+class Entitlement(ResponseMicroService):
 
     """This Satosa microservice joins
     eduPersonEntitlement, forwardedEduPersonEntitlement,
     resource capabilities and facility capabilities"""
 
     def __init__(self, config, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -45,14 +46,15 @@
             self.__extended = True
 
         self.__global_cfg = ConfigStore.get_global_cfg(config["global_cfg_path"])
 
         self.__attr_map_cfg = ConfigStore.get_attributes_map(
             self.__global_cfg["attrs_cfg_path"]
         )
+        self.__allowed_requesters = self.__global_cfg.get("allowed_requesters", {})
         self.__adapters_manager = AdaptersManager(
             self.__global_cfg["adapters_manager"], self.__attr_map_cfg
         )
         if not self.__extended:
             self.__edu_person_entitlement = self.__global_cfg[self.OUTPUT_ATTR_NAME]
         else:
             self.__output_attr_name = self.__global_cfg[self.OUTPUT_ATTR_NAME]
@@ -76,33 +78,33 @@
         This is where the micro service should modify the request / response.
         Subclasses must call this method (or in another way make sure the
         next callable is called).
 
         @param context: The current context
         @param data: Data to be modified
         """
-
+        if not Utils.allow_by_requester(context, data, self.__allowed_requesters):
+            return super().process(context, data)
         edu_person_entitlement = []
         edu_person_entitlement_extended = []
         capabilities = []
         forwarded_edu_person_entitlement = []
-
         if data.data["perun"]["groups"]:
             if not self.__extended:
                 edu_person_entitlement = self.__get_edu_person_entitlement(data)
             else:
                 edu_person_entitlement_extended = (
                     self.__get_edu_person_entitlement_extended(data)
                 )
 
             capabilities = self.__get_capabilities(data)
 
         else:
             self.__logger.debug(
-                "perun:PerunEntitlement: There are no user "
+                "perun:Entitlement: There are no user "
                 "groups assigned to facility. => Skipping "
                 "getEduPersonEntitlement and getCapabilities"
             )
 
         if self.__release_forwarded_entitlement:
             forwarded_edu_person_entitlement = (
                 self.__get_forwarded_edu_person_entitlement(
@@ -143,15 +145,15 @@
         for group in groups:
             group_name = group.unique_name
             group_name = sub(r"^(\w*):members$", r"\1", group_name)
 
             if self.__config["group_name_AARC"] or self.__group_name_aarc:
                 if not self.__entitlement_authority or not self.__entitlement_prefix:
                     raise SATOSAError(
-                        "perun:PerunEntitlement: missing "
+                        "perun:Entitlement: missing "
                         "mandatory configuration options "
                         "'groupNameAuthority' "
                         "or 'groupNamePrefix'."
                     )
 
                 group_name = self.__group_name_wrapper(group_name)
             else:
```

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/perun_user_microservice.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/idm/perun_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,18 @@
     def __init__(self, config, *args, **kwargs):
         super().__init__(*args, **kwargs)
         logger.info("PerunUser is active")
         global_config = ConfigStore.get_global_cfg(config["global_cfg_filepath"])
 
         self.__perun_user_id_attr = global_config["perun_user_id_attribute"]
         self.__perun_login_attribute = global_config["perun_login_attribute"]
+        self.__allowed_requesters = global_config.get("allowed_requesters", {})
         self.__internal_login_attribute = config["internal_login_attribute"]
         self.__internal_extsource_attribute = config["internal_extsource_attribute"]
         self.__proxy_extsource_name = config["proxy_extsource_name"]
-        self.__allowed_requesters = config.get("allowed_requesters", [])
         self.__registration_page_url = config.get("registration_page_url", [])
         self.__registration_result_url = config["registration_result_url"]
 
         adapters_manager_cfg = global_config["adapters_manager"]
         attrs_map = ConfigStore.get_attributes_map(global_config["attrs_cfg_path"])
 
         self.__adapters_manager = AdaptersManager(adapters_manager_cfg, attrs_map)
@@ -56,17 +56,16 @@
         """
         Load user login from Perun for specified IdPs.
 
         @param context: request context
         @param data: the internal request
         """
 
-        if data.requester not in self.__allowed_requesters:
-            raise SATOSAError("Data request not allowed.")
-
+        if not Utils.allow_by_requester(context, data, self.__allowed_requesters):
+            return super().process(context, data)
         name = data.auth_info.issuer
         logins = data.attributes[self.__internal_login_attribute]
 
         try:
             user = self.__adapters_manager.get_perun_user(name, logins)
         except AdaptersManagerNotExistsException:
             return self.handle_user_not_found(name, logins, context, data)
```

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/sp_authorization_microservice.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/idm/sp_authorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         super().__init__(*args, **kwargs)
         logger.info(f"{SpAuthorization.__name__} is active")
         self.__DEBUG_PREFIX = self.name
         self.__endpoint = "/process"
         self.__config = config
         self.__global_config = ConfigStore.get_global_cfg(config["global_cfg_filepath"])
         self.__signing_cfg = self.__global_config["jwk"]
+        self.__allowed_requesters = self.__global_config.get("allowed_requesters", {})
 
         self.__filter_config = config["filter_config"]
 
         self.__CHECK_GROUP_MEMBERSHIP_ATTR = "check_group_membership_attr"
         self.__VO_SHORT_NAMES_ATTR = "vo_short_names_attr"
         self.__ALLOW_REGISTRATION_ATTR = "allow_registration_attr"
         self.__REGISTRATION_LINK_ATTR = "registration_link_attr"
@@ -106,14 +107,16 @@
         to the method handle_unsatisfied_membership.
 
         @param context: object for sharing proxy data through the current
                         request
         @param data: data carried between frontend and backend
         @return:
         """
+        if not Utils.allow_by_requester(context, data, self.__allowed_requesters):
+            return super().process(context, data)
         data_requester = data.requester
         user_id = data.attributes.get(self.__global_config["perun_user_id_attribute"])
         if not user_id:
             logger.debug(
                 "Request does not contain Perun user. Did you configure "
                 "PerunUser microservice?"
             )
```

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/micro_services/update_user_ext_source.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from perun.connector.adapters.AdaptersManager import AdaptersManagerException
 from satosa.micro_services.base import ResponseMicroService
 from satosa import exception
 from typing import List, Union, Any
 from satosacontrib.perun.utils.ConfigStore import ConfigStore
 import threading
 
+from satosacontrib.perun.utils.Utils import Utils
+
 
 def is_complex_type(attribute_type: type) -> bool:
     return isinstance(attribute_type, list) or isinstance(attribute_type, dict)
 
 
 def is_simple_type(attribute_type: type) -> bool:
     return (
@@ -57,14 +59,15 @@
 
         self.__global_conf = ConfigStore.get_global_cfg(config["global_cfg_path"])
         self.__attr_map_cfg = ConfigStore.get_attributes_map(
             self.__global_conf["attrs_cfg_path"]
         )
 
         self.__perun_id_attr = self.__global_conf["perun_user_id_attribute"]
+        self.__allowed_requesters = self.__global_conf.get("allowed_requesters", {})
         self.__adapters_manager = AdaptersManager(
             self.__global_conf["adapters_manager"], self.__attr_map_cfg
         )
         self.__append_only_attrs = []
         self.__array_to_str_conversion = []
         if config["array_to_string_conversion"]:
             self.__array_to_str_conversion = config["array_to_string_conversion"]
@@ -75,15 +78,16 @@
         """
         This is where the micro service should modify the request / response.
         Subclasses must call this method (or in another way make sure the
         next callable is called).
         @param context: The current context
         @param data: Data to be modified
         """
-
+        if not Utils.allow_by_requester(context, data, self.__allowed_requesters):
+            return super().process(context, data)
         data_to_conversion = {
             "attributes": data.attributes,
             "attr_map": self.__config["attr_map"],
             "attrs_to_conversion": self.__array_to_str_conversion,
             "append_only_attrs": self.__append_only_attrs,
             "perun_user_id": data.attributes[self.__perun_id_attr],
             "auth_info": data.auth_info,
```

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/utils/ConfigStore.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/utils/ConfigStore.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/utils/CurlConnector.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/utils/CurlConnector.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-1.4.0/satosacontrib/perun/utils/CurlConnectorInterface.py` & `satosacontrib.perun-2.0.0/satosacontrib/perun/utils/CurlConnectorInterface.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-1.4.0/satosacontrib.perun.egg-info/SOURCES.txt` & `satosacontrib.perun-2.0.0/satosacontrib.perun.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 satosacontrib/perun/micro_services/attribute_typing_microservice.py
 satosacontrib/perun/micro_services/auth_event_logging_microservice.py
 satosacontrib/perun/micro_services/cardinality_single_microservice.py
 satosacontrib/perun/micro_services/context_attributes_microservice.py
 satosacontrib/perun/micro_services/is_eligible_microservice.py
 satosacontrib/perun/micro_services/multi_idphint_microservice.py
 satosacontrib/perun/micro_services/nameid_attribute_microservice.py
-satosacontrib/perun/micro_services/perun_attributes_microservice.py
-satosacontrib/perun/micro_services/perun_ensure_member.py
-satosacontrib/perun/micro_services/perun_entitlement.py
-satosacontrib/perun/micro_services/perun_identity_beta_microservice.py
-satosacontrib/perun/micro_services/perun_user_microservice.py
 satosacontrib/perun/micro_services/proxystatistics_microservice.py
-satosacontrib/perun/micro_services/sp_authorization_microservice.py
-satosacontrib/perun/micro_services/update_user_ext_source.py
+satosacontrib/perun/micro_services/idm/__init__.py
+satosacontrib/perun/micro_services/idm/attributes.py
+satosacontrib/perun/micro_services/idm/ensure_member.py
+satosacontrib/perun/micro_services/idm/entitlement.py
+satosacontrib/perun/micro_services/idm/perun_user.py
+satosacontrib/perun/micro_services/idm/sp_authorization.py
+satosacontrib/perun/micro_services/idm/update_user_ext_source.py
 satosacontrib/perun/utils/AuthEventLoggingDbModels.py
 satosacontrib/perun/utils/ConfigStore.py
 satosacontrib/perun/utils/CurlConnector.py
 satosacontrib/perun/utils/CurlConnectorInterface.py
 satosacontrib/perun/utils/PerunConstants.py
 satosacontrib/perun/utils/Utils.py
 satosacontrib/perun/utils/__init__.py
```

### Comparing `satosacontrib.perun-1.4.0/setup.py` & `satosacontrib.perun-2.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,13 +11,13 @@
         "SATOSA~=8.1",
         "pysaml2~=7.1",
         "requests~=2.28",
         "perun.connector~=3.3",
         "PyYAML~=6.0",
         "SQLAlchemy~=1.4",
         "jwcrypto~=1.3",
-        "natsort~=8.2.0",
+        "natsort~=8.3.1",
         "python-dateutil~=2.8",
         "geoip2~=4.6",
         "user_agents~=2.2",
     ],
 )
```

### Comparing `satosacontrib.perun-1.4.0/tests/test_auth_event_logging.py` & `satosacontrib.perun-2.0.0/tests/test_auth_event_logging.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-1.4.0/tests/test_is_eligible_microservice.py` & `satosacontrib.perun-2.0.0/tests/test_is_eligible_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-1.4.0/tests/test_microservice_loader.py` & `satosacontrib.perun-2.0.0/tests/test_microservice_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 
 
 class TestContext(Context):
     __test__ = False
 
     def __init__(self):
         super().__init__()
+        self.internal_data["target_entity_id"] = "example_entity_id"
 
 
 class TestData(InternalData):
     __test__ = False
 
     def __init__(self, data, attributes):
         super().__init__()
         self.data = data
         self.attributes = attributes
         self.auth_info = None
+        self.requester = "example_requester"
 
 
 class Loader:
     GLOBAL_CONFIG = {
         "eduperson_entitlement": "edu_person_entitlement",
         "forwarded_eduperson_entitlement": "forwarded_edu_person_entitlement",
         "perun_user_id_attribute": "example_user_id",
@@ -34,26 +36,37 @@
         "attrs_cfg_path": "example_path",
         "adapters_manager": "adapters manager cfg info",
         "jwk": {
             "keystore": "example_keystore",
             "keyid": "example_keyid",
             "token_alg": "example_token_alg",
         },
+        "allowed_requesters": {
+            "": {"deny": ["forbidden_requester"]},
+            "target_entity_id1": {"allow": ["allowed_requester"]},
+            "target_entity_id2": {"deny": ["forbidden_requester"]},
+        },
     }
 
     def __init__(self, config, name_of_microservice):
         self.config = config
         self.name = name_of_microservice
 
     @patch("satosacontrib.perun.utils.ConfigStore.ConfigStore.get_global_cfg")
     @patch(
         "satosacontrib.perun.utils.ConfigStore.ConfigStore.get_attributes_map"
     )  # noqa
     @patch("perun.connector.adapters.AdaptersManager.AdaptersManager.__init__")
-    def create_mocked_instance(self, mock_request, mock_request2, mock_request3):
+    def create_mocked_instance(
+        self, mock_request, mock_request2, mock_request3, perun_micro_service=False
+    ):
         ConfigStore.get_global_cfg = MagicMock(
             return_value=Loader.GLOBAL_CONFIG
         )  # noqa
         ConfigStore.get_attributes_map = MagicMock(return_value=None)
         AdaptersManager.__init__ = MagicMock(return_value=None)
-        my_class = getattr(satosacontrib.perun.micro_services, self.name)
+        my_class = (
+            getattr(satosacontrib.perun.micro_services.idm, self.name)
+            if perun_micro_service
+            else getattr(satosacontrib.perun.micro_services, self.name)
+        )
         return my_class(self.config, self.name, self.name + "Url")
```

### Comparing `satosacontrib.perun-1.4.0/tests/test_perun_attributes.py` & `satosacontrib.perun-2.0.0/tests/test_perun_attributes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from perun.connector.adapters.AdaptersManager import AdaptersManager
 from satosa.exception import SATOSAError
-from satosacontrib.perun.micro_services.perun_attributes_microservice import (
-    PerunAttributes,
+from satosacontrib.perun.micro_services.idm.attributes import (
+    Attributes,
 )  # noqa
 from tests.test_microservice_loader import Loader, TestData, TestContext
 from unittest.mock import patch, MagicMock
 
 import pytest
 
 
@@ -41,18 +41,20 @@
     "name_id": "name_id",
     "eduperson_targeted_id": "eduperson_targeted_id",
     "eduperson_principal_name": "eduperson_principal_name",
     "eduperson_unique_id": "eduperson_unique_id",
 }
 
 DATA = {}
-TEST_INSTANCE = Loader(CONFIG, PerunAttributes.__name__).create_mocked_instance()
-TEST_INSTANCE_ERROR = Loader(
-    CONFIG_ERROR, PerunAttributes.__name__
-).create_mocked_instance()
+TEST_INSTANCE = Loader(CONFIG, Attributes.__name__).create_mocked_instance(
+    perun_micro_service=True
+)
+TEST_INSTANCE_ERROR = Loader(CONFIG_ERROR, Attributes.__name__).create_mocked_instance(
+    perun_micro_service=True
+)
 
 
 @patch("perun.connector.adapters.AdaptersManager.AdaptersManager.get_user_attributes")
 def test_process_attrs(mock_request):
     user_attrs = {
         "eduperson_unique_id": "unique_id",
         "eduperson_principal_name": "principal_name",
@@ -71,15 +73,15 @@
         "uid": [1],
         "attr": [1, 2],
         "attr2": {"1": 1},
     }
 
     AdaptersManager.get_user_attributes = MagicMock(return_value=user_attrs)
 
-    result = TEST_INSTANCE._PerunAttributes__process_attrs(None, None)
+    result = TEST_INSTANCE._Attributes__process_attrs(None, None)
     assert result == expected_result
 
 
 @patch("perun.connector.adapters.AdaptersManager.AdaptersManager.get_user_attributes")
 def test_process_attrs_error(mock_request):
     user_attrs = {
         "random_attr": 1.1,
@@ -93,26 +95,26 @@
         "PerunAttributes" + "- Unsupported attribute type. "
         "Attribute name: "
         + "random_attr"
         + ", Supported types: null, string, int, dict, list."
     )
 
     with pytest.raises(SATOSAError) as error:
-        TEST_INSTANCE._PerunAttributes__process_attrs(None, None)
+        TEST_INSTANCE._Attributes__process_attrs(None, None)
         assert str(error.value.args[0]) == error_message
 
     AdaptersManager.get_user_attributes = MagicMock(return_value=user_attrs_2)
 
     error_message = (
         "PerunAttributes" + "- Unsupported attribute type. "
         "Attribute name: " + "random_attr" + ", Supported types: string, dict."
     )
 
     with pytest.raises(SATOSAError) as error:
-        TEST_INSTANCE_ERROR._PerunAttributes__process_attrs(None, None)
+        TEST_INSTANCE_ERROR._Attributes__process_attrs(None, None)
         assert str(error.value.args[0]) == error_message
 
 
 def test_process_error():
     error_message = (
         "PerunAttributes: "
         "Missing mandatory attribute "
```

### Comparing `satosacontrib.perun-1.4.0/tests/test_perun_ensure_member.py` & `satosacontrib.perun-2.0.0/tests/test_perun_ensure_member.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import pytest
 
 from perun.connector.adapters.AdaptersManager import AdaptersManager
 from tests.test_microservice_loader import Loader, TestData, TestContext
 from satosa.exception import SATOSAError
-from satosacontrib.perun.micro_services.perun_ensure_member import (
-    PerunEnsureMember,
+from satosacontrib.perun.micro_services.idm.ensure_member import (
+    EnsureMember,
 )
 from perun.connector.models.MemberStatusEnum import MemberStatusEnum
 from perun.connector.models.User import User
 from perun.connector.models.Group import Group
 from perun.connector.models.VO import VO
 from satosa.micro_services.base import ResponseMicroService
 from unittest.mock import patch, MagicMock
@@ -31,372 +31,348 @@
     "eduperson_targeted_id": "eduperson_targeted_id",
     "eduperson_principal_name": "eduperson_principal_name",
     "eduperson_unique_id": "eduperson_unique_id",
 }
 
 DATA = {}
 
-TEST_INSTANCE = Loader(CONFIG, PerunEnsureMember.__name__).create_mocked_instance()
+TEST_INSTANCE = Loader(CONFIG, EnsureMember.__name__).create_mocked_instance(
+    perun_micro_service=True
+)
 TEST_VO = VO(1, "test_vo", "vo")
 TEST_GROUP = Group(1, TEST_VO, "uuid", "test_group", "group", "")
 TEST_USER = User(1, "Joe Doe")
 TEST_CONTEXT = TestContext()
 TEST_DATA = TestData(DATA, ATTRIBUTES)
 
 
 @patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember._PerunEnsureMember__is_user_in_group"
+    "satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember._EnsureMember__is_user_in_group"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_member_status_by_user_and_vo"
 )
 def test_handle_user_valid_in_group(mock_request_1, mock_request_2, caplog):
-    PerunEnsureMember._PerunEnsureMember__is_user_in_group = MagicMock(
-        return_value=True
-    )
+    EnsureMember._EnsureMember__is_user_in_group = MagicMock(return_value=True)
     AdaptersManager.get_member_status_by_user_and_vo = MagicMock(
         return_value=MemberStatusEnum.VALID
     )
 
-    message = "perun:PerunEnsureMember: User is allowed to continue."
+    message = "perun:EnsureMember: User is allowed to continue."
 
     with caplog.at_level(logging.DEBUG):
-        result = TEST_INSTANCE._PerunEnsureMember__handle_user(
+        result = TEST_INSTANCE._EnsureMember__handle_user(
             TEST_USER, TEST_VO, TEST_DATA, TEST_CONTEXT
         )
         assert message in caplog.text
         assert not result
 
 
 @patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember._PerunEnsureMember__is_user_in_group"
+    "satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember._EnsureMember__is_user_in_group"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_member_status_by_user_and_vo"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_member_status_by_user_and_vo"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.has_registration_form_vo"
 )
 @patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember._PerunEnsureMember__group_has_registration_form"
-)
-@patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember.register"
+    "satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember._EnsureMember__group_has_registration_form"
 )
+@patch("satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember.register")
 def test_handle_user_not_in_group_has_registration_form(
     mock_request_1,
     mock_request_2,
     mock_request_3,
     mock_request_4,
     mock_request_5,
     mock_request_6,
     caplog,
 ):
-    PerunEnsureMember._PerunEnsureMember__is_user_in_group = MagicMock(
-        return_value=False
-    )
+    EnsureMember._EnsureMember__is_user_in_group = MagicMock(return_value=False)
     AdaptersManager.get_member_status_by_user_and_vo = MagicMock(return_value=None)
     AdaptersManager.get_member_status_by_user_and_vo = MagicMock(
         return_value=MemberStatusEnum.VALID
     )
     AdaptersManager.has_registration_form_vo = MagicMock(return_value=True)
-    TEST_INSTANCE._PerunEnsureMember__group_has_registration_form = MagicMock(
+    TEST_INSTANCE._EnsureMember__group_has_registration_form = MagicMock(
         return_value=True
     )
-    PerunEnsureMember.register = MagicMock(return_value=None)
+    EnsureMember.register = MagicMock(return_value=None)
 
     message = (
-        "perun:PerunEnsureMember: User is not valid in group "
+        "perun:EnsureMember: User is not valid in group "
         "group_name - sending to registration."
     )
     with caplog.at_level(logging.DEBUG):
-        result = TEST_INSTANCE._PerunEnsureMember__handle_user(
+        result = TEST_INSTANCE._EnsureMember__handle_user(
             TEST_USER, TEST_VO, TEST_DATA, TEST_CONTEXT
         )
         assert message in caplog.text
         assert not result
-        PerunEnsureMember.register.assert_called()
+        EnsureMember.register.assert_called()
 
 
 @patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember._PerunEnsureMember__is_user_in_group"
+    "satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember._EnsureMember__is_user_in_group"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_member_status_by_user_and_vo"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_member_status_by_user_and_vo"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.has_registration_form_vo"
 )
 @patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember._PerunEnsureMember__group_has_registration_form"
-)
-@patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember.register"
+    "satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember._EnsureMember__group_has_registration_form"
 )
+@patch("satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember.register")
 def test_handle_user_in_group_vo_has_registration_form(
     mock_request_1,
     mock_request_2,
     mock_request_3,
     mock_request_4,
     mock_request_5,
     mock_request_6,
     caplog,
 ):
-    PerunEnsureMember._PerunEnsureMember__is_user_in_group = MagicMock(
-        return_value=True
-    )
+    EnsureMember._EnsureMember__is_user_in_group = MagicMock(return_value=True)
     AdaptersManager.get_member_status_by_user_and_vo = MagicMock(return_value=None)
     AdaptersManager.get_member_status_by_user_and_vo = MagicMock(return_value=None)
     AdaptersManager.has_registration_form_vo = MagicMock(return_value=True)
-    TEST_INSTANCE._PerunEnsureMember__group_has_registration_form = MagicMock(
+    TEST_INSTANCE._EnsureMember__group_has_registration_form = MagicMock(
         return_value=None
     )
-    PerunEnsureMember.register = MagicMock(return_value=None)
+    EnsureMember.register = MagicMock(return_value=None)
 
     message = (
-        "perun:PerunEnsureMember: User is not member of vo "
+        "perun:EnsureMember: User is not member of vo "
         "vo_short_name - sending to registration."
     )
     with caplog.at_level(logging.DEBUG):
-        result = TEST_INSTANCE._PerunEnsureMember__handle_user(
+        result = TEST_INSTANCE._EnsureMember__handle_user(
             TEST_USER, TEST_VO, TEST_DATA, TEST_CONTEXT
         )
         assert message in caplog.text
         assert not result
-        PerunEnsureMember.register.assert_called()
+        EnsureMember.register.assert_called()
 
 
 @patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember._PerunEnsureMember__is_user_in_group"
+    "satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember._EnsureMember__is_user_in_group"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_member_status_by_user_and_vo"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_member_status_by_user_and_vo"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.has_registration_form_vo"
 )
 @patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember._PerunEnsureMember__group_has_registration_form"
-)
-@patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember.register"
+    "satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember._EnsureMember__group_has_registration_form"
 )
+@patch("satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember.register")
 def test_handle_user_vo_and_group_have_registratiion_form(
     mock_request_1,
     mock_request_2,
     mock_request_3,
     mock_request_4,
     mock_request_5,
     mock_request_6,
     caplog,
 ):
-    PerunEnsureMember._PerunEnsureMember__is_user_in_group = MagicMock(
-        return_value=False
-    )
+    EnsureMember._EnsureMember__is_user_in_group = MagicMock(return_value=False)
     AdaptersManager.get_member_status_by_user_and_vo = MagicMock(return_value=None)
     AdaptersManager.get_member_status_by_user_and_vo = MagicMock(return_value=None)
     AdaptersManager.has_registration_form_vo = MagicMock(return_value=True)
-    TEST_INSTANCE._PerunEnsureMember__group_has_registration_form = MagicMock(
+    TEST_INSTANCE._EnsureMember__group_has_registration_form = MagicMock(
         return_value=True
     )
-    PerunEnsureMember.register = MagicMock(return_value=None)
+    EnsureMember.register = MagicMock(return_value=None)
 
     message = (
-        "perun:PerunEnsureMember: User is not member of vo "
+        "perun:EnsureMember: User is not member of vo "
         + "vo_short_name and is not in group group_name - sending "
         "to registration."
     )
 
     with caplog.at_level(logging.DEBUG):
-        result = TEST_INSTANCE._PerunEnsureMember__handle_user(
+        result = TEST_INSTANCE._EnsureMember__handle_user(
             TEST_USER, TEST_VO, TEST_DATA, TEST_CONTEXT
         )
         assert message in caplog.text
         assert not result
-        PerunEnsureMember.register.assert_called()
+        EnsureMember.register.assert_called()
 
 
 @patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember._PerunEnsureMember__is_user_in_group"
+    "satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember._EnsureMember__is_user_in_group"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_member_status_by_user_and_vo"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_member_status_by_user_and_vo"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.has_registration_form_vo"
 )
 @patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember._PerunEnsureMember__group_has_registration_form"
-)
-@patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember.register"
+    "satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember._EnsureMember__group_has_registration_form"
 )
+@patch("satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember.register")
 def test_handle_user_expired_user(
     mock_request_1,
     mock_request_2,
     mock_request_3,
     mock_request_4,
     mock_request_5,
     mock_request_6,
     caplog,
 ):
-    PerunEnsureMember._PerunEnsureMember__is_user_in_group = MagicMock(
-        return_value=True
-    )
+    EnsureMember._EnsureMember__is_user_in_group = MagicMock(return_value=True)
     AdaptersManager.get_member_status_by_user_and_vo = MagicMock(return_value=None)
     AdaptersManager.get_member_status_by_user_and_vo = MagicMock(
         return_value=MemberStatusEnum.EXPIRED
     )
     AdaptersManager.has_registration_form_by_vo = MagicMock(return_value=True)
-    TEST_INSTANCE._PerunEnsureMember__group_has_registration_form = MagicMock(
+    TEST_INSTANCE._EnsureMember__group_has_registration_form = MagicMock(
         return_value=None
     )
-    PerunEnsureMember.register = MagicMock(return_value=None)
+    EnsureMember.register = MagicMock(return_value=None)
 
-    message = "perun:PerunEnsureMember: User is expired " "- sending to registration."
+    message = "perun:EnsureMember: User is expired " "- sending to registration."
 
     with caplog.at_level(logging.DEBUG):
-        result = TEST_INSTANCE._PerunEnsureMember__handle_user(
+        result = TEST_INSTANCE._EnsureMember__handle_user(
             TEST_USER, TEST_VO, TEST_DATA, TEST_CONTEXT
         )
         assert message in caplog.text
         assert not result
-        PerunEnsureMember.register.assert_called()
+        EnsureMember.register.assert_called()
 
 
 @patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember._PerunEnsureMember__is_user_in_group"
+    "satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember._EnsureMember__is_user_in_group"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_member_status_by_user_and_vo"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_member_status_by_user_and_vo"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.has_registration_form_vo"
 )
 @patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember._PerunEnsureMember__group_has_registration_form"
-)
-@patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember.register"
+    "satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember._EnsureMember__group_has_registration_form"
 )
+@patch("satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember.register")
 def test_handle_user_expired_not_in_group(
     mock_request_1,
     mock_request_2,
     mock_request_3,
     mock_request_4,
     mock_request_5,
     mock_request_6,
     caplog,
 ):
-    PerunEnsureMember._PerunEnsureMember__is_user_in_group = MagicMock(
-        return_value=False
-    )
+    EnsureMember._EnsureMember__is_user_in_group = MagicMock(return_value=False)
     AdaptersManager.get_member_status_by_user_and_vo = MagicMock(return_value=None)
     AdaptersManager.get_member_status_by_user_and_vo = MagicMock(
         return_value=MemberStatusEnum.EXPIRED
     )
     AdaptersManager.has_registration_form_by_vo = MagicMock(return_value=True)
-    TEST_INSTANCE._PerunEnsureMember__group_has_registration_form = MagicMock(
+    TEST_INSTANCE._EnsureMember__group_has_registration_form = MagicMock(
         return_value=True
     )
-    PerunEnsureMember.register = MagicMock(return_value=None)
+    EnsureMember.register = MagicMock(return_value=None)
 
     message = (
-        "perun:PerunEnsureMember: User is expired and not in group "
+        "perun:EnsureMember: User is expired and not in group "
         "group_name - sending to registration."
     )
 
     with caplog.at_level(logging.DEBUG):
-        result = TEST_INSTANCE._PerunEnsureMember__handle_user(
+        result = TEST_INSTANCE._EnsureMember__handle_user(
             TEST_USER, TEST_VO, TEST_DATA, TEST_CONTEXT
         )
         assert message in caplog.text
         assert not result
-        PerunEnsureMember.register.assert_called()
+        EnsureMember.register.assert_called()
 
 
 @patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember._PerunEnsureMember__is_user_in_group"
+    "satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember._EnsureMember__is_user_in_group"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_member_status_by_user_and_vo"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_member_status_by_user_and_vo"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.has_registration_form_vo"
 )
 @patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember._PerunEnsureMember__group_has_registration_form"
-)
-@patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember.unauthorized"
+    "satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember._EnsureMember__group_has_registration_form"
 )
+@patch("satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember.unauthorized")
 def test_handle_user_unauthorized(
     mock_request_1,
     mock_request_2,
     mock_request_3,
     mock_request_4,
     mock_request_5,
     mock_request_6,
     caplog,
 ):
-    PerunEnsureMember._PerunEnsureMember__is_user_in_group = MagicMock(
-        return_value=False
-    )
+    EnsureMember._EnsureMember__is_user_in_group = MagicMock(return_value=False)
     AdaptersManager.get_member_status_by_user_and_vo = MagicMock(
         return_value=MemberStatusEnum.INVALID
     )
     AdaptersManager.get_member_status_by_user_and_vo = MagicMock(
         return_value=MemberStatusEnum.INVALID
     )
     AdaptersManager.has_registration_form_vo = MagicMock(return_value=False)
-    TEST_INSTANCE._PerunEnsureMember__group_has_registration_form = MagicMock(
+    TEST_INSTANCE._EnsureMember__group_has_registration_form = MagicMock(
         return_value=False
     )
-    PerunEnsureMember.unauthorized = MagicMock(return_value=None)
+    EnsureMember.unauthorized = MagicMock(return_value=None)
 
     message = (
-        "perun:PerunEnsureMember: User is not valid in vo/group and "
+        "perun:EnsureMember: User is not valid in vo/group and "
         "cannot be sent to the registration - sending to unauthorized"
     )
 
     with caplog.at_level(logging.DEBUG):
-        result = TEST_INSTANCE._PerunEnsureMember__handle_user(
+        result = TEST_INSTANCE._EnsureMember__handle_user(
             TEST_USER, TEST_VO, TEST_DATA, TEST_CONTEXT
         )
         assert message in caplog.text
         assert not result
-        PerunEnsureMember.unauthorized.assert_called()
+        EnsureMember.unauthorized.assert_called()
 
 
 @patch("perun.connector.adapters.AdaptersManager.AdaptersManager.get_vo")
 def test_process_error(mock_request):
     data_wrong = {"example_user_id": None}
 
     data_correct = {"example_user_id": 1}
 
     expected_error_message = (
-        "perun:PerunEnsureMember: "
+        "perun:EnsureMember: "
         + "Missing mandatory attribute "
         + "'example_user_id' "
         + "in data.attributes. Hint: Did you "
         + "configured PerunUser microservice "
         + "before this microservice?"
     )
 
@@ -404,33 +380,33 @@
         _ = TEST_INSTANCE.process(TEST_CONTEXT, TestData(DATA, data_wrong))
 
     assert str(error.value.args[0]) == expected_error_message
 
     AdaptersManager.get_vo = MagicMock(return_value=None)
 
     expected_error_message = (
-        "perun:PerunEnsureMember: VO with" " vo_short_name 'vo_short_name' not found."
+        "perun:EnsureMember: VO with" " vo_short_name 'vo_short_name' not found."
     )
 
     with pytest.raises(SATOSAError) as error:
         _ = TEST_INSTANCE.process(TEST_CONTEXT, TestData(DATA, data_correct))
 
     assert str(error.value.args[0]) == expected_error_message
 
 
 @patch("perun.connector.adapters.AdaptersManager.AdaptersManager.get_vo")
 @patch(
-    "satosacontrib.perun.micro_services.perun_ensure_member.PerunEnsureMember._PerunEnsureMember__handle_user"
+    "satosacontrib.perun.micro_services.idm.ensure_member.EnsureMember._EnsureMember__handle_user"
 )
 @patch("satosa.micro_services.base.ResponseMicroService.process")
 def test_process(mock_request_1, mock_request_2, mock_request_3):
     data = {"example_user_id": 1}
 
     AdaptersManager.get_vo = MagicMock(return_value="not None")
 
-    PerunEnsureMember._PerunEnsureMember__handle_user = MagicMock(return_value=None)
+    EnsureMember._EnsureMember__handle_user = MagicMock(return_value=None)
 
     ResponseMicroService.process = MagicMock(return_value=None)
 
     _ = TEST_INSTANCE.process(TEST_CONTEXT, TestData(DATA, data))
-    PerunEnsureMember._PerunEnsureMember__handle_user.assert_called()
+    EnsureMember._EnsureMember__handle_user.assert_called()
     ResponseMicroService.process.assert_called()
```

### Comparing `satosacontrib.perun-1.4.0/tests/test_perun_entitlement.py` & `satosacontrib.perun-2.0.0/tests/test_perun_entitlement.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from perun.connector.adapters.AdaptersManager import AdaptersManager
 from perun.connector.models.User import User
 from perun.connector.models.Group import Group
 from perun.connector.models.VO import VO
 from tests.test_microservice_loader import Loader, TestContext, TestData
-from satosacontrib.perun.micro_services.perun_entitlement import (
-    PerunEntitlement,
+from satosacontrib.perun.micro_services.idm.entitlement import (
+    Entitlement,
 )
 from unittest.mock import patch, MagicMock
 
 import pytest
 
 
 TEST_VO = VO(1, "vo", "vo_short_name")
@@ -76,44 +76,44 @@
         "entity_id_2": {"group1": "mapped_group1"},
         "entity_id_3": {"default_group": "default_group_mapped"},
     },
     "entitlement_prefix": "prefix:",
     "entitlement_authority": None,
 }
 
-TEST_INSTANCE = Loader(CONFIG, PerunEntitlement.__name__).create_mocked_instance()
+TEST_INSTANCE = Loader(CONFIG, Entitlement.__name__).create_mocked_instance(
+    perun_micro_service=True
+)
 TEST_INSTANCE_WITHOUT_PREFIX = Loader(
-    CONFIG_2, PerunEntitlement.__name__
-).create_mocked_instance()
+    CONFIG_2, Entitlement.__name__
+).create_mocked_instance(perun_micro_service=True)
 TEST_INSTANCE_WITHOUT_AUTHORITY = Loader(
-    CONFIG_3, PerunEntitlement.__name__
-).create_mocked_instance()
+    CONFIG_3, Entitlement.__name__
+).create_mocked_instance(perun_micro_service=True)
 
 
 def test_map_group_name():
     group_name_1 = "group1"
     group_name_2 = "group2"
     not_existing_group = "group420"
 
     result_1 = "mapped_group1"
     result_2 = "mapped_group2"
     result_3 = "prefix:group:group420"
 
     assert (
-        TEST_INSTANCE._PerunEntitlement__map_group_name(group_name_1, "entity_id_1")
+        TEST_INSTANCE._Entitlement__map_group_name(group_name_1, "entity_id_1")
         == result_1
     )
     assert (
-        TEST_INSTANCE._PerunEntitlement__map_group_name(group_name_2, "entity_id_1")
+        TEST_INSTANCE._Entitlement__map_group_name(group_name_2, "entity_id_1")
         == result_2
     )
     assert (
-        TEST_INSTANCE._PerunEntitlement__map_group_name(
-            not_existing_group, "entity_id_1"
-        )
+        TEST_INSTANCE._Entitlement__map_group_name(not_existing_group, "entity_id_1")
         == result_3
     )
 
 
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_resource_capabilities_by_rp_id"
 )
@@ -134,36 +134,36 @@
     result = [
         "prefix:fac_cap_2#authority",
         "prefix:fac_cap_1#authority",
         "prefix:res_cap_1#authority",
         "prefix:res_cap_2#authority",
     ]
 
-    for capability in TEST_INSTANCE._PerunEntitlement__get_capabilities(
+    for capability in TEST_INSTANCE._Entitlement__get_capabilities(
         TestData(DATA, None)
     ):
         assert capability in result
 
 
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_resource_capabilities_by_rp_id"
 )
 def test_get_capabilities_exception(mock_request_1):
     AdaptersManager.get_resource_capabilities_by_rp_id = MagicMock(
         side_effect=[Exception("sth went wrong")]
     )
 
-    assert TEST_INSTANCE._PerunEntitlement__get_capabilities(TestData(DATA, None)) == []
+    assert TEST_INSTANCE._Entitlement__get_capabilities(TestData(DATA, None)) == []
 
 
 def test_get_forwarded_edu_person_entitlement_user_missing():
     attrs = {"example_user_id": "example_user_id"}
 
     test_data = TestData(data=DATA_WITHOUT_USER, attributes=attrs)
-    assert not TEST_INSTANCE._PerunEntitlement__get_forwarded_edu_person_entitlement(
+    assert not TEST_INSTANCE._Entitlement__get_forwarded_edu_person_entitlement(
         test_data
     )
 
 
 @patch("perun.connector.adapters.AdaptersManager.AdaptersManager.get_user_attributes")
 def test_get_forwarded_edu_person_entitlement(mock_request):
     ext_src_attrs = {"attr1": "this_is_entitlement", "attr2": "attr2", "attr3": "attr3"}
@@ -172,58 +172,58 @@
 
     test_data = TestData(data=DATA, attributes=attrs)
 
     result = ["this_is_entitlement"]
     AdaptersManager.get_user_attributes = MagicMock(return_value=ext_src_attrs)
 
     assert (
-        TEST_INSTANCE._PerunEntitlement__get_forwarded_edu_person_entitlement(test_data)
+        TEST_INSTANCE._Entitlement__get_forwarded_edu_person_entitlement(test_data)
         == result
     )
 
 
 def test_get_edu_person_entitlement_extended():
     expected_result = [
         "prefix:groupuuid#authority",
         "prefix:groupAttributes:uuid?=displayName=group1#authority",  # noqa
         "prefix:groupuuid#authority",
         "prefix:groupAttributes:uuid?=displayName=group2#authority",
     ]  # noqa
 
-    result = TEST_INSTANCE._PerunEntitlement__get_edu_person_entitlement_extended(
+    result = TEST_INSTANCE._Entitlement__get_edu_person_entitlement_extended(
         TestData(DATA, None)
     )  # noqa
 
     assert expected_result == result
 
 
 def test_get_edu_person_entitlement():
     expected_result = ["prefix:group:group1#authority", "prefix:group:group2#authority"]
 
-    result = TEST_INSTANCE._PerunEntitlement__get_edu_person_entitlement(
+    result = TEST_INSTANCE._Entitlement__get_edu_person_entitlement(
         TestData(DATA, None)
     )  # noqa
 
     assert expected_result == result
 
 
 def test_get_edu_person_entitlement_exception():
     expected_error_message = (
-        "perun:PerunEntitlement: missing "
+        "perun:Entitlement: missing "
         "mandatory configuration options "
         "'groupNameAuthority' "
         "or 'groupNamePrefix'."
     )
 
     with pytest.raises(Exception) as error:
-        _ = TEST_INSTANCE_WITHOUT_PREFIX._PerunEntitlement__get_edu_person_entitlement(
+        _ = TEST_INSTANCE_WITHOUT_PREFIX._Entitlement__get_edu_person_entitlement(
             TestData(DATA, None)
         )
 
     assert str(error.value.args[0]) == expected_error_message
 
     with pytest.raises(Exception) as error:
-        _ = TEST_INSTANCE_WITHOUT_AUTHORITY._PerunEntitlement__get_edu_person_entitlement(
+        _ = TEST_INSTANCE_WITHOUT_AUTHORITY._Entitlement__get_edu_person_entitlement(
             TestData(DATA, None)
         )
 
     assert str(error.value.args[0]) == expected_error_message
```

### Comparing `satosacontrib.perun-1.4.0/tests/test_perun_user_microservice.py` & `satosacontrib.perun-2.0.0/tests/test_perun_user_microservice.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 import copy
+import logging
 from unittest.mock import patch, MagicMock
 
 import pytest
 from perun.connector import User
 from perun.connector.adapters.AdaptersManager import (
     AdaptersManager,
     AdaptersManagerNotExistsException,
 )
-from satosa.context import Context
 from satosa.exception import SATOSAError
 from satosa.internal import InternalData
 from satosa.micro_services.base import MicroService
 
-from satosacontrib.perun.micro_services.perun_user_microservice import PerunUser  # noqa
+from satosacontrib.perun.micro_services.idm.perun_user import (
+    PerunUser,
+)  # noqa
 from satosacontrib.perun.utils.Utils import Utils
 from tests.test_microservice_loader import Loader
+from tests.test_microservice_loader import TestContext
 
 MICROSERVICE_CONFIG = {
     "global_cfg_filepath": "example_path",
     "internal_login_attribute": "example_internal_login",
     "internal_extsource_attribute": "example_internal_extsource",
     "proxy_extsource_name": "example_extsource_name",
-    "allowed_requesters": ["allowed_req_1", "allowed_req_2"],
     "registration_page_url": "example_url",
     "registration_result_url": "example_url",
 }
 
-MICROSERVICE = Loader(MICROSERVICE_CONFIG, "PerunUser").create_mocked_instance()
+MICROSERVICE = Loader(MICROSERVICE_CONFIG, "PerunUser").create_mocked_instance(
+    perun_micro_service=True
+)
 
 
-def test_process_requester_not_allowed():
+@patch("satosa.context.Context.get_decoration")
+def test_process_requester_not_allowed(mock_method, caplog):
+    mock_method.return_value = "target_entity_id2"
     data_with_disallowed_requester = InternalData()
-    data_with_disallowed_requester.requester = "not_allowed_req"
-    disallowed_requester_error_message = "Data request not allowed."
-
-    with pytest.raises(SATOSAError) as error:
-        MICROSERVICE.process(Context(), data_with_disallowed_requester)
-
-        assert str(error.value.args[0]) == disallowed_requester_error_message
+    data_with_disallowed_requester.requester = "forbidden_requester"
+    disallowed_requester_log = "Requester 'forbidden_requester' is not allowed for 'target_entity_id2' due to deny rules"
+    MicroService.process = MagicMock(return_value=None)
+    with caplog.at_level(logging.DEBUG):
+        MICROSERVICE.process(TestContext(), data_with_disallowed_requester)
+        assert disallowed_requester_log in caplog.text
+        MicroService.process.assert_called()
 
 
 @patch("perun.connector.adapters.AdaptersManager.AdaptersManager.get_perun_user")
 @patch(
-    "satosacontrib.perun.micro_services.perun_user_microservice.PerunUser.handle_user_not_found"  # noqa
+    "satosacontrib.perun.micro_services.idm.perun_user.PerunUser.handle_user_not_found"  # noqa
 )
 def test_process_user_not_found(mock_request_1, mock_request_2):
     data_with_non_existent_user = InternalData()
     data_with_non_existent_user.requester = "allowed_req_1"
     data_with_non_existent_user.auth_info.issuer = "example_non_existent_name"
     data_with_non_existent_user.attributes["example_internal_login"] = []
 
@@ -54,15 +60,15 @@
         side_effect=AdaptersManagerNotExistsException(
             '"name":"UserExtSourceNotExistsException"'
         )
     )
     expected_error_message = '"name":"UserExtSourceNotExistsException"'
     PerunUser.handle_user_not_found = MagicMock(return_value=None)
     with pytest.raises(Exception) as error:
-        MICROSERVICE.process(Context(), data_with_non_existent_user)
+        MICROSERVICE.process(TestContext(), data_with_non_existent_user)
         assert str(error.value.args[0]) == expected_error_message
         PerunUser.handle_user_not_found.assert_called()
 
 
 @patch("perun.connector.adapters.AdaptersManager.AdaptersManager.get_perun_user")
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_user_attributes"  # noqa
@@ -77,58 +83,56 @@
 
     AdaptersManager.get_perun_user = MagicMock(return_value=example_user)
     AdaptersManager.get_user_attributes = MagicMock(
         return_value={"perun_login_attribute": "example_login"}
     )
     MicroService.process = MagicMock(return_value=None)
 
-    MICROSERVICE.process(Context(), data_with_existing_user)
+    MICROSERVICE.process(TestContext(), data_with_existing_user)
 
     MicroService.process.assert_called()
 
 
 def test_handle_user_not_found_missing_registration_link():
     config_without_registration_link = copy.deepcopy(MICROSERVICE_CONFIG)
     config_without_registration_link.pop("registration_page_url")
     microservice = Loader(
         config_without_registration_link, "PerunUser"
-    ).create_mocked_instance()
+    ).create_mocked_instance(perun_micro_service=True)
 
     user_name = "example_name"
     user_logins = ["example_login_1", "example_login_2"]
     missing_registration_link_error_message = (
         f"User with name {user_name} and idp IDs {user_logins} was not found"
         " in Perun. And redirect link to registration page is missing in the"
         " config file."
     )
 
     with pytest.raises(SATOSAError) as error:
         microservice.handle_user_not_found(
-            user_name, user_logins, Context(), InternalData()
+            user_name, user_logins, TestContext(), InternalData()
         )
 
         assert str(error.value.args[0]) == missing_registration_link_error_message
 
 
 @patch("satosacontrib.perun.utils.Utils.Utils.secure_redirect_with_nonce")
 def test_handle_user_not_found_successful_redirect(mock_request_1):
     Utils.secure_redirect_with_nonce = MagicMock(return_value=None)
     MICROSERVICE.handle_user_not_found(None, None, None, None)
 
     Utils.secure_redirect_with_nonce.assert_called()
 
 
 @patch("satosacontrib.perun.utils.Utils.Utils.handle_registration_response")
-@patch(
-    "satosacontrib.perun.micro_services.perun_user_microservice.PerunUser.process"  # noqa
-)
+@patch("satosacontrib.perun.micro_services.idm.perun_user.PerunUser.process")  # noqa
 def test_handle_registration_response(mock_request_1, mock_request_2):
     expected_result = "process result"
     Utils.handle_registration_response = MagicMock(
-        return_value=(Context(), InternalData())
+        return_value=(TestContext(), InternalData())
     )
     PerunUser.process = MagicMock(return_value=expected_result)
 
     result = MICROSERVICE._PerunUser__handle_registration_response(None)
 
     Utils.handle_registration_response.assert_called()
     PerunUser.process.assert_called()
```

### Comparing `satosacontrib.perun-1.4.0/tests/test_sp_authorization_microservice.py` & `satosacontrib.perun-2.0.0/tests/test_sp_authorization_microservice.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 from perun.connector.adapters.AdaptersManager import AdaptersManager
 from satosa.context import Context
 from satosa.exception import SATOSAError
 from satosa.internal import InternalData
 from satosa.micro_services.base import MicroService
 from satosa.response import Redirect
 
-from satosacontrib.perun.micro_services.sp_authorization_microservice import (
+from satosacontrib.perun.micro_services.idm.sp_authorization import (
     SpAuthorization,
 )
 from satosacontrib.perun.utils.PerunConstants import PerunConstants
 from satosacontrib.perun.utils.Utils import Utils
-from tests.test_microservice_loader import Loader
+from tests.test_microservice_loader import Loader, TestContext
 
 MICROSERVICE_CONFIG = {
     "global_cfg_filepath": "example_path",
     "filter_config": {
         "check_group_membership_attr": "example_attr",
         "vo_short_names_attr": "example_attr",
         "allow_registration_attr": "example_attr",
@@ -35,15 +35,15 @@
     "notification_url": "example_url",
     "registration_result_url": "example_url",
 }
 
 
 MICROSERVICE = Loader(
     MICROSERVICE_CONFIG, SpAuthorization.__name__
-).create_mocked_instance()
+).create_mocked_instance(perun_micro_service=True)
 
 DEBUG_PREFIX = MICROSERVICE._SpAuthorization__DEBUG_PREFIX
 REGISTRAR_URL = MICROSERVICE._SpAuthorization__REGISTRAR_URL
 REGISTRATION_LINK_ATTR = MICROSERVICE._SpAuthorization__REGISTRATION_LINK_ATTR
 
 
 def test_initial_misconfiguration():
@@ -57,33 +57,35 @@
         " nor registration_link_attr have been configured. Use option"
         f" '{REGISTRAR_URL}' to configure the registrar location or/and option"
         f" '{REGISTRATION_LINK_ATTR}' to configure attribute for Service"
         " defined registration link."
     )
 
     with pytest.raises(SATOSAError) as error:
-        _ = Loader(bad_config, SpAuthorization.__name__).create_mocked_instance()
+        _ = Loader(bad_config, SpAuthorization.__name__).create_mocked_instance(
+            perun_micro_service=True
+        )
         assert str(error.value.args[0]) == misconfiguration_error_message
 
 
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization.unauthorized"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization.unauthorized"  # noqa
 )
 def test_process_no_user_in_request(mock_request_1, caplog):
     no_user_error_message = (
         "Request does not contain Perun user. Did you configure PerunUser"
         " microservice?"
     )
     data_without_user = InternalData()
     data_without_user.attributes["example_user_id"] = None
 
     SpAuthorization.unauthorized = MagicMock(return_value=None)
 
     with caplog.at_level(logging.DEBUG):
-        MICROSERVICE.process(None, data_without_user)
+        MICROSERVICE.process(TestContext(), data_without_user)
         assert no_user_error_message in caplog.text
         SpAuthorization.unauthorized.assert_called()
 
 
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_facility_by_rp_identifier"  # noqa
 )
@@ -96,27 +98,27 @@
     data_with_non_existent_sp_id = InternalData()
     data_with_non_existent_sp_id.requester = non_existent_sp_id
     data_with_non_existent_sp_id.attributes["example_user_id"] = "example user"
 
     AdaptersManager.get_facility_by_rp_identifier = MagicMock(return_value=None)
 
     with caplog.at_level(logging.DEBUG):
-        result = MICROSERVICE.process(None, data_with_non_existent_sp_id)
+        result = MICROSERVICE.process(TestContext(), data_with_non_existent_sp_id)
         assert no_facility_error_message in caplog.text
         assert result is None
 
 
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_facility_by_rp_identifier"  # noqa
 )
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization._SpAuthorization__get_sp_attributes"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization._SpAuthorization__get_sp_attributes"  # noqa
 )
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization.unauthorized"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization.unauthorized"  # noqa
 )
 def test_process_no_attrs_in_facility(
     mock_request_1, mock_request_2, mock_request_3, caplog
 ):
     no_facility_attrs_error_message = (
         "Could not fetch SP attributes, user will be redirected to"
         " unauthorized for security reasons"
@@ -127,25 +129,25 @@
     AdaptersManager.get_facility_by_rp_identifier = MagicMock(
         return_value="example facility"
     )
     SpAuthorization._SpAuthorization__get_sp_attributes = MagicMock(return_value={})
     SpAuthorization.unauthorized = MagicMock(return_value=None)
 
     with caplog.at_level(logging.DEBUG):
-        MICROSERVICE.process(None, data_without_facility_attrs)
+        MICROSERVICE.process(TestContext(), data_without_facility_attrs)
         assert no_facility_attrs_error_message in caplog.text
         SpAuthorization.unauthorized.assert_called()
 
 
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager"
     ".get_facility_by_rp_identifier"
 )
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization"  # noqa
     "._SpAuthorization__get_sp_attributes"
 )
 def test_process_group_membership_check_not_required(
     mock_request_1, mock_request_2, caplog
 ):
     group_membership_not_required_message = (
         "Group membership check not requested by the service."
@@ -157,33 +159,35 @@
         return_value="example facility"
     )
     SpAuthorization._SpAuthorization__get_sp_attributes = MagicMock(
         return_value={"check_group_membership": False}
     )
 
     with caplog.at_level(logging.WARNING):
-        result = MICROSERVICE.process(None, data_without_group_membership_check)
+        result = MICROSERVICE.process(
+            TestContext(), data_without_group_membership_check
+        )
         assert group_membership_not_required_message in caplog.text
         assert result is None
 
 
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager"
     ".get_facility_by_rp_identifier"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager"
     ".get_users_groups_on_facility"
 )
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization"  # noqa
     "._SpAuthorization__get_sp_attributes"
 )
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization"  # noqa
     ".handle_unsatisfied_membership"
 )
 def test_process_no_users_groups_found(
     mock_request_1, mock_request_2, mock_request_3, mock_request_4
 ):
     data_user_without_groups = InternalData()
     data_user_without_groups.attributes["example_user_id"] = "example user"
@@ -193,33 +197,33 @@
     )
     SpAuthorization._SpAuthorization__get_sp_attributes = MagicMock(
         return_value={"check_group_membership": True}
     )
     AdaptersManager.get_users_groups_on_facility = MagicMock(return_value=[])
     SpAuthorization.handle_unsatisfied_membership = MagicMock(return_value=None)
 
-    result = MICROSERVICE.process(None, data_user_without_groups)
+    result = MICROSERVICE.process(TestContext(), data_user_without_groups)
     assert result is None
     SpAuthorization.handle_unsatisfied_membership.assert_called()
 
 
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager"
     ".get_facility_by_rp_identifier"
 )
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager"
     ".get_users_groups_on_facility"
 )
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization"  # noqa
     "._SpAuthorization__get_sp_attributes"
 )
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization"  # noqa
     ".handle_unsatisfied_membership"
 )
 @patch("satosa.micro_services.base.MicroService.process")
 def test_process_users_groups_found(
     mock_request_1,
     mock_request_2,
     mock_request_3,
@@ -239,15 +243,15 @@
     )
     AdaptersManager.get_users_groups_on_facility = MagicMock(
         return_value=["group1", "group2"]
     )
     MicroService.process = MagicMock(return_value=None)
 
     with caplog.at_level(logging.INFO):
-        MICROSERVICE.process(None, data_user_with_groups)
+        MICROSERVICE.process(TestContext(), data_user_with_groups)
         assert user_satisfies_check_message in caplog.text
         MicroService.process.assert_called()
 
 
 def test_unauthorized_access():
     result = MICROSERVICE.unauthorized()
     expected_header = (
@@ -256,71 +260,71 @@
     )
 
     assert isinstance(result, Redirect)
     assert expected_header in result.headers
 
 
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization.unauthorized"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization.unauthorized"  # noqa
 )
 def test_handle_unsatisfied_membership_disabled(mock_request_1, caplog):
     handling_disabled_message = (
         "Handling unsatisfied membership is disabled, redirecting to" " unauthorized"
     )
     custom_config = copy.deepcopy(MICROSERVICE_CONFIG)
     custom_config["filter_config"]["handle_unsatisfied_membership"] = False
     microservice = Loader(
         custom_config, SpAuthorization.__name__
-    ).create_mocked_instance()
+    ).create_mocked_instance(perun_micro_service=True)
 
     SpAuthorization.unauthorized = MagicMock(return_value=None)
 
     with caplog.at_level(logging.DEBUG):
         microservice.handle_unsatisfied_membership(None, None, None, None, None, None)
         assert handling_disabled_message in caplog.text
         SpAuthorization.unauthorized.assert_called()
 
 
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization.unauthorized"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization.unauthorized"  # noqa
 )
 def test_handle_unsatisfied_membership_registration_unspecified(mock_request_1, caplog):
     handling_disabled_message = (
         "Handling unsatisfied membership is disabled, redirecting to" " unauthorized"
     )
     custom_config = copy.deepcopy(MICROSERVICE_CONFIG)
     custom_config["filter_config"]["handle_unsatisfied_membership"] = False
     microservice = Loader(
         custom_config, SpAuthorization.__name__
-    ).create_mocked_instance()
+    ).create_mocked_instance(perun_micro_service=True)
 
     SpAuthorization.unauthorized = MagicMock(return_value=None)
 
     with caplog.at_level(logging.DEBUG):
         microservice.handle_unsatisfied_membership(
             None, None, None, None, None, facility_attributes={}
         )
         assert handling_disabled_message in caplog.text
         SpAuthorization.unauthorized.assert_called()
 
 
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization.unauthorized"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization.unauthorized"  # noqa
 )
 def test_handle_unsatisfied_membership_registration_disallowed(mock_request_1, caplog):
     data_requester = "example_entity_id"
     registration_disallowed_message = (
         "User is not member of any assigned groups of resources for service"
         f" ('{data_requester}'). Registration to the groups is disabled."
     )
     custom_config = copy.deepcopy(MICROSERVICE_CONFIG)
     custom_config["filter_config"]["handle_unsatisfied_membership"] = True
     microservice = Loader(
         custom_config, SpAuthorization.__name__
-    ).create_mocked_instance()
+    ).create_mocked_instance(perun_micro_service=True)
 
     SpAuthorization.unauthorized = MagicMock(return_value=None)
 
     with caplog.at_level(logging.DEBUG):
         facility_attrs = {"allow_registration": False}
         microservice.handle_unsatisfied_membership(
             context=None,
@@ -331,27 +335,27 @@
             facility_attributes=facility_attrs,
         )
         assert registration_disallowed_message in caplog.text
         SpAuthorization.unauthorized.assert_called()
 
 
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization.unauthorized"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization.unauthorized"  # noqa
 )
 def test_handle_unsatisfied_membership_registration_not_set(mock_request_1, caplog):
     data_requester = "example_entity_id"
     registration_not_set_message = (
         "User is not member of any assigned groups of resources for service"
         f" ('{data_requester}'). Registration to the groups is disabled."
     )
     custom_config = copy.deepcopy(MICROSERVICE_CONFIG)
     custom_config["filter_config"]["handle_unsatisfied_membership"] = True
     microservice = Loader(
         custom_config, SpAuthorization.__name__
-    ).create_mocked_instance()
+    ).create_mocked_instance(perun_micro_service=True)
 
     SpAuthorization.unauthorized = MagicMock(return_value=None)
 
     with caplog.at_level(logging.DEBUG):
         microservice.handle_unsatisfied_membership(
             context=None,
             data=None,
@@ -371,15 +375,15 @@
         f"Redirecting user to custom registration link '{registration_link}'"
         f" configured for service ('{data_requester}')."
     )
     custom_config = copy.deepcopy(MICROSERVICE_CONFIG)
     custom_config["filter_config"]["handle_unsatisfied_membership"] = True
     microservice = Loader(
         custom_config, SpAuthorization.__name__
-    ).create_mocked_instance()
+    ).create_mocked_instance(perun_micro_service=True)
 
     expected_header = ("Location", registration_link)
 
     with caplog.at_level(logging.DEBUG):
         facility_attrs = {
             "allow_registration": True,
             "registration_link": registration_link,
@@ -396,27 +400,27 @@
         )
         assert isinstance(result, Redirect)
         assert expected_header in result.headers
         assert registration_redirect_message in caplog.text
 
 
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization._SpAuthorization__get_registration_data"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization._SpAuthorization__get_registration_data"  # noqa
 )
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization.register"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization.register"  # noqa
 )
 def test_handle_unsatisfied_membership_has_available_groups(
     mock_request_1, mock_request_2
 ):
     custom_config = copy.deepcopy(MICROSERVICE_CONFIG)
     custom_config["filter_config"]["handle_unsatisfied_membership"] = True
     microservice = Loader(
         custom_config, SpAuthorization.__name__
-    ).create_mocked_instance()
+    ).create_mocked_instance(perun_micro_service=True)
 
     SpAuthorization._SpAuthorization__get_registration_data = MagicMock(
         return_value=["group1", "group2"]
     )
     SpAuthorization.register = MagicMock(return_value=None)
 
     facility_attrs = {"allow_registration": True}
@@ -428,32 +432,32 @@
         facility=None,
         facility_attributes=facility_attrs,
     )
     SpAuthorization.register.assert_called()
 
 
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization.unauthorized"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization.unauthorized"  # noqa
 )
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization._SpAuthorization__get_registration_data"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization._SpAuthorization__get_registration_data"  # noqa
 )
 def test_handle_unsatisfied_membership_no_available_groups(
     mock_request_1, mock_request_2, caplog
 ):
     data_requester = "example_entity_id"
     no_available_groups_message = (
         "No VO is available for registration into groups of resources for"
         f" service '{data_requester}'"
     )
     custom_config = copy.deepcopy(MICROSERVICE_CONFIG)
     custom_config["filter_config"]["handle_unsatisfied_membership"] = True
     microservice = Loader(
         custom_config, SpAuthorization.__name__
-    ).create_mocked_instance()
+    ).create_mocked_instance(perun_micro_service=True)
 
     SpAuthorization.unauthorized = MagicMock(return_value=None)
     SpAuthorization._SpAuthorization__get_registration_data = MagicMock(return_value=[])
 
     with caplog.at_level(logging.DEBUG):
         facility_attrs = {"allow_registration": True}
         microservice.handle_unsatisfied_membership(
@@ -465,32 +469,32 @@
             facility_attributes=facility_attrs,
         )
         assert no_available_groups_message in caplog.text
         SpAuthorization.unauthorized.assert_called()
 
 
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization._SpAuthorization__get_registration_data"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization._SpAuthorization__get_registration_data"  # noqa
 )
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization.unauthorized"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization.unauthorized"  # noqa
 )
 def test_handle_unsatisfied_membership_exception(
     mock_request_1, mock_request_2, caplog
 ):
     exception_occurred_message = (
         "Caught an exception, user will be redirected to unauthorized for"
         " security reasons"
     )
     exception_message = "Some error happened"
     custom_config = copy.deepcopy(MICROSERVICE_CONFIG)
     custom_config["filter_config"]["handle_unsatisfied_membership"] = True
     microservice = Loader(
         custom_config, SpAuthorization.__name__
-    ).create_mocked_instance()
+    ).create_mocked_instance(perun_micro_service=True)
 
     SpAuthorization._SpAuthorization__get_registration_data = MagicMock(
         side_effect=Exception(exception_message)
     )
     SpAuthorization.unauthorized = MagicMock(return_value=None)
 
     facility_attrs = {"allow_registration": True}
@@ -517,15 +521,15 @@
             facility_attributes=facility_attrs,
         )
         assert exception_message in caplog.text
         SpAuthorization.unauthorized.assert_called()
 
 
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization._SpAuthorization__register_directly"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization._SpAuthorization__register_directly"  # noqa
 )
 def test_register_single_option(mock_request_1, caplog):
     single_registration_message = (
         "Registration possible to only single VO and GROUP, redirecting"
         " directly to this registration."
     )
 
@@ -539,15 +543,15 @@
             skip_notification=None,
         )
         assert single_registration_message in caplog.text
         SpAuthorization._SpAuthorization__register_directly.assert_called()
 
 
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization._SpAuthorization__register_choose_vo_and_group"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization._SpAuthorization__register_choose_vo_and_group"  # noqa
 )
 def test_register_multiple_options(mock_request_1, caplog):
     multiple_options_message = (
         "Registration possible to more than a single VO and GROUP, letting"
         " user choose."
     )
 
@@ -571,15 +575,15 @@
         "Unable to register user into group: None, redirect link to"
         " registration page is missing in the config file."
     )
     custom_config = copy.deepcopy(MICROSERVICE_CONFIG)
     custom_config["single_group_registration_url"] = None
     microservice = Loader(
         custom_config, SpAuthorization.__name__
-    ).create_mocked_instance()
+    ).create_mocked_instance(perun_micro_service=True)
 
     with pytest.raises(SATOSAError) as error:
         microservice._SpAuthorization__register_directly(None, None, None, None)
         assert str(error.value.args[0]) == no_url_error_message
 
 
 def test_register_directly_no_notification_url():
@@ -588,15 +592,15 @@
         " notification page is missing in the config file."
     )
     custom_config = copy.deepcopy(MICROSERVICE_CONFIG)
     custom_config["single_group_registration_url"] = "example url"
     custom_config["notification_url"] = None
     microservice = Loader(
         custom_config, SpAuthorization.__name__
-    ).create_mocked_instance()
+    ).create_mocked_instance(perun_micro_service=True)
 
     with pytest.raises(SATOSAError) as error:
         microservice._SpAuthorization__register_directly(
             context=None,
             data=InternalData(),
             group=None,
             skip_notification=False,
@@ -611,15 +615,15 @@
         "Skipping registration notification. Redirecting directly to"
         f" '{registration_url}."
     )
     custom_config = copy.deepcopy(MICROSERVICE_CONFIG)
     custom_config["single_group_registration_url"] = registration_url
     microservice = Loader(
         custom_config, SpAuthorization.__name__
-    ).create_mocked_instance()
+    ).create_mocked_instance(perun_micro_service=True)
 
     Utils.secure_redirect_with_nonce = MagicMock(return_value=None)
 
     with caplog.at_level(logging.DEBUG):
         microservice._SpAuthorization__register_directly(
             context=None,
             data=InternalData(),
@@ -638,15 +642,15 @@
         f" '{registration_url}'."
     )
     custom_config = copy.deepcopy(MICROSERVICE_CONFIG)
     custom_config["single_group_registration_url"] = registration_url
     custom_config["notification_url"] = "example url"
     microservice = Loader(
         custom_config, SpAuthorization.__name__
-    ).create_mocked_instance()
+    ).create_mocked_instance(perun_micro_service=True)
 
     Utils.secure_redirect_with_nonce = MagicMock(return_value=None)
 
     with caplog.at_level(logging.DEBUG):
         microservice._SpAuthorization__register_directly(
             context=None,
             data=InternalData(),
@@ -654,15 +658,15 @@
             skip_notification=False,
         )
         assert sending_notification_message in caplog.text
         Utils.secure_redirect_with_nonce.assert_called()  # noqa
 
 
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization._SpAuthorization__register_choose_vo_and_group"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization._SpAuthorization__register_choose_vo_and_group"  # noqa
 )
 def test_register_choose_vo_and_group(mock_request_1):
     SpAuthorization._SpAuthorization__register_vo_and_group = MagicMock(
         return_value=None
     )
 
     MICROSERVICE._SpAuthorization__register_choose_vo_and_group(
@@ -685,18 +689,18 @@
         MICROSERVICE._SpAuthorization__get_registration_data(
             None, None, None, facility_attributes={}
         )
         assert str(error.value.args[0]) == no_resources_error_message
 
 
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization._SpAuthorization__get_registration_vo_short_names"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization._SpAuthorization__get_registration_vo_short_names"  # noqa
 )
 @patch(
-    "satosacontrib.perun.micro_services.sp_authorization_microservice.SpAuthorization._SpAuthorization__get_registration_groups"  # noqa
+    "satosacontrib.perun.micro_services.idm.sp_authorization.SpAuthorization._SpAuthorization__get_registration_groups"  # noqa
 )
 def test_get_registration_data(mock_request_1, mock_request_2):
     SpAuthorization._SpAuthorization__get_registration_vo_short_names = MagicMock(
         return_value=None
     )
     SpAuthorization._SpAuthorization__get_registration_groups = MagicMock(
         return_value=None
```

### Comparing `satosacontrib.perun-1.4.0/tests/test_update_ues.py` & `satosacontrib.perun-2.0.0/tests/test_update_ues.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import threading
 
 from perun.connector.adapters.AdaptersManager import AdaptersManager
 from perun.connector.models.User import User
 from perun.connector.models.UserExtSource import UserExtSource
-from satosacontrib.perun.micro_services.update_user_ext_source import (
+from satosacontrib.perun.micro_services.idm.update_user_ext_source import (
     UpdateUserExtSource,
 )
 from satosa.exception import SATOSAError
 from satosa.micro_services.base import ResponseMicroService
 from unittest.mock import patch, MagicMock
 from tests.test_microservice_loader import Loader, TestData, TestContext
 
@@ -46,22 +46,24 @@
     "mail": ["mail"],
     "eduperson_scoped_affiliation": ["eduperson_scoped_affiliation"],
     "eduperson_entitlement": ["eduperson_entitlement"],
 }
 
 DATA = {}
 
-TEST_INSTANCE = Loader(CONFIG, UpdateUserExtSource.__name__).create_mocked_instance()
+TEST_INSTANCE = Loader(CONFIG, UpdateUserExtSource.__name__).create_mocked_instance(
+    perun_micro_service=True
+)
 TEST_DATA = TestData(DATA, ATTRIBUTES)
 USER = User(1, "Joe Doe")
 EXT_SOURCE = UserExtSource(1, "ext_source", "login", USER)
 
 
 @patch(
-    "satosacontrib.perun.micro_services.update_user_ext_source.UpdateUserExtSource._UpdateUserExtSource__get_user_ext_source"
+    "satosacontrib.perun.micro_services.idm.update_user_ext_source.UpdateUserExtSource._UpdateUserExtSource__get_user_ext_source"
 )
 def test_find_user_ext_source(mock_request_1):
     TEST_INSTANCE._UpdateUserExtSource__find_user_ext_source = MagicMock(
         return_value=EXT_SOURCE
     )
 
     assert (
@@ -133,15 +135,15 @@
         ATTRIBUTES,
     )
 
     assert result == expected_result
 
 
 @patch(
-    "satosacontrib.perun.micro_services.update_user_ext_source.UpdateUserExtSource._UpdateUserExtSource__find_user_ext_source"
+    "satosacontrib.perun.micro_services.idm.update_user_ext_source.UpdateUserExtSource._UpdateUserExtSource__find_user_ext_source"
 )
 def test_run_error(mock_request_1):
     data_to_conversion = {
         "attributes": CONFIG["user_identifiers"],
         "attr_map": CONFIG["attr_map"],
         "attrs_to_conversion": CONFIG["array_to_string_conversion"],
         "append_only_attrs": CONFIG["append_only_attrs"],
@@ -163,24 +165,24 @@
 
     with pytest.raises(SATOSAError) as error:
         TEST_INSTANCE._UpdateUserExtSource__run(data_to_conversion)
         assert str(error.value.args[0]) == error_msg
 
 
 @patch(
-    "satosacontrib.perun.micro_services.update_user_ext_source.UpdateUserExtSource._UpdateUserExtSource__find_user_ext_source"
+    "satosacontrib.perun.micro_services.idm.update_user_ext_source.UpdateUserExtSource._UpdateUserExtSource__find_user_ext_source"
 )
 @patch(
-    "satosacontrib.perun.micro_services.update_user_ext_source.UpdateUserExtSource._UpdateUserExtSource__get_attributes_from_perun"
+    "satosacontrib.perun.micro_services.idm.update_user_ext_source.UpdateUserExtSource._UpdateUserExtSource__get_attributes_from_perun"
 )
 @patch(
-    "satosacontrib.perun.micro_services.update_user_ext_source.UpdateUserExtSource._UpdateUserExtSource__get_attributes_to_update"
+    "satosacontrib.perun.micro_services.idm.update_user_ext_source.UpdateUserExtSource._UpdateUserExtSource__get_attributes_to_update"
 )
 @patch(
-    "satosacontrib.perun.micro_services.update_user_ext_source.UpdateUserExtSource._UpdateUserExtSource__update_user_ext_source"
+    "satosacontrib.perun.micro_services.idm.update_user_ext_source.UpdateUserExtSource._UpdateUserExtSource__update_user_ext_source"
 )
 def test_run(mock_request_1, mock_request_2, mock_request_3, mock_request_4):
     data_to_conversion = {
         "attributes": CONFIG["user_identifiers"],
         "attr_map": CONFIG["attr_map"],
         "attrs_to_conversion": CONFIG["array_to_string_conversion"],
         "append_only_attrs": CONFIG["append_only_attrs"],
```

