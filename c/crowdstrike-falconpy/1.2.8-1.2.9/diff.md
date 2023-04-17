# Comparing `tmp/crowdstrike-falconpy-1.2.8.tar.gz` & `tmp/crowdstrike-falconpy-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdstrike-falconpy-1.2.8.tar", last modified: Fri Dec 23 13:03:27 2022, max compression
+gzip compressed data, was "crowdstrike-falconpy-1.2.9.tar", last modified: Wed Jan  4 05:06:18 2023, max compression
```

## Comparing `crowdstrike-falconpy-1.2.8.tar` & `crowdstrike-falconpy-1.2.9.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:03:27.241683 crowdstrike-falconpy-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    31814 2022-12-23 13:03:27.241683 crowdstrike-falconpy-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30050 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-23 13:03:27.241683 crowdstrike-falconpy-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:03:27.217695 crowdstrike-falconpy-1.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:03:27.221693 crowdstrike-falconpy-1.2.8/src/crowdstrike_falconpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31814 2022-12-23 13:03:27.000000 crowdstrike-falconpy-1.2.8/src/crowdstrike_falconpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2022-12-23 13:03:27.000000 crowdstrike-falconpy-1.2.8/src/crowdstrike_falconpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 13:03:27.000000 crowdstrike-falconpy-1.2.8/src/crowdstrike_falconpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2022-12-23 13:03:27.000000 crowdstrike-falconpy-1.2.8/src/crowdstrike_falconpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-23 13:03:27.000000 crowdstrike-falconpy-1.2.8/src/crowdstrike_falconpy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:03:27.233687 crowdstrike-falconpy-1.2.8/src/falconpy/
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_base_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_container_base_url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:03:27.237685 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_cloud_connect_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    24875 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_cspm_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13488 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_custom_ioa.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_d4c_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_detects.py
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_device_control_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_discover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_event_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)    12391 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_falcon_complete_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_falcon_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12780 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_falconx_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_filevantage.py
--rw-r--r--   0 runner    (1001) docker     (123)    23292 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_firewall_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    10008 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_firewall_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_host_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10176 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_identity_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_incidents.py
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_installation_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)    20988 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_intel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_ioa_exclusions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13556 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_iocs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10743 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_kubernetes_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_malquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_message_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_ml_exclusions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_mobile_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_mssp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12911 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_ods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_overwatch_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_prevention_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_quarantine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_quick_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    24729 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_real_time_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16057 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_real_time_response_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17745 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_recon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_report_executions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_response_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    11813 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_sample_uploads.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_scheduled_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_sensor_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    15516 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_sensor_update_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_sensor_visibility_exclusions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_spotlight_evaluation_logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_spotlight_vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_tailored_intelligence.py
--rw-r--r--   0 runner    (1001) docker     (123)    15659 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_user_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_zero_trust_assessment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:03:27.241683 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13207 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_custom_ioa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_discover.py
--rw-r--r--   0 runner    (1001) docker     (123)    17702 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_firewall_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_identity_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_installation_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)    11312 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_iocs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12911 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_ods.py
--rw-r--r--   0 runner    (1001) docker     (123)    13678 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_real_time_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_real_time_response_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_report_executions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_scheduled_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 13:03:27.241683 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_cloud_connect_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_cspm_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_d4c_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_detects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_device_control_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_falconx.py
--rw-r--r--   0 runner    (1001) docker     (123)    16024 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     8462 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_host_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_incidents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_ioa.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_malquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_message_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_mssp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_ods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_prevention_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_real_time_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_recon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_response_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_sample_uploads.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_sensor_update_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_service_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_token_fail_reason.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_uber_default_preference.py
--rw-r--r--   0 runner    (1001) docker     (123)    22817 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16200 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/api_complete.py
--rw-r--r--   0 runner    (1001) docker     (123)    15709 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/cloud_connect_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    39156 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/cspm_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    33740 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/custom_ioa.py
--rw-r--r--   0 runner    (1001) docker     (123)    22512 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/d4c_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/detects.py
--rw-r--r--   0 runner    (1001) docker     (123)    23575 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/device_control_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    14382 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/discover.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/event_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)    34729 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/falcon_complete_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/falcon_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    23759 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/falconx_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/filevantage.py
--rw-r--r--   0 runner    (1001) docker     (123)    76935 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/firewall_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    19971 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/firewall_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    18631 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/host_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    27079 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/identity_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/incidents.py
--rw-r--r--   0 runner    (1001) docker     (123)    13423 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/installation_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)    30717 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/intel.py
--rw-r--r--   0 runner    (1001) docker     (123)    10491 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/ioa_exclusions.py
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13794 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/iocs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/kubernetes_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16167 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/malquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    20985 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/message_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     9946 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/ml_exclusions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/mobile_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)    42732 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/mssp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)    30144 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/ods.py
--rw-r--r--   0 runner    (1001) docker     (123)    13021 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/overwatch_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/prevention_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13564 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/quarantine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/quick_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    42242 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/real_time_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    24897 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/real_time_response_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    42718 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/recon.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/report_executions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19630 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/response_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    21814 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/sample_uploads.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/scheduled_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/sensor_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    34534 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/sensor_update_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/sensor_visibility_exclusions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/spotlight_evaluation_logic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10505 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/spotlight_vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     9645 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/tailored_intelligence.py
--rw-r--r--   0 runner    (1001) docker     (123)    38033 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/user_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2022-12-23 13:03:19.000000 crowdstrike-falconpy-1.2.8/src/falconpy/zero_trust_assessment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 05:06:18.338079 crowdstrike-falconpy-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    31814 2023-01-04 05:06:18.338079 crowdstrike-falconpy-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30050 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-04 05:06:18.338079 crowdstrike-falconpy-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 05:06:18.302079 crowdstrike-falconpy-1.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 05:06:18.306079 crowdstrike-falconpy-1.2.9/src/crowdstrike_falconpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31814 2023-01-04 05:06:18.000000 crowdstrike-falconpy-1.2.9/src/crowdstrike_falconpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-01-04 05:06:18.000000 crowdstrike-falconpy-1.2.9/src/crowdstrike_falconpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 05:06:18.000000 crowdstrike-falconpy-1.2.9/src/crowdstrike_falconpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-04 05:06:18.000000 crowdstrike-falconpy-1.2.9/src/crowdstrike_falconpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-04 05:06:18.000000 crowdstrike-falconpy-1.2.9/src/crowdstrike_falconpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 05:06:18.314079 crowdstrike-falconpy-1.2.9/src/falconpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_base_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_container_base_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 05:06:18.326079 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_cloud_connect_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24875 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_cspm_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13488 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_custom_ioa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_d4c_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_detects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_device_control_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_event_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_falcon_complete_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_falcon_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_falconx_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_filevantage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23292 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_firewall_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10008 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_firewall_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_host_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_identity_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_incidents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_installation_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20988 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_intel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_ioa_exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_iocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_kubernetes_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_malquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_message_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_ml_exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_mobile_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_mssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_ods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_overwatch_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_prevention_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_quarantine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_quick_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24729 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_real_time_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_real_time_response_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17745 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_recon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_report_executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_response_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_sample_uploads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_scheduled_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_sensor_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_sensor_update_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_sensor_visibility_exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_spotlight_evaluation_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_spotlight_vulnerabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_tailored_intelligence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15659 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_user_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_zero_trust_assessment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 05:06:18.334079 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13207 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_custom_ioa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17702 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_firewall_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_identity_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_installation_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_iocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_ods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_real_time_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_real_time_response_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_report_executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_scheduled_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 05:06:18.338079 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_cloud_connect_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_cspm_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_d4c_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_detects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_device_control_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_falconx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16024 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8462 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_host_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_incidents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_ioa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_malquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_message_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_mssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_ods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_prevention_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_real_time_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_recon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_response_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_sample_uploads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_sensor_update_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_service_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_token_fail_reason.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_uber_default_preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22936 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/api_complete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/cloud_connect_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39156 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/cspm_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33740 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/custom_ioa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22512 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/d4c_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/detects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23575 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/device_control_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14382 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/event_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34729 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/falcon_complete_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/falcon_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23759 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/falconx_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/filevantage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76935 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/firewall_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19971 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/firewall_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18631 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/host_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27079 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/identity_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/incidents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13423 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/installation_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30717 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/intel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/ioa_exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/iocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/kubernetes_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16167 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/malquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20985 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/message_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/ml_exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/mobile_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42732 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/mssp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30144 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/ods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/overwatch_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/prevention_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/quarantine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/quick_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42242 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/real_time_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24897 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/real_time_response_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42718 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/recon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/report_executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/response_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21814 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/sample_uploads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/scheduled_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/sensor_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34534 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/sensor_update_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/sensor_visibility_exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/spotlight_evaluation_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10505 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/spotlight_vulnerabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/tailored_intelligence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38033 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-01-04 05:06:07.000000 crowdstrike-falconpy-1.2.9/src/falconpy/zero_trust_assessment.py
```

### Comparing `crowdstrike-falconpy-1.2.8/AUTHORS.md` & `crowdstrike-falconpy-1.2.9/AUTHORS.md`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 + `@WDmoose` 
 + Arifur, `@arahman63`
 + `@areino`
 + `@kmccb`
 + Carlos Matos, `@carlosmmatos`
 + `@ffalor`
 + `@jmillerca`
++ `@davidt99`
 
 
 ## Sponsors
 Without the support of these executives, the FalconPy project would not have happened.
 
 | Name | Role |
 | :-- | :-- |
```

### Comparing `crowdstrike-falconpy-1.2.8/LICENSE` & `crowdstrike-falconpy-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/PKG-INFO` & `crowdstrike-falconpy-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowdstrike-falconpy
-Version: 1.2.8
+Version: 1.2.9
 Summary: The CrowdStrike Falcon SDK for Python 3
 Home-page: https://github.com/CrowdStrike/falconpy
 Author: CrowdStrike
 Author-email: falconpy@crowdstrike.com
 Maintainer: Joshua Hiller
 Maintainer-email: falconpy@crowdstrike.com
 Project-URL: Documentation, https://www.falconpy.io
```

### Comparing `crowdstrike-falconpy-1.2.8/README.md` & `crowdstrike-falconpy-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/setup.py` & `crowdstrike-falconpy-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/crowdstrike_falconpy.egg-info/PKG-INFO` & `crowdstrike-falconpy-1.2.9/src/crowdstrike_falconpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowdstrike-falconpy
-Version: 1.2.8
+Version: 1.2.9
 Summary: The CrowdStrike Falcon SDK for Python 3
 Home-page: https://github.com/CrowdStrike/falconpy
 Author: CrowdStrike
 Author-email: falconpy@crowdstrike.com
 Maintainer: Joshua Hiller
 Maintainer-email: falconpy@crowdstrike.com
 Project-URL: Documentation, https://www.falconpy.io
```

### Comparing `crowdstrike-falconpy-1.2.8/src/crowdstrike_falconpy.egg-info/SOURCES.txt` & `crowdstrike-falconpy-1.2.9/src/crowdstrike_falconpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/__init__.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_base_url.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_base_url.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_container_base_url.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_container_base_url.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/__init__.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_alerts.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_cloud_connect_aws.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_cspm_registration.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_cspm_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_custom_ioa.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_d4c_registration.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_detects.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_device_control_policies.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_device_control_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_discover.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_discover.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_event_streams.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_event_streams.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_falcon_complete_dashboard.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_falcon_complete_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_falcon_container.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_falcon_container.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_falconx_sandbox.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_falconx_sandbox.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_filevantage.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_filevantage.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_firewall_management.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_firewall_policies.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_firewall_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_host_group.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_hosts.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_identity_protection.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_incidents.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_installation_tokens.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_intel.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_intel.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_ioa_exclusions.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_ioa_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_ioc.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_iocs.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_kubernetes_protection.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_kubernetes_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_malquery.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_message_center.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_message_center.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_ml_exclusions.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_ml_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_mobile_enrollment.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_mobile_enrollment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_mssp.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_mssp.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_oauth2.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_oauth2.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_ods.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_overwatch_dashboard.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_overwatch_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_prevention_policies.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_prevention_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_quarantine.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_quarantine.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_quick_scan.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_quick_scan.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_real_time_response.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_real_time_response_admin.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_recon.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_recon.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_report_executions.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_response_policies.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_response_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_sample_uploads.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_sample_uploads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_scheduled_reports.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_sensor_download.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_sensor_download.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_sensor_update_policies.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_sensor_update_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_sensor_visibility_exclusions.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_sensor_visibility_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_spotlight_evaluation_logic.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_spotlight_evaluation_logic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_spotlight_vulnerabilities.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_spotlight_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_tailored_intelligence.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_tailored_intelligence.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_user_management.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_user_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/_zero_trust_assessment.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/_zero_trust_assessment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/__init__.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_custom_ioa.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_discover.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_discover.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_firewall_management.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_hosts.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_identity_protection.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_installation_tokens.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_ioc.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_iocs.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_ods.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_real_time_response.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_real_time_response_admin.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_report_executions.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_endpoint/deprecated/_scheduled_reports.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_endpoint/deprecated/_scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/__init__.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_alerts.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_cloud_connect_aws.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_container.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_container.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_cspm_registration.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_cspm_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_d4c_registration.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_detects.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_device_control_policy.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_device_control_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_falconx.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_falconx.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_firewall.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_firewall.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_generic.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_generic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_host_group.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_incidents.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_ioa.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_ioc.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_malquery.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_message_center.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_message_center.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_mssp.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_mssp.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_ods.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_prevention_policy.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_prevention_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_real_time_response.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_recon.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_recon.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_reports.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_response_policy.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_response_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_sample_uploads.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_sample_uploads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_payload/_sensor_update_policy.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_payload/_sensor_update_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_result.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_result.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_service_class.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_service_class.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_token_fail_reason.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_token_fail_reason.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_uber_default_preference.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_uber_default_preference.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_util.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,16 @@
             if caller.auth_object:
                 if caller.auth_object.token_expired():
                     auth_response = caller.auth_object.token()
                     if auth_response["status_code"] == 201:
                         caller.headers['Authorization'] = f"Bearer {auth_response['body']['access_token']}"
                     else:
                         caller.headers['Authorization'] = "Bearer "
+                else:
+                    caller.headers['Authorization'] = f"Bearer {caller.auth_object.token_value}"
         except AttributeError:
             pass
 
         try:
             proxy = caller.proxy
         except AttributeError:
             proxy = None
```

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/_version.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
-_VERSION = '1.2.8'
+_VERSION = '1.2.9'
 _MAINTAINER = 'Joshua Hiller'
 _AUTHOR = 'CrowdStrike'
 _AUTHOR_EMAIL = 'falconpy@crowdstrike.com'
 _CREDITS = 'CrowdStrike'
 _DESCRIPTION = "The CrowdStrike Falcon SDK for Python 3"
 _TITLE = "crowdstrike-falconpy"
 _PROJECT_URL = "https://github.com/CrowdStrike/falconpy"
```

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/alerts.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/api_complete.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/api_complete.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/cloud_connect_aws.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/cspm_registration.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/cspm_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/custom_ioa.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/d4c_registration.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/debug.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/debug.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/detects.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/device_control_policies.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/device_control_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/discover.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/discover.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/event_streams.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/event_streams.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/falcon_complete_dashboard.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/falcon_complete_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/falcon_container.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/falcon_container.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/falconx_sandbox.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/falconx_sandbox.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/filevantage.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/filevantage.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/firewall_management.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/firewall_policies.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/firewall_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/host_group.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/hosts.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/identity_protection.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/incidents.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/installation_tokens.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/intel.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/intel.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/ioa_exclusions.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/ioa_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/ioc.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/iocs.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/kubernetes_protection.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/kubernetes_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/malquery.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/message_center.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/message_center.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/ml_exclusions.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/ml_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/mobile_enrollment.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/mobile_enrollment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/mssp.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/mssp.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/oauth2.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/oauth2.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/ods.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/overwatch_dashboard.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/overwatch_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/prevention_policy.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/prevention_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/quarantine.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/quarantine.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/quick_scan.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/quick_scan.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/real_time_response.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/real_time_response_admin.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/recon.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/recon.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/report_executions.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/response_policies.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/response_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/sample_uploads.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/sample_uploads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/scheduled_reports.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/sensor_download.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/sensor_download.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/sensor_update_policy.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/sensor_update_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/sensor_visibility_exclusions.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/sensor_visibility_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/spotlight_evaluation_logic.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/spotlight_evaluation_logic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/spotlight_vulnerabilities.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/spotlight_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/tailored_intelligence.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/tailored_intelligence.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/user_management.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/user_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-1.2.8/src/falconpy/zero_trust_assessment.py` & `crowdstrike-falconpy-1.2.9/src/falconpy/zero_trust_assessment.py`

 * *Files identical despite different names*

