# Comparing `tmp/cythereal-magic-1.9.0.tar.gz` & `tmp/cythereal-magic-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cythereal-magic-1.9.0.tar", last modified: Wed Sep  5 03:13:41 2018, max compression
+gzip compressed data, was "dist/cythereal-magic-1.9.1.tar", last modified: Wed Sep  5 15:55:22 2018, max compression
```

## Comparing `cythereal-magic-1.9.0.tar` & `cythereal-magic-1.9.1.tar`

### file list

```diff
@@ -1,85 +1,83 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2018-09-05 03:13:41.000000 cythereal-magic-1.9.0/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2018-09-05 03:13:41.000000 cythereal-magic-1.9.0/cythereal_cli/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4955 2018-09-04 17:59:55.000000 cythereal-magic-1.9.0/cythereal_cli/upload.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2018-09-04 17:59:55.000000 cythereal-magic-1.9.0/cythereal_cli/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2018-09-05 03:13:41.000000 cythereal-magic-1.9.0/cythereal_cli/util/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1873 2018-09-04 17:59:55.000000 cythereal-magic-1.9.0/cythereal_cli/util/hashing.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2018-09-04 17:59:55.000000 cythereal-magic-1.9.0/cythereal_cli/util/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      800 2018-09-04 17:59:55.000000 cythereal-magic-1.9.0/cythereal_cli/api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      559 2018-09-04 17:59:55.000000 cythereal-magic-1.9.0/cythereal_cli/cli.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10867 2018-09-05 03:13:12.000000 cythereal-magic-1.9.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2018-09-05 03:13:41.000000 cythereal-magic-1.9.0/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2018-09-05 03:13:41.000000 cythereal-magic-1.9.0/cythereal_magic.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2018-09-05 03:13:41.000000 cythereal-magic-1.9.0/cythereal_magic.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3305 2018-09-05 03:13:41.000000 cythereal-magic-1.9.0/cythereal_magic.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2018-09-05 03:13:41.000000 cythereal-magic-1.9.0/cythereal_magic.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2018-09-05 03:13:41.000000 cythereal-magic-1.9.0/cythereal_magic.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2905 2018-09-05 03:13:41.000000 cythereal-magic-1.9.0/cythereal_magic.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       60 2018-09-05 03:13:41.000000 cythereal-magic-1.9.0/cythereal_magic.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5988 2018-09-05 03:13:12.000000 cythereal-magic-1.9.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2018-09-05 03:13:41.000000 cythereal-magic-1.9.0/cythereal_magic/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2018-09-05 03:13:41.000000 cythereal-magic-1.9.0/cythereal_magic/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6822 2018-09-04 18:00:55.000000 cythereal-magic-1.9.0/cythereal_magic/models/campaign_procedures_response_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8852 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/file_info_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6675 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/magic_matches_match_subtypes.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8908 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/campaign_id_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9222 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/procedure_signatures_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9110 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/campaign_members_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9830 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/campaign_info_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9160 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/procedure_similarity_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6483 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/magic_category.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9139 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/procedure_similarity.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9021 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/owned_files_list_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8860 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/success_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8267 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/error_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5435 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/campaign_id.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14829 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/magic_report.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6612 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/procedure_signatures_response_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18922 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/procedure_genomics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4624 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/control_flow_graph.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6178 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/owned_files_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13439 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/file_info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6529 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/binary_similarity_binaries.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5259 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/file_upload_response_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8303 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/binary_similarity.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8964 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/magic_matches_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9194 2018-09-04 18:00:55.000000 cythereal-magic-1.9.0/cythereal_magic/models/campaign_procedures_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8219 2018-09-05 03:13:10.000000 cythereal-magic-1.9.0/cythereal_magic/models/api_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8660 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/file_upload_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8023 2018-09-05 03:13:10.000000 cythereal-magic-1.9.0/cythereal_magic/models/analysis_status.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7237 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/magic_label.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7379 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/child_info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6216 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/magic_categories.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11044 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/file_status.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7284 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/magic_matches.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5339 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/magic_labels.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6038 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/campaign_info_response_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6733 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/procedure_similarity_procedures.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6049 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/magic_report_detection_stats.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16818 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/procedure_signatures_response_data_procedures.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6703 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/campaign_members_response_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6583 2018-09-05 03:13:12.000000 cythereal-magic-1.9.0/cythereal_magic/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8936 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/magic_report_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9048 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/magic_categories_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6428 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/magic_category_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9020 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/binary_genomics_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9104 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/procedure_genomics_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13221 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/binary_genomics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8936 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/magic_labels_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11514 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/block_genomics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5654 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/campaign_members_response_data_members.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16797 2018-09-04 18:00:55.000000 cythereal-magic-1.9.0/cythereal_magic/models/campaign_procedures_response_data_procedures.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7489 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/owned_files_list_files.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8908 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/file_status_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5490 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/campaign_info_response_links.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9076 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/binary_similarity_response.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8679 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/models/magic_matches_matches.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2018-09-05 03:13:41.000000 cythereal-magic-1.9.0/cythereal_magic/api/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23860 2018-09-05 03:13:11.000000 cythereal-magic-1.9.0/cythereal_magic/api/alpha_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    67794 2018-09-05 03:13:12.000000 cythereal-magic-1.9.0/cythereal_magic/api/cythereal_magic_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      208 2018-09-05 03:13:12.000000 cythereal-magic-1.9.0/cythereal_magic/api/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10725 2018-09-05 03:13:12.000000 cythereal-magic-1.9.0/cythereal_magic/configuration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15490 2018-09-05 03:13:12.000000 cythereal-magic-1.9.0/cythereal_magic/rest.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6859 2018-09-05 03:13:12.000000 cythereal-magic-1.9.0/cythereal_magic/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26715 2018-09-05 03:13:12.000000 cythereal-magic-1.9.0/cythereal_magic/api_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2905 2018-09-05 03:13:41.000000 cythereal-magic-1.9.0/PKG-INFO
+drwxrwxr-x   0 cledoux   (1000) cledoux   (1000)        0 2018-09-05 15:55:22.000000 cythereal-magic-1.9.1/
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     5988 2018-09-05 15:54:57.000000 cythereal-magic-1.9.1/setup.py
+drwxrwxr-x   0 cledoux   (1000) cledoux   (1000)        0 2018-09-05 15:55:22.000000 cythereal-magic-1.9.1/cythereal_magic/
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)    10725 2018-09-05 15:54:57.000000 cythereal-magic-1.9.1/cythereal_magic/configuration.py
+drwxrwxr-x   0 cledoux   (1000) cledoux   (1000)        0 2018-09-05 15:55:22.000000 cythereal-magic-1.9.1/cythereal_magic/models/
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)    11044 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/file_status.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     5259 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/file_upload_response_data.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     8908 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/campaign_id_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     5339 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/magic_labels.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     5490 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/campaign_info_response_links.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     8908 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/file_status_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     8679 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/magic_matches_matches.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     9160 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/procedure_similarity_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     6529 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/binary_similarity_binaries.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     6703 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/campaign_members_response_data.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     6216 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/magic_categories.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     6675 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/magic_matches_match_subtypes.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     8023 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/analysis_status.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     8852 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/file_info_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     9830 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/campaign_info_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     9139 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/procedure_similarity.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     9020 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/binary_genomics_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     7379 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/child_info.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     5435 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/campaign_id.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     6428 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/magic_category_list.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     9048 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/magic_categories_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     4736 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/procedure_signature_list.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     9104 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/procedure_genomics_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     9076 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/binary_similarity_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     5654 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/campaign_members_response_data_members.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     9110 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/campaign_members_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     4624 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/control_flow_graph.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     7489 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/owned_files_list_files.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     9222 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/procedure_signatures_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     6497 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/procedure_signatures_response_data.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)    13221 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/binary_genomics.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     8964 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/magic_matches_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     8936 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/magic_labels_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     6049 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/magic_report_detection_stats.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     8267 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/error_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)    14829 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/magic_report.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)    13439 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/file_info.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     6178 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/owned_files_list.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     7237 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/magic_label.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     9021 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/owned_files_list_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     6483 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/magic_category.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     6038 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/campaign_info_response_data.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     6617 2018-09-05 15:54:57.000000 cythereal-magic-1.9.1/cythereal_magic/models/__init__.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     8303 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/binary_similarity.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)    11514 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/block_genomics.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     7284 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/magic_matches.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)    15645 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/procedure_signature.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)    18922 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/procedure_genomics.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     8860 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/success_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     8219 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/api_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     8936 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/magic_report_response.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     6733 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/procedure_similarity_procedures.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     8660 2018-09-05 15:54:56.000000 cythereal-magic-1.9.1/cythereal_magic/models/file_upload_response.py
+drwxrwxr-x   0 cledoux   (1000) cledoux   (1000)        0 2018-09-05 15:55:22.000000 cythereal-magic-1.9.1/cythereal_magic/api/
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)    23860 2018-09-05 15:54:57.000000 cythereal-magic-1.9.1/cythereal_magic/api/alpha_api.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)      208 2018-09-05 15:54:57.000000 cythereal-magic-1.9.1/cythereal_magic/api/__init__.py
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)    67794 2018-09-05 15:54:57.000000 cythereal-magic-1.9.1/cythereal_magic/api/cythereal_magic_api.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)     6893 2018-09-05 15:54:57.000000 cythereal-magic-1.9.1/cythereal_magic/__init__.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)    15490 2018-09-05 15:54:57.000000 cythereal-magic-1.9.1/cythereal_magic/rest.py
+-rw-r--r--   0 cledoux   (1000) cledoux   (1000)    26715 2018-09-05 15:54:57.000000 cythereal-magic-1.9.1/cythereal_magic/api_client.py
+drwxrwxr-x   0 cledoux   (1000) cledoux   (1000)        0 2018-09-05 15:55:22.000000 cythereal-magic-1.9.1/cythereal_magic.egg-info/
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)       59 2018-09-05 15:55:22.000000 cythereal-magic-1.9.1/cythereal_magic.egg-info/requires.txt
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)       60 2018-09-05 15:55:22.000000 cythereal-magic-1.9.1/cythereal_magic.egg-info/entry_points.txt
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     2905 2018-09-05 15:55:22.000000 cythereal-magic-1.9.1/cythereal_magic.egg-info/PKG-INFO
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     3144 2018-09-05 15:55:22.000000 cythereal-magic-1.9.1/cythereal_magic.egg-info/SOURCES.txt
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)       30 2018-09-05 15:55:22.000000 cythereal-magic-1.9.1/cythereal_magic.egg-info/top_level.txt
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)        1 2018-09-05 15:55:22.000000 cythereal-magic-1.9.1/cythereal_magic.egg-info/dependency_links.txt
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)       38 2018-09-05 15:55:22.000000 cythereal-magic-1.9.1/setup.cfg
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     2905 2018-09-05 15:55:22.000000 cythereal-magic-1.9.1/PKG-INFO
+drwxrwxr-x   0 cledoux   (1000) cledoux   (1000)        0 2018-09-05 15:55:22.000000 cythereal-magic-1.9.1/cythereal_cli/
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      559 2018-02-21 04:59:23.000000 cythereal-magic-1.9.1/cythereal_cli/cli.py
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     4955 2018-07-03 04:16:10.000000 cythereal-magic-1.9.1/cythereal_cli/upload.py
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)        0 2018-02-21 03:10:20.000000 cythereal-magic-1.9.1/cythereal_cli/__init__.py
+drwxrwxr-x   0 cledoux   (1000) cledoux   (1000)        0 2018-09-05 15:55:22.000000 cythereal-magic-1.9.1/cythereal_cli/util/
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)        0 2018-02-21 03:10:20.000000 cythereal-magic-1.9.1/cythereal_cli/util/__init__.py
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)     1873 2018-02-21 03:10:20.000000 cythereal-magic-1.9.1/cythereal_cli/util/hashing.py
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)      800 2018-02-21 03:58:13.000000 cythereal-magic-1.9.1/cythereal_cli/api_client.py
+-rw-rw-r--   0 cledoux   (1000) cledoux   (1000)    10881 2018-09-05 15:54:57.000000 cythereal-magic-1.9.1/README.md
```

### Comparing `cythereal-magic-1.9.0/cythereal_cli/upload.py` & `cythereal-magic-1.9.1/cythereal_cli/upload.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_cli/util/hashing.py` & `cythereal-magic-1.9.1/cythereal_cli/util/hashing.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_cli/api_client.py` & `cythereal-magic-1.9.1/cythereal_cli/api_client.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_cli/cli.py` & `cythereal-magic-1.9.1/cythereal_cli/cli.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/README.md` & `cythereal-magic-1.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # cythereal-magic
  The API for accessing Cythereal MAGIC products and services.  # API Clients  We provide clients in several languages for accessing the MAGIC API. https://bitbucket.org/cythereal/magic-clients  These clients are provided to make integration of the MAGIC API into your existing applications as easy as possible.  If you want to use a language that is not currently supported, please contact us at support@cythereal.com and we will be glad to help.  # Example Inputs  Here are some example inputs that can be used for testing the service:  * Binary SHA1: `ff9790d7902fea4c910b182f6e0b00221a40d616`   * Can be used for `file_hash` parameters. * Procedure RVA: `0x1000`   * Use with the above SHA1 for `proc_rva` parameters.   # API Conventions  Properties MUST be named using `snake_case`.  This API is inspired by the [google json style guide](https://google.github.io/styleguide/jsoncstyleguide.xml). Any questions about conventions not documented here should be addressed by this style guide.  **All responses** MUST be of type `APIResponse` and contain the following fields:  * `api_version` |  The current api version * `success` | Boolean value indicating if the operation succeeded. * `code` | Status code. Typically corresponds to the HTTP status code.  * `message` | A human readable message providing more details about the operation. Can be null or empty.  **Successful operations** MUST return a `SuccessResponse`, which extends `APIResponse` by adding:  * `data` | Properties containing the response object. * `success` | MUST equal True  When returning objects from a successful response, the `data` object SHOULD contain a property named after the requested object type. For example, the `/matches` endpoint should return a response object with `data.matches`. This property SHOULD  contain a list of the returned objects. For the `/matches` endpoint, the `data.matches` property contains a list of MagicMatch objects. See the `/matches` endpoint documentation for an example.  **Failed Operations** MUST return an `ErrorResponse`, which extends `APIResponse` by adding:  * `errors` | Array of error objects. An error object contains the following properties:     * `ErrorObject.reason` | Unique identifier for this error. Example: \"FileNotFoundError\".     * `ErrorObject.message`| Human readable error message. * `success` | MUST equal False. 
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 1
-- Package version: 1.9.0
+- Package version: 1.9.1
 - Build package: io.swagger.codegen.languages.PythonClientCodegen
 For more information, please visit [http://cythereal.com](http://cythereal.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -124,16 +124,17 @@
  - [MagicMatchesMatchSubtypes](docs/MagicMatchesMatchSubtypes.md)
  - [MagicMatchesMatches](docs/MagicMatchesMatches.md)
  - [MagicReport](docs/MagicReport.md)
  - [MagicReportDetectionStats](docs/MagicReportDetectionStats.md)
  - [OwnedFilesList](docs/OwnedFilesList.md)
  - [OwnedFilesListFiles](docs/OwnedFilesListFiles.md)
  - [ProcedureGenomics](docs/ProcedureGenomics.md)
+ - [ProcedureSignature](docs/ProcedureSignature.md)
+ - [ProcedureSignatureList](docs/ProcedureSignatureList.md)
  - [ProcedureSignaturesResponseData](docs/ProcedureSignaturesResponseData.md)
- - [ProcedureSignaturesResponseDataProcedures](docs/ProcedureSignaturesResponseDataProcedures.md)
  - [ProcedureSimilarity](docs/ProcedureSimilarity.md)
  - [ProcedureSimilarityProcedures](docs/ProcedureSimilarityProcedures.md)
  - [ErrorResponse](docs/ErrorResponse.md)
  - [SuccessResponse](docs/SuccessResponse.md)
  - [BinaryGenomicsResponse](docs/BinaryGenomicsResponse.md)
  - [BinarySimilarityResponse](docs/BinarySimilarityResponse.md)
  - [CampaignIdResponse](docs/CampaignIdResponse.md)
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic.egg-info/SOURCES.txt` & `cythereal-magic-1.9.1/cythereal_magic.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -32,17 +32,14 @@
 cythereal_magic/models/campaign_id_response.py
 cythereal_magic/models/campaign_info_response.py
 cythereal_magic/models/campaign_info_response_data.py
 cythereal_magic/models/campaign_info_response_links.py
 cythereal_magic/models/campaign_members_response.py
 cythereal_magic/models/campaign_members_response_data.py
 cythereal_magic/models/campaign_members_response_data_members.py
-cythereal_magic/models/campaign_procedures_response.py
-cythereal_magic/models/campaign_procedures_response_data.py
-cythereal_magic/models/campaign_procedures_response_data_procedures.py
 cythereal_magic/models/child_info.py
 cythereal_magic/models/control_flow_graph.py
 cythereal_magic/models/error_response.py
 cythereal_magic/models/file_info.py
 cythereal_magic/models/file_info_response.py
 cythereal_magic/models/file_status.py
 cythereal_magic/models/file_status_response.py
@@ -63,14 +60,15 @@
 cythereal_magic/models/magic_report_detection_stats.py
 cythereal_magic/models/magic_report_response.py
 cythereal_magic/models/owned_files_list.py
 cythereal_magic/models/owned_files_list_files.py
 cythereal_magic/models/owned_files_list_response.py
 cythereal_magic/models/procedure_genomics.py
 cythereal_magic/models/procedure_genomics_response.py
+cythereal_magic/models/procedure_signature.py
+cythereal_magic/models/procedure_signature_list.py
 cythereal_magic/models/procedure_signatures_response.py
 cythereal_magic/models/procedure_signatures_response_data.py
-cythereal_magic/models/procedure_signatures_response_data_procedures.py
 cythereal_magic/models/procedure_similarity.py
 cythereal_magic/models/procedure_similarity_procedures.py
 cythereal_magic/models/procedure_similarity_response.py
 cythereal_magic/models/success_response.py
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic.egg-info/PKG-INFO` & `cythereal-magic-1.9.1/cythereal_magic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: cythereal-magic
-Version: 1.9.0
+Version: 1.9.1
 Summary: Cythereal MAGIC API
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: support@cythereal.com
 License: UNKNOWN
 Description:      The API for accessing Cythereal MAGIC products and services.  # API Clients  We provide clients in several languages for accessing the MAGIC API. https://bitbucket.org/cythereal/magic-clients  These clients are provided to make integration of the MAGIC API into your existing applications as easy as possible.  If you want to use a language that is not currently supported, please contact us at support@cythereal.com and we will be glad to help.  # Example Inputs  Here are some example inputs that can be used for testing the service:  * Binary SHA1: &#x60;ff9790d7902fea4c910b182f6e0b00221a40d616&#x60;   * Can be used for &#x60;file_hash&#x60; parameters. * Procedure RVA: &#x60;0x1000&#x60;   * Use with the above SHA1 for &#x60;proc_rva&#x60; parameters.   # API Conventions  Properties MUST be named using &#x60;snake_case&#x60;.  This API is inspired by the [google json style guide](https://google.github.io/styleguide/jsoncstyleguide.xml). Any questions about conventions not documented here should be addressed by this style guide.  **All responses** MUST be of type &#x60;APIResponse&#x60; and contain the following fields:  * &#x60;api_version&#x60; |  The current api version * &#x60;success&#x60; | Boolean value indicating if the operation succeeded. * &#x60;code&#x60; | Status code. Typically corresponds to the HTTP status code.  * &#x60;message&#x60; | A human readable message providing more details about the operation. Can be null or empty.  **Successful operations** MUST return a &#x60;SuccessResponse&#x60;, which extends &#x60;APIResponse&#x60; by adding:  * &#x60;data&#x60; | Properties containing the response object. * &#x60;success&#x60; | MUST equal True  When returning objects from a successful response, the &#x60;data&#x60; object SHOULD contain a property named after the requested object type. For example, the &#x60;/matches&#x60; endpoint should return a response object with &#x60;data.matches&#x60;. This property SHOULD  contain a list of the returned objects. For the &#x60;/matches&#x60; endpoint, the &#x60;data.matches&#x60; property contains a list of MagicMatch objects. See the &#x60;/matches&#x60; endpoint documentation for an example.  **Failed Operations** MUST return an &#x60;ErrorResponse&#x60;, which extends &#x60;APIResponse&#x60; by adding:  * &#x60;errors&#x60; | Array of error objects. An error object contains the following properties:     * &#x60;ErrorObject.reason&#x60; | Unique identifier for this error. Example: \&quot;FileNotFoundError\&quot;.     * &#x60;ErrorObject.message&#x60;| Human readable error message. * &#x60;success&#x60; | MUST equal False.   # noqa: E501
```

### Comparing `cythereal-magic-1.9.0/setup.py` & `cythereal-magic-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "cythereal-magic"
-VERSION = "1.9.0"
+VERSION = "1.9.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/campaign_procedures_response_data.py` & `cythereal-magic-1.9.1/cythereal_magic/models/procedure_signatures_response_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,94 +12,92 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cythereal_magic.models.campaign_procedures_response_data_procedures import CampaignProceduresResponseDataProcedures  # noqa: F401,E501
+from cythereal_magic.models.procedure_signature_list import ProcedureSignatureList  # noqa: F401,E501
 
 
-class CampaignProceduresResponseData(object):
+class ProcedureSignaturesResponseData(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'campaign_id': 'str',
-        'procedures': 'list[CampaignProceduresResponseDataProcedures]'
+        'binaries': 'list[str]',
+        'procedures': 'ProcedureSignatureList'
     }
 
     attribute_map = {
-        'campaign_id': 'campaign_id',
+        'binaries': 'binaries',
         'procedures': 'procedures'
     }
 
-    def __init__(self, campaign_id=None, procedures=None):  # noqa: E501
-        """CampaignProceduresResponseData - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, binaries=None, procedures=None):  # noqa: E501
+        """ProcedureSignaturesResponseData - a model defined in Swagger"""  # noqa: E501
 
-        self._campaign_id = None
+        self._binaries = None
         self._procedures = None
         self.discriminator = None
 
-        if campaign_id is not None:
-            self.campaign_id = campaign_id
+        if binaries is not None:
+            self.binaries = binaries
         if procedures is not None:
             self.procedures = procedures
 
     @property
-    def campaign_id(self):
-        """Gets the campaign_id of this CampaignProceduresResponseData.  # noqa: E501
+    def binaries(self):
+        """Gets the binaries of this ProcedureSignaturesResponseData.  # noqa: E501
 
-        The id of the campaign.  # noqa: E501
+        List of binaries used to generate the signatures.  # noqa: E501
 
-        :return: The campaign_id of this CampaignProceduresResponseData.  # noqa: E501
-        :rtype: str
+        :return: The binaries of this ProcedureSignaturesResponseData.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._campaign_id
+        return self._binaries
 
-    @campaign_id.setter
-    def campaign_id(self, campaign_id):
-        """Sets the campaign_id of this CampaignProceduresResponseData.
+    @binaries.setter
+    def binaries(self, binaries):
+        """Sets the binaries of this ProcedureSignaturesResponseData.
 
-        The id of the campaign.  # noqa: E501
+        List of binaries used to generate the signatures.  # noqa: E501
 
-        :param campaign_id: The campaign_id of this CampaignProceduresResponseData.  # noqa: E501
-        :type: str
+        :param binaries: The binaries of this ProcedureSignaturesResponseData.  # noqa: E501
+        :type: list[str]
         """
-        if campaign_id is not None and not re.search('[a-fA-F0-9]{40}', campaign_id):  # noqa: E501
-            raise ValueError("Invalid value for `campaign_id`, must be a follow pattern or equal to `/[a-fA-F0-9]{40}/`")  # noqa: E501
 
-        self._campaign_id = campaign_id
+        self._binaries = binaries
 
     @property
     def procedures(self):
-        """Gets the procedures of this CampaignProceduresResponseData.  # noqa: E501
+        """Gets the procedures of this ProcedureSignaturesResponseData.  # noqa: E501
 
 
-        :return: The procedures of this CampaignProceduresResponseData.  # noqa: E501
-        :rtype: list[CampaignProceduresResponseDataProcedures]
+        :return: The procedures of this ProcedureSignaturesResponseData.  # noqa: E501
+        :rtype: ProcedureSignatureList
         """
         return self._procedures
 
     @procedures.setter
     def procedures(self, procedures):
-        """Sets the procedures of this CampaignProceduresResponseData.
+        """Sets the procedures of this ProcedureSignaturesResponseData.
 
 
-        :param procedures: The procedures of this CampaignProceduresResponseData.  # noqa: E501
-        :type: list[CampaignProceduresResponseDataProcedures]
+        :param procedures: The procedures of this ProcedureSignaturesResponseData.  # noqa: E501
+        :type: ProcedureSignatureList
         """
 
         self._procedures = procedures
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -130,15 +128,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CampaignProceduresResponseData):
+        if not isinstance(other, ProcedureSignaturesResponseData):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/file_info_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/file_info_response.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/magic_matches_match_subtypes.py` & `cythereal-magic-1.9.1/cythereal_magic/models/magic_matches_match_subtypes.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/campaign_id_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/campaign_id_response.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/procedure_signatures_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/procedure_signatures_response.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/campaign_members_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/campaign_members_response.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/campaign_info_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/campaign_info_response.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/procedure_similarity_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/procedure_similarity_response.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/magic_category.py` & `cythereal-magic-1.9.1/cythereal_magic/models/magic_category.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/procedure_similarity.py` & `cythereal-magic-1.9.1/cythereal_magic/models/procedure_similarity.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/owned_files_list_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/owned_files_list_response.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/success_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/success_response.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/error_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/error_response.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/campaign_id.py` & `cythereal-magic-1.9.1/cythereal_magic/models/campaign_id.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/magic_report.py` & `cythereal-magic-1.9.1/cythereal_magic/models/magic_report.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/procedure_signatures_response_data.py` & `cythereal-magic-1.9.1/cythereal_magic/models/campaign_info_response_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,95 +12,91 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cythereal_magic.models.procedure_signatures_response_data_procedures import ProcedureSignaturesResponseDataProcedures  # noqa: F401,E501
 
-
-class ProcedureSignaturesResponseData(object):
+class CampaignInfoResponseData(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'binaries': 'list[str]',
-        'procedures': 'list[ProcedureSignaturesResponseDataProcedures]'
+        'campaign_id': 'str',
+        'size': 'int'
     }
 
     attribute_map = {
-        'binaries': 'binaries',
-        'procedures': 'procedures'
+        'campaign_id': 'campaign_id',
+        'size': 'size'
     }
 
-    def __init__(self, binaries=None, procedures=None):  # noqa: E501
-        """ProcedureSignaturesResponseData - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, campaign_id=None, size=None):  # noqa: E501
+        """CampaignInfoResponseData - a model defined in Swagger"""  # noqa: E501
 
-        self._binaries = None
-        self._procedures = None
+        self._campaign_id = None
+        self._size = None
         self.discriminator = None
 
-        if binaries is not None:
-            self.binaries = binaries
-        if procedures is not None:
-            self.procedures = procedures
+        if campaign_id is not None:
+            self.campaign_id = campaign_id
+        if size is not None:
+            self.size = size
 
     @property
-    def binaries(self):
-        """Gets the binaries of this ProcedureSignaturesResponseData.  # noqa: E501
+    def campaign_id(self):
+        """Gets the campaign_id of this CampaignInfoResponseData.  # noqa: E501
 
-        List of binaries used to generate the signatures.  # noqa: E501
 
-        :return: The binaries of this ProcedureSignaturesResponseData.  # noqa: E501
-        :rtype: list[str]
+        :return: The campaign_id of this CampaignInfoResponseData.  # noqa: E501
+        :rtype: str
         """
-        return self._binaries
+        return self._campaign_id
 
-    @binaries.setter
-    def binaries(self, binaries):
-        """Sets the binaries of this ProcedureSignaturesResponseData.
+    @campaign_id.setter
+    def campaign_id(self, campaign_id):
+        """Sets the campaign_id of this CampaignInfoResponseData.
 
-        List of binaries used to generate the signatures.  # noqa: E501
 
-        :param binaries: The binaries of this ProcedureSignaturesResponseData.  # noqa: E501
-        :type: list[str]
+        :param campaign_id: The campaign_id of this CampaignInfoResponseData.  # noqa: E501
+        :type: str
         """
 
-        self._binaries = binaries
+        self._campaign_id = campaign_id
 
     @property
-    def procedures(self):
-        """Gets the procedures of this ProcedureSignaturesResponseData.  # noqa: E501
+    def size(self):
+        """Gets the size of this CampaignInfoResponseData.  # noqa: E501
 
 
-        :return: The procedures of this ProcedureSignaturesResponseData.  # noqa: E501
-        :rtype: list[ProcedureSignaturesResponseDataProcedures]
+        :return: The size of this CampaignInfoResponseData.  # noqa: E501
+        :rtype: int
         """
-        return self._procedures
+        return self._size
 
-    @procedures.setter
-    def procedures(self, procedures):
-        """Sets the procedures of this ProcedureSignaturesResponseData.
+    @size.setter
+    def size(self, size):
+        """Sets the size of this CampaignInfoResponseData.
 
 
-        :param procedures: The procedures of this ProcedureSignaturesResponseData.  # noqa: E501
-        :type: list[ProcedureSignaturesResponseDataProcedures]
+        :param size: The size of this CampaignInfoResponseData.  # noqa: E501
+        :type: int
         """
 
-        self._procedures = procedures
+        self._size = size
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -128,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProcedureSignaturesResponseData):
+        if not isinstance(other, CampaignInfoResponseData):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/procedure_genomics.py` & `cythereal-magic-1.9.1/cythereal_magic/models/procedure_genomics.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/control_flow_graph.py` & `cythereal-magic-1.9.1/cythereal_magic/models/control_flow_graph.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/owned_files_list.py` & `cythereal-magic-1.9.1/cythereal_magic/models/owned_files_list.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/file_info.py` & `cythereal-magic-1.9.1/cythereal_magic/models/file_info.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/binary_similarity_binaries.py` & `cythereal-magic-1.9.1/cythereal_magic/models/binary_similarity_binaries.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/file_upload_response_data.py` & `cythereal-magic-1.9.1/cythereal_magic/models/file_upload_response_data.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/binary_similarity.py` & `cythereal-magic-1.9.1/cythereal_magic/models/binary_similarity.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/magic_matches_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/magic_matches_response.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/campaign_procedures_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/binary_genomics_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cythereal_magic.models.campaign_procedures_response_data import CampaignProceduresResponseData  # noqa: F401,E501
+from cythereal_magic.models.binary_genomics import BinaryGenomics  # noqa: F401,E501
 from cythereal_magic.models.success_response import SuccessResponse  # noqa: F401,E501
 
 
-class CampaignProceduresResponse(object):
+class BinaryGenomicsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
@@ -34,27 +34,27 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'api_version': 'str',
         'success': 'bool',
         'code': 'int',
         'message': 'str',
-        'data': 'CampaignProceduresResponseData'
+        'data': 'BinaryGenomics'
     }
 
     attribute_map = {
         'api_version': 'api_version',
         'success': 'success',
         'code': 'code',
         'message': 'message',
         'data': 'data'
     }
 
     def __init__(self, api_version=None, success=None, code=None, message=None, data=None):  # noqa: E501
-        """CampaignProceduresResponse - a model defined in Swagger"""  # noqa: E501
+        """BinaryGenomicsResponse - a model defined in Swagger"""  # noqa: E501
 
         self._api_version = None
         self._success = None
         self._code = None
         self._message = None
         self._data = None
         self.discriminator = None
@@ -64,125 +64,125 @@
         self.code = code
         if message is not None:
             self.message = message
         self.data = data
 
     @property
     def api_version(self):
-        """Gets the api_version of this CampaignProceduresResponse.  # noqa: E501
+        """Gets the api_version of this BinaryGenomicsResponse.  # noqa: E501
 
         The current api version.  # noqa: E501
 
-        :return: The api_version of this CampaignProceduresResponse.  # noqa: E501
+        :return: The api_version of this BinaryGenomicsResponse.  # noqa: E501
         :rtype: str
         """
         return self._api_version
 
     @api_version.setter
     def api_version(self, api_version):
-        """Sets the api_version of this CampaignProceduresResponse.
+        """Sets the api_version of this BinaryGenomicsResponse.
 
         The current api version.  # noqa: E501
 
-        :param api_version: The api_version of this CampaignProceduresResponse.  # noqa: E501
+        :param api_version: The api_version of this BinaryGenomicsResponse.  # noqa: E501
         :type: str
         """
         if api_version is None:
             raise ValueError("Invalid value for `api_version`, must not be `None`")  # noqa: E501
 
         self._api_version = api_version
 
     @property
     def success(self):
-        """Gets the success of this CampaignProceduresResponse.  # noqa: E501
+        """Gets the success of this BinaryGenomicsResponse.  # noqa: E501
 
         MUST equal true.  # noqa: E501
 
-        :return: The success of this CampaignProceduresResponse.  # noqa: E501
+        :return: The success of this BinaryGenomicsResponse.  # noqa: E501
         :rtype: bool
         """
         return self._success
 
     @success.setter
     def success(self, success):
-        """Sets the success of this CampaignProceduresResponse.
+        """Sets the success of this BinaryGenomicsResponse.
 
         MUST equal true.  # noqa: E501
 
-        :param success: The success of this CampaignProceduresResponse.  # noqa: E501
+        :param success: The success of this BinaryGenomicsResponse.  # noqa: E501
         :type: bool
         """
         if success is None:
             raise ValueError("Invalid value for `success`, must not be `None`")  # noqa: E501
 
         self._success = success
 
     @property
     def code(self):
-        """Gets the code of this CampaignProceduresResponse.  # noqa: E501
+        """Gets the code of this BinaryGenomicsResponse.  # noqa: E501
 
 
-        :return: The code of this CampaignProceduresResponse.  # noqa: E501
+        :return: The code of this BinaryGenomicsResponse.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
-        """Sets the code of this CampaignProceduresResponse.
+        """Sets the code of this BinaryGenomicsResponse.
 
 
-        :param code: The code of this CampaignProceduresResponse.  # noqa: E501
+        :param code: The code of this BinaryGenomicsResponse.  # noqa: E501
         :type: int
         """
         if code is None:
             raise ValueError("Invalid value for `code`, must not be `None`")  # noqa: E501
 
         self._code = code
 
     @property
     def message(self):
-        """Gets the message of this CampaignProceduresResponse.  # noqa: E501
+        """Gets the message of this BinaryGenomicsResponse.  # noqa: E501
 
         A human readable message providing more details about the operation. Can be null or empty if no additional information is required.   # noqa: E501
 
-        :return: The message of this CampaignProceduresResponse.  # noqa: E501
+        :return: The message of this BinaryGenomicsResponse.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this CampaignProceduresResponse.
+        """Sets the message of this BinaryGenomicsResponse.
 
         A human readable message providing more details about the operation. Can be null or empty if no additional information is required.   # noqa: E501
 
-        :param message: The message of this CampaignProceduresResponse.  # noqa: E501
+        :param message: The message of this BinaryGenomicsResponse.  # noqa: E501
         :type: str
         """
 
         self._message = message
 
     @property
     def data(self):
-        """Gets the data of this CampaignProceduresResponse.  # noqa: E501
+        """Gets the data of this BinaryGenomicsResponse.  # noqa: E501
 
 
-        :return: The data of this CampaignProceduresResponse.  # noqa: E501
-        :rtype: CampaignProceduresResponseData
+        :return: The data of this BinaryGenomicsResponse.  # noqa: E501
+        :rtype: BinaryGenomics
         """
         return self._data
 
     @data.setter
     def data(self, data):
-        """Sets the data of this CampaignProceduresResponse.
+        """Sets the data of this BinaryGenomicsResponse.
 
 
-        :param data: The data of this CampaignProceduresResponse.  # noqa: E501
-        :type: CampaignProceduresResponseData
+        :param data: The data of this BinaryGenomicsResponse.  # noqa: E501
+        :type: BinaryGenomics
         """
         if data is None:
             raise ValueError("Invalid value for `data`, must not be `None`")  # noqa: E501
 
         self._data = data
 
     def to_dict(self):
@@ -215,15 +215,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CampaignProceduresResponse):
+        if not isinstance(other, BinaryGenomicsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/api_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/api_response.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/file_upload_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/file_upload_response.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/analysis_status.py` & `cythereal-magic-1.9.1/cythereal_magic/models/analysis_status.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/magic_label.py` & `cythereal-magic-1.9.1/cythereal_magic/models/magic_label.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/child_info.py` & `cythereal-magic-1.9.1/cythereal_magic/models/child_info.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/magic_categories.py` & `cythereal-magic-1.9.1/cythereal_magic/models/magic_categories.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/file_status.py` & `cythereal-magic-1.9.1/cythereal_magic/models/file_status.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/magic_matches.py` & `cythereal-magic-1.9.1/cythereal_magic/models/magic_matches.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/magic_labels.py` & `cythereal-magic-1.9.1/cythereal_magic/models/magic_labels.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/campaign_info_response_data.py` & `cythereal-magic-1.9.1/cythereal_magic/models/campaign_members_response_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,91 +12,97 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
+from cythereal_magic.models.campaign_members_response_data_members import CampaignMembersResponseDataMembers  # noqa: F401,E501
 
-class CampaignInfoResponseData(object):
+
+class CampaignMembersResponseData(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'campaign_id': 'str',
-        'size': 'int'
+        'members': 'list[CampaignMembersResponseDataMembers]'
     }
 
     attribute_map = {
         'campaign_id': 'campaign_id',
-        'size': 'size'
+        'members': 'members'
     }
 
-    def __init__(self, campaign_id=None, size=None):  # noqa: E501
-        """CampaignInfoResponseData - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, campaign_id=None, members=None):  # noqa: E501
+        """CampaignMembersResponseData - a model defined in Swagger"""  # noqa: E501
 
         self._campaign_id = None
-        self._size = None
+        self._members = None
         self.discriminator = None
 
         if campaign_id is not None:
             self.campaign_id = campaign_id
-        if size is not None:
-            self.size = size
+        if members is not None:
+            self.members = members
 
     @property
     def campaign_id(self):
-        """Gets the campaign_id of this CampaignInfoResponseData.  # noqa: E501
+        """Gets the campaign_id of this CampaignMembersResponseData.  # noqa: E501
 
+        A SHA1 cryptographic hash  # noqa: E501
 
-        :return: The campaign_id of this CampaignInfoResponseData.  # noqa: E501
+        :return: The campaign_id of this CampaignMembersResponseData.  # noqa: E501
         :rtype: str
         """
         return self._campaign_id
 
     @campaign_id.setter
     def campaign_id(self, campaign_id):
-        """Sets the campaign_id of this CampaignInfoResponseData.
+        """Sets the campaign_id of this CampaignMembersResponseData.
 
+        A SHA1 cryptographic hash  # noqa: E501
 
-        :param campaign_id: The campaign_id of this CampaignInfoResponseData.  # noqa: E501
+        :param campaign_id: The campaign_id of this CampaignMembersResponseData.  # noqa: E501
         :type: str
         """
+        if campaign_id is not None and not re.search('[a-fA-F0-9]{40}', campaign_id):  # noqa: E501
+            raise ValueError("Invalid value for `campaign_id`, must be a follow pattern or equal to `/[a-fA-F0-9]{40}/`")  # noqa: E501
 
         self._campaign_id = campaign_id
 
     @property
-    def size(self):
-        """Gets the size of this CampaignInfoResponseData.  # noqa: E501
+    def members(self):
+        """Gets the members of this CampaignMembersResponseData.  # noqa: E501
 
 
-        :return: The size of this CampaignInfoResponseData.  # noqa: E501
-        :rtype: int
+        :return: The members of this CampaignMembersResponseData.  # noqa: E501
+        :rtype: list[CampaignMembersResponseDataMembers]
         """
-        return self._size
+        return self._members
 
-    @size.setter
-    def size(self, size):
-        """Sets the size of this CampaignInfoResponseData.
+    @members.setter
+    def members(self, members):
+        """Sets the members of this CampaignMembersResponseData.
 
 
-        :param size: The size of this CampaignInfoResponseData.  # noqa: E501
-        :type: int
+        :param members: The members of this CampaignMembersResponseData.  # noqa: E501
+        :type: list[CampaignMembersResponseDataMembers]
         """
 
-        self._size = size
+        self._members = members
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -124,15 +130,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CampaignInfoResponseData):
+        if not isinstance(other, CampaignMembersResponseData):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/procedure_similarity_procedures.py` & `cythereal-magic-1.9.1/cythereal_magic/models/procedure_similarity_procedures.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/magic_report_detection_stats.py` & `cythereal-magic-1.9.1/cythereal_magic/models/magic_report_detection_stats.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/procedure_signatures_response_data_procedures.py` & `cythereal-magic-1.9.1/cythereal_magic/models/procedure_signature.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 
-class ProcedureSignaturesResponseDataProcedures(object):
+class ProcedureSignature(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
@@ -57,15 +57,15 @@
         'procedure_names': 'procedure_names',
         'name_counts': 'name_counts',
         'signature': 'signature',
         'example_procedure': 'example_procedure'
     }
 
     def __init__(self, hard_hash=None, is_library=None, status=None, coverage=None, byte_counts=None, instr_counts=None, block_counts=None, occurrence_counts=None, procedure_names=None, name_counts=None, signature=None, example_procedure=None):  # noqa: E501
-        """ProcedureSignaturesResponseDataProcedures - a model defined in Swagger"""  # noqa: E501
+        """ProcedureSignature - a model defined in Swagger"""  # noqa: E501
 
         self._hard_hash = None
         self._is_library = None
         self._status = None
         self._coverage = None
         self._byte_counts = None
         self._instr_counts = None
@@ -100,273 +100,273 @@
         if signature is not None:
             self.signature = signature
         if example_procedure is not None:
             self.example_procedure = example_procedure
 
     @property
     def hard_hash(self):
-        """Gets the hard_hash of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        """Gets the hard_hash of this ProcedureSignature.  # noqa: E501
 
         The proc hash for this procedure group.  # noqa: E501
 
-        :return: The hard_hash of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :return: The hard_hash of this ProcedureSignature.  # noqa: E501
         :rtype: str
         """
         return self._hard_hash
 
     @hard_hash.setter
     def hard_hash(self, hard_hash):
-        """Sets the hard_hash of this ProcedureSignaturesResponseDataProcedures.
+        """Sets the hard_hash of this ProcedureSignature.
 
         The proc hash for this procedure group.  # noqa: E501
 
-        :param hard_hash: The hard_hash of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :param hard_hash: The hard_hash of this ProcedureSignature.  # noqa: E501
         :type: str
         """
         if hard_hash is not None and not re.search('[a-fA-F0-9]{32}', hard_hash):  # noqa: E501
             raise ValueError("Invalid value for `hard_hash`, must be a follow pattern or equal to `/[a-fA-F0-9]{32}/`")  # noqa: E501
 
         self._hard_hash = hard_hash
 
     @property
     def is_library(self):
-        """Gets the is_library of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        """Gets the is_library of this ProcedureSignature.  # noqa: E501
 
         Is one or more procedures in this group marked as a library function?  # noqa: E501
 
-        :return: The is_library of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :return: The is_library of this ProcedureSignature.  # noqa: E501
         :rtype: bool
         """
         return self._is_library
 
     @is_library.setter
     def is_library(self, is_library):
-        """Sets the is_library of this ProcedureSignaturesResponseDataProcedures.
+        """Sets the is_library of this ProcedureSignature.
 
         Is one or more procedures in this group marked as a library function?  # noqa: E501
 
-        :param is_library: The is_library of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :param is_library: The is_library of this ProcedureSignature.  # noqa: E501
         :type: bool
         """
 
         self._is_library = is_library
 
     @property
     def status(self):
-        """Gets the status of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        """Gets the status of this ProcedureSignature.  # noqa: E501
 
         Indicates the current status of the signature. Must be one of the following -    empty - No procedure added to the group   clone - All the procedures in the group are clones   variant-{blocks,instr,bytes} - Procedures had a different number of {blocks,instr,bytes}   variant-alignment - Procedures have the same number of {blocks,instr,bytes}, but something else isn't lining up  # noqa: E501
 
-        :return: The status of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :return: The status of this ProcedureSignature.  # noqa: E501
         :rtype: str
         """
         return self._status
 
     @status.setter
     def status(self, status):
-        """Sets the status of this ProcedureSignaturesResponseDataProcedures.
+        """Sets the status of this ProcedureSignature.
 
         Indicates the current status of the signature. Must be one of the following -    empty - No procedure added to the group   clone - All the procedures in the group are clones   variant-{blocks,instr,bytes} - Procedures had a different number of {blocks,instr,bytes}   variant-alignment - Procedures have the same number of {blocks,instr,bytes}, but something else isn't lining up  # noqa: E501
 
-        :param status: The status of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :param status: The status of this ProcedureSignature.  # noqa: E501
         :type: str
         """
 
         self._status = status
 
     @property
     def coverage(self):
-        """Gets the coverage of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        """Gets the coverage of this ProcedureSignature.  # noqa: E501
 
         Percentage of given binaries this procedure is in. Will be between 0 and 1 inclusive.  # noqa: E501
 
-        :return: The coverage of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :return: The coverage of this ProcedureSignature.  # noqa: E501
         :rtype: float
         """
         return self._coverage
 
     @coverage.setter
     def coverage(self, coverage):
-        """Sets the coverage of this ProcedureSignaturesResponseDataProcedures.
+        """Sets the coverage of this ProcedureSignature.
 
         Percentage of given binaries this procedure is in. Will be between 0 and 1 inclusive.  # noqa: E501
 
-        :param coverage: The coverage of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :param coverage: The coverage of this ProcedureSignature.  # noqa: E501
         :type: float
         """
 
         self._coverage = coverage
 
     @property
     def byte_counts(self):
-        """Gets the byte_counts of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        """Gets the byte_counts of this ProcedureSignature.  # noqa: E501
 
 
-        :return: The byte_counts of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :return: The byte_counts of this ProcedureSignature.  # noqa: E501
         :rtype: list[int]
         """
         return self._byte_counts
 
     @byte_counts.setter
     def byte_counts(self, byte_counts):
-        """Sets the byte_counts of this ProcedureSignaturesResponseDataProcedures.
+        """Sets the byte_counts of this ProcedureSignature.
 
 
-        :param byte_counts: The byte_counts of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :param byte_counts: The byte_counts of this ProcedureSignature.  # noqa: E501
         :type: list[int]
         """
 
         self._byte_counts = byte_counts
 
     @property
     def instr_counts(self):
-        """Gets the instr_counts of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        """Gets the instr_counts of this ProcedureSignature.  # noqa: E501
 
 
-        :return: The instr_counts of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :return: The instr_counts of this ProcedureSignature.  # noqa: E501
         :rtype: list[int]
         """
         return self._instr_counts
 
     @instr_counts.setter
     def instr_counts(self, instr_counts):
-        """Sets the instr_counts of this ProcedureSignaturesResponseDataProcedures.
+        """Sets the instr_counts of this ProcedureSignature.
 
 
-        :param instr_counts: The instr_counts of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :param instr_counts: The instr_counts of this ProcedureSignature.  # noqa: E501
         :type: list[int]
         """
 
         self._instr_counts = instr_counts
 
     @property
     def block_counts(self):
-        """Gets the block_counts of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        """Gets the block_counts of this ProcedureSignature.  # noqa: E501
 
 
-        :return: The block_counts of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :return: The block_counts of this ProcedureSignature.  # noqa: E501
         :rtype: list[int]
         """
         return self._block_counts
 
     @block_counts.setter
     def block_counts(self, block_counts):
-        """Sets the block_counts of this ProcedureSignaturesResponseDataProcedures.
+        """Sets the block_counts of this ProcedureSignature.
 
 
-        :param block_counts: The block_counts of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :param block_counts: The block_counts of this ProcedureSignature.  # noqa: E501
         :type: list[int]
         """
 
         self._block_counts = block_counts
 
     @property
     def occurrence_counts(self):
-        """Gets the occurrence_counts of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        """Gets the occurrence_counts of this ProcedureSignature.  # noqa: E501
 
         Number of ProcedureGenomics objects with the same hard_hash.  # noqa: E501
 
-        :return: The occurrence_counts of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :return: The occurrence_counts of this ProcedureSignature.  # noqa: E501
         :rtype: int
         """
         return self._occurrence_counts
 
     @occurrence_counts.setter
     def occurrence_counts(self, occurrence_counts):
-        """Sets the occurrence_counts of this ProcedureSignaturesResponseDataProcedures.
+        """Sets the occurrence_counts of this ProcedureSignature.
 
         Number of ProcedureGenomics objects with the same hard_hash.  # noqa: E501
 
-        :param occurrence_counts: The occurrence_counts of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :param occurrence_counts: The occurrence_counts of this ProcedureSignature.  # noqa: E501
         :type: int
         """
 
         self._occurrence_counts = occurrence_counts
 
     @property
     def procedure_names(self):
-        """Gets the procedure_names of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        """Gets the procedure_names of this ProcedureSignature.  # noqa: E501
 
 
-        :return: The procedure_names of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :return: The procedure_names of this ProcedureSignature.  # noqa: E501
         :rtype: list[str]
         """
         return self._procedure_names
 
     @procedure_names.setter
     def procedure_names(self, procedure_names):
-        """Sets the procedure_names of this ProcedureSignaturesResponseDataProcedures.
+        """Sets the procedure_names of this ProcedureSignature.
 
 
-        :param procedure_names: The procedure_names of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :param procedure_names: The procedure_names of this ProcedureSignature.  # noqa: E501
         :type: list[str]
         """
 
         self._procedure_names = procedure_names
 
     @property
     def name_counts(self):
-        """Gets the name_counts of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        """Gets the name_counts of this ProcedureSignature.  # noqa: E501
 
         Number of unique procedures in this procedure group  # noqa: E501
 
-        :return: The name_counts of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :return: The name_counts of this ProcedureSignature.  # noqa: E501
         :rtype: int
         """
         return self._name_counts
 
     @name_counts.setter
     def name_counts(self, name_counts):
-        """Sets the name_counts of this ProcedureSignaturesResponseDataProcedures.
+        """Sets the name_counts of this ProcedureSignature.
 
         Number of unique procedures in this procedure group  # noqa: E501
 
-        :param name_counts: The name_counts of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :param name_counts: The name_counts of this ProcedureSignature.  # noqa: E501
         :type: int
         """
 
         self._name_counts = name_counts
 
     @property
     def signature(self):
-        """Gets the signature of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        """Gets the signature of this ProcedureSignature.  # noqa: E501
 
 
-        :return: The signature of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :return: The signature of this ProcedureSignature.  # noqa: E501
         :rtype: list[list[str]]
         """
         return self._signature
 
     @signature.setter
     def signature(self, signature):
-        """Sets the signature of this ProcedureSignaturesResponseDataProcedures.
+        """Sets the signature of this ProcedureSignature.
 
 
-        :param signature: The signature of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :param signature: The signature of this ProcedureSignature.  # noqa: E501
         :type: list[list[str]]
         """
 
         self._signature = signature
 
     @property
     def example_procedure(self):
-        """Gets the example_procedure of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        """Gets the example_procedure of this ProcedureSignature.  # noqa: E501
 
 
-        :return: The example_procedure of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :return: The example_procedure of this ProcedureSignature.  # noqa: E501
         :rtype: list[list[str]]
         """
         return self._example_procedure
 
     @example_procedure.setter
     def example_procedure(self, example_procedure):
-        """Sets the example_procedure of this ProcedureSignaturesResponseDataProcedures.
+        """Sets the example_procedure of this ProcedureSignature.
 
 
-        :param example_procedure: The example_procedure of this ProcedureSignaturesResponseDataProcedures.  # noqa: E501
+        :param example_procedure: The example_procedure of this ProcedureSignature.  # noqa: E501
         :type: list[list[str]]
         """
 
         self._example_procedure = example_procedure
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -398,15 +398,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProcedureSignaturesResponseDataProcedures):
+        if not isinstance(other, ProcedureSignature):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/campaign_members_response_data.py` & `cythereal-magic-1.9.1/cythereal_magic/models/magic_category_list.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,97 +12,98 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cythereal_magic.models.campaign_members_response_data_members import CampaignMembersResponseDataMembers  # noqa: F401,E501
+from cythereal_magic.models.magic_category import MagicCategory  # noqa: F401,E501
 
 
-class CampaignMembersResponseData(object):
+class MagicCategoryList(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'campaign_id': 'str',
-        'members': 'list[CampaignMembersResponseDataMembers]'
+        'count': 'int',
+        'categories': 'list[MagicCategory]'
     }
 
     attribute_map = {
-        'campaign_id': 'campaign_id',
-        'members': 'members'
+        'count': 'count',
+        'categories': 'categories'
     }
 
-    def __init__(self, campaign_id=None, members=None):  # noqa: E501
-        """CampaignMembersResponseData - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, count=None, categories=None):  # noqa: E501
+        """MagicCategoryList - a model defined in Swagger"""  # noqa: E501
 
-        self._campaign_id = None
-        self._members = None
+        self._count = None
+        self._categories = None
         self.discriminator = None
 
-        if campaign_id is not None:
-            self.campaign_id = campaign_id
-        if members is not None:
-            self.members = members
+        if count is not None:
+            self.count = count
+        self.categories = categories
 
     @property
-    def campaign_id(self):
-        """Gets the campaign_id of this CampaignMembersResponseData.  # noqa: E501
+    def count(self):
+        """Gets the count of this MagicCategoryList.  # noqa: E501
 
-        A SHA1 cryptographic hash  # noqa: E501
+        Count of total number of categories.  # noqa: E501
 
-        :return: The campaign_id of this CampaignMembersResponseData.  # noqa: E501
-        :rtype: str
+        :return: The count of this MagicCategoryList.  # noqa: E501
+        :rtype: int
         """
-        return self._campaign_id
+        return self._count
 
-    @campaign_id.setter
-    def campaign_id(self, campaign_id):
-        """Sets the campaign_id of this CampaignMembersResponseData.
+    @count.setter
+    def count(self, count):
+        """Sets the count of this MagicCategoryList.
 
-        A SHA1 cryptographic hash  # noqa: E501
+        Count of total number of categories.  # noqa: E501
 
-        :param campaign_id: The campaign_id of this CampaignMembersResponseData.  # noqa: E501
-        :type: str
+        :param count: The count of this MagicCategoryList.  # noqa: E501
+        :type: int
         """
-        if campaign_id is not None and not re.search('[a-fA-F0-9]{40}', campaign_id):  # noqa: E501
-            raise ValueError("Invalid value for `campaign_id`, must be a follow pattern or equal to `/[a-fA-F0-9]{40}/`")  # noqa: E501
 
-        self._campaign_id = campaign_id
+        self._count = count
 
     @property
-    def members(self):
-        """Gets the members of this CampaignMembersResponseData.  # noqa: E501
+    def categories(self):
+        """Gets the categories of this MagicCategoryList.  # noqa: E501
 
+        List of categories for this query binary.  # noqa: E501
 
-        :return: The members of this CampaignMembersResponseData.  # noqa: E501
-        :rtype: list[CampaignMembersResponseDataMembers]
+        :return: The categories of this MagicCategoryList.  # noqa: E501
+        :rtype: list[MagicCategory]
         """
-        return self._members
+        return self._categories
 
-    @members.setter
-    def members(self, members):
-        """Sets the members of this CampaignMembersResponseData.
+    @categories.setter
+    def categories(self, categories):
+        """Sets the categories of this MagicCategoryList.
 
+        List of categories for this query binary.  # noqa: E501
 
-        :param members: The members of this CampaignMembersResponseData.  # noqa: E501
-        :type: list[CampaignMembersResponseDataMembers]
+        :param categories: The categories of this MagicCategoryList.  # noqa: E501
+        :type: list[MagicCategory]
         """
+        if categories is None:
+            raise ValueError("Invalid value for `categories`, must not be `None`")  # noqa: E501
 
-        self._members = members
+        self._categories = categories
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -130,15 +131,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CampaignMembersResponseData):
+        if not isinstance(other, MagicCategoryList):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/__init__.py` & `cythereal-magic-1.9.1/cythereal_magic/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,17 @@
 from cythereal_magic.models.magic_matches_match_subtypes import MagicMatchesMatchSubtypes
 from cythereal_magic.models.magic_matches_matches import MagicMatchesMatches
 from cythereal_magic.models.magic_report import MagicReport
 from cythereal_magic.models.magic_report_detection_stats import MagicReportDetectionStats
 from cythereal_magic.models.owned_files_list import OwnedFilesList
 from cythereal_magic.models.owned_files_list_files import OwnedFilesListFiles
 from cythereal_magic.models.procedure_genomics import ProcedureGenomics
+from cythereal_magic.models.procedure_signature import ProcedureSignature
+from cythereal_magic.models.procedure_signature_list import ProcedureSignatureList
 from cythereal_magic.models.procedure_signatures_response_data import ProcedureSignaturesResponseData
-from cythereal_magic.models.procedure_signatures_response_data_procedures import ProcedureSignaturesResponseDataProcedures
 from cythereal_magic.models.procedure_similarity import ProcedureSimilarity
 from cythereal_magic.models.procedure_similarity_procedures import ProcedureSimilarityProcedures
 from cythereal_magic.models.error_response import ErrorResponse
 from cythereal_magic.models.success_response import SuccessResponse
 from cythereal_magic.models.binary_genomics_response import BinaryGenomicsResponse
 from cythereal_magic.models.binary_similarity_response import BinarySimilarityResponse
 from cythereal_magic.models.campaign_id_response import CampaignIdResponse
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/magic_report_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/magic_report_response.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/magic_categories_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/magic_categories_response.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/magic_category_list.py` & `cythereal-magic-1.9.1/cythereal_magic/models/campaign_info_response_links.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,98 +12,67 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cythereal_magic.models.magic_category import MagicCategory  # noqa: F401,E501
 
-
-class MagicCategoryList(object):
+class CampaignInfoResponseLinks(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'count': 'int',
-        'categories': 'list[MagicCategory]'
+        'members': 'str'
     }
 
     attribute_map = {
-        'count': 'count',
-        'categories': 'categories'
+        'members': 'members'
     }
 
-    def __init__(self, count=None, categories=None):  # noqa: E501
-        """MagicCategoryList - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, members=None):  # noqa: E501
+        """CampaignInfoResponseLinks - a model defined in Swagger"""  # noqa: E501
 
-        self._count = None
-        self._categories = None
+        self._members = None
         self.discriminator = None
 
-        if count is not None:
-            self.count = count
-        self.categories = categories
-
-    @property
-    def count(self):
-        """Gets the count of this MagicCategoryList.  # noqa: E501
-
-        Count of total number of categories.  # noqa: E501
-
-        :return: The count of this MagicCategoryList.  # noqa: E501
-        :rtype: int
-        """
-        return self._count
-
-    @count.setter
-    def count(self, count):
-        """Sets the count of this MagicCategoryList.
-
-        Count of total number of categories.  # noqa: E501
-
-        :param count: The count of this MagicCategoryList.  # noqa: E501
-        :type: int
-        """
-
-        self._count = count
+        if members is not None:
+            self.members = members
 
     @property
-    def categories(self):
-        """Gets the categories of this MagicCategoryList.  # noqa: E501
+    def members(self):
+        """Gets the members of this CampaignInfoResponseLinks.  # noqa: E501
 
-        List of categories for this query binary.  # noqa: E501
+        Link to the endpoint for retrieving campaign members  # noqa: E501
 
-        :return: The categories of this MagicCategoryList.  # noqa: E501
-        :rtype: list[MagicCategory]
+        :return: The members of this CampaignInfoResponseLinks.  # noqa: E501
+        :rtype: str
         """
-        return self._categories
+        return self._members
 
-    @categories.setter
-    def categories(self, categories):
-        """Sets the categories of this MagicCategoryList.
+    @members.setter
+    def members(self, members):
+        """Sets the members of this CampaignInfoResponseLinks.
 
-        List of categories for this query binary.  # noqa: E501
+        Link to the endpoint for retrieving campaign members  # noqa: E501
 
-        :param categories: The categories of this MagicCategoryList.  # noqa: E501
-        :type: list[MagicCategory]
+        :param members: The members of this CampaignInfoResponseLinks.  # noqa: E501
+        :type: str
         """
-        if categories is None:
-            raise ValueError("Invalid value for `categories`, must not be `None`")  # noqa: E501
 
-        self._categories = categories
+        self._members = members
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -131,15 +100,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MagicCategoryList):
+        if not isinstance(other, CampaignInfoResponseLinks):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/binary_genomics_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/magic_labels_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cythereal_magic.models.binary_genomics import BinaryGenomics  # noqa: F401,E501
+from cythereal_magic.models.magic_labels import MagicLabels  # noqa: F401,E501
 from cythereal_magic.models.success_response import SuccessResponse  # noqa: F401,E501
 
 
-class BinaryGenomicsResponse(object):
+class MagicLabelsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
@@ -34,27 +34,27 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'api_version': 'str',
         'success': 'bool',
         'code': 'int',
         'message': 'str',
-        'data': 'BinaryGenomics'
+        'data': 'MagicLabels'
     }
 
     attribute_map = {
         'api_version': 'api_version',
         'success': 'success',
         'code': 'code',
         'message': 'message',
         'data': 'data'
     }
 
     def __init__(self, api_version=None, success=None, code=None, message=None, data=None):  # noqa: E501
-        """BinaryGenomicsResponse - a model defined in Swagger"""  # noqa: E501
+        """MagicLabelsResponse - a model defined in Swagger"""  # noqa: E501
 
         self._api_version = None
         self._success = None
         self._code = None
         self._message = None
         self._data = None
         self.discriminator = None
@@ -64,125 +64,125 @@
         self.code = code
         if message is not None:
             self.message = message
         self.data = data
 
     @property
     def api_version(self):
-        """Gets the api_version of this BinaryGenomicsResponse.  # noqa: E501
+        """Gets the api_version of this MagicLabelsResponse.  # noqa: E501
 
         The current api version.  # noqa: E501
 
-        :return: The api_version of this BinaryGenomicsResponse.  # noqa: E501
+        :return: The api_version of this MagicLabelsResponse.  # noqa: E501
         :rtype: str
         """
         return self._api_version
 
     @api_version.setter
     def api_version(self, api_version):
-        """Sets the api_version of this BinaryGenomicsResponse.
+        """Sets the api_version of this MagicLabelsResponse.
 
         The current api version.  # noqa: E501
 
-        :param api_version: The api_version of this BinaryGenomicsResponse.  # noqa: E501
+        :param api_version: The api_version of this MagicLabelsResponse.  # noqa: E501
         :type: str
         """
         if api_version is None:
             raise ValueError("Invalid value for `api_version`, must not be `None`")  # noqa: E501
 
         self._api_version = api_version
 
     @property
     def success(self):
-        """Gets the success of this BinaryGenomicsResponse.  # noqa: E501
+        """Gets the success of this MagicLabelsResponse.  # noqa: E501
 
         MUST equal true.  # noqa: E501
 
-        :return: The success of this BinaryGenomicsResponse.  # noqa: E501
+        :return: The success of this MagicLabelsResponse.  # noqa: E501
         :rtype: bool
         """
         return self._success
 
     @success.setter
     def success(self, success):
-        """Sets the success of this BinaryGenomicsResponse.
+        """Sets the success of this MagicLabelsResponse.
 
         MUST equal true.  # noqa: E501
 
-        :param success: The success of this BinaryGenomicsResponse.  # noqa: E501
+        :param success: The success of this MagicLabelsResponse.  # noqa: E501
         :type: bool
         """
         if success is None:
             raise ValueError("Invalid value for `success`, must not be `None`")  # noqa: E501
 
         self._success = success
 
     @property
     def code(self):
-        """Gets the code of this BinaryGenomicsResponse.  # noqa: E501
+        """Gets the code of this MagicLabelsResponse.  # noqa: E501
 
 
-        :return: The code of this BinaryGenomicsResponse.  # noqa: E501
+        :return: The code of this MagicLabelsResponse.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
-        """Sets the code of this BinaryGenomicsResponse.
+        """Sets the code of this MagicLabelsResponse.
 
 
-        :param code: The code of this BinaryGenomicsResponse.  # noqa: E501
+        :param code: The code of this MagicLabelsResponse.  # noqa: E501
         :type: int
         """
         if code is None:
             raise ValueError("Invalid value for `code`, must not be `None`")  # noqa: E501
 
         self._code = code
 
     @property
     def message(self):
-        """Gets the message of this BinaryGenomicsResponse.  # noqa: E501
+        """Gets the message of this MagicLabelsResponse.  # noqa: E501
 
         A human readable message providing more details about the operation. Can be null or empty if no additional information is required.   # noqa: E501
 
-        :return: The message of this BinaryGenomicsResponse.  # noqa: E501
+        :return: The message of this MagicLabelsResponse.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this BinaryGenomicsResponse.
+        """Sets the message of this MagicLabelsResponse.
 
         A human readable message providing more details about the operation. Can be null or empty if no additional information is required.   # noqa: E501
 
-        :param message: The message of this BinaryGenomicsResponse.  # noqa: E501
+        :param message: The message of this MagicLabelsResponse.  # noqa: E501
         :type: str
         """
 
         self._message = message
 
     @property
     def data(self):
-        """Gets the data of this BinaryGenomicsResponse.  # noqa: E501
+        """Gets the data of this MagicLabelsResponse.  # noqa: E501
 
 
-        :return: The data of this BinaryGenomicsResponse.  # noqa: E501
-        :rtype: BinaryGenomics
+        :return: The data of this MagicLabelsResponse.  # noqa: E501
+        :rtype: MagicLabels
         """
         return self._data
 
     @data.setter
     def data(self, data):
-        """Sets the data of this BinaryGenomicsResponse.
+        """Sets the data of this MagicLabelsResponse.
 
 
-        :param data: The data of this BinaryGenomicsResponse.  # noqa: E501
-        :type: BinaryGenomics
+        :param data: The data of this MagicLabelsResponse.  # noqa: E501
+        :type: MagicLabels
         """
         if data is None:
             raise ValueError("Invalid value for `data`, must not be `None`")  # noqa: E501
 
         self._data = data
 
     def to_dict(self):
@@ -215,15 +215,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, BinaryGenomicsResponse):
+        if not isinstance(other, MagicLabelsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/procedure_genomics_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/procedure_genomics_response.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/binary_genomics.py` & `cythereal-magic-1.9.1/cythereal_magic/models/binary_genomics.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/magic_labels_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/binary_similarity_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cythereal_magic.models.magic_labels import MagicLabels  # noqa: F401,E501
+from cythereal_magic.models.binary_similarity import BinarySimilarity  # noqa: F401,E501
 from cythereal_magic.models.success_response import SuccessResponse  # noqa: F401,E501
 
 
-class MagicLabelsResponse(object):
+class BinarySimilarityResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
@@ -34,27 +34,27 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'api_version': 'str',
         'success': 'bool',
         'code': 'int',
         'message': 'str',
-        'data': 'MagicLabels'
+        'data': 'BinarySimilarity'
     }
 
     attribute_map = {
         'api_version': 'api_version',
         'success': 'success',
         'code': 'code',
         'message': 'message',
         'data': 'data'
     }
 
     def __init__(self, api_version=None, success=None, code=None, message=None, data=None):  # noqa: E501
-        """MagicLabelsResponse - a model defined in Swagger"""  # noqa: E501
+        """BinarySimilarityResponse - a model defined in Swagger"""  # noqa: E501
 
         self._api_version = None
         self._success = None
         self._code = None
         self._message = None
         self._data = None
         self.discriminator = None
@@ -64,125 +64,125 @@
         self.code = code
         if message is not None:
             self.message = message
         self.data = data
 
     @property
     def api_version(self):
-        """Gets the api_version of this MagicLabelsResponse.  # noqa: E501
+        """Gets the api_version of this BinarySimilarityResponse.  # noqa: E501
 
         The current api version.  # noqa: E501
 
-        :return: The api_version of this MagicLabelsResponse.  # noqa: E501
+        :return: The api_version of this BinarySimilarityResponse.  # noqa: E501
         :rtype: str
         """
         return self._api_version
 
     @api_version.setter
     def api_version(self, api_version):
-        """Sets the api_version of this MagicLabelsResponse.
+        """Sets the api_version of this BinarySimilarityResponse.
 
         The current api version.  # noqa: E501
 
-        :param api_version: The api_version of this MagicLabelsResponse.  # noqa: E501
+        :param api_version: The api_version of this BinarySimilarityResponse.  # noqa: E501
         :type: str
         """
         if api_version is None:
             raise ValueError("Invalid value for `api_version`, must not be `None`")  # noqa: E501
 
         self._api_version = api_version
 
     @property
     def success(self):
-        """Gets the success of this MagicLabelsResponse.  # noqa: E501
+        """Gets the success of this BinarySimilarityResponse.  # noqa: E501
 
         MUST equal true.  # noqa: E501
 
-        :return: The success of this MagicLabelsResponse.  # noqa: E501
+        :return: The success of this BinarySimilarityResponse.  # noqa: E501
         :rtype: bool
         """
         return self._success
 
     @success.setter
     def success(self, success):
-        """Sets the success of this MagicLabelsResponse.
+        """Sets the success of this BinarySimilarityResponse.
 
         MUST equal true.  # noqa: E501
 
-        :param success: The success of this MagicLabelsResponse.  # noqa: E501
+        :param success: The success of this BinarySimilarityResponse.  # noqa: E501
         :type: bool
         """
         if success is None:
             raise ValueError("Invalid value for `success`, must not be `None`")  # noqa: E501
 
         self._success = success
 
     @property
     def code(self):
-        """Gets the code of this MagicLabelsResponse.  # noqa: E501
+        """Gets the code of this BinarySimilarityResponse.  # noqa: E501
 
 
-        :return: The code of this MagicLabelsResponse.  # noqa: E501
+        :return: The code of this BinarySimilarityResponse.  # noqa: E501
         :rtype: int
         """
         return self._code
 
     @code.setter
     def code(self, code):
-        """Sets the code of this MagicLabelsResponse.
+        """Sets the code of this BinarySimilarityResponse.
 
 
-        :param code: The code of this MagicLabelsResponse.  # noqa: E501
+        :param code: The code of this BinarySimilarityResponse.  # noqa: E501
         :type: int
         """
         if code is None:
             raise ValueError("Invalid value for `code`, must not be `None`")  # noqa: E501
 
         self._code = code
 
     @property
     def message(self):
-        """Gets the message of this MagicLabelsResponse.  # noqa: E501
+        """Gets the message of this BinarySimilarityResponse.  # noqa: E501
 
         A human readable message providing more details about the operation. Can be null or empty if no additional information is required.   # noqa: E501
 
-        :return: The message of this MagicLabelsResponse.  # noqa: E501
+        :return: The message of this BinarySimilarityResponse.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this MagicLabelsResponse.
+        """Sets the message of this BinarySimilarityResponse.
 
         A human readable message providing more details about the operation. Can be null or empty if no additional information is required.   # noqa: E501
 
-        :param message: The message of this MagicLabelsResponse.  # noqa: E501
+        :param message: The message of this BinarySimilarityResponse.  # noqa: E501
         :type: str
         """
 
         self._message = message
 
     @property
     def data(self):
-        """Gets the data of this MagicLabelsResponse.  # noqa: E501
+        """Gets the data of this BinarySimilarityResponse.  # noqa: E501
 
 
-        :return: The data of this MagicLabelsResponse.  # noqa: E501
-        :rtype: MagicLabels
+        :return: The data of this BinarySimilarityResponse.  # noqa: E501
+        :rtype: BinarySimilarity
         """
         return self._data
 
     @data.setter
     def data(self, data):
-        """Sets the data of this MagicLabelsResponse.
+        """Sets the data of this BinarySimilarityResponse.
 
 
-        :param data: The data of this MagicLabelsResponse.  # noqa: E501
-        :type: MagicLabels
+        :param data: The data of this BinarySimilarityResponse.  # noqa: E501
+        :type: BinarySimilarity
         """
         if data is None:
             raise ValueError("Invalid value for `data`, must not be `None`")  # noqa: E501
 
         self._data = data
 
     def to_dict(self):
@@ -215,15 +215,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MagicLabelsResponse):
+        if not isinstance(other, BinarySimilarityResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/block_genomics.py` & `cythereal-magic-1.9.1/cythereal_magic/models/block_genomics.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/campaign_members_response_data_members.py` & `cythereal-magic-1.9.1/cythereal_magic/models/campaign_members_response_data_members.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/owned_files_list_files.py` & `cythereal-magic-1.9.1/cythereal_magic/models/owned_files_list_files.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/file_status_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/file_status_response.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/campaign_info_response_links.py` & `cythereal-magic-1.9.1/cythereal_magic/models/procedure_signature_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,68 +12,40 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
+from cythereal_magic.models.procedure_signature import ProcedureSignature  # noqa: F401,E501
 
-class CampaignInfoResponseLinks(object):
+
+class ProcedureSignatureList(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'members': 'str'
     }
 
     attribute_map = {
-        'members': 'members'
     }
 
-    def __init__(self, members=None):  # noqa: E501
-        """CampaignInfoResponseLinks - a model defined in Swagger"""  # noqa: E501
-
-        self._members = None
+    def __init__(self):  # noqa: E501
+        """ProcedureSignatureList - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
-        if members is not None:
-            self.members = members
-
-    @property
-    def members(self):
-        """Gets the members of this CampaignInfoResponseLinks.  # noqa: E501
-
-        Link to the endpoint for retrieving campaign members  # noqa: E501
-
-        :return: The members of this CampaignInfoResponseLinks.  # noqa: E501
-        :rtype: str
-        """
-        return self._members
-
-    @members.setter
-    def members(self, members):
-        """Sets the members of this CampaignInfoResponseLinks.
-
-        Link to the endpoint for retrieving campaign members  # noqa: E501
-
-        :param members: The members of this CampaignInfoResponseLinks.  # noqa: E501
-        :type: str
-        """
-
-        self._members = members
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -100,15 +72,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CampaignInfoResponseLinks):
+        if not isinstance(other, ProcedureSignatureList):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic/models/binary_similarity_response.py` & `cythereal-magic-1.9.1/cythereal_magic/models/magic_matches_matches.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,182 +12,159 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cythereal_magic.models.binary_similarity import BinarySimilarity  # noqa: F401,E501
-from cythereal_magic.models.success_response import SuccessResponse  # noqa: F401,E501
+from cythereal_magic.models.magic_matches_match_subtypes import MagicMatchesMatchSubtypes  # noqa: F401,E501
 
 
-class BinarySimilarityResponse(object):
+class MagicMatchesMatches(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'api_version': 'str',
-        'success': 'bool',
-        'code': 'int',
-        'message': 'str',
-        'data': 'BinarySimilarity'
+        'sha1': 'str',
+        'match_type': 'str',
+        'match_subtypes': 'list[MagicMatchesMatchSubtypes]',
+        'max_similarity': 'float'
     }
 
     attribute_map = {
-        'api_version': 'api_version',
-        'success': 'success',
-        'code': 'code',
-        'message': 'message',
-        'data': 'data'
+        'sha1': 'sha1',
+        'match_type': 'match_type',
+        'match_subtypes': 'match_subtypes',
+        'max_similarity': 'max_similarity'
     }
 
-    def __init__(self, api_version=None, success=None, code=None, message=None, data=None):  # noqa: E501
-        """BinarySimilarityResponse - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, sha1=None, match_type=None, match_subtypes=None, max_similarity=None):  # noqa: E501
+        """MagicMatchesMatches - a model defined in Swagger"""  # noqa: E501
 
-        self._api_version = None
-        self._success = None
-        self._code = None
-        self._message = None
-        self._data = None
+        self._sha1 = None
+        self._match_type = None
+        self._match_subtypes = None
+        self._max_similarity = None
         self.discriminator = None
 
-        self.api_version = api_version
-        self.success = success
-        self.code = code
-        if message is not None:
-            self.message = message
-        self.data = data
+        if sha1 is not None:
+            self.sha1 = sha1
+        if match_type is not None:
+            self.match_type = match_type
+        if match_subtypes is not None:
+            self.match_subtypes = match_subtypes
+        if max_similarity is not None:
+            self.max_similarity = max_similarity
 
     @property
-    def api_version(self):
-        """Gets the api_version of this BinarySimilarityResponse.  # noqa: E501
+    def sha1(self):
+        """Gets the sha1 of this MagicMatchesMatches.  # noqa: E501
 
-        The current api version.  # noqa: E501
+        The SHA1 of the matched binary.  # noqa: E501
 
-        :return: The api_version of this BinarySimilarityResponse.  # noqa: E501
+        :return: The sha1 of this MagicMatchesMatches.  # noqa: E501
         :rtype: str
         """
-        return self._api_version
+        return self._sha1
 
-    @api_version.setter
-    def api_version(self, api_version):
-        """Sets the api_version of this BinarySimilarityResponse.
+    @sha1.setter
+    def sha1(self, sha1):
+        """Sets the sha1 of this MagicMatchesMatches.
 
-        The current api version.  # noqa: E501
+        The SHA1 of the matched binary.  # noqa: E501
 
-        :param api_version: The api_version of this BinarySimilarityResponse.  # noqa: E501
+        :param sha1: The sha1 of this MagicMatchesMatches.  # noqa: E501
         :type: str
         """
-        if api_version is None:
-            raise ValueError("Invalid value for `api_version`, must not be `None`")  # noqa: E501
 
-        self._api_version = api_version
+        self._sha1 = sha1
 
     @property
-    def success(self):
-        """Gets the success of this BinarySimilarityResponse.  # noqa: E501
+    def match_type(self):
+        """Gets the match_type of this MagicMatchesMatches.  # noqa: E501
 
-        MUST equal true.  # noqa: E501
+        The MAGIC classification for the match.  # noqa: E501
 
-        :return: The success of this BinarySimilarityResponse.  # noqa: E501
-        :rtype: bool
-        """
-        return self._success
-
-    @success.setter
-    def success(self, success):
-        """Sets the success of this BinarySimilarityResponse.
-
-        MUST equal true.  # noqa: E501
-
-        :param success: The success of this BinarySimilarityResponse.  # noqa: E501
-        :type: bool
-        """
-        if success is None:
-            raise ValueError("Invalid value for `success`, must not be `None`")  # noqa: E501
-
-        self._success = success
-
-    @property
-    def code(self):
-        """Gets the code of this BinarySimilarityResponse.  # noqa: E501
-
-
-        :return: The code of this BinarySimilarityResponse.  # noqa: E501
-        :rtype: int
+        :return: The match_type of this MagicMatchesMatches.  # noqa: E501
+        :rtype: str
         """
-        return self._code
+        return self._match_type
 
-    @code.setter
-    def code(self, code):
-        """Sets the code of this BinarySimilarityResponse.
+    @match_type.setter
+    def match_type(self, match_type):
+        """Sets the match_type of this MagicMatchesMatches.
 
+        The MAGIC classification for the match.  # noqa: E501
 
-        :param code: The code of this BinarySimilarityResponse.  # noqa: E501
-        :type: int
+        :param match_type: The match_type of this MagicMatchesMatches.  # noqa: E501
+        :type: str
         """
-        if code is None:
-            raise ValueError("Invalid value for `code`, must not be `None`")  # noqa: E501
+        allowed_values = ["similar_packer_similar_payload", "similar_packer_different_payload", "different_packer_similar_payload", "weak_similar"]  # noqa: E501
+        if match_type not in allowed_values:
+            raise ValueError(
+                "Invalid value for `match_type` ({0}), must be one of {1}"  # noqa: E501
+                .format(match_type, allowed_values)
+            )
 
-        self._code = code
+        self._match_type = match_type
 
     @property
-    def message(self):
-        """Gets the message of this BinarySimilarityResponse.  # noqa: E501
+    def match_subtypes(self):
+        """Gets the match_subtypes of this MagicMatchesMatches.  # noqa: E501
 
-        A human readable message providing more details about the operation. Can be null or empty if no additional information is required.   # noqa: E501
+        Finer grained identification of match types.  # noqa: E501
 
-        :return: The message of this BinarySimilarityResponse.  # noqa: E501
-        :rtype: str
+        :return: The match_subtypes of this MagicMatchesMatches.  # noqa: E501
+        :rtype: list[MagicMatchesMatchSubtypes]
         """
-        return self._message
+        return self._match_subtypes
 
-    @message.setter
-    def message(self, message):
-        """Sets the message of this BinarySimilarityResponse.
+    @match_subtypes.setter
+    def match_subtypes(self, match_subtypes):
+        """Sets the match_subtypes of this MagicMatchesMatches.
 
-        A human readable message providing more details about the operation. Can be null or empty if no additional information is required.   # noqa: E501
+        Finer grained identification of match types.  # noqa: E501
 
-        :param message: The message of this BinarySimilarityResponse.  # noqa: E501
-        :type: str
+        :param match_subtypes: The match_subtypes of this MagicMatchesMatches.  # noqa: E501
+        :type: list[MagicMatchesMatchSubtypes]
         """
 
-        self._message = message
+        self._match_subtypes = match_subtypes
 
     @property
-    def data(self):
-        """Gets the data of this BinarySimilarityResponse.  # noqa: E501
+    def max_similarity(self):
+        """Gets the max_similarity of this MagicMatchesMatches.  # noqa: E501
 
+        The maximum similarity value from `match_subtypes`.  # noqa: E501
 
-        :return: The data of this BinarySimilarityResponse.  # noqa: E501
-        :rtype: BinarySimilarity
+        :return: The max_similarity of this MagicMatchesMatches.  # noqa: E501
+        :rtype: float
         """
-        return self._data
+        return self._max_similarity
 
-    @data.setter
-    def data(self, data):
-        """Sets the data of this BinarySimilarityResponse.
+    @max_similarity.setter
+    def max_similarity(self, max_similarity):
+        """Sets the max_similarity of this MagicMatchesMatches.
 
+        The maximum similarity value from `match_subtypes`.  # noqa: E501
 
-        :param data: The data of this BinarySimilarityResponse.  # noqa: E501
-        :type: BinarySimilarity
+        :param max_similarity: The max_similarity of this MagicMatchesMatches.  # noqa: E501
+        :type: float
         """
-        if data is None:
-            raise ValueError("Invalid value for `data`, must not be `None`")  # noqa: E501
 
-        self._data = data
+        self._max_similarity = max_similarity
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -215,15 +192,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, BinarySimilarityResponse):
+        if not isinstance(other, MagicMatchesMatches):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic/api/alpha_api.py` & `cythereal-magic-1.9.1/cythereal_magic/api/alpha_api.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/api/cythereal_magic_api.py` & `cythereal-magic-1.9.1/cythereal_magic/api/cythereal_magic_api.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/configuration.py` & `cythereal-magic-1.9.1/cythereal_magic/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,9 +248,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1\n"\
-               "SDK Package Version: 1.9.0".\
+               "SDK Package Version: 1.9.1".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic/rest.py` & `cythereal-magic-1.9.1/cythereal_magic/rest.py`

 * *Files identical despite different names*

### Comparing `cythereal-magic-1.9.0/cythereal_magic/__init__.py` & `cythereal-magic-1.9.1/cythereal_magic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,16 +48,17 @@
 from cythereal_magic.models.magic_matches_match_subtypes import MagicMatchesMatchSubtypes
 from cythereal_magic.models.magic_matches_matches import MagicMatchesMatches
 from cythereal_magic.models.magic_report import MagicReport
 from cythereal_magic.models.magic_report_detection_stats import MagicReportDetectionStats
 from cythereal_magic.models.owned_files_list import OwnedFilesList
 from cythereal_magic.models.owned_files_list_files import OwnedFilesListFiles
 from cythereal_magic.models.procedure_genomics import ProcedureGenomics
+from cythereal_magic.models.procedure_signature import ProcedureSignature
+from cythereal_magic.models.procedure_signature_list import ProcedureSignatureList
 from cythereal_magic.models.procedure_signatures_response_data import ProcedureSignaturesResponseData
-from cythereal_magic.models.procedure_signatures_response_data_procedures import ProcedureSignaturesResponseDataProcedures
 from cythereal_magic.models.procedure_similarity import ProcedureSimilarity
 from cythereal_magic.models.procedure_similarity_procedures import ProcedureSimilarityProcedures
 from cythereal_magic.models.error_response import ErrorResponse
 from cythereal_magic.models.success_response import SuccessResponse
 from cythereal_magic.models.binary_genomics_response import BinaryGenomicsResponse
 from cythereal_magic.models.binary_similarity_response import BinarySimilarityResponse
 from cythereal_magic.models.campaign_id_response import CampaignIdResponse
```

### Comparing `cythereal-magic-1.9.0/cythereal_magic/api_client.py` & `cythereal-magic-1.9.1/cythereal_magic/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/1.9.0/python'
+        self.user_agent = 'Swagger-Codegen/1.9.1/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `cythereal-magic-1.9.0/PKG-INFO` & `cythereal-magic-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: cythereal-magic
-Version: 1.9.0
+Version: 1.9.1
 Summary: Cythereal MAGIC API
 Home-page: UNKNOWN
 Author: UNKNOWN
 Author-email: support@cythereal.com
 License: UNKNOWN
 Description:      The API for accessing Cythereal MAGIC products and services.  # API Clients  We provide clients in several languages for accessing the MAGIC API. https://bitbucket.org/cythereal/magic-clients  These clients are provided to make integration of the MAGIC API into your existing applications as easy as possible.  If you want to use a language that is not currently supported, please contact us at support@cythereal.com and we will be glad to help.  # Example Inputs  Here are some example inputs that can be used for testing the service:  * Binary SHA1: &#x60;ff9790d7902fea4c910b182f6e0b00221a40d616&#x60;   * Can be used for &#x60;file_hash&#x60; parameters. * Procedure RVA: &#x60;0x1000&#x60;   * Use with the above SHA1 for &#x60;proc_rva&#x60; parameters.   # API Conventions  Properties MUST be named using &#x60;snake_case&#x60;.  This API is inspired by the [google json style guide](https://google.github.io/styleguide/jsoncstyleguide.xml). Any questions about conventions not documented here should be addressed by this style guide.  **All responses** MUST be of type &#x60;APIResponse&#x60; and contain the following fields:  * &#x60;api_version&#x60; |  The current api version * &#x60;success&#x60; | Boolean value indicating if the operation succeeded. * &#x60;code&#x60; | Status code. Typically corresponds to the HTTP status code.  * &#x60;message&#x60; | A human readable message providing more details about the operation. Can be null or empty.  **Successful operations** MUST return a &#x60;SuccessResponse&#x60;, which extends &#x60;APIResponse&#x60; by adding:  * &#x60;data&#x60; | Properties containing the response object. * &#x60;success&#x60; | MUST equal True  When returning objects from a successful response, the &#x60;data&#x60; object SHOULD contain a property named after the requested object type. For example, the &#x60;/matches&#x60; endpoint should return a response object with &#x60;data.matches&#x60;. This property SHOULD  contain a list of the returned objects. For the &#x60;/matches&#x60; endpoint, the &#x60;data.matches&#x60; property contains a list of MagicMatch objects. See the &#x60;/matches&#x60; endpoint documentation for an example.  **Failed Operations** MUST return an &#x60;ErrorResponse&#x60;, which extends &#x60;APIResponse&#x60; by adding:  * &#x60;errors&#x60; | Array of error objects. An error object contains the following properties:     * &#x60;ErrorObject.reason&#x60; | Unique identifier for this error. Example: \&quot;FileNotFoundError\&quot;.     * &#x60;ErrorObject.message&#x60;| Human readable error message. * &#x60;success&#x60; | MUST equal False.   # noqa: E501
```

