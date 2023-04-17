# Comparing `tmp/bc_time-6.0.0.tar.gz` & `tmp/bc_time-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bc_time-6.0.0.tar", last modified: Fri Mar 17 11:36:18 2023, max compression
+gzip compressed data, was "bc_time-7.0.0.tar", last modified: Mon Apr 17 10:49:12 2023, max compression
```

## Comparing `bc_time-6.0.0.tar` & `bc_time-7.0.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-03-17 11:36:18.841595 bc_time-6.0.0/
--rw-r--r--   0 dburger    (501) staff       (20)     1067 2022-05-24 07:44:21.000000 bc_time-6.0.0/LICENSE.txt
--rw-r--r--   0 dburger    (501) staff       (20)     4070 2023-03-17 11:36:18.841639 bc_time-6.0.0/PKG-INFO
--rw-r--r--   0 dburger    (501) staff       (20)     3577 2023-03-17 11:10:47.000000 bc_time-6.0.0/README.md
--rw-r--r--   0 dburger    (501) staff       (20)      653 2023-03-17 11:36:18.841866 bc_time-6.0.0/setup.cfg
--rw-r--r--   0 dburger    (501) staff       (20)       38 2022-05-30 08:48:56.000000 bc_time-6.0.0/setup.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-03-17 11:36:18.830326 bc_time-6.0.0/src/
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-03-17 11:36:18.831919 bc_time-6.0.0/src/bc_time/
--rw-r--r--   0 dburger    (501) staff       (20)      932 2022-09-08 09:24:55.000000 bc_time-6.0.0/src/bc_time/__init__.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-03-17 11:36:18.832788 bc_time-6.0.0/src/bc_time/api/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-30 07:05:50.000000 bc_time-6.0.0/src/bc_time/api/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)    10300 2023-03-17 11:28:56.000000 bc_time-6.0.0/src/bc_time/api/api.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-03-17 11:36:18.833127 bc_time-6.0.0/src/bc_time/api/constants/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:26:48.000000 bc_time-6.0.0/src/bc_time/api/constants/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)      316 2023-03-17 10:38:21.000000 bc_time-6.0.0/src/bc_time/api/constants/api.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-03-17 11:36:18.834901 bc_time-6.0.0/src/bc_time/api/enumerators/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:26:53.000000 bc_time-6.0.0/src/bc_time/api/enumerators/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)      127 2022-09-01 13:03:48.000000 bc_time-6.0.0/src/bc_time/api/enumerators/api_authorisation_type.py
--rw-r--r--   0 dburger    (501) staff       (20)      800 2022-09-08 09:24:55.000000 bc_time-6.0.0/src/bc_time/api/enumerators/content_type.py
--rw-r--r--   0 dburger    (501) staff       (20)      118 2022-07-13 12:37:22.000000 bc_time-6.0.0/src/bc_time/api/enumerators/device_communication_type.py
--rw-r--r--   0 dburger    (501) staff       (20)      883 2023-03-17 11:21:31.000000 bc_time-6.0.0/src/bc_time/api/enumerators/request_status.py
--rw-r--r--   0 dburger    (501) staff       (20)       96 2022-05-30 10:21:47.000000 bc_time-6.0.0/src/bc_time/api/enumerators/status.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-03-17 11:36:18.838672 bc_time-6.0.0/src/bc_time/api/objects/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-30 07:57:56.000000 bc_time-6.0.0/src/bc_time/api/objects/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)      780 2023-03-17 11:22:52.000000 bc_time-6.0.0/src/bc_time/api/objects/api_authorisations.py
--rw-r--r--   0 dburger    (501) staff       (20)      239 2022-06-08 10:01:59.000000 bc_time-6.0.0/src/bc_time/api/objects/base.py
--rw-r--r--   0 dburger    (501) staff       (20)      400 2022-09-01 12:52:18.000000 bc_time-6.0.0/src/bc_time/api/objects/branches.py
--rw-r--r--   0 dburger    (501) staff       (20)     1312 2022-06-10 09:39:34.000000 bc_time-6.0.0/src/bc_time/api/objects/company_profiles.py
--rw-r--r--   0 dburger    (501) staff       (20)      407 2022-09-01 12:52:56.000000 bc_time-6.0.0/src/bc_time/api/objects/controllers.py
--rw-r--r--   0 dburger    (501) staff       (20)      339 2022-09-08 09:24:55.000000 bc_time-6.0.0/src/bc_time/api/objects/daily_overtime_data.py
--rw-r--r--   0 dburger    (501) staff       (20)      407 2022-09-01 13:12:19.000000 bc_time-6.0.0/src/bc_time/api/objects/departments.py
--rw-r--r--   0 dburger    (501) staff       (20)      399 2022-09-01 12:53:07.000000 bc_time-6.0.0/src/bc_time/api/objects/devices.py
--rw-r--r--   0 dburger    (501) staff       (20)      413 2022-09-01 12:53:22.000000 bc_time-6.0.0/src/bc_time/api/objects/employee_leave.py
--rw-r--r--   0 dburger    (501) staff       (20)      403 2022-09-29 07:57:01.000000 bc_time-6.0.0/src/bc_time/api/objects/employees.py
--rw-r--r--   0 dburger    (501) staff       (20)     1294 2022-06-08 10:01:52.000000 bc_time-6.0.0/src/bc_time/api/objects/group_base.py
--rw-r--r--   0 dburger    (501) staff       (20)      817 2022-09-01 12:12:32.000000 bc_time-6.0.0/src/bc_time/api/objects/object_base_read.py
--rw-r--r--   0 dburger    (501) staff       (20)      965 2022-09-01 12:12:38.000000 bc_time-6.0.0/src/bc_time/api/objects/object_base_write.py
--rw-r--r--   0 dburger    (501) staff       (20)      362 2022-06-08 10:35:28.000000 bc_time-6.0.0/src/bc_time/api/objects/settings.py
--rw-r--r--   0 dburger    (501) staff       (20)      556 2022-09-01 12:54:17.000000 bc_time-6.0.0/src/bc_time/api/objects/visitor_groups.py
--rw-r--r--   0 dburger    (501) staff       (20)      401 2022-09-01 12:54:29.000000 bc_time-6.0.0/src/bc_time/api/objects/visitors.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-03-17 11:36:18.838903 bc_time-6.0.0/src/bc_time/oauth2/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:27:12.000000 bc_time-6.0.0/src/bc_time/oauth2/__init__.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-03-17 11:36:18.839198 bc_time-6.0.0/src/bc_time/oauth2/constants/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:27:17.000000 bc_time-6.0.0/src/bc_time/oauth2/constants/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)      257 2023-01-31 17:27:38.000000 bc_time-6.0.0/src/bc_time/oauth2/constants/grant_type.py
--rw-r--r--   0 dburger    (501) staff       (20)     6110 2023-03-17 11:33:47.000000 bc_time-6.0.0/src/bc_time/oauth2/token.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-03-17 11:36:18.839612 bc_time-6.0.0/src/bc_time/requests/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:27:26.000000 bc_time-6.0.0/src/bc_time/requests/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)      513 2022-09-07 09:21:24.000000 bc_time-6.0.0/src/bc_time/requests/base.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-03-17 11:36:18.840083 bc_time-6.0.0/src/bc_time/system/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-20 14:56:44.000000 bc_time-6.0.0/src/bc_time/system/__init__.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-03-17 11:36:18.840483 bc_time-6.0.0/src/bc_time/system/constants/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 14:36:08.000000 bc_time-6.0.0/src/bc_time/system/constants/__init__.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-03-17 11:36:18.840662 bc_time-6.0.0/src/bc_time/system/constants/datetime/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 14:35:09.000000 bc_time-6.0.0/src/bc_time/system/constants/datetime/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)       78 2022-05-18 10:11:58.000000 bc_time-6.0.0/src/bc_time/system/constants/datetime/format.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-03-17 11:36:18.841067 bc_time-6.0.0/src/bc_time/system/constants/encryption/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-09-02 13:20:51.000000 bc_time-6.0.0/src/bc_time/system/constants/encryption/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)       47 2022-08-30 08:08:54.000000 bc_time-6.0.0/src/bc_time/system/constants/encryption/crypt.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-03-17 11:36:18.841372 bc_time-6.0.0/src/bc_time/system/encryption/
--rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-20 14:56:50.000000 bc_time-6.0.0/src/bc_time/system/encryption/__init__.py
--rw-r--r--   0 dburger    (501) staff       (20)     4759 2022-10-18 13:53:04.000000 bc_time-6.0.0/src/bc_time/system/encryption/crypt.py
--rw-r--r--   0 dburger    (501) staff       (20)      473 2022-05-19 07:56:45.000000 bc_time-6.0.0/src/bc_time/system/validate.py
-drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-03-17 11:36:18.832589 bc_time-6.0.0/src/bc_time.egg-info/
--rw-r--r--   0 dburger    (501) staff       (20)     4070 2023-03-17 11:36:18.000000 bc_time-6.0.0/src/bc_time.egg-info/PKG-INFO
--rw-r--r--   0 dburger    (501) staff       (20)     1901 2023-03-17 11:36:18.000000 bc_time-6.0.0/src/bc_time.egg-info/SOURCES.txt
--rw-r--r--   0 dburger    (501) staff       (20)        1 2023-03-17 11:36:18.000000 bc_time-6.0.0/src/bc_time.egg-info/dependency_links.txt
--rw-r--r--   0 dburger    (501) staff       (20)       22 2023-03-17 11:36:18.000000 bc_time-6.0.0/src/bc_time.egg-info/requires.txt
--rw-r--r--   0 dburger    (501) staff       (20)        8 2023-03-17 11:36:18.000000 bc_time-6.0.0/src/bc_time.egg-info/top_level.txt
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:49:12.070670 bc_time-7.0.0/
+-rw-r--r--   0 dburger    (501) staff       (20)     1067 2022-05-24 07:44:21.000000 bc_time-7.0.0/LICENSE.txt
+-rw-r--r--   0 dburger    (501) staff       (20)     4989 2023-04-17 10:49:12.070715 bc_time-7.0.0/PKG-INFO
+-rw-r--r--   0 dburger    (501) staff       (20)     4496 2023-04-17 10:41:31.000000 bc_time-7.0.0/README.md
+-rw-r--r--   0 dburger    (501) staff       (20)      653 2023-04-17 10:49:12.070952 bc_time-7.0.0/setup.cfg
+-rw-r--r--   0 dburger    (501) staff       (20)       38 2022-05-30 08:48:56.000000 bc_time-7.0.0/setup.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:49:12.059985 bc_time-7.0.0/src/
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:49:12.061263 bc_time-7.0.0/src/bc_time/
+-rw-r--r--   0 dburger    (501) staff       (20)      932 2022-09-08 09:24:55.000000 bc_time-7.0.0/src/bc_time/__init__.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:49:12.062171 bc_time-7.0.0/src/bc_time/api/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-30 07:05:50.000000 bc_time-7.0.0/src/bc_time/api/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)    10300 2023-03-17 11:28:56.000000 bc_time-7.0.0/src/bc_time/api/api.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:49:12.062516 bc_time-7.0.0/src/bc_time/api/constants/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:26:48.000000 bc_time-7.0.0/src/bc_time/api/constants/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)      316 2023-03-17 10:38:21.000000 bc_time-7.0.0/src/bc_time/api/constants/api.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:49:12.063796 bc_time-7.0.0/src/bc_time/api/enumerators/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:26:53.000000 bc_time-7.0.0/src/bc_time/api/enumerators/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)      127 2022-09-01 13:03:48.000000 bc_time-7.0.0/src/bc_time/api/enumerators/api_authorisation_type.py
+-rw-r--r--   0 dburger    (501) staff       (20)      800 2022-09-08 09:24:55.000000 bc_time-7.0.0/src/bc_time/api/enumerators/content_type.py
+-rw-r--r--   0 dburger    (501) staff       (20)      118 2022-07-13 12:37:22.000000 bc_time-7.0.0/src/bc_time/api/enumerators/device_communication_type.py
+-rw-r--r--   0 dburger    (501) staff       (20)      883 2023-03-24 14:21:28.000000 bc_time-7.0.0/src/bc_time/api/enumerators/request_status.py
+-rw-r--r--   0 dburger    (501) staff       (20)       96 2022-05-30 10:21:47.000000 bc_time-7.0.0/src/bc_time/api/enumerators/status.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:49:12.068095 bc_time-7.0.0/src/bc_time/api/objects/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-30 07:57:56.000000 bc_time-7.0.0/src/bc_time/api/objects/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)      780 2023-03-17 11:22:52.000000 bc_time-7.0.0/src/bc_time/api/objects/api_authorisations.py
+-rw-r--r--   0 dburger    (501) staff       (20)      239 2022-06-08 10:01:59.000000 bc_time-7.0.0/src/bc_time/api/objects/base.py
+-rw-r--r--   0 dburger    (501) staff       (20)      400 2022-09-01 12:52:18.000000 bc_time-7.0.0/src/bc_time/api/objects/branches.py
+-rw-r--r--   0 dburger    (501) staff       (20)     1312 2022-06-10 09:39:34.000000 bc_time-7.0.0/src/bc_time/api/objects/company_profiles.py
+-rw-r--r--   0 dburger    (501) staff       (20)      407 2022-09-01 12:52:56.000000 bc_time-7.0.0/src/bc_time/api/objects/controllers.py
+-rw-r--r--   0 dburger    (501) staff       (20)      339 2022-09-08 09:24:55.000000 bc_time-7.0.0/src/bc_time/api/objects/daily_overtime_data.py
+-rw-r--r--   0 dburger    (501) staff       (20)      407 2022-09-01 13:12:19.000000 bc_time-7.0.0/src/bc_time/api/objects/departments.py
+-rw-r--r--   0 dburger    (501) staff       (20)      399 2022-09-01 12:53:07.000000 bc_time-7.0.0/src/bc_time/api/objects/devices.py
+-rw-r--r--   0 dburger    (501) staff       (20)      413 2022-09-01 12:53:22.000000 bc_time-7.0.0/src/bc_time/api/objects/employee_leave.py
+-rw-r--r--   0 dburger    (501) staff       (20)      403 2022-09-29 07:57:01.000000 bc_time-7.0.0/src/bc_time/api/objects/employees.py
+-rw-r--r--   0 dburger    (501) staff       (20)     1294 2022-06-08 10:01:52.000000 bc_time-7.0.0/src/bc_time/api/objects/group_base.py
+-rw-r--r--   0 dburger    (501) staff       (20)      817 2022-09-01 12:12:32.000000 bc_time-7.0.0/src/bc_time/api/objects/object_base_read.py
+-rw-r--r--   0 dburger    (501) staff       (20)      965 2022-09-01 12:12:38.000000 bc_time-7.0.0/src/bc_time/api/objects/object_base_write.py
+-rw-r--r--   0 dburger    (501) staff       (20)      362 2022-06-08 10:35:28.000000 bc_time-7.0.0/src/bc_time/api/objects/settings.py
+-rw-r--r--   0 dburger    (501) staff       (20)      556 2022-09-01 12:54:17.000000 bc_time-7.0.0/src/bc_time/api/objects/visitor_groups.py
+-rw-r--r--   0 dburger    (501) staff       (20)      401 2022-09-01 12:54:29.000000 bc_time-7.0.0/src/bc_time/api/objects/visitors.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:49:12.068314 bc_time-7.0.0/src/bc_time/oauth2/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:27:12.000000 bc_time-7.0.0/src/bc_time/oauth2/__init__.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:49:12.068499 bc_time-7.0.0/src/bc_time/oauth2/constants/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:27:17.000000 bc_time-7.0.0/src/bc_time/oauth2/constants/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)      258 2023-04-17 10:31:54.000000 bc_time-7.0.0/src/bc_time/oauth2/constants/grant_type.py
+-rw-r--r--   0 dburger    (501) staff       (20)     7366 2023-04-17 10:42:19.000000 bc_time-7.0.0/src/bc_time/oauth2/token.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:49:12.068684 bc_time-7.0.0/src/bc_time/requests/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 11:27:26.000000 bc_time-7.0.0/src/bc_time/requests/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)      513 2022-09-07 09:21:24.000000 bc_time-7.0.0/src/bc_time/requests/base.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:49:12.069090 bc_time-7.0.0/src/bc_time/system/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-20 14:56:44.000000 bc_time-7.0.0/src/bc_time/system/__init__.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:49:12.069505 bc_time-7.0.0/src/bc_time/system/constants/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 14:36:08.000000 bc_time-7.0.0/src/bc_time/system/constants/__init__.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:49:12.069686 bc_time-7.0.0/src/bc_time/system/constants/datetime/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-23 14:35:09.000000 bc_time-7.0.0/src/bc_time/system/constants/datetime/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)       78 2022-05-18 10:11:58.000000 bc_time-7.0.0/src/bc_time/system/constants/datetime/format.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:49:12.070142 bc_time-7.0.0/src/bc_time/system/constants/encryption/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-09-02 13:20:51.000000 bc_time-7.0.0/src/bc_time/system/constants/encryption/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)       47 2022-08-30 08:08:54.000000 bc_time-7.0.0/src/bc_time/system/constants/encryption/crypt.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:49:12.070438 bc_time-7.0.0/src/bc_time/system/encryption/
+-rw-r--r--   0 dburger    (501) staff       (20)        0 2022-05-20 14:56:50.000000 bc_time-7.0.0/src/bc_time/system/encryption/__init__.py
+-rw-r--r--   0 dburger    (501) staff       (20)     4759 2022-10-18 13:53:04.000000 bc_time-7.0.0/src/bc_time/system/encryption/crypt.py
+-rw-r--r--   0 dburger    (501) staff       (20)      473 2022-05-19 07:56:45.000000 bc_time-7.0.0/src/bc_time/system/validate.py
+drwxr-xr-x   0 dburger    (501) staff       (20)        0 2023-04-17 10:49:12.061977 bc_time-7.0.0/src/bc_time.egg-info/
+-rw-r--r--   0 dburger    (501) staff       (20)     4989 2023-04-17 10:49:12.000000 bc_time-7.0.0/src/bc_time.egg-info/PKG-INFO
+-rw-r--r--   0 dburger    (501) staff       (20)     1901 2023-04-17 10:49:12.000000 bc_time-7.0.0/src/bc_time.egg-info/SOURCES.txt
+-rw-r--r--   0 dburger    (501) staff       (20)        1 2023-04-17 10:49:12.000000 bc_time-7.0.0/src/bc_time.egg-info/dependency_links.txt
+-rw-r--r--   0 dburger    (501) staff       (20)       22 2023-04-17 10:49:12.000000 bc_time-7.0.0/src/bc_time.egg-info/requires.txt
+-rw-r--r--   0 dburger    (501) staff       (20)        8 2023-04-17 10:49:12.000000 bc_time-7.0.0/src/bc_time.egg-info/top_level.txt
```

### Comparing `bc_time-6.0.0/LICENSE.txt` & `bc_time-7.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bc_time-6.0.0/PKG-INFO` & `bc_time-7.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bc_time
-Version: 6.0.0
+Version: 7.0.0
 Summary: SDK that helps with integration via the Binary City Time API.
 Home-page: https://bitbucket.org/dburger/bc_time_api_sdk/src/master/
 Author: Darius Burger
 Author-email: darius@bcity.me
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -80,14 +80,32 @@
 >>> visitors = bc_time.Visitors(api)
 >>> response_data = visitors.get_all_using_pagination()
 >>> if response_data['status'] == bc_time.RequestStatus.success:
                 for visitor in response_data['data']:
                         print(visitor)
 ~~~
 
+Using grant type, password (constant, bc_time.GrantType.CLIENT_CREDENTIALS):
+~~~
+>>> import bc_time
+>>> api = bc_time.Api(
+                client_secret = 'YOUR_CLIENT_SECRET', # If the client secret is specified in ~/.bc_time/config then this parameter can be safely omitted.
+                grant_type=bc_time.GrantType.USER_CREDENTIALS # Override grant type as specified in ~/.bc_time/config; consider using the bc_time.GrantType constant.
+        )
+>>> api.token.username = 'THE_USERNAME'
+>>> api.token.password = 'THE_PASSWORD'
+>>> token_acquired, _ = api.token.request_token()
+>>> if token_acquired:
+                employees = bc_time.Employees(api)
+                response_data = employees.get_all_using_pagination()
+                if response_data['status'] == bc_time.RequestStatus.success:
+                        for employee in response_data['data']:
+                                print(employee)
+~~~
+
 # Available enumerators
 * ApiAuthorisationType
 * DeviceCommunicationType
 * GrantType
 * RequestStatus
 * Status
```

### Comparing `bc_time-6.0.0/README.md` & `bc_time-7.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -65,14 +65,32 @@
 >>> visitors = bc_time.Visitors(api)
 >>> response_data = visitors.get_all_using_pagination()
 >>> if response_data['status'] == bc_time.RequestStatus.success:
                 for visitor in response_data['data']:
                         print(visitor)
 ~~~
 
+Using grant type, password (constant, bc_time.GrantType.CLIENT_CREDENTIALS):
+~~~
+>>> import bc_time
+>>> api = bc_time.Api(
+                client_secret = 'YOUR_CLIENT_SECRET', # If the client secret is specified in ~/.bc_time/config then this parameter can be safely omitted.
+                grant_type=bc_time.GrantType.USER_CREDENTIALS # Override grant type as specified in ~/.bc_time/config; consider using the bc_time.GrantType constant.
+        )
+>>> api.token.username = 'THE_USERNAME'
+>>> api.token.password = 'THE_PASSWORD'
+>>> token_acquired, _ = api.token.request_token()
+>>> if token_acquired:
+                employees = bc_time.Employees(api)
+                response_data = employees.get_all_using_pagination()
+                if response_data['status'] == bc_time.RequestStatus.success:
+                        for employee in response_data['data']:
+                                print(employee)
+~~~
+
 # Available enumerators
 * ApiAuthorisationType
 * DeviceCommunicationType
 * GrantType
 * RequestStatus
 * Status
```

### Comparing `bc_time-6.0.0/setup.cfg` & `bc_time-7.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bc_time
-version = 6.0.0
+version = 7.0.0
 author = Darius Burger
 author_email = darius@bcity.me
 description = SDK that helps with integration via the Binary City Time API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/dburger/bc_time_api_sdk/src/master/
 classifiers =
```

### Comparing `bc_time-6.0.0/src/bc_time/__init__.py` & `bc_time-7.0.0/src/bc_time/__init__.py`

 * *Files identical despite different names*

### Comparing `bc_time-6.0.0/src/bc_time/api/api.py` & `bc_time-7.0.0/src/bc_time/api/api.py`

 * *Files identical despite different names*

### Comparing `bc_time-6.0.0/src/bc_time/api/enumerators/content_type.py` & `bc_time-7.0.0/src/bc_time/api/enumerators/content_type.py`

 * *Files identical despite different names*

### Comparing `bc_time-6.0.0/src/bc_time/api/enumerators/request_status.py` & `bc_time-7.0.0/src/bc_time/api/enumerators/request_status.py`

 * *Files identical despite different names*

### Comparing `bc_time-6.0.0/src/bc_time/api/objects/api_authorisations.py` & `bc_time-7.0.0/src/bc_time/api/objects/api_authorisations.py`

 * *Files identical despite different names*

### Comparing `bc_time-6.0.0/src/bc_time/api/objects/company_profiles.py` & `bc_time-7.0.0/src/bc_time/api/objects/company_profiles.py`

 * *Files identical despite different names*

### Comparing `bc_time-6.0.0/src/bc_time/api/objects/group_base.py` & `bc_time-7.0.0/src/bc_time/api/objects/group_base.py`

 * *Files identical despite different names*

### Comparing `bc_time-6.0.0/src/bc_time/api/objects/object_base_read.py` & `bc_time-7.0.0/src/bc_time/api/objects/object_base_read.py`

 * *Files identical despite different names*

### Comparing `bc_time-6.0.0/src/bc_time/api/objects/object_base_write.py` & `bc_time-7.0.0/src/bc_time/api/objects/object_base_write.py`

 * *Files identical despite different names*

### Comparing `bc_time-6.0.0/src/bc_time/api/objects/visitor_groups.py` & `bc_time-7.0.0/src/bc_time/api/objects/visitor_groups.py`

 * *Files identical despite different names*

### Comparing `bc_time-6.0.0/src/bc_time/oauth2/token.py` & `bc_time-7.0.0/src/bc_time/oauth2/token.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     # Public
     client_id = None
     client_secret = None
     crypt_key = None
     grant_type = None
     code = None
     private_key_file_path = None
+    username = None
+    password = None
     token = None
     token_expire_as_str = None # This will be stored in UTC.
 
     @property
     def crypt(self) -> Crypt:
         if self.__crypt is None:
             self.__crypt = Crypt(key=self.crypt_key)
@@ -42,51 +44,65 @@
         self.crypt_key = crypt_key
         self.grant_type = grant_type
         self.code = code
         self.private_key_file_path = private_key_file_path
         self.__oauth2_token_url = oauth2_token_url
 
     def request_token(self) -> tuple[bool, dict]:
-        if self.__has_valid_token():
-            return True, None
-        if not self.__validate_data():
-            return False, None
-        data = self.__get_data()
-        if data is None:
-            return False, None
-        request_response = requests_post(
-            url=self.__oauth2_token_url,
-            data=data
-        )
-        if request_response.status_code != requests_status_codes.ok:
-            return False, None
-        response_data = self._get_response_data(request_response.text)
-        if not set(('access_token', 'expires_in')).issubset(response_data.keys()):
-            return False, response_data
-        self.token = response_data['access_token']
-        token_expire = datetime.now(timezone.utc) + timedelta(seconds=response_data['expires_in'])
-        self.token_expire_as_str = token_expire.strftime(DateTimeFormat.MY_SQL_DATE_TIME)
-        return True, response_data
+        try:
+            if self.__has_valid_token():
+                return True, None
+            if not self.__validate_data():
+                return False, None
+            data = self.__get_data()
+            if data is None:
+                return False, None
+            request_response = requests_post(
+                url=self.__oauth2_token_url,
+                data=data
+            )
+            if request_response.status_code != requests_status_codes.ok:
+                return False, None
+            response_data = self._get_response_data(request_response.text)
+            if not set(('access_token', 'expires_in')).issubset(response_data.keys()):
+                return False, response_data
+            self.token = response_data['access_token']
+            token_expire = datetime.now(timezone.utc) + timedelta(seconds=response_data['expires_in'])
+            self.token_expire_as_str = token_expire.strftime(DateTimeFormat.MY_SQL_DATE_TIME)
+            return True, response_data
+        finally:
+            # Clear up sensitive user credentials.
+            if self.username is not None:
+                self.username = None
+            if self.password is not None:
+                self.password = None
 
     def __has_valid_token(self) -> bool:
         if self.token is None or self.token_expire_as_str is None:
             return False
         now = datetime.now(timezone.utc)
         return self.token_expire_as_str > now.strftime(DateTimeFormat.MY_SQL_DATE_TIME)
 
     def __validate_data(self) -> bool:
         if self.__oauth2_token_url is None:
             return False
+        data = ()
         if self.grant_type == OAuth2GrantType.AUTH_CODE:
-            return self.client_id is not None and self.client_secret is not None and self.code is not None
+            data = (self.client_id, self.client_secret, self.code)
         elif self.grant_type == OAuth2GrantType.CLIENT_CREDENTIALS:
-            return self.client_id is not None and self.client_secret is not None
+            data = (self.client_id, self.client_secret)
         elif self.grant_type == OAuth2GrantType.JWT_BEARER:
-            return self.client_id is not None and self.private_key_file_path is not None
-        return False
+            data = (self.client_id, self.private_key_file_path)
+        elif self.grant_type == OAuth2GrantType.USER_CREDENTIALS:
+            data = (self.client_id, self.client_secret, self.username, self.password)
+        # We don't expect this to ever be true, but if it is, let's rather be sceptical.
+        if not data:
+            return False
+        none_values = [value for value in data if value is None] # Grab all values that are None.
+        return len(none_values) == 0 # We want no data to be None.
 
     def __get_data(self) -> dict:
         if self.grant_type == OAuth2GrantType.AUTH_CODE:
             return {
                 'grant_type': self.grant_type,
                 'client_id': self.client_id,
                 'client_secret': self.__get_client_secret(),
@@ -99,14 +115,22 @@
                 'client_secret': self.__get_client_secret(),
             }
         elif self.grant_type == OAuth2GrantType.JWT_BEARER:
             return {
                 'grant_type': self.grant_type,
                 'assertion': self.__get_jwt_assertion(),
             }
+        elif self.grant_type == OAuth2GrantType.USER_CREDENTIALS:
+            return {
+                'grant_type': self.grant_type,
+                'client_id': self.client_id,
+                'client_secret': self.__get_client_secret(),
+                'username': self.username,
+                'password': self.__get_password(),
+            }
 
     def __get_client_secret(self) -> str:
         if self.crypt_key is not None:
             self.crypt.data = self.client_secret
             return self.crypt.encrypt()
         return self.client_secret
 
@@ -138,8 +162,14 @@
             )
         sign_data = separator.join(assertion_data)
         signature = private_key.sign(
             data=bytes(sign_data, 'utf8'),
             padding=padding.PKCS1v15(),
             algorithm=hashes.SHA1()
         )
-        return str(b64encode(signature), 'utf8')
+        return str(b64encode(signature), 'utf8')
+
+    def __get_password(self) -> str:
+        if self.crypt_key is not None:
+            self.crypt.data = self.password
+            return self.crypt.encrypt()
+        return self.password
```

### Comparing `bc_time-6.0.0/src/bc_time/requests/base.py` & `bc_time-7.0.0/src/bc_time/requests/base.py`

 * *Files identical despite different names*

### Comparing `bc_time-6.0.0/src/bc_time/system/encryption/crypt.py` & `bc_time-7.0.0/src/bc_time/system/encryption/crypt.py`

 * *Files identical despite different names*

### Comparing `bc_time-6.0.0/src/bc_time.egg-info/PKG-INFO` & `bc_time-7.0.0/src/bc_time.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bc-time
-Version: 6.0.0
+Version: 7.0.0
 Summary: SDK that helps with integration via the Binary City Time API.
 Home-page: https://bitbucket.org/dburger/bc_time_api_sdk/src/master/
 Author: Darius Burger
 Author-email: darius@bcity.me
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -80,14 +80,32 @@
 >>> visitors = bc_time.Visitors(api)
 >>> response_data = visitors.get_all_using_pagination()
 >>> if response_data['status'] == bc_time.RequestStatus.success:
                 for visitor in response_data['data']:
                         print(visitor)
 ~~~
 
+Using grant type, password (constant, bc_time.GrantType.CLIENT_CREDENTIALS):
+~~~
+>>> import bc_time
+>>> api = bc_time.Api(
+                client_secret = 'YOUR_CLIENT_SECRET', # If the client secret is specified in ~/.bc_time/config then this parameter can be safely omitted.
+                grant_type=bc_time.GrantType.USER_CREDENTIALS # Override grant type as specified in ~/.bc_time/config; consider using the bc_time.GrantType constant.
+        )
+>>> api.token.username = 'THE_USERNAME'
+>>> api.token.password = 'THE_PASSWORD'
+>>> token_acquired, _ = api.token.request_token()
+>>> if token_acquired:
+                employees = bc_time.Employees(api)
+                response_data = employees.get_all_using_pagination()
+                if response_data['status'] == bc_time.RequestStatus.success:
+                        for employee in response_data['data']:
+                                print(employee)
+~~~
+
 # Available enumerators
 * ApiAuthorisationType
 * DeviceCommunicationType
 * GrantType
 * RequestStatus
 * Status
```

### Comparing `bc_time-6.0.0/src/bc_time.egg-info/SOURCES.txt` & `bc_time-7.0.0/src/bc_time.egg-info/SOURCES.txt`

 * *Files identical despite different names*

