# Comparing `tmp/pycti-5.6.post562.tar.gz` & `tmp/pycti-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-5.6.post562.tar", last modified: Fri Mar 10 15:42:57 2023, max compression
+gzip compressed data, was "pycti-5.7.0.tar", last modified: Mon Apr 17 10:34:15 2023, max compression
```

## Comparing `pycti-5.6.post562.tar` & `pycti-5.7.0.tar`

### file list

```diff
@@ -1,70 +1,73 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-10 15:42:57.425139 pycti-5.6.post562/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-03-10 15:42:42.000000 pycti-5.6.post562/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3970 2023-03-10 15:42:57.425139 pycti-5.6.post562/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3054 2023-03-10 15:42:42.000000 pycti-5.6.post562/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-10 15:42:57.413139 pycti-5.6.post562/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3570 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-10 15:42:57.417139 pycti-5.6.post562/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27719 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6824 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-10 15:42:57.417139 pycti-5.6.post562/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    41672 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/connector/opencti_connector_helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-10 15:42:57.421139 pycti-5.6.post562/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18873 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13395 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24371 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_case.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13878 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14531 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14618 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14175 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14023 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10890 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22933 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17579 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14043 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23075 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15937 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14475 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7853 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7349 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13002 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14543 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16314 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11664 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13968 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22349 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22690 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21070 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23801 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31406 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    41821 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11361 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_stix_cyber_observable_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    63935 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18392 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14229 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17702 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-10 15:42:57.421139 pycti-5.6.post562/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3260 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    98015 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14520 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-03-10 15:42:42.000000 pycti-5.6.post562/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-10 15:42:57.417139 pycti-5.6.post562/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3970 2023-03-10 15:42:57.000000 pycti-5.6.post562/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2142 2023-03-10 15:42:57.000000 pycti-5.6.post562/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-10 15:42:57.000000 pycti-5.6.post562/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-03-10 15:42:57.000000 pycti-5.6.post562/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-03-10 15:42:57.000000 pycti-5.6.post562/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-03-10 15:42:42.000000 pycti-5.6.post562/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-03-10 15:42:57.425139 pycti-5.6.post562/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 10:34:15.564091 pycti-5.7.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-04-17 10:34:00.000000 pycti-5.7.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4051 2023-04-17 10:34:15.564091 pycti-5.7.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3141 2023-04-17 10:34:00.000000 pycti-5.7.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 10:34:15.552091 pycti-5.7.0/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3718 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 10:34:15.552091 pycti-5.7.0/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28104 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6824 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 10:34:15.556091 pycti-5.7.0/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42485 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/connector/opencti_connector_helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 10:34:15.564091 pycti-5.7.0/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18873 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13395 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24396 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23838 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23846 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13878 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14531 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14618 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14175 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14023 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10890 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24602 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22933 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17579 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14043 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23075 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15937 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14475 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7853 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7349 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13002 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14543 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16314 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12155 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13968 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22349 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22661 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20977 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23801 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32054 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41821 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    63935 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18392 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14229 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17702 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 10:34:15.564091 pycti-5.7.0/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3308 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   101748 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14520 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-04-17 10:34:00.000000 pycti-5.7.0/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-17 10:34:15.552091 pycti-5.7.0/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4051 2023-04-17 10:34:15.000000 pycti-5.7.0/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2250 2023-04-17 10:34:15.000000 pycti-5.7.0/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-17 10:34:15.000000 pycti-5.7.0/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-04-17 10:34:15.000000 pycti-5.7.0/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-04-17 10:34:15.000000 pycti-5.7.0/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-04-17 10:34:00.000000 pycti-5.7.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-04-17 10:34:15.564091 pycti-5.7.0/setup.cfg
```

### Comparing `pycti-5.6.post562/LICENSE` & `pycti-5.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/PKG-INFO` & `pycti-5.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.6.post562
+Version: 5.7.0
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,15 +27,15 @@
 # OpenCTI client for Python
 
 [![Website](https://img.shields.io/badge/website-opencti.io-blue.svg)](https://www.opencti.io)
 [![CircleCI](https://circleci.com/gh/OpenCTI-Platform/client-python.svg?style=shield)](https://circleci.com/gh/OpenCTI-Platform/client-python/tree/master)
 [![readthedocs](https://readthedocs.org/projects/opencti-client-for-python/badge/?style=flat)](https://opencti-client-for-python.readthedocs.io/en/latest/)
 [![GitHub release](https://img.shields.io/github/release/OpenCTI-Platform/client-python.svg)](https://github.com/OpenCTI-Platform/client-python/releases/latest)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/pycti.svg)](https://pypi.python.org/pypi/pycti/)
-[![Slack Status](https://slack.filigran.io/badge.svg)](https://community.filigran.io)
+[![Slack Status](https://img.shields.io/badge/slack-3K%2B%20members-4A154B)](https://community.filigran.io)
 
 The official OpenCTI Python client helps developers to use the OpenCTI API by providing easy to use methods and utils.
 This client is also used by some OpenCTI components.
 
 ## Install
 
 To install the latest Python client library, please use `pip`:
@@ -66,14 +66,20 @@
 # Push you feature/fix on Github
 $ git add [file(s)]
 $ git commit -m "[descriptive message]"
 $ git push origin [branch-name]
 # Open a pull request
 ```
 
+### Install the package locally
+
+```bash
+$ pip install -e .
+```
+
 ## Documentation
 
 ### Client usage
 
 To learn about how to use the OpenCTI Python client and read some examples and cases, refer to [the client documentation](https://opencti-client-for-python.readthedocs.io/en/latest/client_usage/getting_started.html).
 
 ### API reference
```

#### html2text {}

```diff
@@ -1,52 +1,52 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.6.post562 Summary: Python API
-client for OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-
-python Author: Filigran Author-email: contact@filigran.io Maintainer: Filigran
-License: Apache Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Information Technology Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Natural Language :: English Classifier: Natural Language :: French Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3 Classifier: Topic :: Security Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Requires-Python: >=3.7 Description-Content-Type:
-text/markdown Provides-Extra: dev Provides-Extra: doc License-File: LICENSE #
-OpenCTI client for Python [![Website](https://img.shields.io/badge/website-
-opencti.io-blue.svg)](https://www.opencti.io) [![CircleCI](https://
-circleci.com/gh/OpenCTI-Platform/client-python.svg?style=shield)](https://
-circleci.com/gh/OpenCTI-Platform/client-python/tree/master) [![readthedocs]
-(https://readthedocs.org/projects/opencti-client-for-python/badge/?style=flat)]
-(https://opencti-client-for-python.readthedocs.io/en/latest/) [![GitHub
-release](https://img.shields.io/github/release/OpenCTI-Platform/client-
-python.svg)](https://github.com/OpenCTI-Platform/client-python/releases/latest)
-[![Number of PyPI downloads](https://img.shields.io/pypi/dm/pycti.svg)](https:/
-/pypi.python.org/pypi/pycti/) [![Slack Status](https://slack.filigran.io/
-badge.svg)](https://community.filigran.io) The official OpenCTI Python client
-helps developers to use the OpenCTI API by providing easy to use methods and
-utils. This client is also used by some OpenCTI components. ## Install To
-install the latest Python client library, please use `pip`: ```bash $ pip3
-install pycti ``` ## Local development ```bash # Fork the current repository,
-then clone your fork $ git clone https://github.com/YOUR-USERNAME/client-python
-$ cd client-python $ git remote add upstream https://github.com/OpenCTI-
-Platform/client-python.git # Create a branch for your feature/fix $ git
+Metadata-Version: 2.1 Name: pycti Version: 5.7.0 Summary: Python API client for
+OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
+Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Natural Language :: English
+Classifier: Natural Language :: French Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier: Topic
+:: Security Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: doc License-File: LICENSE # OpenCTI client
+for Python [![Website](https://img.shields.io/badge/website-opencti.io-
+blue.svg)](https://www.opencti.io) [![CircleCI](https://circleci.com/gh/
+OpenCTI-Platform/client-python.svg?style=shield)](https://circleci.com/gh/
+OpenCTI-Platform/client-python/tree/master) [![readthedocs](https://
+readthedocs.org/projects/opencti-client-for-python/badge/?style=flat)](https://
+opencti-client-for-python.readthedocs.io/en/latest/) [![GitHub release](https:/
+/img.shields.io/github/release/OpenCTI-Platform/client-python.svg)](https://
+github.com/OpenCTI-Platform/client-python/releases/latest) [![Number of PyPI
+downloads](https://img.shields.io/pypi/dm/pycti.svg)](https://pypi.python.org/
+pypi/pycti/) [![Slack Status](https://img.shields.io/badge/slack-
+3K%2B%20members-4A154B)](https://community.filigran.io) The official OpenCTI
+Python client helps developers to use the OpenCTI API by providing easy to use
+methods and utils. This client is also used by some OpenCTI components. ##
+Install To install the latest Python client library, please use `pip`: ```bash
+$ pip3 install pycti ``` ## Local development ```bash # Fork the current
+repository, then clone your fork $ git clone https://github.com/YOUR-USERNAME/
+client-python $ cd client-python $ git remote add upstream https://github.com/
+OpenCTI-Platform/client-python.git # Create a branch for your feature/fix $ git
 checkout -b [branch-name] # Create a virtualenv $ python3 -m venv .venv $
 source .venv/bin/activate # Install the client-python and dependencies for the
 development and the documentation $ python3 -m pip install -e .[dev,doc] # Set
 up the git hook scripts $ pre-commit install # Create your feature/fix # Create
 tests for your changes $ pytest # Push you feature/fix on Github $ git add
 [file(s)] $ git commit -m "[descriptive message]" $ git push origin [branch-
-name] # Open a pull request ``` ## Documentation ### Client usage To learn
-about how to use the OpenCTI Python client and read some examples and cases,
-refer to [the client documentation](https://opencti-client-for-
-python.readthedocs.io/en/latest/client_usage/getting_started.html). ### API
-reference To learn about the methods available for executing queries and
-retrieving their answers, refer to [the client API Reference](https://opencti-
-client-for-python.readthedocs.io/en/latest/pycti/pycti.html). ## Tests ###
-Install dependencies ```bash $ pip install -r ./test-requirements.txt ```
-[pytest](https://docs.pytest.org/en/7.2.x/) is used to launch the tests. ###
-Launch tests #### Prerequisite Your OpenCTI API should be running. Your
-conftest.py should be configured with your API url and your token. ####
-Launching Unit tests ```bash $ pytest ./tests/01-unit/ ``` Integration testing
-```bash $ pytest ./tests/02-integration/ ``` ## About OpenCTI is a product
-designed and developed by the company [Filigran](https://www.filigran.io).
-[https://www.filigran.io/wp-content/uploads/2022/08/
+name] # Open a pull request ``` ### Install the package locally ```bash $ pip
+install -e . ``` ## Documentation ### Client usage To learn about how to use
+the OpenCTI Python client and read some examples and cases, refer to [the
+client documentation](https://opencti-client-for-python.readthedocs.io/en/
+latest/client_usage/getting_started.html). ### API reference To learn about the
+methods available for executing queries and retrieving their answers, refer to
+[the client API Reference](https://opencti-client-for-python.readthedocs.io/en/
+latest/pycti/pycti.html). ## Tests ### Install dependencies ```bash $ pip
+install -r ./test-requirements.txt ``` [pytest](https://docs.pytest.org/en/
+7.2.x/) is used to launch the tests. ### Launch tests #### Prerequisite Your
+OpenCTI API should be running. Your conftest.py should be configured with your
+API url and your token. #### Launching Unit tests ```bash $ pytest ./tests/01-
+unit/ ``` Integration testing ```bash $ pytest ./tests/02-integration/ ``` ##
+About OpenCTI is a product designed and developed by the company [Filigran]
+(https://www.filigran.io). [https://www.filigran.io/wp-content/uploads/2022/08/
 filigran_text_horizontal_dense_margin.png]
```

### Comparing `pycti-5.6.post562/README.md` & `pycti-5.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # OpenCTI client for Python
 
 [![Website](https://img.shields.io/badge/website-opencti.io-blue.svg)](https://www.opencti.io)
 [![CircleCI](https://circleci.com/gh/OpenCTI-Platform/client-python.svg?style=shield)](https://circleci.com/gh/OpenCTI-Platform/client-python/tree/master)
 [![readthedocs](https://readthedocs.org/projects/opencti-client-for-python/badge/?style=flat)](https://opencti-client-for-python.readthedocs.io/en/latest/)
 [![GitHub release](https://img.shields.io/github/release/OpenCTI-Platform/client-python.svg)](https://github.com/OpenCTI-Platform/client-python/releases/latest)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/pycti.svg)](https://pypi.python.org/pypi/pycti/)
-[![Slack Status](https://slack.filigran.io/badge.svg)](https://community.filigran.io)
+[![Slack Status](https://img.shields.io/badge/slack-3K%2B%20members-4A154B)](https://community.filigran.io)
 
 The official OpenCTI Python client helps developers to use the OpenCTI API by providing easy to use methods and utils.
 This client is also used by some OpenCTI components.
 
 ## Install
 
 To install the latest Python client library, please use `pip`:
@@ -40,14 +40,20 @@
 # Push you feature/fix on Github
 $ git add [file(s)]
 $ git commit -m "[descriptive message]"
 $ git push origin [branch-name]
 # Open a pull request
 ```
 
+### Install the package locally
+
+```bash
+$ pip install -e .
+```
+
 ## Documentation
 
 ### Client usage
 
 To learn about how to use the OpenCTI Python client and read some examples and cases, refer to [the client documentation](https://opencti-client-for-python.readthedocs.io/en/latest/client_usage/getting_started.html).
 
 ### API reference
```

#### html2text {}

```diff
@@ -3,38 +3,38 @@
 circleci.com/gh/OpenCTI-Platform/client-python.svg?style=shield)](https://
 circleci.com/gh/OpenCTI-Platform/client-python/tree/master) [![readthedocs]
 (https://readthedocs.org/projects/opencti-client-for-python/badge/?style=flat)]
 (https://opencti-client-for-python.readthedocs.io/en/latest/) [![GitHub
 release](https://img.shields.io/github/release/OpenCTI-Platform/client-
 python.svg)](https://github.com/OpenCTI-Platform/client-python/releases/latest)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/pycti.svg)](https:/
-/pypi.python.org/pypi/pycti/) [![Slack Status](https://slack.filigran.io/
-badge.svg)](https://community.filigran.io) The official OpenCTI Python client
-helps developers to use the OpenCTI API by providing easy to use methods and
-utils. This client is also used by some OpenCTI components. ## Install To
-install the latest Python client library, please use `pip`: ```bash $ pip3
-install pycti ``` ## Local development ```bash # Fork the current repository,
-then clone your fork $ git clone https://github.com/YOUR-USERNAME/client-python
-$ cd client-python $ git remote add upstream https://github.com/OpenCTI-
-Platform/client-python.git # Create a branch for your feature/fix $ git
-checkout -b [branch-name] # Create a virtualenv $ python3 -m venv .venv $
-source .venv/bin/activate # Install the client-python and dependencies for the
-development and the documentation $ python3 -m pip install -e .[dev,doc] # Set
-up the git hook scripts $ pre-commit install # Create your feature/fix # Create
-tests for your changes $ pytest # Push you feature/fix on Github $ git add
-[file(s)] $ git commit -m "[descriptive message]" $ git push origin [branch-
-name] # Open a pull request ``` ## Documentation ### Client usage To learn
-about how to use the OpenCTI Python client and read some examples and cases,
-refer to [the client documentation](https://opencti-client-for-
-python.readthedocs.io/en/latest/client_usage/getting_started.html). ### API
-reference To learn about the methods available for executing queries and
-retrieving their answers, refer to [the client API Reference](https://opencti-
-client-for-python.readthedocs.io/en/latest/pycti/pycti.html). ## Tests ###
-Install dependencies ```bash $ pip install -r ./test-requirements.txt ```
-[pytest](https://docs.pytest.org/en/7.2.x/) is used to launch the tests. ###
-Launch tests #### Prerequisite Your OpenCTI API should be running. Your
-conftest.py should be configured with your API url and your token. ####
-Launching Unit tests ```bash $ pytest ./tests/01-unit/ ``` Integration testing
-```bash $ pytest ./tests/02-integration/ ``` ## About OpenCTI is a product
-designed and developed by the company [Filigran](https://www.filigran.io).
-[https://www.filigran.io/wp-content/uploads/2022/08/
+/pypi.python.org/pypi/pycti/) [![Slack Status](https://img.shields.io/badge/
+slack-3K%2B%20members-4A154B)](https://community.filigran.io) The official
+OpenCTI Python client helps developers to use the OpenCTI API by providing easy
+to use methods and utils. This client is also used by some OpenCTI components.
+## Install To install the latest Python client library, please use `pip`:
+```bash $ pip3 install pycti ``` ## Local development ```bash # Fork the
+current repository, then clone your fork $ git clone https://github.com/YOUR-
+USERNAME/client-python $ cd client-python $ git remote add upstream https://
+github.com/OpenCTI-Platform/client-python.git # Create a branch for your
+feature/fix $ git checkout -b [branch-name] # Create a virtualenv $ python3 -
+m venv .venv $ source .venv/bin/activate # Install the client-python and
+dependencies for the development and the documentation $ python3 -m pip install
+-e .[dev,doc] # Set up the git hook scripts $ pre-commit install # Create your
+feature/fix # Create tests for your changes $ pytest # Push you feature/fix on
+Github $ git add [file(s)] $ git commit -m "[descriptive message]" $ git push
+origin [branch-name] # Open a pull request ``` ### Install the package locally
+```bash $ pip install -e . ``` ## Documentation ### Client usage To learn about
+how to use the OpenCTI Python client and read some examples and cases, refer to
+[the client documentation](https://opencti-client-for-python.readthedocs.io/en/
+latest/client_usage/getting_started.html). ### API reference To learn about the
+methods available for executing queries and retrieving their answers, refer to
+[the client API Reference](https://opencti-client-for-python.readthedocs.io/en/
+latest/pycti/pycti.html). ## Tests ### Install dependencies ```bash $ pip
+install -r ./test-requirements.txt ``` [pytest](https://docs.pytest.org/en/
+7.2.x/) is used to launch the tests. ### Launch tests #### Prerequisite Your
+OpenCTI API should be running. Your conftest.py should be configured with your
+API url and your token. #### Launching Unit tests ```bash $ pytest ./tests/01-
+unit/ ``` Integration testing ```bash $ pytest ./tests/02-integration/ ``` ##
+About OpenCTI is a product designed and developed by the company [Filigran]
+(https://www.filigran.io). [https://www.filigran.io/wp-content/uploads/2022/08/
 filigran_text_horizontal_dense_margin.png]
```

### Comparing `pycti-5.6.post562/pycti/__init__.py` & `pycti-5.7.0/pycti/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # -*- coding: utf-8 -*-
-__version__ = "5.6.post562"
+__version__ = "5.7.0"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
     get_config_variable,
 )
 from .entities.opencti_attack_pattern import AttackPattern
 from .entities.opencti_campaign import Campaign
-from .entities.opencti_case import Case
+from .entities.opencti_case_incident import CaseIncident
+from .entities.opencti_case_rfi import CaseRfi
+from .entities.opencti_case_rft import CaseRft
 from .entities.opencti_course_of_action import CourseOfAction
 from .entities.opencti_data_component import DataComponent
 from .entities.opencti_data_source import DataSource
 from .entities.opencti_external_reference import ExternalReference
+from .entities.opencti_feedback import Feedback
 from .entities.opencti_grouping import Grouping
 from .entities.opencti_identity import Identity
 from .entities.opencti_incident import Incident
 from .entities.opencti_indicator import Indicator
 from .entities.opencti_infrastructure import Infrastructure
 from .entities.opencti_intrusion_set import IntrusionSet
 from .entities.opencti_kill_chain_phase import KillChainPhase
@@ -29,44 +32,45 @@
 from .entities.opencti_marking_definition import MarkingDefinition
 from .entities.opencti_note import Note
 from .entities.opencti_observed_data import ObservedData
 from .entities.opencti_opinion import Opinion
 from .entities.opencti_report import Report
 from .entities.opencti_stix_core_relationship import StixCoreRelationship
 from .entities.opencti_stix_cyber_observable import StixCyberObservable
-from .entities.opencti_stix_cyber_observable_relationship import (
-    StixCyberObservableRelationship,
-)
 from .entities.opencti_stix_domain_object import StixDomainObject
+from .entities.opencti_stix_nested_ref_relationship import StixNestedRefRelationship
 from .entities.opencti_stix_object_or_stix_relationship import (
     StixObjectOrStixRelationship,
 )
 from .entities.opencti_stix_sighting_relationship import StixSightingRelationship
 from .entities.opencti_threat_actor import ThreatActor
 from .entities.opencti_tool import Tool
 from .entities.opencti_vulnerability import Vulnerability
 from .utils.constants import (
-    MultipleStixCyberObservableRelationship,
+    MultipleRefRelationship,
     StixCyberObservableTypes,
     StixMetaTypes,
 )
 from .utils.opencti_stix2 import OpenCTIStix2
 from .utils.opencti_stix2_splitter import OpenCTIStix2Splitter
 from .utils.opencti_stix2_update import OpenCTIStix2Update
 from .utils.opencti_stix2_utils import OpenCTIStix2Utils
 
 __all__ = [
     "AttackPattern",
     "Campaign",
-    "Case",
+    "CaseIncident",
+    "CaseRfi",
+    "CaseRft",
     "ConnectorType",
     "CourseOfAction",
     "DataComponent",
     "DataSource",
     "ExternalReference",
+    "Feedback",
     "Grouping",
     "Identity",
     "Incident",
     "Indicator",
     "Infrastructure",
     "IntrusionSet",
     "KillChainPhase",
@@ -85,19 +89,19 @@
     "OpenCTIStix2Splitter",
     "OpenCTIStix2Update",
     "OpenCTIStix2Utils",
     "Opinion",
     "Report",
     "StixCoreRelationship",
     "StixCyberObservable",
-    "StixCyberObservableRelationship",
+    "StixNestedRefRelationship",
     "StixCyberObservableTypes",
     "StixDomainObject",
     "StixMetaTypes",
-    "MultipleStixCyberObservableRelationship",
+    "MultipleRefRelationship",
     "StixObjectOrStixRelationship",
     "StixSightingRelationship",
     "ThreatActor",
     "Tool",
     "Vulnerability",
     "get_config_variable",
 ]
```

### Comparing `pycti-5.6.post562/pycti/api/opencti_api_client.py` & `pycti-5.7.0/pycti/api/opencti_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,30 @@
 from typing import Union
 
 import magic
 import requests
 import urllib3
 from pythonjsonlogger import jsonlogger
 
+from pycti import __version__
 from pycti.api import LOGGER
 from pycti.api.opencti_api_connector import OpenCTIApiConnector
 from pycti.api.opencti_api_work import OpenCTIApiWork
 from pycti.entities.opencti_attack_pattern import AttackPattern
 from pycti.entities.opencti_campaign import Campaign
-from pycti.entities.opencti_case import Case
+from pycti.entities.opencti_case_incident import CaseIncident
+from pycti.entities.opencti_case_rfi import CaseRfi
+from pycti.entities.opencti_case_rft import CaseRft
 from pycti.entities.opencti_channel import Channel
 from pycti.entities.opencti_course_of_action import CourseOfAction
 from pycti.entities.opencti_data_component import DataComponent
 from pycti.entities.opencti_data_source import DataSource
 from pycti.entities.opencti_event import Event
 from pycti.entities.opencti_external_reference import ExternalReference
+from pycti.entities.opencti_feedback import Feedback
 from pycti.entities.opencti_grouping import Grouping
 from pycti.entities.opencti_identity import Identity
 from pycti.entities.opencti_incident import Incident
 from pycti.entities.opencti_indicator import Indicator
 from pycti.entities.opencti_infrastructure import Infrastructure
 from pycti.entities.opencti_intrusion_set import IntrusionSet
 from pycti.entities.opencti_kill_chain_phase import KillChainPhase
@@ -40,18 +44,18 @@
 from pycti.entities.opencti_observed_data import ObservedData
 from pycti.entities.opencti_opinion import Opinion
 from pycti.entities.opencti_report import Report
 from pycti.entities.opencti_stix import Stix
 from pycti.entities.opencti_stix_core_object import StixCoreObject
 from pycti.entities.opencti_stix_core_relationship import StixCoreRelationship
 from pycti.entities.opencti_stix_cyber_observable import StixCyberObservable
-from pycti.entities.opencti_stix_cyber_observable_relationship import (
-    StixCyberObservableRelationship,
-)
 from pycti.entities.opencti_stix_domain_object import StixDomainObject
+from pycti.entities.opencti_stix_nested_ref_relationship import (
+    StixNestedRefRelationship,
+)
 from pycti.entities.opencti_stix_object_or_stix_relationship import (
     StixObjectOrStixRelationship,
 )
 from pycti.entities.opencti_stix_sighting_relationship import StixSightingRelationship
 from pycti.entities.opencti_threat_actor import ThreatActor
 from pycti.entities.opencti_tool import Tool
 from pycti.entities.opencti_vocabulary import Vocabulary
@@ -138,15 +142,18 @@
             logging.basicConfig(handlers=[log_handler], level=log_level, force=True)
         else:
             logging.basicConfig(level=log_level)
 
         # Define API
         self.api_token = token
         self.api_url = url + "/graphql"
-        self.request_headers = {"Authorization": "Bearer " + token}
+        self.request_headers = {
+            "User-Agent": "pycti/" + __version__,
+            "Authorization": "Bearer " + token,
+        }
         self.session = requests.session()
 
         # Define the dependencies
         self.work = OpenCTIApiWork(self)
         self.connector = OpenCTIApiConnector(self)
         self.stix2 = OpenCTIStix2(self)
 
@@ -161,23 +168,26 @@
         )
         self.stix = Stix(self)
         self.stix_domain_object = StixDomainObject(self, File)
         self.stix_core_object = StixCoreObject(self, File)
         self.stix_cyber_observable = StixCyberObservable(self, File)
         self.stix_core_relationship = StixCoreRelationship(self)
         self.stix_sighting_relationship = StixSightingRelationship(self)
-        self.stix_cyber_observable_relationship = StixCyberObservableRelationship(self)
+        self.stix_nested_ref_relationship = StixNestedRefRelationship(self)
         self.identity = Identity(self)
         self.event = Event(self)
         self.location = Location(self)
         self.threat_actor = ThreatActor(self)
         self.intrusion_set = IntrusionSet(self)
         self.infrastructure = Infrastructure(self)
         self.campaign = Campaign(self)
-        self.case = Case(self)
+        self.case_incident = CaseIncident(self)
+        self.feedback = Feedback(self)
+        self.case_rfi = CaseRfi(self)
+        self.case_rft = CaseRft(self)
         self.incident = Incident(self)
         self.malware = Malware(self)
         self.tool = Tool(self)
         self.channel = Channel(self)
         self.narrative = Narrative(self)
         self.language = Language(self)
         self.vulnerability = Vulnerability(self)
```

### Comparing `pycti-5.6.post562/pycti/api/opencti_api_connector.py` & `pycti-5.7.0/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/api/opencti_api_work.py` & `pycti-5.7.0/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/connector/opencti_connector.py` & `pycti-5.7.0/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/connector/opencti_connector_helper.py` & `pycti-5.7.0/pycti/connector/opencti_connector_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,14 +636,34 @@
         #     self.listen_stream.stop()
         self.ping.stop()
         self.api.connector.unregister(self.connector_id)
 
     def get_name(self) -> Optional[Union[bool, int, str]]:
         return self.connect_name
 
+    def get_stream_name(self):
+        if self.connect_live_stream_id is not None:
+            if self.connect_live_stream_id in ["live", "raw"]:
+                return self.connect_live_stream_id
+            else:
+                query = """
+                    query StreamCollection($id: String!) {
+                        streamCollection(id: $id)  {
+                            name
+                            description
+                            stream_live
+                            stream_public
+                        }
+                    }
+                """
+                result = self.api.query(query, {"id": self.connect_live_stream_id})
+                return result["data"]["streamCollection"]
+        else:
+            raise ValueError("This connector is not connected to any stream")
+
     def get_only_contextual(self) -> Optional[Union[bool, int, str]]:
         return self.connect_only_contextual
 
     def get_run_and_terminate(self) -> Optional[Union[bool, int, str]]:
         return self.connect_run_and_terminate
 
     def get_validate_before_import(self) -> Optional[Union[bool, int, str]]:
```

### Comparing `pycti-5.6.post562/pycti/entities/opencti_attack_pattern.py` & `pycti-5.7.0/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_campaign.py` & `pycti-5.7.0/pycti/entities/opencti_campaign.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_case.py` & `pycti-5.7.0/pycti/entities/opencti_case_rft.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-# coding: utf-8
-
-import datetime
 import json
 import uuid
 
 from dateutil.parser import parse
 from stix2.canonicalization.Canonicalize import canonicalize
 
 
-class Case:
+class CaseRft:
     def __init__(self, opencti):
         self.opencti = opencti
         self.properties = """
             id
             standard_id
             entity_type
             parent_types
@@ -108,18 +105,15 @@
             }
             revoked
             confidence
             created
             modified
             name
             description
-            case_type
-            severity
-            priority
-            rating
+            takedown_types
             objects {
                 edges {
                     node {
                         ... on BasicObject {
                             id
                             entity_type
                             parent_types
@@ -238,57 +232,55 @@
                         }
                     }
                 }
             }
         """
 
     @staticmethod
-    def generate_id(name, case_type, created):
+    def generate_id(name):
         name = name.lower().strip()
-        case_type = case_type.lower().strip()
-        if isinstance(created, datetime.datetime):
-            created = created.isoformat()
-        data = {"name": name, "case_type": case_type, "created": created}
+        data = {"name": name}
         data = canonicalize(data, utf8=False)
         id = str(uuid.uuid5(uuid.UUID("00abedb4-aa42-466c-9c01-fed23315a9b7"), data))
-        return "case--" + id
+        return "case-rft--" + id
 
     """
-        List Cases objects
-
+        List Case Rft objects
+        
         :param filters: the filters to apply
         :param search: the search keyword
         :param first: return the first n rows from the after ID (or the beginning if not set)
         :param after: ID of the first row for pagination
-        :return List of Case objects
+        :return List of Case Rft objects
     """
 
     def list(self, **kwargs):
         filters = kwargs.get("filters", None)
         search = kwargs.get("search", None)
-        first = kwargs.get("first", 100)
+        first = kwargs.get("first", 500)
         after = kwargs.get("after", None)
         order_by = kwargs.get("orderBy", None)
         order_mode = kwargs.get("orderMode", None)
         custom_attributes = kwargs.get("customAttributes", None)
         get_all = kwargs.get("getAll", False)
         with_pagination = kwargs.get("withPagination", False)
         if get_all:
-            first = 100
+            first = 500
 
         self.opencti.log(
-            "info", "Listing Cases with filters " + json.dumps(filters) + "."
+            "info",
+            "Listing Case Rfts with filters " + json.dumps(filters) + ".",
         )
         query = (
             """
-            query Cases($filters: [CasesFiltering!], $search: String, $first: Int, $after: ID, $orderBy: CasesOrdering, $orderMode: OrderingMode) {
-                cases(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
-                    edges {
-                        node {
-                            """
+                        query CaseRfts($filters: [CaseRftsFiltering!], $search: String, $first: Int, $after: ID, $orderBy: CaseRftsOrdering, $orderMode: OrderingMode) {
+                            caseRfts(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
+                                edges {
+                                    node {
+                                        """
             + (custom_attributes if custom_attributes is not None else self.properties)
             + """
                         }
                     }
                     pageInfo {
                         startCursor
                         endCursor
@@ -309,78 +301,78 @@
                 "after": after,
                 "orderBy": order_by,
                 "orderMode": order_mode,
             },
         )
         if get_all:
             final_data = []
-            data = self.opencti.process_multiple(result["data"]["cases"])
+            data = self.opencti.process_multiple(result["data"]["caseRfts"])
             final_data = final_data + data
-            while result["data"]["cases"]["pageInfo"]["hasNextPage"]:
-                after = result["data"]["cases"]["pageInfo"]["endCursor"]
-                self.opencti.log("info", "Listing Cases after " + after)
+            while result["data"]["caseRfts"]["pageInfo"]["hasNextPage"]:
+                after = result["date"]["caseRfts"]["pageInfo"]["endCursor"]
+                self.opencti.log("info", "Listing Case Rfts after " + after)
                 result = self.opencti.query(
                     query,
                     {
                         "filters": filters,
                         "search": search,
                         "first": first,
                         "after": after,
                         "orderBy": order_by,
                         "orderMode": order_mode,
                     },
                 )
-                data = self.opencti.process_multiple(result["data"]["cases"])
+                data = self.opencti.process_multiple(result["data"]["caseRfts"])
                 final_data = final_data + data
             return final_data
         else:
             return self.opencti.process_multiple(
-                result["data"]["cases"], with_pagination
+                result["data"]["caseRfts"], with_pagination
             )
 
     """
-        Read a Case object
+        Read a Case Rft object
 
-        :param id: the id of the Case
+        :param id: the id of the Case Rft
         :param filters: the filters to apply if no id provided
-        :return Case object
+        :return Case Rft object
     """
 
     def read(self, **kwargs):
         id = kwargs.get("id", None)
         filters = kwargs.get("filters", None)
         custom_attributes = kwargs.get("customAttributes", None)
         if id is not None:
-            self.opencti.log("info", "Reading Case {" + id + "}.")
+            self.opencti.log("info", "Reading Case Rft { " + id + "}.")
             query = (
                 """
-                query Case($id: String!) {
-                    case(id: $id) {
-                        """
+                            query CaseRft($id: String!) {
+                                caseRft(id: $id) {
+                                    """
                 + (
                     custom_attributes
                     if custom_attributes is not None
                     else self.properties
                 )
                 + """
                     }
                 }
             """
             )
             result = self.opencti.query(query, {"id": id})
-            return self.opencti.process_multiple_fields(result["data"]["case"])
+            return self.opencti.process_multiple_fields(result["data"]["caseRft"])
         elif filters is not None:
             result = self.list(filters=filters)
             if len(result) > 0:
                 return result[0]
             else:
                 return None
 
     """
-        Read a Case object by stix_id or name
+        Read a Case Rft object by stix_id or name
 
         :param type: the Stix-Domain-Entity type
         :param stix_id: the STIX ID of the Stix-Domain-Entity
         :param name: the name of the Stix-Domain-Entity
         :return Stix-Domain-Entity object
     """
 
@@ -400,59 +392,59 @@
                     {"key": "created_day", "values": [created_final]},
                 ],
                 customAttributes=custom_attributes,
             )
         return object_result
 
     """
-        Check if a case already contains a thing (Stix Object or Stix Relationship)
+        Check if a case rft already contains a thing (Stix Object or Stix Relationship)
 
-        :param id: the id of the Case
+        :param id: the id of the Case Rft
         :param stixObjectOrStixRelationshipId: the id of the Stix-Entity
         :return Boolean
     """
 
     def contains_stix_object_or_stix_relationship(self, **kwargs):
         id = kwargs.get("id", None)
         stix_object_or_stix_relationship_id = kwargs.get(
             "stixObjectOrStixRelationshipId", None
         )
         if id is not None and stix_object_or_stix_relationship_id is not None:
             self.opencti.log(
                 "info",
                 "Checking StixObjectOrStixRelationship {"
                 + stix_object_or_stix_relationship_id
-                + "} in Case {"
+                + "} in CaseRft {"
                 + id
                 + "}",
             )
             query = """
-                query CaseContainsStixObjectOrStixRelationship($id: String!, $stixObjectOrStixRelationshipId: String!) {
-                    caseContainsStixObjectOrStixRelationship(id: $id, stixObjectOrStixRelationshipId: $stixObjectOrStixRelationshipId)
+                query CaseRftContainsStixObjectOrStixRelationship($id: String!, $stixObjectOrStixRelationshipId: String!) {
+                    caseRftContainsStixObjectOrStixRelationship(id: $id, stixObjectOrStixRelationshipId: $stixObjectOrStixRelationshipId)
                 }
             """
             result = self.opencti.query(
                 query,
                 {
                     "id": id,
                     "stixObjectOrStixRelationshipId": stix_object_or_stix_relationship_id,
                 },
             )
-            return result["data"]["caseContainsStixObjectOrStixRelationship"]
+            return result["data"]["caseRftContainsStixObjectOrStixRelationship"]
         else:
             self.opencti.log(
                 "error",
-                "[opencti_case] Missing parameters: id or stixObjectOrStixRelationshipId",
+                "[opencti_caseRft] Missing parameters: id or stixObjectOrStixRelationshipId",
             )
 
     """
-        Create a Case object
+        Create a Case Rft object
 
-        :param name: the name of the Case
-        :return Case object
+        :param name: the name of the Case Rft
+        :return Case Rft object
     """
 
     def create(self, **kwargs):
         stix_id = kwargs.get("stix_id", None)
         created_by = kwargs.get("createdBy", None)
         objects = kwargs.get("objects", None)
         object_marking = kwargs.get("objectMarking", None)
@@ -461,27 +453,24 @@
         revoked = kwargs.get("revoked", None)
         confidence = kwargs.get("confidence", None)
         lang = kwargs.get("lang", None)
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
         description = kwargs.get("description", "")
-        case_type = kwargs.get("case_type", None)
-        severity = kwargs.get("severity", None)
-        priority = kwargs.get("priority", None)
-        rating = kwargs.get("rating", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
+        takedown_types = kwargs.get("takedown_types", None)
 
-        if name is not None and description is not None and case_type is not None:
-            self.opencti.log("info", "Creating Case {" + name + "}.")
+        if name is not None:
+            self.opencti.log("info", "Creating Case Rft {" + name + "}.")
             query = """
-                mutation CaseAdd($input: CaseAddInput!) {
-                    caseAdd(input: $input) {
+                mutation CaseRftAdd($input: CaseRftAddInput!) {
+                    caseRftAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
             """
@@ -499,55 +488,52 @@
                         "revoked": revoked,
                         "confidence": confidence,
                         "lang": lang,
                         "created": created,
                         "modified": modified,
                         "name": name,
                         "description": description,
-                        "case_type": case_type,
-                        "severity": severity,
-                        "priority": priority,
-                        "rating": rating,
                         "x_opencti_stix_ids": x_opencti_stix_ids,
                         "update": update,
+                        "takedown_types": takedown_types,
                     }
                 },
             )
-            return self.opencti.process_multiple_fields(result["data"]["caseAdd"])
+            return self.opencti.process_multiple_fields(result["data"]["caseRftAdd"])
         else:
             self.opencti.log(
                 "error",
-                "[opencti_case] Missing parameters: name and description and case_type",
+                "[opencti_caseRft] Missing parameters: name",
             )
 
-    """
-        Add a Stix-Entity object to Case object (object_refs)
+        """
+        Add a Stix-Entity object to Case Rft object (object_refs)
 
-        :param id: the id of the Case
+        :param id: the id of the Case Rft
         :param stixObjectOrStixRelationshipId: the id of the Stix-Entity
         :return Boolean
     """
 
     def add_stix_object_or_stix_relationship(self, **kwargs):
         id = kwargs.get("id", None)
         stix_object_or_stix_relationship_id = kwargs.get(
             "stixObjectOrStixRelationshipId", None
         )
         if id is not None and stix_object_or_stix_relationship_id is not None:
             self.opencti.log(
                 "info",
                 "Adding StixObjectOrStixRelationship {"
                 + stix_object_or_stix_relationship_id
-                + "} to Case {"
+                + "} to CaseRft {"
                 + id
                 + "}",
             )
             query = """
-               mutation CaseEditRelationAdd($id: ID!, $input: StixMetaRelationshipAddInput) {
-                   caseEdit(id: $id) {
+               mutation CaseRftEditRelationAdd($id: ID!, $input: StixMetaRelationshipAddInput) {
+                   caseRftEdit(id: $id) {
                         relationAdd(input: $input) {
                             id
                         }
                    }
                }
             """
             self.opencti.query(
@@ -560,43 +546,43 @@
                     },
                 },
             )
             return True
         else:
             self.opencti.log(
                 "error",
-                "[opencti_case] Missing parameters: id and stixObjectOrStixRelationshipId",
+                "[opencti_caseRft] Missing parameters: id and stixObjectOrStixRelationshipId",
             )
             return False
 
-    """
-        Remove a Stix-Entity object to Case object (object_refs)
+        """
+        Remove a Stix-Entity object to Case Rft object (object_refs)
 
-        :param id: the id of the Case
+        :param id: the id of the Case Rft
         :param stixObjectOrStixRelationshipId: the id of the Stix-Entity
         :return Boolean
     """
 
     def remove_stix_object_or_stix_relationship(self, **kwargs):
         id = kwargs.get("id", None)
         stix_object_or_stix_relationship_id = kwargs.get(
             "stixObjectOrStixRelationshipId", None
         )
         if id is not None and stix_object_or_stix_relationship_id is not None:
             self.opencti.log(
                 "info",
                 "Removing StixObjectOrStixRelationship {"
                 + stix_object_or_stix_relationship_id
-                + "} to Case {"
+                + "} to CaseRft {"
                 + id
                 + "}",
             )
             query = """
-               mutation CaseEditRelationDelete($id: ID!, $toId: StixRef!, $relationship_type: String!) {
-                   caseEdit(id: $id) {
+               mutation CaseRftEditRelationDelete($id: ID!, $toId: StixRef!, $relationship_type: String!) {
+                   caseRftEdit(id: $id) {
                         relationDelete(toId: $toId, relationship_type: $relationship_type) {
                             id
                         }
                    }
                }
             """
             self.opencti.query(
@@ -607,24 +593,24 @@
                     "relationship_type": "object",
                 },
             )
             return True
         else:
             self.opencti.log(
                 "error",
-                "[opencti_case] Missing parameters: id and stixObjectOrStixRelationshipId",
+                "[opencti_caseRft] Missing parameters: id and stixObjectOrStixRelationshipId",
             )
             return False
 
-    """
-        Import a Case object from a STIX2 object
+        """
+        Import a Case Rft object from a STIX2 object
 
-        :param stixObject: the Stix-Object Case
-        :return Case object
-    """
+        :param stixObject: the Stix-Object Case Rft
+        :return Case Rft object
+        """
 
     def import_from_stix2(self, **kwargs):
         stix_object = kwargs.get("stixObject", None)
         extras = kwargs.get("extras", {})
         update = kwargs.get("update", False)
         if stix_object is not None:
             # Search in extensions
@@ -661,23 +647,22 @@
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
                 else "",
-                case_type=stix_object["case_type"]
-                if "case_type" in stix_object
+                takedown_types=stix_object["takedown_types"]
+                if "takedown_types" in stix_object
                 else None,
-                severity=stix_object["severity"] if "severity" in stix_object else None,
-                priority=stix_object["priority"] if "priority" in stix_object else None,
-                rating=stix_object["rating"] if "rating" in stix_object else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
-            self.opencti.log("error", "[opencti_case] Missing parameters: stixObject")
+            self.opencti.log(
+                "error", "[opencti_caseRft] Missing parameters: stixObject"
+            )
```

### Comparing `pycti-5.6.post562/pycti/entities/opencti_channel.py` & `pycti-5.7.0/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_course_of_action.py` & `pycti-5.7.0/pycti/entities/opencti_course_of_action.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_data_component.py` & `pycti-5.7.0/pycti/entities/opencti_data_component.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_data_source.py` & `pycti-5.7.0/pycti/entities/opencti_data_source.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_event.py` & `pycti-5.7.0/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_external_reference.py` & `pycti-5.7.0/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_grouping.py` & `pycti-5.7.0/pycti/entities/opencti_grouping.py`

 * *Files 0% similar despite different names*

```diff
@@ -499,15 +499,15 @@
         )
         if id is not None and stix_object_or_stix_relationship_id is not None:
             LOGGER.info(
                 "Adding StixObjectOrStixRelationship {%s} to Grouping {%s}",
                 *(stix_object_or_stix_relationship_id, id),
             )
             query = """
-               mutation GroupingEditRelationAdd($id: ID!, $input: StixMetaRelationshipAddInput) {
+               mutation GroupingEditRelationAdd($id: ID!, $input: StixRefRelationshipAddInput!) {
                    groupingRelationAdd(id: $id, input: $input) {
                         id
                    }
                }
             """
             self.opencti.query(
                 query,
```

### Comparing `pycti-5.6.post562/pycti/entities/opencti_identity.py` & `pycti-5.7.0/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_incident.py` & `pycti-5.7.0/pycti/entities/opencti_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_indicator.py` & `pycti-5.7.0/pycti/entities/opencti_indicator.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_infrastructure.py` & `pycti-5.7.0/pycti/entities/opencti_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_intrusion_set.py` & `pycti-5.7.0/pycti/entities/opencti_intrusion_set.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_kill_chain_phase.py` & `pycti-5.7.0/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_label.py` & `pycti-5.7.0/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_language.py` & `pycti-5.7.0/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_location.py` & `pycti-5.7.0/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_malware.py` & `pycti-5.7.0/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_marking_definition.py` & `pycti-5.7.0/pycti/entities/opencti_marking_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,39 +233,49 @@
         :return MarkingDefinition object
     """
 
     def import_from_stix2(self, **kwargs):
         stix_object = kwargs.get("stixObject", None)
         update = kwargs.get("update", False)
         if stix_object is not None:
-            definition = None
-            definition_type = stix_object["definition_type"]
-            if stix_object["definition_type"] == "tlp":
-                definition_type = definition_type.upper()
-                if "definition" in stix_object:
-                    definition = (
-                        definition_type + ":" + stix_object["definition"]["tlp"].upper()
-                    )
-                elif "name" in stix_object:
-                    definition = stix_object["name"]
+            if (
+                "x_opencti_definition_type" in stix_object
+                and "x_opencti_definition" in stix_object
+            ):
+                definition_type = stix_object["x_opencti_definition_type"]
+                definition = stix_object["x_opencti_definition"]
             else:
-                if "definition" in stix_object:
-                    if isinstance(stix_object["definition"], str):
-                        definition = stix_object["definition"]
-                    elif (
-                        isinstance(stix_object["definition"], dict)
-                        and stix_object["definition_type"] in stix_object["definition"]
-                    ):
-                        definition = stix_object["definition"][
-                            stix_object["definition_type"]
-                        ]
-                    else:
+                definition_type = stix_object["definition_type"]
+                definition = None
+                if stix_object["definition_type"] == "tlp":
+                    definition_type = definition_type.upper()
+                    if "definition" in stix_object:
+                        definition = (
+                            definition_type
+                            + ":"
+                            + stix_object["definition"]["tlp"].upper()
+                        )
+                    elif "name" in stix_object:
+                        definition = stix_object["name"]
+                else:
+                    if "definition" in stix_object:
+                        if isinstance(stix_object["definition"], str):
+                            definition = stix_object["definition"]
+                        elif (
+                            isinstance(stix_object["definition"], dict)
+                            and stix_object["definition_type"]
+                            in stix_object["definition"]
+                        ):
+                            definition = stix_object["definition"][
+                                stix_object["definition_type"]
+                            ]
+                        else:
+                            definition = stix_object["name"]
+                    elif "name" in stix_object:
                         definition = stix_object["name"]
-                elif "name" in stix_object:
-                    definition = stix_object["name"]
 
             # Replace TLP:WHITE
             if definition == "TLP:WHITE":
                 definition = "TLP:CLEAR"
 
             # Search in extensions
             if (
```

### Comparing `pycti-5.6.post562/pycti/entities/opencti_narrative.py` & `pycti-5.7.0/pycti/entities/opencti_narrative.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_note.py` & `pycti-5.7.0/pycti/entities/opencti_note.py`

 * *Files 1% similar despite different names*

```diff
@@ -491,15 +491,15 @@
             ):
                 return True
             LOGGER.info(
                 "Adding StixObjectOrStixRelationship {%s} to Note {%s}",
                 *(stix_object_or_stix_relationship_id, id),
             )
             query = """
-               mutation NoteEdit($id: ID!, $input: StixMetaRelationshipAddInput) {
+               mutation NoteEdit($id: ID!, $input: StixRefRelationshipAddInput!) {
                    noteEdit(id: $id) {
                         relationAdd(input: $input) {
                             id
                         }
                    }
                }
             """
```

### Comparing `pycti-5.6.post562/pycti/entities/opencti_observed_data.py` & `pycti-5.7.0/pycti/entities/opencti_observed_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
                             name
                         }
                         ... on DataSource {
                             name
                         }
                         ... on Case {
                             name
-                        }                             
+                        }
                         ... on StixCoreRelationship {
                             standard_id
                             spec_version
                             created_at
                             updated_at
                         }
                     }
@@ -467,15 +467,15 @@
             ):
                 return True
             LOGGER.info(
                 "Adding StixObjectOrStixRelationship {%s} to ObservedData {%s}",
                 *(stix_object_or_stix_relationship_id, id),
             )
             query = """
-               mutation ObservedDataEdit($id: ID!, $input: StixMetaRelationshipAddInput) {
+               mutation ObservedDataEdit($id: ID!, $input: StixRefRelationshipAddInput!) {
                    observedDataEdit(id: $id) {
                         relationAdd(input: $input) {
                             id
                         }
                    }
                }
             """
```

### Comparing `pycti-5.6.post562/pycti/entities/opencti_opinion.py` & `pycti-5.7.0/pycti/entities/opencti_opinion.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
                             name
                         }
                         ... on Incident {
                             name
                         }
                         ... on Case {
                             name
-                        }                        
+                        }
                         ... on StixCoreRelationship {
                             standard_id
                             spec_version
                             created_at
                             updated_at
                             relationship_type
                         }
@@ -458,15 +458,15 @@
             ):
                 return True
             LOGGER.info(
                 "Adding StixObjectOrStixRelationship {%s} to Opinion {%s}",
                 *(stix_object_or_stix_relationship_id, id),
             )
             query = """
-               mutation OpinionEdit($id: ID!, $input: StixMetaRelationshipAddInput) {
+               mutation OpinionEdit($id: ID!, $input: StixRefRelationshipAddInput!) {
                    opinionEdit(id: $id) {
                         relationAdd(input: $input) {
                             id
                         }
                    }
                }
             """
@@ -572,17 +572,15 @@
                 created=stix_object["created"] if "created" in stix_object else None,
                 modified=stix_object["modified"] if "modified" in stix_object else None,
                 explanation=self.opencti.stix2.convert_markdown(
                     stix_object["explanation"]
                 )
                 if "explanation" in stix_object
                 else None,
-                authors=self.opencti.stix2.convert_markdown(stix_object["authors"])
-                if "authors" in stix_object
-                else None,
+                authors=stix_object["authors"] if "authors" in stix_object else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
                 opinion=stix_object["opinion"] if "opinion" in stix_object else None,
                 objectOrganization=stix_object["granted_refs"]
                 if "granted_refs" in stix_object
                 else None,
```

### Comparing `pycti-5.6.post562/pycti/entities/opencti_report.py` & `pycti-5.7.0/pycti/entities/opencti_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -525,15 +525,15 @@
         )
         if id is not None and stix_object_or_stix_relationship_id is not None:
             LOGGER.info(
                 "Adding StixObjectOrStixRelationship {%s} to Report {%s}",
                 *(stix_object_or_stix_relationship_id, id),
             )
             query = """
-               mutation ReportEditRelationAdd($id: ID!, $input: StixMetaRelationshipAddInput) {
+               mutation ReportEditRelationAdd($id: ID!, $input: StixRefRelationshipAddInput!) {
                    reportEdit(id: $id) {
                         relationAdd(input: $input) {
                             id
                         }
                    }
                }
             """
```

### Comparing `pycti-5.6.post562/pycti/entities/opencti_stix.py` & `pycti-5.7.0/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_stix_core_object.py` & `pycti-5.7.0/pycti/entities/opencti_stix_core_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,15 +419,35 @@
                                 id
                                 entity_type
                                 standard_id
                             }
                         }
                     }
                 }
-            }            
+            }
+            ... on Feedback {
+                name
+                description
+                objects {
+                    edges {
+                        node {
+                            ... on BasicObject {
+                                id
+                                entity_type
+                                standard_id
+                            }
+                            ... on BasicRelationship {
+                                id
+                                entity_type
+                                standard_id
+                            }
+                        }
+                    }
+                }
+            }      
             ... on StixCyberObservable {
                 observable_value
             }
             ... on AutonomousSystem {
                 number
                 name_alt: name
                 rir
```

### Comparing `pycti-5.6.post562/pycti/entities/opencti_stix_core_relationship.py` & `pycti-5.7.0/pycti/entities/opencti_stix_core_relationship.py`

 * *Files 1% similar despite different names*

```diff
@@ -740,15 +740,15 @@
                 return True
             else:
                 LOGGER.info(
                     "Adding Marking-Definition {%s} to Stix-Domain-Object {%s}",
                     *(marking_definition_id, id),
                 )
                 query = """
-                   mutation StixCoreRelationshipAddRelation($id: ID!, $input: StixMetaRelationshipAddInput) {
+                   mutation StixCoreRelationshipAddRelation($id: ID!, $input: StixRefRelationshipAddInput!) {
                        stixCoreRelationshipEdit(id: $id) {
                             relationAdd(input: $input) {
                                 id
                             }
                        }
                    }
                 """
@@ -827,15 +827,15 @@
                 label = self.opencti.label.create(value=label_name)
                 label_id = label["id"]
         if id is not None and label_id is not None:
             LOGGER.info(
                 "Adding label {%s} to stix-core-relationship {%s}", label_id, id
             )
             query = """
-               mutation StixCoreRelationshipAddRelation($id: ID!, $input: StixMetaRelationshipAddInput) {
+               mutation StixCoreRelationshipAddRelation($id: ID!, $input: StixRefRelationshipAddInput!) {
                    stixCoreRelationshipEdit(id: $id) {
                         relationAdd(input: $input) {
                             id
                         }
                    }
                }
             """
@@ -867,15 +867,15 @@
         external_reference_id = kwargs.get("external_reference_id", None)
         if id is not None and external_reference_id is not None:
             LOGGER.info(
                 "Adding External-Reference {%s} to stix-core-relationship {%s}",
                 *(external_reference_id, id),
             )
             query = """
-               mutation StixCoreRelationshipEditRelationAdd($id: ID!, $input: StixMetaRelationshipAddInput) {
+               mutation StixCoreRelationshipEditRelationAdd($id: ID!, $input: StixRefRelationshipAddInput!) {
                    stixCoreRelationshipEdit(id: $id) {
                         relationAdd(input: $input) {
                             id
                         }
                    }
                }
             """
@@ -945,15 +945,15 @@
         kill_chain_phase_id = kwargs.get("kill_chain_phase_id", None)
         if id is not None and kill_chain_phase_id is not None:
             LOGGER.info(
                 "Adding Kill-Chain-Phase {%s} to stix-core-relationship {%s}",
                 *(kill_chain_phase_id, id),
             )
             query = """
-               mutation StixCoreRelationshipAddRelation($id: ID!, $input: StixMetaRelationshipAddInput) {
+               mutation StixCoreRelationshipAddRelation($id: ID!, $input: StixRefRelationshipAddInput!) {
                    stixCoreRelationshipEdit(id: $id) {
                         relationAdd(input: $input) {
                             id
                         }
                    }
                }
             """
@@ -1072,15 +1072,15 @@
                         "toId": stix_domain_object["createdBy"]["id"],
                         "relationship_type": "created-by",
                     },
                 )
             if identity_id is not None:
                 # Add the new relation
                 query = """
-                    mutation StixCoreRelationshipEdit($id: ID!, $input: StixMetaRelationshipAddInput) {
+                    mutation StixCoreRelationshipEdit($id: ID!, $input: StixRefRelationshipAddInput!) {
                         stixCoreRelationshipEdit(id: $id) {
                             relationAdd(input: $input) {
                                 id
                             }
                         }
                     }
                """
```

### Comparing `pycti-5.6.post562/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-5.7.0/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1485,15 +1485,15 @@
                         "toId": stix_domain_object["createdBy"]["id"],
                         "relationship_type": "created-by",
                     },
                 )
             if identity_id is not None:
                 # Add the new relation
                 query = """
-                    mutation StixCyberObservableEdit($id: ID!, $input: StixMetaRelationshipAddInput) {
+                    mutation StixCyberObservableEdit($id: ID!, $input: StixRefRelationshipAddInput!) {
                         stixCyberObservableEdit(id: $id) {
                             relationAdd(input: $input) {
                                 id
                             }
                         }
                     }
                """
@@ -1547,15 +1547,15 @@
                 return True
             else:
                 LOGGER.info(
                     "Adding Marking-Definition {%s} to Stix-Cyber-Observable {%s}",
                     *(marking_definition_id, id),
                 )
                 query = """
-                   mutation StixCyberObservableAddRelation($id: ID!, $input: StixMetaRelationshipAddInput) {
+                   mutation StixCyberObservableAddRelation($id: ID!, $input: StixRefRelationshipAddInput!) {
                        stixCyberObservableEdit(id: $id) {
                             relationAdd(input: $input) {
                                 id
                             }
                        }
                    }
                 """
@@ -1632,15 +1632,15 @@
                 label_id = label["id"]
             else:
                 label = self.opencti.label.create(value=label_name)
                 label_id = label["id"]
         if id is not None and label_id is not None:
             LOGGER.info("Adding label {%s} to Stix-Cyber-Observable {%s}", label_id, id)
             query = """
-               mutation StixCyberObservableAddRelation($id: ID!, $input: StixMetaRelationshipAddInput) {
+               mutation StixCyberObservableAddRelation($id: ID!, $input: StixRefRelationshipAddInput!) {
                    stixCyberObservableEdit(id: $id) {
                         relationAdd(input: $input) {
                             id
                         }
                    }
                }
             """
@@ -1742,15 +1742,15 @@
                 return True
             else:
                 LOGGER.info(
                     "Adding External-Reference {%s} to Stix-Cyber-Observable {%s}",
                     *(external_reference_id, id),
                 )
                 query = """
-                   mutation StixCyberObservabletEditRelationAdd($id: ID!, $input: StixMetaRelationshipAddInput) {
+                   mutation StixCyberObservabletEditRelationAdd($id: ID!, $input: StixRefRelationshipAddInput!) {
                        stixCyberObservableEdit(id: $id) {
                             relationAdd(input: $input) {
                                 id
                             }
                        }
                    }
                 """
```

### Comparing `pycti-5.6.post562/pycti/entities/opencti_stix_cyber_observable_relationship.py` & `pycti-5.7.0/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,69 @@
 # coding: utf-8
 
 from pycti.entities import LOGGER
 
 
-class StixCyberObservableRelationship:
+class StixNestedRefRelationship:
     def __init__(self, opencti):
         self.opencti = opencti
         self.properties = """
             id
             entity_type
             parent_types
             spec_version
             created_at
             updated_at
             standard_id
             relationship_type
             start_time
             stop_time
             from {
-                ... on StixCyberObservable {
+                ... on StixObject {
+                    id
+                    standard_id
+                    entity_type
+                    parent_types
+                }
+                ... on StixCoreRelationship {
                     id
                     standard_id
                     entity_type
                     parent_types
+                } 
+                ... on StixSightingRelationship {
+                    id
+                    standard_id
+                    entity_type
+                    parent_types
+                }                 
+                ... on StixCyberObservable {
                     observable_value
                 }
             }
             to {
-                ... on StixCyberObservable {
+                ... on StixObject {
+                    id
+                    standard_id
+                    entity_type
+                    parent_types
+                }
+                ... on StixCoreRelationship {
                     id
                     standard_id
                     entity_type
                     parent_types
+                } 
+                ... on StixSightingRelationship {
+                    id
+                    standard_id
+                    entity_type
+                    parent_types
+                }                 
+                ... on StixCyberObservable {
                     observable_value
                 }
             }
         """
 
     """
         List stix_observable_relationship objects
@@ -71,21 +99,21 @@
         custom_attributes = kwargs.get("customAttributes", None)
         get_all = kwargs.get("getAll", False)
         with_pagination = kwargs.get("withPagination", False)
         if get_all:
             first = 500
 
         LOGGER.info(
-            "Listing stix_observable_relationships with {type: %s, from_id: %s, to_id: %s}",
+            "Listing stix_nested_ref_relationships with {type: %s, from_id: %s, to_id: %s}",
             *(relationship_type, from_id, to_id),
         )
         query = (
             """
-            query StixCyberObservableRelationships($elementId: String, $fromId: StixRef, $fromTypes: [String], $toId: StixRef, $toTypes: [String], $relationship_type: [String], $startTimeStart: DateTime, $startTimeStop: DateTime, $stopTimeStart: DateTime, $stopTimeStop: DateTime, $filters: [StixCyberObservableRelationshipsFiltering], $first: Int, $after: ID, $orderBy: StixCyberObservableRelationshipsOrdering, $orderMode: OrderingMode) {
-                stixCyberObservableRelationships(elementId: $elementId, fromId: $fromId, fromTypes: $fromTypes, toId: $toId, toTypes: $toTypes, relationship_type: $relationship_type, startTimeStart: $startTimeStart, startTimeStop: $startTimeStop, stopTimeStart: $stopTimeStart, stopTimeStop: $stopTimeStop, filters: $filters, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
+            query StixNestedRefRelationships($elementId: String, $fromId: StixRef, $fromTypes: [String], $toId: StixRef, $toTypes: [String], $relationship_type: [String], $startTimeStart: DateTime, $startTimeStop: DateTime, $stopTimeStart: DateTime, $stopTimeStop: DateTime, $filters: [StixRefRelationshipsFiltering], $first: Int, $after: ID, $orderBy: StixRefRelationshipsOrdering, $orderMode: OrderingMode) {
+                stixNestedRefRelationships(elementId: $elementId, fromId: $fromId, fromTypes: $fromTypes, toId: $toId, toTypes: $toTypes, relationship_type: $relationship_type, startTimeStart: $startTimeStart, startTimeStop: $startTimeStop, stopTimeStart: $stopTimeStart, stopTimeStop: $stopTimeStop, filters: $filters, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
                     edges {
                         node {
                             """
             + (custom_attributes if custom_attributes is not None else self.properties)
             + """
                         }
                     }
@@ -118,15 +146,15 @@
                 "first": first,
                 "after": after,
                 "orderBy": order_by,
                 "orderMode": order_mode,
             },
         )
         return self.opencti.process_multiple(
-            result["data"]["stixCyberObservableRelationships"], with_pagination
+            result["data"]["stixNestedRefRelationships"], with_pagination
         )
 
     """
         Read a stix_observable_relationship object
 
         :param id: the id of the stix_observable_relationship
         :param stix_id: the STIX id of the stix_observable_relationship
@@ -151,30 +179,30 @@
         stop_time_start = kwargs.get("stopTimeStart", None)
         stop_time_stop = kwargs.get("stopTimeStop", None)
         custom_attributes = kwargs.get("customAttributes", None)
         if id is not None:
             LOGGER.info("Reading stix_observable_relationship {%s}.", id)
             query = (
                 """
-                query StixCyberObservableRelationship($id: String!) {
-                    stixCyberObservableRelationship(id: $id) {
+                query StixRefRelationship($id: String!) {
+                    stixRefRelationship(id: $id) {
                         """
                 + (
                     custom_attributes
                     if custom_attributes is not None
                     else self.properties
                 )
                 + """
                     }
                 }
              """
             )
             result = self.opencti.query(query, {"id": id})
             return self.opencti.process_multiple_fields(
-                result["data"]["stixCyberObservableRelationship"]
+                result["data"]["stixRefRelationship"]
             )
         else:
             result = self.list(
                 elementId=element_id,
                 fromId=from_id,
                 toId=to_id,
                 relationship_type=relationship_type,
@@ -217,16 +245,16 @@
             relationship_type = "obs_content"
 
         LOGGER.info(
             "Creating stix_observable_relationship '%s' {%s, %s}.",
             *(relationship_type, from_id, to_id),
         )
         query = """
-                mutation StixCyberObservableRelationshipAdd($input: StixCyberObservableRelationshipAddInput!) {
-                    stixCyberObservableRelationshipAdd(input: $input) {
+                mutation StixRefRelationshipAdd($input: StixRefRelationshipAddInput!) {
+                    stixRefRelationshipAdd(input: $input) {
                         id
                         standard_id
                         entity_type
                         parent_types
                     }
                 }
                 """
@@ -246,15 +274,15 @@
                     "objectMarking": object_marking,
                     "x_opencti_stix_ids": x_opencti_stix_ids,
                     "update": update,
                 }
             },
         )
         return self.opencti.process_multiple_fields(
-            result["data"]["stixCyberObservableRelationshipAdd"]
+            result["data"]["stixRefRelationshipAdd"]
         )
 
     """
         Update a stix_observable_relationship object field
 
         :param id: the stix_observable_relationship id
         :param input: the input of the field
@@ -264,25 +292,25 @@
     def update_field(self, **kwargs):
         id = kwargs.get("id", None)
         input = kwargs.get("input", None)
         if id is not None and input is not None:
             LOGGER.info("Updating stix_observable_relationship {%s}.", id)
             query = (
                 """
-                mutation StixCyberObservableRelationshipEdit($id: ID!, $input: [EditInput]!) {
-                    stixCyberObservableRelationshipEdit(id: $id) {
+                mutation StixRefRelationshipEdit($id: ID!, $input: [EditInput]!) {
+                    stixRefRelationshipEdit(id: $id) {
                         fieldPatch(input: $input) {
                             """
                 + self.properties
                 + """
                         }
                     }
                 }
             """
             )
             result = self.opencti.query(query, {"id": id, "input": input})
             return self.opencti.process_multiple_fields(
-                result["data"]["stixCyberObservableRelationshipEdit"]["fieldPatch"]
+                result["data"]["stixRefRelationshipEdit"]["fieldPatch"]
             )
         else:
             LOGGER.error("Missing parameters: id and key and value")
             return None
```

### Comparing `pycti-5.6.post562/pycti/entities/opencti_stix_domain_object.py` & `pycti-5.7.0/pycti/entities/opencti_stix_domain_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -902,15 +902,15 @@
                         "toId": stix_domain_object["createdBy"]["id"],
                         "relationship_type": "created-by",
                     },
                 )
             if identity_id is not None:
                 # Add the new relation
                 query = """
-                    mutation StixDomainObjectEdit($id: ID!, $input: StixMetaRelationshipAddInput) {
+                    mutation StixDomainObjectEdit($id: ID!, $input: StixRefRelationshipAddInput!) {
                         stixDomainObjectEdit(id: $id) {
                             relationAdd(input: $input) {
                                 id
                             }
                         }
                     }
                """
@@ -964,15 +964,15 @@
                 return True
             else:
                 LOGGER.info(
                     "Adding Marking-Definition {%s} to Stix-Domain-Object {%s}",
                     *(marking_definition_id, id),
                 )
                 query = """
-                   mutation StixDomainObjectAddRelation($id: ID!, $input: StixMetaRelationshipAddInput) {
+                   mutation StixDomainObjectAddRelation($id: ID!, $input: StixRefRelationshipAddInput!) {
                        stixDomainObjectEdit(id: $id) {
                             relationAdd(input: $input) {
                                 id
                             }
                        }
                    }
                 """
@@ -1049,15 +1049,15 @@
                 label_id = label["id"]
             else:
                 label = self.opencti.label.create(value=label_name)
                 label_id = label["id"]
         if id is not None and label_id is not None:
             LOGGER.info("Adding label {%s} to Stix-Domain-Object {%s}", label_id, id)
             query = """
-               mutation StixDomainObjectAddRelation($id: ID!, $input: StixMetaRelationshipAddInput) {
+               mutation StixDomainObjectAddRelation($id: ID!, $input: StixRefRelationshipAddInput!) {
                    stixDomainObjectEdit(id: $id) {
                         relationAdd(input: $input) {
                             id
                         }
                    }
                }
             """
@@ -1133,15 +1133,15 @@
         external_reference_id = kwargs.get("external_reference_id", None)
         if id is not None and external_reference_id is not None:
             LOGGER.info(
                 "Adding External-Reference {%s} to Stix-Domain-Object {%s}",
                 *(external_reference_id, id),
             )
             query = """
-               mutation StixDomainObjectEditRelationAdd($id: ID!, $input: StixMetaRelationshipAddInput) {
+               mutation StixDomainObjectEditRelationAdd($id: ID!, $input: StixRefRelationshipAddInput!) {
                    stixDomainObjectEdit(id: $id) {
                         relationAdd(input: $input) {
                             id
                         }
                    }
                }
             """
@@ -1212,15 +1212,15 @@
         if id is not None and kill_chain_phase_id is not None:
             LOGGER.info(
                 "Adding Kill-Chain-Phase {%s} to Stix-Domain-Object {%s}",
                 kill_chain_phase_id,
                 id,
             )
             query = """
-               mutation StixDomainObjectAddRelation($id: ID!, $input: StixMetaRelationshipAddInput) {
+               mutation StixDomainObjectAddRelation($id: ID!, $input: StixRefRelationshipAddInput!) {
                    stixDomainObjectEdit(id: $id) {
                         relationAdd(input: $input) {
                             id
                         }
                    }
                }
             """
```

### Comparing `pycti-5.6.post562/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-5.7.0/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-5.7.0/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files 0% similar despite different names*

```diff
@@ -620,15 +620,15 @@
                 return True
             else:
                 LOGGER.info(
                     "Adding Marking-Definition {%s} to stix_sighting_relationship {%s}",
                     *(marking_definition_id, id),
                 )
                 query = """
-                   mutation StixSightingRelationshipEdit($id: ID!, $input: StixMetaRelationshipAddInput) {
+                   mutation StixSightingRelationshipEdit($id: ID!, $input: StixRefRelationshipAddInput!) {
                        stixSightingRelationshipEdit(id: $id) {
                             relationAdd(input: $input) {
                                 id
                             }
                        }
                    }
                 """
@@ -743,15 +743,15 @@
                         "toId": stix_domain_object["createdBy"]["id"],
                         "relationship_type": "created-by",
                     },
                 )
             if identity_id is not None:
                 # Add the new relation
                 query = """
-                    mutation StixSightingRelationshipEdit($id: ID!, $input: StixMetaRelationshipAddInput) {
+                    mutation StixSightingRelationshipEdit($id: ID!, $input: StixRefRelationshipAddInput!) {
                         stixSightingRelationshipEdit(id: $id) {
                             relationAdd(input: $input) {
                                 id
                             }
                         }
                     }
                """
```

### Comparing `pycti-5.6.post562/pycti/entities/opencti_threat_actor.py` & `pycti-5.7.0/pycti/entities/opencti_threat_actor.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_tool.py` & `pycti-5.7.0/pycti/entities/opencti_tool.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_vocabulary.py` & `pycti-5.7.0/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/entities/opencti_vulnerability.py` & `pycti-5.7.0/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/utils/constants.py` & `pycti-5.7.0/pycti/utils/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,26 +89,28 @@
 
     @classmethod
     def has_value(cls, value):
         lower_attr = list(map(lambda x: x.lower(), cls._value2member_map_))
         return value.lower() in lower_attr
 
 
-class MultipleStixCyberObservableRelationship(Enum):
+class MultipleRefRelationship(Enum):
     OPERATING_SYSTEM = "operating-system"
+    SAMPLE = "sample"
     CONTAINS = "contains"
     RESOLVES_TO = "obs_resolves-to"
     BELONGS_TO = "obs_belongs-to"
     TO = "to"
     CC = "cc"
     BCC = "bcc"
     ENCAPSULATES = "encapsulates"
     OPENED_CONNECTION = "opened-connection"
     CHILD = "child"
     BODY_MULTIPART = "body-multipart"
     VALUES = "values"
-    LINKED = "linked-to"
+    LINKED = "x_opencti_linked-to"
+    SERVICE_DDL = "service-dll"
 
     @classmethod
     def has_value(cls, value):
         lower_attr = list(map(lambda x: x.lower(), cls._value2member_map_))
         return value.lower() in lower_attr
```

### Comparing `pycti-5.6.post562/pycti/utils/opencti_stix2.py` & `pycti-5.7.0/pycti/utils/opencti_stix2.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from cachetools import TTLCache
 
 from pycti.api import LOGGER as API_LOGGER
 from pycti.entities.opencti_identity import Identity
 from pycti.utils.constants import (
     IdentityTypes,
     LocationTypes,
-    MultipleStixCyberObservableRelationship,
+    MultipleRefRelationship,
     StixCyberObservableTypes,
 )
 from pycti.utils.opencti_stix2_splitter import OpenCTIStix2Splitter
 from pycti.utils.opencti_stix2_update import OpenCTIStix2Update
 from pycti.utils.opencti_stix2_utils import (
     OBSERVABLES_VALUE_INT,
     STIX_CYBER_OBSERVABLE_MAPPING,
@@ -769,15 +769,18 @@
             "channel": self.opencti.channel.import_from_stix2,
             "event": self.opencti.event.import_from_stix2,
             "note": self.opencti.note.import_from_stix2,
             "observed-data": self.opencti.observed_data.import_from_stix2,
             "opinion": self.opencti.opinion.import_from_stix2,
             "report": self.opencti.report.import_from_stix2,
             "grouping": self.opencti.grouping.import_from_stix2,
-            "case": self.opencti.case.import_from_stix2,
+            "case-rfi": self.opencti.case_rfi.import_from_stix2,
+            "case-rft": self.opencti.case_rft.import_from_stix2,
+            "case-incident": self.opencti.case_incident.import_from_stix2,
+            "feedback": self.opencti.feedback.import_from_stix2,
             "course-of-action": self.opencti.course_of_action.import_from_stix2,
             "data-component": self.opencti.data_component.import_from_stix2,
             "x-mitre-data-component": self.opencti.data_component.import_from_stix2,
             "data-source": self.opencti.data_source.import_from_stix2,
             "x-mitre-data-source": self.opencti.data_source.import_from_stix2,
             "identity": self.opencti.identity.import_from_stix2,
             "indicator": self.opencti.indicator.import_from_stix2,
@@ -967,24 +970,40 @@
             for key in stix_object.keys():
                 if key not in [
                     "created_by_ref",
                     "object_marking_refs",
                     "x_opencti_created_by_ref",
                 ]:
                     if key.endswith("_ref"):
-                        relationship_type = key.replace("_ref", "").replace("_", "-")
-                        self.opencti.stix_cyber_observable_relationship.create(
+                        relationship_type = key.replace("_ref", "")
+                        if relationship_type.startswith("x_opencti_"):
+                            relationship_type = relationship_type.split(
+                                "x_opencti_", 1
+                            )[1]
+                            relationship_type = relationship_type.replace("_", "-")
+                            relationship_type = "x_opencti_" + relationship_type
+                        else:
+                            relationship_type = relationship_type.replace("_", "-")
+                        self.opencti.stix_nested_ref_relationship.create(
                             fromId=stix_observable_result["id"],
                             toId=stix_object[key],
                             relationship_type=relationship_type,
                         )
                     elif key.endswith("_refs"):
-                        relationship_type = key.replace("_refs", "").replace("_", "-")
+                        relationship_type = key.replace("_refs", "")
+                        if relationship_type.startswith("x_opencti_"):
+                            relationship_type = relationship_type.split(
+                                "x_opencti_", 1
+                            )[1]
+                            relationship_type = relationship_type.replace("_", "-")
+                            relationship_type = "x_opencti_" + relationship_type
+                        else:
+                            relationship_type = relationship_type.replace("_", "-")
                         for value in stix_object[key]:
-                            self.opencti.stix_cyber_observable_relationship.create(
+                            self.opencti.stix_nested_ref_relationship.create(
                                 fromId=stix_observable_result["id"],
                                 toId=value,
                                 relationship_type=relationship_type,
                             )
         else:
             return None
 
@@ -1461,34 +1480,70 @@
             not no_custom_attributes
             and "objects" in entity
             and len(entity["objects"]) > 0
         ):
             entity["object_refs"] = []
             objects_to_get = entity["objects"]
             for entity_object in entity["objects"]:
-                if entity["type"] == "report" and entity_object["entity_type"] not in [
-                    "Note",
-                    "Report",
-                    "Opinion",
-                ]:
+                if (
+                    entity["type"] == "report"
+                    and entity_object["entity_type"]
+                    not in [
+                        "Note",
+                        "Report",
+                        "Opinion",
+                    ]
+                    and "stix-ref-relationship" not in entity_object["parent_types"]
+                ):
                     entity["object_refs"].append(entity_object["standard_id"])
-                elif entity["type"] == "note" and entity_object["entity_type"] not in [
-                    "Note",
-                    "Opinion",
-                ]:
+                elif (
+                    entity["type"] == "note"
+                    and entity_object["entity_type"]
+                    not in [
+                        "Note",
+                        "Opinion",
+                    ]
+                    and "stix-ref-relationship" not in entity_object["parent_types"]
+                ):
+                    entity["object_refs"].append(entity_object["standard_id"])
+                elif (
+                    entity["type"] == "opinion"
+                    and entity_object["entity_type"] not in ["Opinion"]
+                    and "stix-ref-relationship" not in entity_object["parent_types"]
+                ):
+                    entity["object_refs"].append(entity_object["standard_id"])
+                elif (
+                    entity["type"] == "observed-data"
+                    and "stix-ref-relationship" not in entity_object["parent_types"]
+                ):
                     entity["object_refs"].append(entity_object["standard_id"])
-                elif entity["type"] == "opinion" and entity_object[
-                    "entity_type"
-                ] not in ["Opinion"]:
+                elif (
+                    entity["type"] == "grouping"
+                    and "stix-ref-relationship" not in entity_object["parent_types"]
+                ):
+                    entity["object_refs"].append(entity_object["standard_id"])
+                elif (
+                    entity["type"] == "case-incident"
+                    and "stix-ref-relationship" not in entity_object["parent_types"]
+                ):
                     entity["object_refs"].append(entity_object["standard_id"])
-                elif entity["type"] == "observed-data":
+                elif (
+                    entity["type"] == "feedback"
+                    and "stix-ref-relationship" not in entity_object["parent_types"]
+                ):
                     entity["object_refs"].append(entity_object["standard_id"])
-                elif entity["type"] == "grouping":
+                elif (
+                    entity["type"] == "case-rfi"
+                    and "stix-ref-relationship" not in entity_object["parent_types"]
+                ):
                     entity["object_refs"].append(entity_object["standard_id"])
-                elif entity["type"] == "case":
+                elif (
+                    entity["type"] == "case-rft"
+                    and "stix-ref-relationship" not in entity_object["parent_types"]
+                ):
                     entity["object_refs"].append(entity_object["standard_id"])
         if "objects" in entity:
             del entity["objects"]
             del entity["objectsIds"]
         # Stix Sighting Relationship
         if entity["type"] == "stix-sighting-relationship":
             entity["type"] = "sighting"
@@ -1548,81 +1603,92 @@
                         "mime_type": file["metaData"]["mimetype"],
                         "version": file["metaData"]["version"],
                     }
                 )
             del entity["importFiles"]
             del entity["importFilesIds"]
 
-        # StixCyberObservable
-        if entity["type"] in STIX_CYBER_OBSERVABLE_MAPPING:
-            stix_observable_relationships = (
-                self.opencti.stix_cyber_observable_relationship.list(
-                    fromId=entity["x_opencti_id"]
-                )
-            )
-            for stix_observable_relationship in stix_observable_relationships:
-                if "standard_id" in stix_observable_relationship["to"]:
-                    if MultipleStixCyberObservableRelationship.has_value(
-                        stix_observable_relationship["relationship_type"]
-                    ):
-                        key = (
-                            stix_observable_relationship["relationship_type"]
-                            .replace("obs_", "")
-                            .replace("-", "_")
-                            + "_refs"
-                        )
-                        if key in entity:
-                            entity[key].append(
-                                stix_observable_relationship["to"]["standard_id"]
-                            )
-                        else:
-                            entity[key] = [
-                                stix_observable_relationship["to"]["standard_id"]
-                            ]
-                    else:
-                        key = (
-                            stix_observable_relationship["relationship_type"]
-                            .replace("obs_", "")
-                            .replace("-", "_")
-                            + "_ref"
+        # StixRefRelationship
+        stix_nested_ref_relationships = self.opencti.stix_nested_ref_relationship.list(
+            fromId=entity["x_opencti_id"]
+        )
+        for stix_nested_ref_relationship in stix_nested_ref_relationships:
+            if "standard_id" in stix_nested_ref_relationship["to"]:
+                if MultipleRefRelationship.has_value(
+                    stix_nested_ref_relationship["relationship_type"]
+                ):
+                    key = (
+                        stix_nested_ref_relationship["relationship_type"]
+                        .replace("obs_", "")
+                        .replace("-", "_")
+                        + "_refs"
+                    )
+                    if key in entity:
+                        entity[key].append(
+                            stix_nested_ref_relationship["to"]["standard_id"]
                         )
-                        entity[key] = stix_observable_relationship["to"]["standard_id"]
-
+                    else:
+                        entity[key] = [
+                            stix_nested_ref_relationship["to"]["standard_id"]
+                        ]
+                else:
+                    key = (
+                        stix_nested_ref_relationship["relationship_type"]
+                        .replace("obs_", "")
+                        .replace("-", "_")
+                        + "_ref"
+                    )
+                    entity[key] = stix_nested_ref_relationship["to"]["standard_id"]
         result.append(entity)
 
         if mode == "simple":
             return result
         elif mode == "full":
             uuids = [entity["id"]]
             for x in result:
                 uuids.append(x["id"])
             # Get extra refs
             for key in entity.keys():
-                if entity["type"] in STIX_CYBER_OBSERVABLE_MAPPING:
-                    if key.endswith("_ref"):
-                        type = entity[key].split("--")[0]
+                if key.endswith("_ref"):
+                    type = entity[key].split("--")[0]
+                    if type in STIX_CYBER_OBSERVABLE_MAPPING:
+                        objects_to_get.append(
+                            {
+                                "id": entity[key],
+                                "entity_type": "Stix-Cyber-Observable",
+                                "parent_types": ["Stix-Cyber-Observable"],
+                            }
+                        )
+                    else:
+                        objects_to_get.append(
+                            {
+                                "id": entity[key],
+                                "entity_type": "Stix-Domain-Object",
+                                "parent_types": ["Stix-Domain-Object"],
+                            }
+                        )
+                elif key.endswith("_refs"):
+                    for value in entity[key]:
+                        type = value.split("--")[0]
                         if type in STIX_CYBER_OBSERVABLE_MAPPING:
                             objects_to_get.append(
                                 {
-                                    "id": entity[key],
+                                    "id": value,
                                     "entity_type": "Stix-Cyber-Observable",
-                                    "parent_types": ["Styx-Cyber-Observable"],
+                                    "parent_types": ["Stix-Cyber-Observable"],
+                                }
+                            )
+                        else:
+                            objects_to_get.append(
+                                {
+                                    "id": value,
+                                    "entity_type": "Stix-Domain-Object",
+                                    "parent_types": ["Stix-Domain-Object"],
                                 }
                             )
-                    elif key.endswith("_refs"):
-                        for value in entity[key]:
-                            type = value.split("--")[0]
-                            if type in STIX_CYBER_OBSERVABLE_MAPPING:
-                                objects_to_get.append(
-                                    {
-                                        "id": value,
-                                        "entity_type": "Stix-Cyber-Observable",
-                                        "parent_types": ["Styx-Cyber-Observable"],
-                                    }
-                                )
             # Get extra relations (from)
             stix_core_relationships = self.opencti.stix_core_relationship.list(
                 elementId=entity["x_opencti_id"]
             )
             for stix_core_relationship in stix_core_relationships:
                 if self.check_max_marking_definition(
                     max_marking_definition_entity,
@@ -1694,30 +1760,35 @@
                 "Attack-Pattern": self.opencti.attack_pattern.read,
                 "Campaign": self.opencti.campaign.read,
                 "Channel": self.opencti.channel.read,
                 "Note": self.opencti.note.read,
                 "Observed-Data": self.opencti.observed_data.read,
                 "Opinion": self.opencti.opinion.read,
                 "Report": self.opencti.report.read,
-                "Case": self.opencti.case.read,
+                "Case-Incident": self.opencti.case_incident.read,
+                "Feedback": self.opencti.feedback.read,
+                "Case-Rfi": self.opencti.case_rfi.read,
+                "Case-Rft": self.opencti.case_rft.read,
                 "Course-Of-Action": self.opencti.course_of_action.read,
                 "Data-Component": self.opencti.data_component.read,
                 "Data-Source": self.opencti.data_source.read,
                 "Identity": self.opencti.identity.read,
                 "Indicator": self.opencti.indicator.read,
                 "Infrastructure": self.opencti.infrastructure.read,
                 "Intrusion-Set": self.opencti.intrusion_set.read,
                 "Location": self.opencti.location.read,
                 "Language": self.opencti.language.read,
                 "Malware": self.opencti.malware.read,
                 "Threat-Actor": self.opencti.threat_actor.read,
                 "Tool": self.opencti.tool.read,
                 "Vulnerability": self.opencti.vulnerability.read,
                 "Incident": self.opencti.incident.read,
+                "Stix-Core-Object": self.opencti.stix_core_object.read,
                 "Stix-Cyber-Observable": self.opencti.stix_cyber_observable.read,
+                "Stix-Domain-Object": self.opencti.stix_domain_object.read,
                 "stix-core-relationship": self.opencti.stix_core_relationship.read,
                 "stix-sighting-relationship": self.opencti.stix_sighting_relationship.read,
             }
             # Get extra objects
             for entity_object in objects_to_get:
                 # Map types
                 if entity_object["entity_type"] == "StixFile":
@@ -1727,36 +1798,36 @@
                     entity_object["entity_type"] = "Identity"
                 elif LocationTypes.has_value(entity_object["entity_type"]):
                     entity_object["entity_type"] = "Location"
                 elif StixCyberObservableTypes.has_value(entity_object["entity_type"]):
                     entity_object["entity_type"] = "Stix-Cyber-Observable"
                 elif "stix-core-relationship" in entity_object["parent_types"]:
                     entity_object["entity_type"] = "stix-core-relationship"
-                elif (
-                    "stix-cyber-observable-relationship"
-                    in entity_object["parent_types"]
-                ):
-                    entity_object["entity_type"] = "stix-cyber-observable-relationship"
+                elif "stix-ref-relationship" in entity_object["parent_types"]:
+                    entity_object["entity_type"] = "stix-ref-relationship"
 
                 do_read = reader.get(
                     entity_object["entity_type"],
                     lambda **kwargs: self.unknown_type(
                         {"type": entity_object["entity_type"]}
                     ),
                 )
                 entity_object_data = do_read(id=entity_object["id"])
-                stix_entity_object = self.prepare_export(
-                    self.generate_export(entity_object_data),
-                    "simple",
-                    max_marking_definition_entity,
-                )
-                # Add to result
-                entity_object_bundle = self.filter_objects(uuids, stix_entity_object)
-                uuids = uuids + [x["id"] for x in entity_object_bundle]
-                result = result + entity_object_bundle
+                if entity_object_data is not None:
+                    stix_entity_object = self.prepare_export(
+                        self.generate_export(entity_object_data),
+                        "simple",
+                        max_marking_definition_entity,
+                    )
+                    # Add to result
+                    entity_object_bundle = self.filter_objects(
+                        uuids, stix_entity_object
+                    )
+                    uuids = uuids + [x["id"] for x in entity_object_bundle]
+                    result = result + entity_object_bundle
             for relation_object in relations_to_get:
                 relation_object_data = self.prepare_export(
                     self.opencti.stix_core_relationship.read(id=relation_object["id"])
                 )
                 relation_object_bundle = self.filter_objects(
                     uuids, relation_object_data
                 )
@@ -1804,15 +1875,14 @@
             for entity in result:
                 if entity["type"] in [
                     "report",
                     "note",
                     "opinion",
                     "observed-data",
                     "grouping",
-                    "case",
                 ]:
                     if "object_refs" in entity:
                         entity["object_refs"] = [
                             k for k in entity["object_refs"] if k in uuids
                         ]
                     final_result.append(entity)
                 else:
@@ -1852,15 +1922,18 @@
             "Channel": self.opencti.channel.read,
             "Event": self.opencti.campaign.read,
             "Note": self.opencti.note.read,
             "Observed-Data": self.opencti.observed_data.read,
             "Opinion": self.opencti.opinion.read,
             "Report": self.opencti.report.read,
             "Grouping": self.opencti.grouping.read,
-            "Case": self.opencti.case.read,
+            "Case-Incident": self.opencti.case_incident.read,
+            "Feedback": self.opencti.feedback.read,
+            "Case-Rfi": self.opencti.case_rfi.read,
+            "Case-Rft": self.opencti.case_rft.read,
             "Course-Of-Action": self.opencti.course_of_action.read,
             "Data-Component": self.opencti.data_component.read,
             "Data-Source": self.opencti.data_source.read,
             "Identity": self.opencti.identity.read,
             "Indicator": self.opencti.indicator.read,
             "Infrastructure": self.opencti.infrastructure.read,
             "Intrusion-Set": self.opencti.intrusion_set.read,
@@ -1953,29 +2026,27 @@
                         "key": "entity_type",
                         "values": [
                             "Report",
                             "Grouping",
                             "Note",
                             "Observed-Data",
                             "Opinion",
-                            "Case",
                         ],
                     }
                 )
             else:
                 filters = [
                     {
                         "key": "entity_type",
                         "values": [
                             "Report",
                             "Grouping",
                             "Note",
                             "Observed-Data",
                             "Opinion",
-                            "Case",
                         ],
                     }
                 ]
             entity_type = "Stix-Domain-Object"
 
         # List
         lister = {
@@ -1986,15 +2057,18 @@
             "Channel": self.opencti.channel.list,
             "Event": self.opencti.event.list,
             "Note": self.opencti.note.list,
             "Observed-Data": self.opencti.observed_data.list,
             "Opinion": self.opencti.opinion.list,
             "Report": self.opencti.report.list,
             "Grouping": self.opencti.grouping.list,
-            "Case": self.opencti.case.list,
+            "Case-Incident": self.opencti.case_incident.list,
+            "Feedback": self.opencti.feedback.list,
+            "Case-Rfi": self.opencti.case_rfi.list,
+            "Case-Rft": self.opencti.case_rft.list,
             "Course-Of-Action": self.opencti.course_of_action.list,
             "Data-Component": self.opencti.data_component.list,
             "Data-Source": self.opencti.data_source.list,
             "Identity": self.opencti.identity.list,
             "Indicator": self.opencti.indicator.list,
             "Infrastructure": self.opencti.infrastructure.list,
             "Intrusion-Set": self.opencti.intrusion_set.list,
```

### Comparing `pycti-5.6.post562/pycti/utils/opencti_stix2_splitter.py` & `pycti-5.7.0/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/utils/opencti_stix2_update.py` & `pycti-5.7.0/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti/utils/opencti_stix2_utils.py` & `pycti-5.7.0/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pycti.egg-info/PKG-INFO` & `pycti-5.7.0/pycti.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.6.post562
+Version: 5.7.0
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,15 +27,15 @@
 # OpenCTI client for Python
 
 [![Website](https://img.shields.io/badge/website-opencti.io-blue.svg)](https://www.opencti.io)
 [![CircleCI](https://circleci.com/gh/OpenCTI-Platform/client-python.svg?style=shield)](https://circleci.com/gh/OpenCTI-Platform/client-python/tree/master)
 [![readthedocs](https://readthedocs.org/projects/opencti-client-for-python/badge/?style=flat)](https://opencti-client-for-python.readthedocs.io/en/latest/)
 [![GitHub release](https://img.shields.io/github/release/OpenCTI-Platform/client-python.svg)](https://github.com/OpenCTI-Platform/client-python/releases/latest)
 [![Number of PyPI downloads](https://img.shields.io/pypi/dm/pycti.svg)](https://pypi.python.org/pypi/pycti/)
-[![Slack Status](https://slack.filigran.io/badge.svg)](https://community.filigran.io)
+[![Slack Status](https://img.shields.io/badge/slack-3K%2B%20members-4A154B)](https://community.filigran.io)
 
 The official OpenCTI Python client helps developers to use the OpenCTI API by providing easy to use methods and utils.
 This client is also used by some OpenCTI components.
 
 ## Install
 
 To install the latest Python client library, please use `pip`:
@@ -66,14 +66,20 @@
 # Push you feature/fix on Github
 $ git add [file(s)]
 $ git commit -m "[descriptive message]"
 $ git push origin [branch-name]
 # Open a pull request
 ```
 
+### Install the package locally
+
+```bash
+$ pip install -e .
+```
+
 ## Documentation
 
 ### Client usage
 
 To learn about how to use the OpenCTI Python client and read some examples and cases, refer to [the client documentation](https://opencti-client-for-python.readthedocs.io/en/latest/client_usage/getting_started.html).
 
 ### API reference
```

#### html2text {}

```diff
@@ -1,52 +1,52 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.6.post562 Summary: Python API
-client for OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-
-python Author: Filigran Author-email: contact@filigran.io Maintainer: Filigran
-License: Apache Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
-Information Technology Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Natural Language :: English Classifier: Natural Language :: French Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3 Classifier: Topic :: Security Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Requires-Python: >=3.7 Description-Content-Type:
-text/markdown Provides-Extra: dev Provides-Extra: doc License-File: LICENSE #
-OpenCTI client for Python [![Website](https://img.shields.io/badge/website-
-opencti.io-blue.svg)](https://www.opencti.io) [![CircleCI](https://
-circleci.com/gh/OpenCTI-Platform/client-python.svg?style=shield)](https://
-circleci.com/gh/OpenCTI-Platform/client-python/tree/master) [![readthedocs]
-(https://readthedocs.org/projects/opencti-client-for-python/badge/?style=flat)]
-(https://opencti-client-for-python.readthedocs.io/en/latest/) [![GitHub
-release](https://img.shields.io/github/release/OpenCTI-Platform/client-
-python.svg)](https://github.com/OpenCTI-Platform/client-python/releases/latest)
-[![Number of PyPI downloads](https://img.shields.io/pypi/dm/pycti.svg)](https:/
-/pypi.python.org/pypi/pycti/) [![Slack Status](https://slack.filigran.io/
-badge.svg)](https://community.filigran.io) The official OpenCTI Python client
-helps developers to use the OpenCTI API by providing easy to use methods and
-utils. This client is also used by some OpenCTI components. ## Install To
-install the latest Python client library, please use `pip`: ```bash $ pip3
-install pycti ``` ## Local development ```bash # Fork the current repository,
-then clone your fork $ git clone https://github.com/YOUR-USERNAME/client-python
-$ cd client-python $ git remote add upstream https://github.com/OpenCTI-
-Platform/client-python.git # Create a branch for your feature/fix $ git
+Metadata-Version: 2.1 Name: pycti Version: 5.7.0 Summary: Python API client for
+OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
+Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
+Approved :: Apache Software License Classifier: Natural Language :: English
+Classifier: Natural Language :: French Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier: Topic
+:: Security Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Python: >=3.7 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: doc License-File: LICENSE # OpenCTI client
+for Python [![Website](https://img.shields.io/badge/website-opencti.io-
+blue.svg)](https://www.opencti.io) [![CircleCI](https://circleci.com/gh/
+OpenCTI-Platform/client-python.svg?style=shield)](https://circleci.com/gh/
+OpenCTI-Platform/client-python/tree/master) [![readthedocs](https://
+readthedocs.org/projects/opencti-client-for-python/badge/?style=flat)](https://
+opencti-client-for-python.readthedocs.io/en/latest/) [![GitHub release](https:/
+/img.shields.io/github/release/OpenCTI-Platform/client-python.svg)](https://
+github.com/OpenCTI-Platform/client-python/releases/latest) [![Number of PyPI
+downloads](https://img.shields.io/pypi/dm/pycti.svg)](https://pypi.python.org/
+pypi/pycti/) [![Slack Status](https://img.shields.io/badge/slack-
+3K%2B%20members-4A154B)](https://community.filigran.io) The official OpenCTI
+Python client helps developers to use the OpenCTI API by providing easy to use
+methods and utils. This client is also used by some OpenCTI components. ##
+Install To install the latest Python client library, please use `pip`: ```bash
+$ pip3 install pycti ``` ## Local development ```bash # Fork the current
+repository, then clone your fork $ git clone https://github.com/YOUR-USERNAME/
+client-python $ cd client-python $ git remote add upstream https://github.com/
+OpenCTI-Platform/client-python.git # Create a branch for your feature/fix $ git
 checkout -b [branch-name] # Create a virtualenv $ python3 -m venv .venv $
 source .venv/bin/activate # Install the client-python and dependencies for the
 development and the documentation $ python3 -m pip install -e .[dev,doc] # Set
 up the git hook scripts $ pre-commit install # Create your feature/fix # Create
 tests for your changes $ pytest # Push you feature/fix on Github $ git add
 [file(s)] $ git commit -m "[descriptive message]" $ git push origin [branch-
-name] # Open a pull request ``` ## Documentation ### Client usage To learn
-about how to use the OpenCTI Python client and read some examples and cases,
-refer to [the client documentation](https://opencti-client-for-
-python.readthedocs.io/en/latest/client_usage/getting_started.html). ### API
-reference To learn about the methods available for executing queries and
-retrieving their answers, refer to [the client API Reference](https://opencti-
-client-for-python.readthedocs.io/en/latest/pycti/pycti.html). ## Tests ###
-Install dependencies ```bash $ pip install -r ./test-requirements.txt ```
-[pytest](https://docs.pytest.org/en/7.2.x/) is used to launch the tests. ###
-Launch tests #### Prerequisite Your OpenCTI API should be running. Your
-conftest.py should be configured with your API url and your token. ####
-Launching Unit tests ```bash $ pytest ./tests/01-unit/ ``` Integration testing
-```bash $ pytest ./tests/02-integration/ ``` ## About OpenCTI is a product
-designed and developed by the company [Filigran](https://www.filigran.io).
-[https://www.filigran.io/wp-content/uploads/2022/08/
+name] # Open a pull request ``` ### Install the package locally ```bash $ pip
+install -e . ``` ## Documentation ### Client usage To learn about how to use
+the OpenCTI Python client and read some examples and cases, refer to [the
+client documentation](https://opencti-client-for-python.readthedocs.io/en/
+latest/client_usage/getting_started.html). ### API reference To learn about the
+methods available for executing queries and retrieving their answers, refer to
+[the client API Reference](https://opencti-client-for-python.readthedocs.io/en/
+latest/pycti/pycti.html). ## Tests ### Install dependencies ```bash $ pip
+install -r ./test-requirements.txt ``` [pytest](https://docs.pytest.org/en/
+7.2.x/) is used to launch the tests. ### Launch tests #### Prerequisite Your
+OpenCTI API should be running. Your conftest.py should be configured with your
+API url and your token. #### Launching Unit tests ```bash $ pytest ./tests/01-
+unit/ ``` Integration testing ```bash $ pytest ./tests/02-integration/ ``` ##
+About OpenCTI is a product designed and developed by the company [Filigran]
+(https://www.filigran.io). [https://www.filigran.io/wp-content/uploads/2022/08/
 filigran_text_horizontal_dense_margin.png]
```

### Comparing `pycti-5.6.post562/pycti.egg-info/SOURCES.txt` & `pycti-5.7.0/pycti.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,21 +14,24 @@
 pycti/api/opencti_api_work.py
 pycti/connector/__init__.py
 pycti/connector/opencti_connector.py
 pycti/connector/opencti_connector_helper.py
 pycti/entities/__init__.py
 pycti/entities/opencti_attack_pattern.py
 pycti/entities/opencti_campaign.py
-pycti/entities/opencti_case.py
+pycti/entities/opencti_case_incident.py
+pycti/entities/opencti_case_rfi.py
+pycti/entities/opencti_case_rft.py
 pycti/entities/opencti_channel.py
 pycti/entities/opencti_course_of_action.py
 pycti/entities/opencti_data_component.py
 pycti/entities/opencti_data_source.py
 pycti/entities/opencti_event.py
 pycti/entities/opencti_external_reference.py
+pycti/entities/opencti_feedback.py
 pycti/entities/opencti_grouping.py
 pycti/entities/opencti_identity.py
 pycti/entities/opencti_incident.py
 pycti/entities/opencti_indicator.py
 pycti/entities/opencti_infrastructure.py
 pycti/entities/opencti_intrusion_set.py
 pycti/entities/opencti_kill_chain_phase.py
@@ -42,16 +45,16 @@
 pycti/entities/opencti_observed_data.py
 pycti/entities/opencti_opinion.py
 pycti/entities/opencti_report.py
 pycti/entities/opencti_stix.py
 pycti/entities/opencti_stix_core_object.py
 pycti/entities/opencti_stix_core_relationship.py
 pycti/entities/opencti_stix_cyber_observable.py
-pycti/entities/opencti_stix_cyber_observable_relationship.py
 pycti/entities/opencti_stix_domain_object.py
+pycti/entities/opencti_stix_nested_ref_relationship.py
 pycti/entities/opencti_stix_object_or_stix_relationship.py
 pycti/entities/opencti_stix_sighting_relationship.py
 pycti/entities/opencti_threat_actor.py
 pycti/entities/opencti_tool.py
 pycti/entities/opencti_vocabulary.py
 pycti/entities/opencti_vulnerability.py
 pycti/utils/__init__.py
```

### Comparing `pycti-5.6.post562/pycti.egg-info/requires.txt` & `pycti-5.7.0/pycti.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/pyproject.toml` & `pycti-5.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-5.6.post562/setup.cfg` & `pycti-5.7.0/setup.cfg`

 * *Files identical despite different names*

