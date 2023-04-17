# Comparing `tmp/inuits_policy_based_auth-2.0.1.tar.gz` & `tmp/inuits_policy_based_auth-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inuits_policy_based_auth-2.0.1.tar", last modified: Wed Apr 12 16:39:45 2023, max compression
+gzip compressed data, was "inuits_policy_based_auth-3.0.0.tar", last modified: Mon Apr 17 16:25:32 2023, max compression
```

## Comparing `inuits_policy_based_auth-2.0.1.tar` & `inuits_policy_based_auth-3.0.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/
--rw-r--r--   0 gverm     (1000) gverm     (1001)    18092 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/LICENSE
--rw-r--r--   0 gverm     (1000) gverm     (1001)     7015 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/PKG-INFO
--rw-r--r--   0 gverm     (1000) gverm     (1001)     6553 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/README.md
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.416447 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1100 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/__init__.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.416447 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1856 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/base_authentication_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.416447 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/policies/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/policies/__init__.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.416447 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/policies/token_based_policies/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/policies/token_based_policies/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     6291 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.416447 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     2665 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/base_authorization_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/policies/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/policies/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      470 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/policies/open_data_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      530 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/policies/scope_based_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      576 2023-04-12 16:37:24.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/policies/super_admin_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/contexts/
--rw-r--r--   0 gverm     (1000) gverm     (1001)      223 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/contexts/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      851 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/contexts/policy_context.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1388 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/contexts/request_context.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     2863 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/contexts/user_context.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1193 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/exceptions.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/helpers/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/helpers/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     4768 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/helpers/immutable_dict.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     6187 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/policy_factory.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.416447 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth.egg-info/
--rw-r--r--   0 gverm     (1000) gverm     (1001)     7015 2023-04-12 16:39:45.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth.egg-info/PKG-INFO
--rw-r--r--   0 gverm     (1000) gverm     (1001)     2621 2023-04-12 16:39:45.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth.egg-info/SOURCES.txt
--rw-r--r--   0 gverm     (1000) gverm     (1001)        1 2023-04-12 16:39:45.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth.egg-info/dependency_links.txt
--rw-r--r--   0 gverm     (1000) gverm     (1001)      129 2023-04-12 16:39:45.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth.egg-info/requires.txt
--rw-r--r--   0 gverm     (1000) gverm     (1001)       31 2023-04-12 16:39:45.000000 inuits_policy_based_auth-2.0.1/inuits_policy_based_auth.egg-info/top_level.txt
--rw-r--r--   0 gverm     (1000) gverm     (1001)       38 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/setup.cfg
--rw-r--r--   0 gverm     (1000) gverm     (1001)      959 2023-04-12 16:37:24.000000 inuits_policy_based_auth-2.0.1/setup.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.416447 inuits_policy_based_auth-2.0.1/tests/
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/integration/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/__init__.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/integration/authentication/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/authentication/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1201 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/authentication/test_authlib_flask_oauth2_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/integration/authorization/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/authorization/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1093 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/authorization/test_open_data_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1317 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/authorization/test_scope_based_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1952 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/authorization/test_super_admin_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      656 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/custom_token.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1490 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/flask_process.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/integration/test_api/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/test_api/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1791 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/test_api/app.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     2341 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/test_api/policy_loader.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     3485 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/integration/test_policy_factory.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/unit/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/__init__.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/unit/authentication/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authentication/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1345 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authentication/test_base_authentication_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/unit/authorization/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authorization/__init__.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)      150 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/dummies.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1138 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/test_open_data_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1105 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/test_scope_based_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     1045 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/test_super_admin_policy.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     2024 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/authorization/test_base_authorization_policy.py
-drwxr-xr-x   0 gverm     (1000) gverm     (1001)        0 2023-04-12 16:39:45.419781 inuits_policy_based_auth-2.0.1/tests/unit/helpers/
--rw-r--r--   0 gverm     (1000) gverm     (1001)        0 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/helpers/__init__.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     3524 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/helpers/test_immutable_dict.py
--rw-r--r--   0 gverm     (1000) gverm     (1001)     6509 2023-04-12 14:29:54.000000 inuits_policy_based_auth-2.0.1/tests/unit/test_policy_factory.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.516754 inuits_policy_based_auth-3.0.0/
+-rw-r--r--   0 eray      (1000) eray      (1000)    18092 2023-01-11 09:40:36.000000 inuits_policy_based_auth-3.0.0/LICENSE
+-rw-r--r--   0 eray      (1000) eray      (1000)     7595 2023-04-17 16:25:32.516754 inuits_policy_based_auth-3.0.0/PKG-INFO
+-rw-r--r--   0 eray      (1000) eray      (1000)     7133 2023-04-17 16:22:33.000000 inuits_policy_based_auth-3.0.0/README.md
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.509754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/
+-rw-r--r--   0 eray      (1000) eray      (1000)     1100 2023-03-17 17:05:37.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/__init__.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.510754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/
+-rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-17 15:56:53.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/__init__.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     1881 2023-04-14 18:07:37.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/base_authentication_policy.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.510754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/policies/
+-rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-17 15:56:58.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/policies/__init__.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.511754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/policies/token_based_policies/
+-rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-17 17:27:12.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/policies/token_based_policies/__init__.py
+-rw-r--r--   0 eray      (1000) eray      (1000)    10967 2023-04-17 15:55:20.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/policies/token_based_policies/authlib_flask_oauth2_policy.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.511754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/
+-rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-17 15:57:41.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/__init__.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     2744 2023-04-14 18:06:21.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/base_authorization_policy.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.511754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/policies/
+-rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-17 17:27:18.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/policies/__init__.py
+-rw-r--r--   0 eray      (1000) eray      (1000)      470 2023-01-11 11:28:59.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/policies/open_data_policy.py
+-rw-r--r--   0 eray      (1000) eray      (1000)      530 2023-03-20 10:09:51.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/policies/scope_based_policy.py
+-rw-r--r--   0 eray      (1000) eray      (1000)      571 2023-04-14 18:06:49.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/policies/super_admin_policy.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.512754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/contexts/
+-rw-r--r--   0 eray      (1000) eray      (1000)      223 2023-01-10 14:21:54.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/contexts/__init__.py
+-rw-r--r--   0 eray      (1000) eray      (1000)      851 2023-04-14 18:01:31.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/contexts/policy_context.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     1435 2023-04-14 18:12:49.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/contexts/request_context.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     2942 2023-04-14 18:18:05.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/contexts/user_context.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     1591 2023-04-17 09:09:37.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/exceptions.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.512754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/helpers/
+-rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-21 08:11:53.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/helpers/__init__.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     4768 2023-03-22 15:11:22.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/helpers/immutable_dict.py
+-rw-r--r--   0 eray      (1000) eray      (1000)    10620 2023-04-17 15:12:55.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/policy_factory.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.510754 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth.egg-info/
+-rw-r--r--   0 eray      (1000) eray      (1000)     7595 2023-04-17 16:25:32.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth.egg-info/PKG-INFO
+-rw-r--r--   0 eray      (1000) eray      (1000)     2621 2023-04-17 16:25:32.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 eray      (1000) eray      (1000)        1 2023-04-17 16:25:32.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 eray      (1000) eray      (1000)      129 2023-04-17 16:25:32.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth.egg-info/requires.txt
+-rw-r--r--   0 eray      (1000) eray      (1000)       31 2023-04-17 16:25:32.000000 inuits_policy_based_auth-3.0.0/inuits_policy_based_auth.egg-info/top_level.txt
+-rw-r--r--   0 eray      (1000) eray      (1000)       38 2023-04-17 16:25:32.516754 inuits_policy_based_auth-3.0.0/setup.cfg
+-rw-r--r--   0 eray      (1000) eray      (1000)      959 2023-04-17 16:24:22.000000 inuits_policy_based_auth-3.0.0/setup.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.508754 inuits_policy_based_auth-3.0.0/tests/
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.513754 inuits_policy_based_auth-3.0.0/tests/integration/
+-rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-13 15:47:05.000000 inuits_policy_based_auth-3.0.0/tests/integration/__init__.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.513754 inuits_policy_based_auth-3.0.0/tests/integration/authentication/
+-rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-19 13:52:33.000000 inuits_policy_based_auth-3.0.0/tests/integration/authentication/__init__.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     1201 2023-04-14 14:07:40.000000 inuits_policy_based_auth-3.0.0/tests/integration/authentication/test_authlib_flask_oauth2_policy.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.513754 inuits_policy_based_auth-3.0.0/tests/integration/authorization/
+-rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-20 08:59:06.000000 inuits_policy_based_auth-3.0.0/tests/integration/authorization/__init__.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     1093 2023-03-20 10:42:01.000000 inuits_policy_based_auth-3.0.0/tests/integration/authorization/test_open_data_policy.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     1317 2023-03-21 17:11:07.000000 inuits_policy_based_auth-3.0.0/tests/integration/authorization/test_scope_based_policy.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     1947 2023-04-17 14:18:39.000000 inuits_policy_based_auth-3.0.0/tests/integration/authorization/test_super_admin_policy.py
+-rw-r--r--   0 eray      (1000) eray      (1000)      656 2023-01-19 15:19:28.000000 inuits_policy_based_auth-3.0.0/tests/integration/custom_token.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     1508 2023-04-17 14:44:09.000000 inuits_policy_based_auth-3.0.0/tests/integration/flask_process.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.514754 inuits_policy_based_auth-3.0.0/tests/integration/test_api/
+-rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-13 15:47:05.000000 inuits_policy_based_auth-3.0.0/tests/integration/test_api/__init__.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     1793 2023-04-17 15:15:06.000000 inuits_policy_based_auth-3.0.0/tests/integration/test_api/app.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     2593 2023-04-17 15:56:03.000000 inuits_policy_based_auth-3.0.0/tests/integration/test_api/policy_loader.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     3480 2023-04-17 14:31:12.000000 inuits_policy_based_auth-3.0.0/tests/integration/test_policy_factory.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.514754 inuits_policy_based_auth-3.0.0/tests/unit/
+-rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-13 14:32:25.000000 inuits_policy_based_auth-3.0.0/tests/unit/__init__.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.514754 inuits_policy_based_auth-3.0.0/tests/unit/authentication/
+-rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-13 14:32:11.000000 inuits_policy_based_auth-3.0.0/tests/unit/authentication/__init__.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     1345 2023-01-11 15:24:33.000000 inuits_policy_based_auth-3.0.0/tests/unit/authentication/test_base_authentication_policy.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.515754 inuits_policy_based_auth-3.0.0/tests/unit/authorization/
+-rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-11 10:19:57.000000 inuits_policy_based_auth-3.0.0/tests/unit/authorization/__init__.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.515754 inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/
+-rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-01-11 11:40:35.000000 inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/__init__.py
+-rw-r--r--   0 eray      (1000) eray      (1000)      150 2023-01-11 11:37:14.000000 inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/dummies.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     1138 2023-01-11 14:27:27.000000 inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/test_open_data_policy.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     1105 2023-03-20 10:20:57.000000 inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/test_scope_based_policy.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     1040 2023-04-14 08:37:28.000000 inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/test_super_admin_policy.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     2024 2023-01-11 15:24:03.000000 inuits_policy_based_auth-3.0.0/tests/unit/authorization/test_base_authorization_policy.py
+drwxr-xr-x   0 eray      (1000) eray      (1000)        0 2023-04-17 16:25:32.516754 inuits_policy_based_auth-3.0.0/tests/unit/helpers/
+-rw-r--r--   0 eray      (1000) eray      (1000)        0 2023-03-21 13:26:01.000000 inuits_policy_based_auth-3.0.0/tests/unit/helpers/__init__.py
+-rw-r--r--   0 eray      (1000) eray      (1000)     3524 2023-03-21 18:25:06.000000 inuits_policy_based_auth-3.0.0/tests/unit/helpers/test_immutable_dict.py
+-rw-r--r--   0 eray      (1000) eray      (1000)    11998 2023-04-17 15:27:47.000000 inuits_policy_based_auth-3.0.0/tests/unit/test_policy_factory.py
```

### Comparing `inuits_policy_based_auth-2.0.1/LICENSE` & `inuits_policy_based_auth-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.1/PKG-INFO` & `inuits_policy_based_auth-3.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,59 @@
-Metadata-Version: 2.1
-Name: inuits_policy_based_auth
-Version: 2.0.1
-Summary: Module for securing API endpoints based on policies.
-Author: Inuits
-Author-email: developers@inuits.eu
-License: GPLv2
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Provides: inuits_policy_based_auth
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # inuits_policy_based_auth
 inuits_policy_based_auth is a python package for securing API endpoints based on policies.
 
 ## Installation
 Install inuits_policy_based_auth as follows:
 ```
 pip install inuits-policy-based-auth
 ```
 
 ## Getting Started
-In your app, instantiate the PolicyFactory by passing a logger as argument. For example, in app.py (all examples given are based on a Python Flask app).
+Instantiate the PolicyFactory in you app, for example in app.py (all examples given are based on a Python Flask app).
 ```python
 from inuits_policy_based_auth import PolicyFactory
 
 
-policy_factory = PolicyFactory(logger)
+policy_factory = PolicyFactory()
 ```
 ### Manually loading policies
-Importing and registering policies can be done manually.
+Importing and registering policies can be done manually. Don't forget to set a fallback key, this ensures that policies of a specific app are applied when the app cannot be determined automatically.
 ```python
 from inuits_policy_based_auth.authentication.policies.token_based_policies.authlib_flask_oauth2_policy import (
     AuthlibFlaskOauth2Policy,
 )
 from inuits_policy_based_auth.authorization.policies.super_admin_policy import (
     SuperAdminPolicy,
 )
 
 
-policy_factory.register_authentication_policy(AuthlibFlaskOauth2Policy(...))
-policy_factory.register_authorization_policy(SuperAdminPolicy())
+policy_factory.register_authentication_policy("apps.[app_name]", AuthlibFlaskOauth2Policy(...))
+policy_factory.register_authorization_policy("apps.[app_name]", SuperAdminPolicy())
+policy_factory.set_fallback_key_for_policy_mapping("apps.[app_name]")
 ```
-However, it is strongly recommended to load policies dynamically as this will allow you to make use of the full potential of this package.
+However, it is recommended to load policies dynamically as this will allow you to make use of the full potential of this package.
 
 ### Dynamically loading policies
 You can write a loader which loads policies dynamically based on a configuration file.
 
 Example configuration file:
 ```json
 {
-  "[app_name]": {
-    "name": "[app_name]",
-    "description": "",
-    "version": 0.1,
-    "author": "Inuits",
-    "author_email": "developers@inuits.eu",
-    "license": "GPLv2",
+  "[app_name_1]": {
+    "policies": {
+      "authentication": [
+        "token_based_policies.authlib_flask_oauth2_policy"
+      ],
+      "authorization": [
+        "super_admin_policy",
+        "scope_based_policy"
+      ]
+    }
+  },
+  "[app_name_2]": {
     "policies": {
       "authentication": [
         "token_based_policies.authlib_flask_oauth2_policy"
       ],
       "authorization": [
         "super_admin_policy",
         "open_data_policy"
@@ -77,42 +69,49 @@
 import os
 
 from importlib import import_module
 from inuits_policy_based_auth import PolicyFactory
 from inuits_policy_based_auth.exceptions import (
     PolicyFactoryException,
 )
+from logging import Logger
 
 
-def load_policies(policy_factory: PolicyFactory):
+def load_policies(policy_factory: PolicyFactory, logger: Logger):
     apps = {}
 
-    configuration_file_name = os.getenv("CONFIGURATION_FILE_NAME") or ""
+    configuration_file_name = os.getenv("[CONFIGURATION_FILE_NAME]") or ""
     with open(configuration_file_name) as configuration_file:
         apps = json.load(configuration_file)
 
     for app in apps:
         try:
             auth_type = "authentication"
             for policy_module_name in apps[app]["policies"].get(auth_type):
                 policy = __get_class(app, auth_type, policy_module_name)
                 policy = __instantiate_authentication_policy(
-                    policy_module_name, policy, policy_factory.logger
+                    policy_module_name, policy, logger
+                )
+                policy_factory.register_authentication_policy(
+                    f"apps.{app}", policy
                 )
-                policy_factory.register_authentication_policy(policy)
 
             auth_type = "authorization"
             for policy_module_name in apps[app]["policies"].get(auth_type):
                 policy = __get_class(app, auth_type, policy_module_name)
-                policy_factory.register_authorization_policy(policy())
+                policy_factory.register_authorization_policy(
+                    f"apps.{app}", policy()
+                )
         except Exception as error:
             raise PolicyFactoryException(
                 f"Policy factory was not configured correctly: {str(error)}"
             ).with_traceback(error.__traceback__)
 
+    policy_factory.set_fallback_key_for_policy_mapping("apps.[app_name]")
+
 
 def __get_class(app, auth_type, policy_module_name):
     module = None
 
     try:
         module = import_module(f"apps.{app}.policies.{auth_type}.{policy_module_name}")
     except:
@@ -121,35 +120,36 @@
         )
 
     policy_class_name = module.__name__.split(".")[-1].title().replace("_", "")
     policy = getattr(module, policy_class_name)
     return policy
 
 
-def __instantiate_authentication_policy(policy_module_name, policy, logger):
+def __instantiate_authentication_policy(policy_module_name, policy, logger: Logger):
     if policy_module_name == "token_based_policies.authlib_flask_oauth2_policy":
         return policy(
             logger,
             os.getenv("STATIC_ISSUER", False),
             os.getenv("STATIC_PUBLIC_KEY", False),
             os.getenv("REALMS", "").split(","),
-            os.getenv("ROLE_PERMISSION_FILE", "role_permission.json"),
+            os.getenv("ROLE_SCOPE_MAPPING", os.getenv("TEST_API_SCOPES")),
             os.getenv("REMOTE_TOKEN_VALIDATION", False) in ["True", "true", True],
             os.getenv("REMOTE_PUBLIC_KEY", False),
         )
 
     return policy()
 ```
 
 Now you can import the loader in app.py and pass ```policy_factory``` as an argument to it.
 ```python
 from apps.policy_loader import load_policies
+from logging import Logger
 
 
-load_policies(policy_factory)
+load_policies(policy_factory, Logger(""))
 ```
 As you can see in these examples, dynamically loading policies will allow you to add new policies and override existing ones, which makes this package highly customizable and generic.
 
 ### Custom policies
 Continuing from the examples above, you can make a custom authorization policy by creating a folder ```policies``` within a specific app. Here you should create the folders ```authentication``` and ```authorization``` that will contain custom policies which you can add to your configuration. In this case we name our new policy the same as an existing one, which will override it. Each authentication policy must inherit from BaseAuthenticationPolicy and implement the abstract method ```authenticate```, while each authorization policy must inherit from BaseAuthorizationPolicy and implement the abstract method ```authorize```.
 
 Example folder structure:
@@ -188,15 +188,17 @@
 ```python
 from app import policy_factory
 from flask import request
 from inuits_policy_based_auth import RequestContext
 
 
 class Entity():
-    @policy_factory.apply_policies(RequestContext(request))
+    @policy_factory.apply_policies(
+        RequestContext(request, ["[scope_1]", "[scope_2]"])
+    )
     def get(self):
         ...
 ```
 
 You can also use the ```authenticate``` decorator to only apply authentication policies:
 ```python
 from app import policy_factory
```

### Comparing `inuits_policy_based_auth-2.0.1/README.md` & `inuits_policy_based_auth-3.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,73 @@
+Metadata-Version: 2.1
+Name: inuits_policy_based_auth
+Version: 3.0.0
+Summary: Module for securing API endpoints based on policies.
+Author: Inuits
+Author-email: developers@inuits.eu
+License: GPLv2
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Provides: inuits_policy_based_auth
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # inuits_policy_based_auth
 inuits_policy_based_auth is a python package for securing API endpoints based on policies.
 
 ## Installation
 Install inuits_policy_based_auth as follows:
 ```
 pip install inuits-policy-based-auth
 ```
 
 ## Getting Started
-In your app, instantiate the PolicyFactory by passing a logger as argument. For example, in app.py (all examples given are based on a Python Flask app).
+Instantiate the PolicyFactory in you app, for example in app.py (all examples given are based on a Python Flask app).
 ```python
 from inuits_policy_based_auth import PolicyFactory
 
 
-policy_factory = PolicyFactory(logger)
+policy_factory = PolicyFactory()
 ```
 ### Manually loading policies
-Importing and registering policies can be done manually.
+Importing and registering policies can be done manually. Don't forget to set a fallback key, this ensures that policies of a specific app are applied when the app cannot be determined automatically.
 ```python
 from inuits_policy_based_auth.authentication.policies.token_based_policies.authlib_flask_oauth2_policy import (
     AuthlibFlaskOauth2Policy,
 )
 from inuits_policy_based_auth.authorization.policies.super_admin_policy import (
     SuperAdminPolicy,
 )
 
 
-policy_factory.register_authentication_policy(AuthlibFlaskOauth2Policy(...))
-policy_factory.register_authorization_policy(SuperAdminPolicy())
+policy_factory.register_authentication_policy("apps.[app_name]", AuthlibFlaskOauth2Policy(...))
+policy_factory.register_authorization_policy("apps.[app_name]", SuperAdminPolicy())
+policy_factory.set_fallback_key_for_policy_mapping("apps.[app_name]")
 ```
-However, it is strongly recommended to load policies dynamically as this will allow you to make use of the full potential of this package.
+However, it is recommended to load policies dynamically as this will allow you to make use of the full potential of this package.
 
 ### Dynamically loading policies
 You can write a loader which loads policies dynamically based on a configuration file.
 
 Example configuration file:
 ```json
 {
-  "[app_name]": {
-    "name": "[app_name]",
-    "description": "",
-    "version": 0.1,
-    "author": "Inuits",
-    "author_email": "developers@inuits.eu",
-    "license": "GPLv2",
+  "[app_name_1]": {
+    "policies": {
+      "authentication": [
+        "token_based_policies.authlib_flask_oauth2_policy"
+      ],
+      "authorization": [
+        "super_admin_policy",
+        "scope_based_policy"
+      ]
+    }
+  },
+  "[app_name_2]": {
     "policies": {
       "authentication": [
         "token_based_policies.authlib_flask_oauth2_policy"
       ],
       "authorization": [
         "super_admin_policy",
         "open_data_policy"
@@ -63,42 +83,49 @@
 import os
 
 from importlib import import_module
 from inuits_policy_based_auth import PolicyFactory
 from inuits_policy_based_auth.exceptions import (
     PolicyFactoryException,
 )
+from logging import Logger
 
 
-def load_policies(policy_factory: PolicyFactory):
+def load_policies(policy_factory: PolicyFactory, logger: Logger):
     apps = {}
 
-    configuration_file_name = os.getenv("CONFIGURATION_FILE_NAME") or ""
+    configuration_file_name = os.getenv("[CONFIGURATION_FILE_NAME]") or ""
     with open(configuration_file_name) as configuration_file:
         apps = json.load(configuration_file)
 
     for app in apps:
         try:
             auth_type = "authentication"
             for policy_module_name in apps[app]["policies"].get(auth_type):
                 policy = __get_class(app, auth_type, policy_module_name)
                 policy = __instantiate_authentication_policy(
-                    policy_module_name, policy, policy_factory.logger
+                    policy_module_name, policy, logger
+                )
+                policy_factory.register_authentication_policy(
+                    f"apps.{app}", policy
                 )
-                policy_factory.register_authentication_policy(policy)
 
             auth_type = "authorization"
             for policy_module_name in apps[app]["policies"].get(auth_type):
                 policy = __get_class(app, auth_type, policy_module_name)
-                policy_factory.register_authorization_policy(policy())
+                policy_factory.register_authorization_policy(
+                    f"apps.{app}", policy()
+                )
         except Exception as error:
             raise PolicyFactoryException(
                 f"Policy factory was not configured correctly: {str(error)}"
             ).with_traceback(error.__traceback__)
 
+    policy_factory.set_fallback_key_for_policy_mapping("apps.[app_name]")
+
 
 def __get_class(app, auth_type, policy_module_name):
     module = None
 
     try:
         module = import_module(f"apps.{app}.policies.{auth_type}.{policy_module_name}")
     except:
@@ -107,35 +134,36 @@
         )
 
     policy_class_name = module.__name__.split(".")[-1].title().replace("_", "")
     policy = getattr(module, policy_class_name)
     return policy
 
 
-def __instantiate_authentication_policy(policy_module_name, policy, logger):
+def __instantiate_authentication_policy(policy_module_name, policy, logger: Logger):
     if policy_module_name == "token_based_policies.authlib_flask_oauth2_policy":
         return policy(
             logger,
             os.getenv("STATIC_ISSUER", False),
             os.getenv("STATIC_PUBLIC_KEY", False),
             os.getenv("REALMS", "").split(","),
-            os.getenv("ROLE_PERMISSION_FILE", "role_permission.json"),
+            os.getenv("ROLE_SCOPE_MAPPING", os.getenv("TEST_API_SCOPES")),
             os.getenv("REMOTE_TOKEN_VALIDATION", False) in ["True", "true", True],
             os.getenv("REMOTE_PUBLIC_KEY", False),
         )
 
     return policy()
 ```
 
 Now you can import the loader in app.py and pass ```policy_factory``` as an argument to it.
 ```python
 from apps.policy_loader import load_policies
+from logging import Logger
 
 
-load_policies(policy_factory)
+load_policies(policy_factory, Logger(""))
 ```
 As you can see in these examples, dynamically loading policies will allow you to add new policies and override existing ones, which makes this package highly customizable and generic.
 
 ### Custom policies
 Continuing from the examples above, you can make a custom authorization policy by creating a folder ```policies``` within a specific app. Here you should create the folders ```authentication``` and ```authorization``` that will contain custom policies which you can add to your configuration. In this case we name our new policy the same as an existing one, which will override it. Each authentication policy must inherit from BaseAuthenticationPolicy and implement the abstract method ```authenticate```, while each authorization policy must inherit from BaseAuthorizationPolicy and implement the abstract method ```authorize```.
 
 Example folder structure:
@@ -174,15 +202,17 @@
 ```python
 from app import policy_factory
 from flask import request
 from inuits_policy_based_auth import RequestContext
 
 
 class Entity():
-    @policy_factory.apply_policies(RequestContext(request))
+    @policy_factory.apply_policies(
+        RequestContext(request, ["[scope_1]", "[scope_2]"])
+    )
     def get(self):
         ...
 ```
 
 You can also use the ```authenticate``` decorator to only apply authentication policies:
 ```python
 from app import policy_factory
```

### Comparing `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/__init__.py` & `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authentication/base_authentication_policy.py` & `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authentication/base_authentication_policy.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,43 +3,45 @@
 from inuits_policy_based_auth.exceptions import (
     AuthenticateMethodDidNotReturnObjectOfTypeUserContextException,
 )
 
 
 class BaseAuthenticationPolicy(ABC):
     """
-    An abstract class used as an interface for concrete implementations of authentication policies.
+    An abstract class used as an interface for concrete implementations of
+    authentication policies.
 
     Methods
     -------
-    apply(user_context)
-        applies the policy
-    authenticate(user_context)
-        authenticates a user
+    apply(user_context):
+        Applies the policy.
+
+    authenticate(user_context):
+        Authenticates a user.
     """
 
     def apply(self, user_context: UserContext) -> UserContext:
         """Applies the policy.
 
         Parameters
         ----------
         user_context : UserContext
-            an object containing data about the authenticated user
+            An object containing data about the authenticated user.
 
         Returns
         -------
         UserContext
-            an object containing data about the authenticated user
+            An object containing data about the authenticated user.
 
         Raises
         ------
-        AuthenticateMethodDidNotReturnObjectOfTypeUserContextException
-            if the authenticate method does not return an object of type UserContext
-        Unauthorized
-            if the user is not authenticated
+        AuthenticateMethodDidNotReturnObjectOfTypeUserContextException:
+            If the authenticate method does not return an object of type UserContext.
+        Unauthorized:
+            If the user is not authenticated.
         """
 
         user_context = self.authenticate(user_context)
         if not isinstance(user_context, UserContext):
             raise AuthenticateMethodDidNotReturnObjectOfTypeUserContextException()
 
         return user_context
@@ -47,21 +49,21 @@
     @abstractmethod
     def authenticate(self, user_context: UserContext) -> UserContext:
         """Authenticates a user.
 
         Parameters
         ----------
         user_context : UserContext
-            an object containing data about the authenticated user
+            An object containing data about the user to be authenticated.
 
         Returns
         -------
         UserContext
-            an object containing data about the authenticated user
+            An object containing data about the authenticated user.
 
         Raises
         ------
-        Unauthorized
-            if the user is not authenticated
+        Unauthorized:
+            If the user is not authenticated.
         """
 
         pass
```

### Comparing `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/base_authorization_policy.py` & `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/base_authorization_policy.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 from inuits_policy_based_auth.exceptions import (
     AuthorizeMethodDidNotReturnObjectOfTypePolicyContextException,
 )
 
 
 class BaseAuthorizationPolicy(ABC):
     """
-    An abstract class used as an interface for concrete implementations of authorization policies.
+    An abstract class used as an interface for concrete implementations of
+    authorization policies.
 
     Methods
     -------
-    apply(user_context, request_context)
-        applies the policy
-    authorize(user_context, request_context)
-        authorizes a user
+    apply(user_context, request_context):
+        Applies the policy.
+
+    authorize(user_context, request_context):
+        Authorizes a user.
     """
 
     def apply(
         self,
         policy_context: PolicyContext,
         user_context: UserContext,
         request_context: RequestContext,
@@ -26,29 +28,32 @@
         """Applies the policy.
 
         Sets policy_context.access_verdict to its default value None before authorizing.
 
         Parameters
         ----------
         policy_context : PolicyContext
-            an object containing data about the context of an applied authorization policy
+            An object containing data about the context of an applied
+            authorization policy.
         user_context : UserContext
-            an object containing data about the authenticated user
+            An object containing data about the authenticated user.
         request_context : RequestContext
-            an object containing data about the context of a request
+            An object containing data about the context of a request.
 
         Returns
         -------
         PolicyContext
-            an object containing data about the context of an applied authorization policy
+            An object containing data about the context of an applied
+            authorization policy.
 
         Raises
         ------
-        AuthorizeMethodDidNotReturnObjectOfTypePolicyContextException
-            if the authorize method does not return an object of type PolicyContext
+        AuthorizeMethodDidNotReturnObjectOfTypePolicyContextException:
+            If the authorize method does not return an object of type
+            PolicyContext.
         """
 
         policy_context.access_verdict = None
         policy_context = self.authorize(policy_context, user_context, request_context)
         if not isinstance(policy_context, PolicyContext):
             raise AuthorizeMethodDidNotReturnObjectOfTypePolicyContextException()
 
@@ -62,20 +67,22 @@
         request_context: RequestContext,
     ) -> PolicyContext:
         """Authorizes a user.
 
         Parameters
         ----------
         policy_context : PolicyContext
-            an object containing data about the context of an applied authorization policy
+            An object containing data about the context of an applied
+            authorization policy.
         user_context : UserContext
-            an object containing data about the authenticated user
+            An object containing data about the authenticated user.
         request_context : RequestContext, optional
-            an object containing data about the context of a request
+            An object containing data about the context of a request.
 
         Returns
         -------
         PolicyContext
-            an object containing data about the context of an applied authorization policy
+            An object containing data about the context of an applied
+            authorization policy.
         """
 
         pass
```

### Comparing `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/policies/scope_based_policy.py` & `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/policies/scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/authorization/policies/super_admin_policy.py` & `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/authorization/policies/super_admin_policy.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from inuits_policy_based_auth.authorization.base_authorization_policy import (
     BaseAuthorizationPolicy,
 )
 
 
 class SuperAdminPolicy(BaseAuthorizationPolicy):
     """
-    An authorization policy that allows a user to do anything if he/she has the role 'role_super_admin'.
+    An authorization policy that allows a user to do anything if he/she has a super
+    admin role.
     """
 
     super_admin_role: str = os.getenv("SUPER_ADMIN_ROLE", "super_admin")
 
     def authorize(self, policy_context, user_context, request_context):
         if self.super_admin_role in user_context.roles:
             policy_context.access_verdict = True
```

### Comparing `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/contexts/policy_context.py` & `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/contexts/policy_context.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 class PolicyContext:
     """
     A class containing data about the context of an applied authorization policy.
 
-    Authorization policies use these class to influence access determination.
+    Authorization policies use this class to influence access determination.
 
     Properties
     ----------
     access_verdict : bool | None
-        the verdict that will influence access determination
+        The verdict that will influence access determination.
     """
 
     def __init__(self):
         self._access_verdict = None
 
     @property
     def access_verdict(self):
```

### Comparing `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/contexts/request_context.py` & `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/contexts/request_context.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 class RequestContext:
-    """
-    A class containing data about the context of a request.
+    """A class containing data about the context of a request.
 
-    The data provided in this class is used in policies to determine whether a user is authenticated/authorized.
+    The data provided in this class is used in policies to determine whether a
+    user is authenticated/authorized.
 
     Properties
     ----------
     http_request : Unknown
-        an HTTP request that is used by policies to determine access to a resource
+        An HTTP request used by policies to determine access to a resource.
     resource_scopes : list[str], optional
-        scopes a user must have for accessing a protected resource when policies rely on scope-based authorization
+        Scopes a user must have for accessing a protected resource when policies
+        rely on scope-based authorization.
     """
 
     def __init__(self, http_request, resource_scopes: list[str] = []):
         """
         Parameters
         ----------
         http_request : Unknown
-            an HTTP request that is used by policies to determine access to a resource.
-        resource_scopes : str, optional
-            scopes a user must have for accessing a protected resource when policies rely on scope-based authorization
+            An HTTP request used by policies to determine access to a resource.
+        resource_scopes : list[str], optional
+            Scopes a user must have for accessing a protected resource when policies
+            rely on scope-based authorization.
         """
 
         self._http_request = http_request
         self._resource_scopes = resource_scopes
 
     @property
     def http_request(self):
-        """An HTTP request that is used by policies to determine access to a resource."""
+        """
+        An HTTP request used by policies to determine access to a resource.
+        """
 
         return self._http_request
 
     @property
     def resource_scopes(self):
-        """A scope a user must have for accessing a protected resource when policies rely on scope-based authorization."""
+        """
+        Scopes a user must have for accessing a protected resource when policies
+        rely on scope-based authorization.
+        """
 
         return self._resource_scopes
```

### Comparing `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/contexts/user_context.py` & `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/contexts/user_context.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,40 +5,44 @@
 class UserContext:
     """
     A class containing data about the authenticated user.
 
     Properties
     ----------
     auth_objects : ImmutableDict
-        an immutable dict containing objects used to authenticate a user, for example a token
+        An immutable dict containing objects used to authenticate a user,
+        for example a token.
     email : str
-        the email of the authenticated user
+        The email of the authenticated user.
     tenant : str
-        the tenant of the authenticated user
+        The tenant of the authenticated user.
     roles : list[str]
-        the roles of the authenticated user
+        The roles of the authenticated user.
     scopes : list[str]
-        the scopes of the authenticated user
+        The scopes of the authenticated user.
 
     Methods
     -------
     flatten_auth_object(data, parent_key)
-        flattens the auth object to be a dict of one level deep
+        Flattens the auth object to be a dict of one level deep.
     """
 
     def __init__(self):
         self._auth_objects = ImmutableDict({})
         self._email = ""
         self._tenant = ""
         self._roles = []
         self._scopes = []
 
     @property
     def auth_objects(self):
-        """An immutable dict containing objects used to authenticate a user, for example a token."""
+        """
+        An immutable dict containing objects used to authenticate a user,
+        for example a token.
+        """
 
         return self._auth_objects
 
     @property
     def email(self):
         """The email of the authenticated user."""
 
@@ -88,18 +92,18 @@
 
     def flatten_auth_object(self, data: MutableMapping, parent_key=""):
         """Flattens the auth object to be a dict of one level deep.
 
         Parameters
         ----------
         data : MutableMapping
-            an object used to authenticate a user with, for example a token
+            An object used to authenticate a user with, for example a token.
         parent_key : str, optional
-            a key that will be the root key
+            A key that will be the root key for the flattened dict.
 
         Returns
         -------
-        dict[Unknown, Unknown]
-            the flattened auth object
+        dict
+            A flattened dictionary representation of the auth object.
         """
 
         return dict(self.__flatten_auth_object_generator(data, parent_key))
```

### Comparing `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/exceptions.py` & `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 class PolicyFactoryException(Exception):
     def __init__(self, message):
         super().__init__(message)
 
 
+class NoUserContextException(PolicyFactoryException):
+    def __init__(self):
+        super().__init__(
+            "Cannot get an object of type UserContext if no policies are applied yet."
+        )
+
+
 class NoAuthenticationPoliciesToApplyException(PolicyFactoryException):
     def __init__(self):
         super().__init__("No authentication policies set to apply.")
 
 
 class NoAuthorizationPoliciesToApplyException(PolicyFactoryException):
     def __init__(self):
         super().__init__("No authorization policies set to apply.")
 
 
-class NoUserContextException(PolicyFactoryException):
-    def __init__(self):
+class InvalidFallbackKey(PolicyFactoryException):
+    def __init__(self, key: str):
         super().__init__(
-            "Cannot get an object of type UserContext if no policies are applied yet."
+            f"Provided fallback key '{key}' is not registered in either authentication policies, authorization policies, or both."
         )
 
 
+class NoFallbackKeySet(PolicyFactoryException):
+    def __init__(self):
+        super().__init__("No fallback key for policy mapping is set.")
+
+
 class PolicyException(Exception):
     pass
 
 
 class AuthenticateMethodDidNotReturnObjectOfTypeUserContextException(PolicyException):
     def __init__(self):
         super().__init__(
```

### Comparing `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth/helpers/immutable_dict.py` & `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth/helpers/immutable_dict.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth.egg-info/PKG-INFO` & `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inuits-policy-based-auth
-Version: 2.0.1
+Version: 3.0.0
 Summary: Module for securing API endpoints based on policies.
 Author: Inuits
 Author-email: developers@inuits.eu
 License: GPLv2
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -18,50 +18,56 @@
 ## Installation
 Install inuits_policy_based_auth as follows:
 ```
 pip install inuits-policy-based-auth
 ```
 
 ## Getting Started
-In your app, instantiate the PolicyFactory by passing a logger as argument. For example, in app.py (all examples given are based on a Python Flask app).
+Instantiate the PolicyFactory in you app, for example in app.py (all examples given are based on a Python Flask app).
 ```python
 from inuits_policy_based_auth import PolicyFactory
 
 
-policy_factory = PolicyFactory(logger)
+policy_factory = PolicyFactory()
 ```
 ### Manually loading policies
-Importing and registering policies can be done manually.
+Importing and registering policies can be done manually. Don't forget to set a fallback key, this ensures that policies of a specific app are applied when the app cannot be determined automatically.
 ```python
 from inuits_policy_based_auth.authentication.policies.token_based_policies.authlib_flask_oauth2_policy import (
     AuthlibFlaskOauth2Policy,
 )
 from inuits_policy_based_auth.authorization.policies.super_admin_policy import (
     SuperAdminPolicy,
 )
 
 
-policy_factory.register_authentication_policy(AuthlibFlaskOauth2Policy(...))
-policy_factory.register_authorization_policy(SuperAdminPolicy())
+policy_factory.register_authentication_policy("apps.[app_name]", AuthlibFlaskOauth2Policy(...))
+policy_factory.register_authorization_policy("apps.[app_name]", SuperAdminPolicy())
+policy_factory.set_fallback_key_for_policy_mapping("apps.[app_name]")
 ```
-However, it is strongly recommended to load policies dynamically as this will allow you to make use of the full potential of this package.
+However, it is recommended to load policies dynamically as this will allow you to make use of the full potential of this package.
 
 ### Dynamically loading policies
 You can write a loader which loads policies dynamically based on a configuration file.
 
 Example configuration file:
 ```json
 {
-  "[app_name]": {
-    "name": "[app_name]",
-    "description": "",
-    "version": 0.1,
-    "author": "Inuits",
-    "author_email": "developers@inuits.eu",
-    "license": "GPLv2",
+  "[app_name_1]": {
+    "policies": {
+      "authentication": [
+        "token_based_policies.authlib_flask_oauth2_policy"
+      ],
+      "authorization": [
+        "super_admin_policy",
+        "scope_based_policy"
+      ]
+    }
+  },
+  "[app_name_2]": {
     "policies": {
       "authentication": [
         "token_based_policies.authlib_flask_oauth2_policy"
       ],
       "authorization": [
         "super_admin_policy",
         "open_data_policy"
@@ -77,42 +83,49 @@
 import os
 
 from importlib import import_module
 from inuits_policy_based_auth import PolicyFactory
 from inuits_policy_based_auth.exceptions import (
     PolicyFactoryException,
 )
+from logging import Logger
 
 
-def load_policies(policy_factory: PolicyFactory):
+def load_policies(policy_factory: PolicyFactory, logger: Logger):
     apps = {}
 
-    configuration_file_name = os.getenv("CONFIGURATION_FILE_NAME") or ""
+    configuration_file_name = os.getenv("[CONFIGURATION_FILE_NAME]") or ""
     with open(configuration_file_name) as configuration_file:
         apps = json.load(configuration_file)
 
     for app in apps:
         try:
             auth_type = "authentication"
             for policy_module_name in apps[app]["policies"].get(auth_type):
                 policy = __get_class(app, auth_type, policy_module_name)
                 policy = __instantiate_authentication_policy(
-                    policy_module_name, policy, policy_factory.logger
+                    policy_module_name, policy, logger
+                )
+                policy_factory.register_authentication_policy(
+                    f"apps.{app}", policy
                 )
-                policy_factory.register_authentication_policy(policy)
 
             auth_type = "authorization"
             for policy_module_name in apps[app]["policies"].get(auth_type):
                 policy = __get_class(app, auth_type, policy_module_name)
-                policy_factory.register_authorization_policy(policy())
+                policy_factory.register_authorization_policy(
+                    f"apps.{app}", policy()
+                )
         except Exception as error:
             raise PolicyFactoryException(
                 f"Policy factory was not configured correctly: {str(error)}"
             ).with_traceback(error.__traceback__)
 
+    policy_factory.set_fallback_key_for_policy_mapping("apps.[app_name]")
+
 
 def __get_class(app, auth_type, policy_module_name):
     module = None
 
     try:
         module = import_module(f"apps.{app}.policies.{auth_type}.{policy_module_name}")
     except:
@@ -121,35 +134,36 @@
         )
 
     policy_class_name = module.__name__.split(".")[-1].title().replace("_", "")
     policy = getattr(module, policy_class_name)
     return policy
 
 
-def __instantiate_authentication_policy(policy_module_name, policy, logger):
+def __instantiate_authentication_policy(policy_module_name, policy, logger: Logger):
     if policy_module_name == "token_based_policies.authlib_flask_oauth2_policy":
         return policy(
             logger,
             os.getenv("STATIC_ISSUER", False),
             os.getenv("STATIC_PUBLIC_KEY", False),
             os.getenv("REALMS", "").split(","),
-            os.getenv("ROLE_PERMISSION_FILE", "role_permission.json"),
+            os.getenv("ROLE_SCOPE_MAPPING", os.getenv("TEST_API_SCOPES")),
             os.getenv("REMOTE_TOKEN_VALIDATION", False) in ["True", "true", True],
             os.getenv("REMOTE_PUBLIC_KEY", False),
         )
 
     return policy()
 ```
 
 Now you can import the loader in app.py and pass ```policy_factory``` as an argument to it.
 ```python
 from apps.policy_loader import load_policies
+from logging import Logger
 
 
-load_policies(policy_factory)
+load_policies(policy_factory, Logger(""))
 ```
 As you can see in these examples, dynamically loading policies will allow you to add new policies and override existing ones, which makes this package highly customizable and generic.
 
 ### Custom policies
 Continuing from the examples above, you can make a custom authorization policy by creating a folder ```policies``` within a specific app. Here you should create the folders ```authentication``` and ```authorization``` that will contain custom policies which you can add to your configuration. In this case we name our new policy the same as an existing one, which will override it. Each authentication policy must inherit from BaseAuthenticationPolicy and implement the abstract method ```authenticate```, while each authorization policy must inherit from BaseAuthorizationPolicy and implement the abstract method ```authorize```.
 
 Example folder structure:
@@ -188,15 +202,17 @@
 ```python
 from app import policy_factory
 from flask import request
 from inuits_policy_based_auth import RequestContext
 
 
 class Entity():
-    @policy_factory.apply_policies(RequestContext(request))
+    @policy_factory.apply_policies(
+        RequestContext(request, ["[scope_1]", "[scope_2]"])
+    )
     def get(self):
         ...
 ```
 
 You can also use the ```authenticate``` decorator to only apply authentication policies:
 ```python
 from app import policy_factory
```

### Comparing `inuits_policy_based_auth-2.0.1/inuits_policy_based_auth.egg-info/SOURCES.txt` & `inuits_policy_based_auth-3.0.0/inuits_policy_based_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.1/setup.py` & `inuits_policy_based_auth-3.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,21 +13,21 @@
         "Programming Language :: Python :: 3",
     ],
     description="Module for securing API endpoints based on policies.",
     install_requires=[
         "Authlib>=1.2.0",
         "cffi>=1.15.1",
         "click>=8.1.3",
-        "cryptography>=39.0.2",
+        "cryptography>=40.0.2",
         "MarkupSafe>=2.1.2",
         "pycparser>=2.21",
         "requests>=2.28.2",
         "Werkzeug>=2.2.3",
     ],
     license="GPLv2",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     name="inuits_policy_based_auth",
     packages=find_packages(exclude=["tests"]),
     provides=["inuits_policy_based_auth"],
-    version="2.0.1",
+    version="3.0.0",
 )
```

### Comparing `inuits_policy_based_auth-2.0.1/tests/integration/authentication/test_authlib_flask_oauth2_policy.py` & `inuits_policy_based_auth-3.0.0/tests/integration/authentication/test_authlib_flask_oauth2_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.1/tests/integration/authorization/test_open_data_policy.py` & `inuits_policy_based_auth-3.0.0/tests/integration/authorization/test_open_data_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.1/tests/integration/authorization/test_scope_based_policy.py` & `inuits_policy_based_auth-3.0.0/tests/integration/authorization/test_scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.1/tests/integration/authorization/test_super_admin_policy.py` & `inuits_policy_based_auth-3.0.0/tests/integration/authorization/test_super_admin_policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 
 load_dotenv()
 
 
 class TestSuperAdminPolicy:
     ENDPOINT = str(os.getenv("ENDPOINT"))
-    SUPER_ADMIN_ROLE = "role_super_admin"
+    SUPER_ADMIN_ROLE = "super_admin"
 
     @classmethod
     def setup_class(cls):
         flask_process.set_app_policies(
             ["token_based_policies.authlib_flask_oauth2_policy"], ["super_admin_policy"]
         )
         flask_process.start()
 
     def setup_method(self):
         flask_process.assert_running()
 
-    def test_token_without_role_super_admin_returns_403(self):
+    def test_token_without_super_admin_role_returns_403(self):
         payload = {"azp": "inuits-policy-based-auth"}
         headers = custom_token.get_authorization_header(payload)
 
         response = requests.get(self.ENDPOINT, headers=headers)
 
         assert response.status_code == 403
```

### Comparing `inuits_policy_based_auth-2.0.1/tests/integration/custom_token.py` & `inuits_policy_based_auth-3.0.0/tests/integration/custom_token.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.1/tests/integration/flask_process.py` & `inuits_policy_based_auth-3.0.0/tests/integration/flask_process.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,19 +34,18 @@
 
 def _overwrite_configuration_file(
     authentication: list[str] = [], authorization: list[str] = []
 ):
     with open(str(os.getenv("TEST_API_CONFIGURATION")), "r+") as configuration_file:
         configuration = json.load(configuration_file)
 
-        if authentication and authorization:
-            configuration["test_api"]["policies"]["authentication"].extend(
-                authentication
-            )
-            configuration["test_api"]["policies"]["authorization"].extend(authorization)
-        else:
-            configuration["test_api"]["policies"]["authentication"] = []
-            configuration["test_api"]["policies"]["authorization"] = []
+        for app in ["test_api", "test_api_backup"]:
+            if authentication and authorization:
+                configuration[app]["policies"]["authentication"].extend(authentication)
+                configuration[app]["policies"]["authorization"].extend(authorization)
+            else:
+                configuration[app]["policies"]["authentication"] = []
+                configuration[app]["policies"]["authorization"] = []
 
         configuration_file.seek(0)
         configuration_file.write(json.dumps(configuration, indent=2))
         configuration_file.truncate()
```

### Comparing `inuits_policy_based_auth-2.0.1/tests/integration/test_api/app.py` & `inuits_policy_based_auth-3.0.0/tests/integration/test_api/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from inuits_policy_based_auth import PolicyFactory, RequestContext
 from logging import Logger
 
 
 app = Flask(__name__)
 api = Api(app)
 
-policy_factory = PolicyFactory(Logger(""))
-load_policies(policy_factory)
+policy_factory = PolicyFactory()
+load_policies(policy_factory, Logger(""))
 
 
 class Entity(Resource):
     @policy_factory.apply_policies(
         RequestContext(request, ["read-entity", "update-entity"])
     )
     def get(self):
```

### Comparing `inuits_policy_based_auth-2.0.1/tests/integration/test_api/policy_loader.py` & `inuits_policy_based_auth-3.0.0/tests/integration/test_api/policy_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,41 +2,48 @@
 import os
 
 from importlib import import_module
 from inuits_policy_based_auth import PolicyFactory
 from inuits_policy_based_auth.exceptions import (
     PolicyFactoryException,
 )
+from logging import Logger
 
 
-def load_policies(policy_factory: PolicyFactory):
+def load_policies(policy_factory: PolicyFactory, logger: Logger):
     apps = {}
 
     with open(str(os.getenv("TEST_API_CONFIGURATION")), "r") as configuration_file:
         apps = json.load(configuration_file)
 
     for app in apps:
         try:
             auth_type = "authentication"
             for policy_module_name in apps[app]["policies"].get(auth_type):
                 policy = __get_class(app, auth_type, policy_module_name)
                 policy = __instantiate_authentication_policy(
-                    policy_module_name, policy, policy_factory.logger
+                    policy_module_name, policy, logger
+                )
+                policy_factory.register_authentication_policy(
+                    f"tests.integration.{app}", policy
                 )
-                policy_factory.register_authentication_policy(policy)
 
             auth_type = "authorization"
             for policy_module_name in apps[app]["policies"].get(auth_type):
                 policy = __get_class(app, auth_type, policy_module_name)
-                policy_factory.register_authorization_policy(policy())
+                policy_factory.register_authorization_policy(
+                    f"tests.integration.{app}", policy()
+                )
         except Exception as error:
             raise PolicyFactoryException(
                 f"Policy factory was not configured correctly: {str(error)}"
             ).with_traceback(error.__traceback__)
 
+    policy_factory.set_fallback_key_for_policy_mapping("tests.integration.test_api")
+
 
 def __get_class(app, auth_type, policy_module_name):
     module = None
 
     try:
         module = import_module(f"apps.{app}.policies.{auth_type}.{policy_module_name}")
     except:
@@ -45,20 +52,20 @@
         )
 
     policy_class_name = module.__name__.split(".")[-1].title().replace("_", "")
     policy = getattr(module, policy_class_name)
     return policy
 
 
-def __instantiate_authentication_policy(policy_module_name, policy, logger):
+def __instantiate_authentication_policy(policy_module_name, policy, logger: Logger):
     if policy_module_name == "token_based_policies.authlib_flask_oauth2_policy":
         return policy(
             logger,
             os.getenv("STATIC_ISSUER", False),
             os.getenv("STATIC_PUBLIC_KEY", False),
             os.getenv("REALMS", "").split(","),
-            os.getenv("ROLE_PERMISSION_FILE", os.getenv("TEST_API_SCOPES")),
+            os.getenv("ROLE_SCOPE_MAPPING", os.getenv("TEST_API_SCOPES")),
             os.getenv("REMOTE_TOKEN_VALIDATION", False) in ["True", "true", True],
             os.getenv("REMOTE_PUBLIC_KEY", False),
         )
 
     return policy()
```

### Comparing `inuits_policy_based_auth-2.0.1/tests/integration/test_policy_factory.py` & `inuits_policy_based_auth-3.0.0/tests/integration/test_policy_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 load_dotenv()
 
 
 class TestPolicyFactory:
     ENDPOINT = str(os.getenv("ENDPOINT"))
-    SUPER_ADMIN_ROLE = "role_super_admin"
+    SUPER_ADMIN_ROLE = "super_admin"
     REGULAR_USER_ROLE = "regular_user"
 
     @classmethod
     def setup_class(cls):
         flask_process.set_app_policies(
             ["token_based_policies.authlib_flask_oauth2_policy"],
             ["super_admin_policy", "scope_based_policy", "open_data_policy"],
```

### Comparing `inuits_policy_based_auth-2.0.1/tests/unit/authentication/test_base_authentication_policy.py` & `inuits_policy_based_auth-3.0.0/tests/unit/authentication/test_base_authentication_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/test_open_data_policy.py` & `inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/test_open_data_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/test_scope_based_policy.py` & `inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/test_scope_based_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.1/tests/unit/authorization/policies/test_super_admin_policy.py` & `inuits_policy_based_auth-3.0.0/tests/unit/authorization/policies/test_super_admin_policy.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def setup_method(self):
         self.super_admin_policy = SuperAdminPolicy()
         self.policy_context = PolicyContext()
         self.user_context = UserContext()
         self.request_context = RequestContext(None)
 
     def test_authorize_allows_access(self):
-        self.user_context.roles = ["role_super_admin"]
+        self.user_context.roles = ["super_admin"]
         policy_context = self.super_admin_policy.authorize(
             self.policy_context, self.user_context, self.request_context
         )
         assert policy_context.access_verdict == True
 
     def test_authorize_does_not_determine_access(self):
         self.user_context.roles = ["regular_user"]
```

### Comparing `inuits_policy_based_auth-2.0.1/tests/unit/authorization/test_base_authorization_policy.py` & `inuits_policy_based_auth-3.0.0/tests/unit/authorization/test_base_authorization_policy.py`

 * *Files identical despite different names*

### Comparing `inuits_policy_based_auth-2.0.1/tests/unit/helpers/test_immutable_dict.py` & `inuits_policy_based_auth-3.0.0/tests/unit/helpers/test_immutable_dict.py`

 * *Files identical despite different names*

