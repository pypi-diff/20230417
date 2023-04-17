# Comparing `tmp/rucio-clients-1.9.5.tar.gz` & `tmp/rucio-clients-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rucio-clients-1.9.5.tar", last modified: Tue Jan 24 09:13:59 2017, max compression
+gzip compressed data, was "dist/rucio-clients-1.9.6.tar", last modified: Tue Feb  7 09:03:44 2017, max compression
```

## Comparing `rucio-clients-1.9.5.tar` & `rucio-clients-1.9.6.tar`

### file list

```diff
@@ -1,788 +1,788 @@
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/bin/
--rwxr-xr-x   0 barisits (51071) zp        (1307)   120671 2017-01-24 09:05:38.000000 rucio-clients-1.9.5/bin/rucio
--rwxr-xr-x   0 barisits (51071) zp        (1307)    44207 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/bin/rucio-admin
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/atlasnote/
--rwxr-xr-x   0 barisits (51071) zp        (1307)   164832 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/AN_atlaslogo.pdf
--rwxr-xr-x   0 barisits (51071) zp        (1307)    88058 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/AN_cernlogo.pdf
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2877 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/AtlasRucioNote.aux
--rw-r--r--   0 barisits (51071) zp        (1307)   440060 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/AtlasRucioNote.pdf
--rwxr-xr-x   0 barisits (51071) zp        (1307)    23795 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/AtlasRucioNote.tex
--rw-r--r--   0 barisits (51071) zp        (1307)    65762 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/accounts.graffle
--rw-r--r--   0 barisits (51071) zp        (1307)    31807 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/accounts.pdf
--rw-r--r--   0 barisits (51071) zp        (1307)    27065 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/accounts.png
--rw-r--r--   0 barisits (51071) zp        (1307)   125132 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/aggregation_hierarchy.graffle
--rw-r--r--   0 barisits (51071) zp        (1307)    44183 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/aggregation_hierarchy.pdf
--rwxr-xr-x   0 barisits (51071) zp        (1307)     6980 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/atlasnote.cls
--rwxr-xr-x   0 barisits (51071) zp        (1307)     6557 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/booktabs.sty
--rw-r--r--   0 barisits (51071) zp        (1307)   132902 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/dataset_hierarchy.graffle
--rw-r--r--   0 barisits (51071) zp        (1307)    44639 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/dataset_hierarchy.pdf
--rwxr-xr-x   0 barisits (51071) zp        (1307)    18775 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/fncychap.sty
--rwxr-xr-x   0 barisits (51071) zp        (1307)    14665 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/sphinx.sty
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2073 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/sphinxhowto.cls
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3421 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/atlasnote/sphinxmanual.cls
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/doctrees/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/doctrees/man/
--rw-r--r--   0 barisits (51071) zp        (1307)    13923 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/man/rucio-admin.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    21710 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/man/rucio.doctree
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/doctrees/rest/
--rw-r--r--   0 barisits (51071) zp        (1307)     6101 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/rest/attach_dids_to_dids.doctree
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/
--rw-r--r--   0 barisits (51071) zp        (1307)     4822 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/add_account_identity.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4818 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/add_metadata_dataset.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4785 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/add_metadata_file.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5249 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/add_scope_to_account.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     8508 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/add_subscription.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    12024 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/authentication.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4960 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/consistency_file_between_storage_and_rucio.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5038 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/delete_file_replica_from_storage.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4927 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/detect_site_reach_watermark.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5230 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4988 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/download_all_files_from_a_given_list_of_files_from_rucio.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5030 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/download_all_files_in_a_dataset_from_rucio.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4835 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/download_files_from_rucio.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4400 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/obsolete_dataset.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5231 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/register_account.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5081 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/register_file_already_on_storage_system.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4524 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/register_transfer_request_file_fts.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4380 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/remove_replication_rules_from_file.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5772 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/reupload_after_failure.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     7617 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/search.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     3221 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/select_unwanted_files_for_deletion.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4412 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/set_replication_rule_to_file.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5464 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/upload_file_with_replication_rule.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     7457 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/usecase_upload_file_into_rucio.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5107 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases/where_are_the_replicas_for_a_file.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     7150 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/Acronyms_and_Abbreviations.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     2393 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/doctrees/Architecture.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    21792 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/Comparison_matrix.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    81561 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/REST_Account.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     8685 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/REST_Intro.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    28088 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/REST_authentication.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    90687 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/REST_did.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     8194 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/REST_identity.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     9921 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/REST_lock.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    19528 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/REST_meta.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     7204 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/REST_redirect.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    43167 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/REST_replica.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    93418 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/REST_rse.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    33047 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/REST_rule.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    14549 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/REST_scope.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    31270 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/REST_subscription.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     8088 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/doctrees/Rucio_Project_Meeting.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    78224 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/account.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    21746 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/accountlimit.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)   196168 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/api_curl_examples.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    27111 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/atlas_integration_testbed.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     2054 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/authentication_and_identity.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    27974 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/cli_admin_examples.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    21844 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/doctrees/cli_examples.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     8060 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/client_examples.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)   116795 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/client_howto.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    39959 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/doctrees/client_tutorial.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)   155605 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/core_constants.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    21418 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/developing.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    18604 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/development_guidelines.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)   153643 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/doctrees/did.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)   452979 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/environment.pickle
--rw-r--r--   0 barisits (51071) zp        (1307)   224246 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/exception.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    37099 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/identity.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    18065 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/index.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    15084 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/installing_atlas_clients.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    11551 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/installing_clients.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    12786 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/installing_server.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    19939 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/lock.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    39479 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/meta-data.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     7248 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/naming_convention_db.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     3506 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Accounting_and_quota.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     2773 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Architecture.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     9766 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Data_Deletion.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     3278 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Database_Schema.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     3459 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Deployment.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     6135 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Exception_Handling.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    17155 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_File_Dataset_Container.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     6672 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Meta-data_attributes.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     3043 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Notifications.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     2956 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Permission_model.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     9183 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Replica_management.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     6869 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Rucio_Storage_Element.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)   117157 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Rucio_Storage_Element_Manager.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5437 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Rucio_account.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    95260 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Rules.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     9339 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Scheduled_Transfers.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    35789 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Subscriptions.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     3214 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_Traceability_and_logging.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     3326 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/overview_flow.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     9984 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/permission.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     3498 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/replica.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    23662 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/replication_rules_examples.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    94015 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/rest.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)   183082 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/rse.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     7070 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/rucio_cli.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5185 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/rucio_clients.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    41739 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/rule.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4903 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/rules_workflow.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    25243 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/doctrees/scope.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    40983 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/setup.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    48626 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/subscription.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    28243 2016-11-25 15:03:17.000000 rucio-clients-1.9.5/doc/build/doctrees/usecases.doctree
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/_images/
--rw-r--r--   0 barisits (51071) zp        (1307)    71679 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_images/RSE_overview.png
--rw-r--r--   0 barisits (51071) zp        (1307)    45789 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_images/RSE_sequence_instantiation.png
--rw-r--r--   0 barisits (51071) zp        (1307)    32727 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_images/RSE_sequence_usage.png
--rw-r--r--   0 barisits (51071) zp        (1307)    56522 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_images/accounts.png
--rw-r--r--   0 barisits (51071) zp        (1307)   136638 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_images/architecture.png
--rw-r--r--   0 barisits (51071) zp        (1307)    82950 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_images/deployment.png
--rw-r--r--   0 barisits (51071) zp        (1307)   163115 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_images/exception_handling.png
--rw-r--r--   0 barisits (51071) zp        (1307)    45282 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_images/rucio-get.png
--rw-r--r--   0 barisits (51071) zp        (1307)    73288 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_images/rucio-put.png
--rw-r--r--   0 barisits (51071) zp        (1307)    55513 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_images/rucio-register.png
--rw-r--r--   0 barisits (51071) zp        (1307)   230376 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_images/rucio_schema.png
--rw-r--r--   0 barisits (51071) zp        (1307)    26628 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_images/scheduled_transfers.png
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/_modules/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/api/
--rw-r--r--   0 barisits (51071) zp        (1307)    16466 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/api/identity.html
--rw-r--r--   0 barisits (51071) zp        (1307)     6844 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/api/permission.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/
--rw-r--r--   0 barisits (51071) zp        (1307)    59303 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/accountclient.html
--rw-r--r--   0 barisits (51071) zp        (1307)    14938 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/accountlimitclient.html
--rw-r--r--   0 barisits (51071) zp        (1307)    93774 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/didclient.html
--rw-r--r--   0 barisits (51071) zp        (1307)    14712 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/lockclient.html
--rw-r--r--   0 barisits (51071) zp        (1307)    23765 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/metaclient.html
--rw-r--r--   0 barisits (51071) zp        (1307)    77886 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/rseclient.html
--rw-r--r--   0 barisits (51071) zp        (1307)    29268 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/ruleclient.html
--rw-r--r--   0 barisits (51071) zp        (1307)    17486 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/scopeclient.html
--rw-r--r--   0 barisits (51071) zp        (1307)    29268 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/subscriptionclient.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/common/
--rw-r--r--   0 barisits (51071) zp        (1307)   100322 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/common/exception.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/db/
--rw-r--r--   0 barisits (51071) zp        (1307)    25179 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/db/constants.html
--rw-r--r--   0 barisits (51071) zp        (1307)    20480 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/db/enum.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/rse/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/rse/protocols/
--rw-r--r--   0 barisits (51071) zp        (1307)    51488 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/rse/protocols/protocol.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/web/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/web/rest/
--rw-r--r--   0 barisits (51071) zp        (1307)    11578 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/rucio/web/rest/ping.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5307 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_modules/index.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/_sources/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/_sources/man/
--rw-r--r--   0 barisits (51071) zp        (1307)      770 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/man/rucio-admin.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1744 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/man/rucio.txt
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/_sources/rest/
--rw-r--r--   0 barisits (51071) zp        (1307)      350 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/rest/attach_dids_to_dids.txt
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/
--rw-r--r--   0 barisits (51071) zp        (1307)      783 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/add_account_identity.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      708 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/add_metadata_dataset.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      691 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/add_metadata_file.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      655 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/add_scope_to_account.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1470 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/add_subscription.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1677 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/authentication.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      804 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/consistency_file_between_storage_and_rucio.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      902 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/delete_file_replica_from_storage.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      795 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/detect_site_reach_watermark.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      940 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      886 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/download_all_files_from_a_given_list_of_files_from_rucio.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      900 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/download_all_files_in_a_dataset_from_rucio.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      794 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/download_files_from_rucio.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      564 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/obsolete_dataset.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      652 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/register_account.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      916 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/register_file_already_on_storage_system.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      646 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/register_transfer_request_file_fts.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      563 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/remove_replication_rules_from_file.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1270 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/reupload_after_failure.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1102 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/search.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      409 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/select_unwanted_files_for_deletion.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      590 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/set_replication_rule_to_file.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      852 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/upload_file_with_replication_rule.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1106 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/usecase_upload_file_into_rucio.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      633 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases/where_are_the_replicas_for_a_file.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      325 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/Acronyms_and_Abbreviations.txt
--rw-r--r--   0 barisits (51071) zp        (1307)       39 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/Architecture.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2067 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/Comparison_matrix.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     7173 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/REST_Account.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1586 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/REST_Intro.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2439 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/REST_authentication.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     7945 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/REST_did.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      611 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/REST_identity.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      637 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/REST_lock.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1444 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/REST_meta.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      349 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/REST_redirect.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     3702 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/REST_replica.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     7502 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/REST_rse.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2509 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/REST_rule.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1034 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/REST_scope.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2512 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/REST_subscription.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      662 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/Rucio_Project_Meeting.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      163 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/account.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      184 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/accountlimit.txt
--rw-r--r--   0 barisits (51071) zp        (1307)    16748 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/api_curl_examples.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2265 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/atlas_integration_testbed.txt
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/authentication_and_identity.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     4204 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/cli_admin_examples.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     4565 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/cli_examples.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1010 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/client_examples.txt
--rw-r--r--   0 barisits (51071) zp        (1307)    24065 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/client_howto.txt
--rw-r--r--   0 barisits (51071) zp        (1307)    11591 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/client_tutorial.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      138 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/core_constants.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     4981 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/developing.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     3281 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/development_guidelines.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      180 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/did.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      165 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/exception.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      162 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/identity.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2917 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/index.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2167 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/installing_atlas_clients.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1601 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/installing_clients.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1693 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/installing_server.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      152 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/lock.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      162 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/meta-data.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1180 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/naming_convention_db.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      475 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Accounting_and_quota.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      157 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Architecture.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1905 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Data_Deletion.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      311 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Database_Schema.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      442 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Deployment.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1514 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Exception_Handling.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     3882 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_File_Dataset_Container.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      894 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Meta-data_attributes.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      292 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Notifications.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      251 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Permission_model.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1911 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Replica_management.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1652 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Rucio_Storage_Element.txt
--rw-r--r--   0 barisits (51071) zp        (1307)    27901 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Rucio_Storage_Element_Manager.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1142 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Rucio_account.txt
--rw-r--r--   0 barisits (51071) zp        (1307)    23147 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Rules.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2701 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Scheduled_Transfers.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     4241 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Subscriptions.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      382 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_Traceability_and_logging.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      347 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/overview_flow.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      169 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/permission.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      155 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/replica.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     3376 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/replication_rules_examples.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     7948 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/rest.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      453 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/rse.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      717 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/rucio_cli.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      814 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/rucio_clients.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      183 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/rule.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1414 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/rules_workflow.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      158 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/scope.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     6529 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/setup.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      190 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/subscription.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2438 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_sources/usecases.txt
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/_static/
--rw-r--r--   0 barisits (51071) zp        (1307)      673 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/ajax-loader.gif
--rw-r--r--   0 barisits (51071) zp        (1307)     8270 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/basic.css
--rw-r--r--   0 barisits (51071) zp        (1307)     4125 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/classic.css
--rw-r--r--   0 barisits (51071) zp        (1307)     3500 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/comment-bright.png
--rw-r--r--   0 barisits (51071) zp        (1307)     3578 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/comment-close.png
--rw-r--r--   0 barisits (51071) zp        (1307)     3445 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/comment.png
--rw-r--r--   0 barisits (51071) zp        (1307)     4041 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/default.css
--rw-r--r--   0 barisits (51071) zp        (1307)     7377 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/doctools.js
--rw-r--r--   0 barisits (51071) zp        (1307)      347 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/down-pressed.png
--rw-r--r--   0 barisits (51071) zp        (1307)      347 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/down.png
--rw-r--r--   0 barisits (51071) zp        (1307)      358 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/file.png
--rw-r--r--   0 barisits (51071) zp        (1307)   282766 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/jquery-1.11.1.js
--rw-r--r--   0 barisits (51071) zp        (1307)    95786 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/jquery.js
--rw-r--r--   0 barisits (51071) zp        (1307)      173 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/minus.png
--rw-r--r--   0 barisits (51071) zp        (1307)      173 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/plus.png
--rw-r--r--   0 barisits (51071) zp        (1307)     3991 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/pygments.css
--rw-r--r--   0 barisits (51071) zp        (1307)    19563 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/rucio_logo.png
--rw-r--r--   0 barisits (51071) zp        (1307)    17880 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/searchtools.js
--rw-r--r--   0 barisits (51071) zp        (1307)     4803 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/sidebar.js
--rw-r--r--   0 barisits (51071) zp        (1307)    35168 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/underscore-1.3.1.js
--rw-r--r--   0 barisits (51071) zp        (1307)    12140 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/underscore.js
--rw-r--r--   0 barisits (51071) zp        (1307)      345 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/up-pressed.png
--rw-r--r--   0 barisits (51071) zp        (1307)      345 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/up.png
--rw-r--r--   0 barisits (51071) zp        (1307)    25350 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/_static/websupport.js
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/man/
--rw-r--r--   0 barisits (51071) zp        (1307)     7794 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/man/rucio-admin.html
--rw-r--r--   0 barisits (51071) zp        (1307)     9052 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/man/rucio.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/rest/
--rw-r--r--   0 barisits (51071) zp        (1307)     5795 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/rest/attach_dids_to_dids.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/build/html/usecases/
--rw-r--r--   0 barisits (51071) zp        (1307)     4477 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/add_account_identity.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4558 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/add_metadata_dataset.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4543 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/add_metadata_file.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4538 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/add_scope_to_account.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4872 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/add_subscription.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5938 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/authentication.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4716 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/consistency_file_between_storage_and_rucio.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4557 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/delete_file_replica_from_storage.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4701 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/detect_site_reach_watermark.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4745 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4665 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/download_all_files_from_a_given_list_of_files_from_rucio.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4595 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/download_all_files_in_a_dataset_from_rucio.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4510 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/download_files_from_rucio.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4433 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/obsolete_dataset.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4551 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/register_account.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4548 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/register_file_already_on_storage_system.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4567 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/register_transfer_request_file_fts.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4523 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/remove_replication_rules_from_file.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4531 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/reupload_after_failure.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4876 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/search.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4523 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/select_unwanted_files_for_deletion.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4549 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/set_replication_rule_to_file.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4671 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/upload_file_with_replication_rule.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5164 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/usecase_upload_file_into_rucio.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4518 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/usecases/where_are_the_replicas_for_a_file.html
--rw-r--r--   0 barisits (51071) zp        (1307)      230 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/.buildinfo
--rw-r--r--   0 barisits (51071) zp        (1307)     5302 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/Acronyms_and_Abbreviations.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4352 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/Architecture.html
--rw-r--r--   0 barisits (51071) zp        (1307)     6632 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/Comparison_matrix.html
--rw-r--r--   0 barisits (51071) zp        (1307)    33965 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/REST_Account.html
--rw-r--r--   0 barisits (51071) zp        (1307)     8155 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/REST_Intro.html
--rw-r--r--   0 barisits (51071) zp        (1307)    13611 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/REST_authentication.html
--rw-r--r--   0 barisits (51071) zp        (1307)    36870 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/REST_did.html
--rw-r--r--   0 barisits (51071) zp        (1307)     7178 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/REST_identity.html
--rw-r--r--   0 barisits (51071) zp        (1307)     8464 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/REST_lock.html
--rw-r--r--   0 barisits (51071) zp        (1307)    11196 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/REST_meta.html
--rw-r--r--   0 barisits (51071) zp        (1307)     6873 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/REST_redirect.html
--rw-r--r--   0 barisits (51071) zp        (1307)    19743 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/REST_replica.html
--rw-r--r--   0 barisits (51071) zp        (1307)    36294 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/REST_rse.html
--rw-r--r--   0 barisits (51071) zp        (1307)    15403 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/REST_rule.html
--rw-r--r--   0 barisits (51071) zp        (1307)     9564 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/REST_scope.html
--rw-r--r--   0 barisits (51071) zp        (1307)    15806 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/REST_subscription.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5982 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/Rucio_Project_Meeting.html
--rw-r--r--   0 barisits (51071) zp        (1307)    24371 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/account.html
--rw-r--r--   0 barisits (51071) zp        (1307)     9490 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/accountlimit.html
--rw-r--r--   0 barisits (51071) zp        (1307)    49271 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/api_curl_examples.html
--rw-r--r--   0 barisits (51071) zp        (1307)     8847 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/atlas_integration_testbed.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4218 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/authentication_and_identity.html
--rw-r--r--   0 barisits (51071) zp        (1307)    20697 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/cli_admin_examples.html
--rw-r--r--   0 barisits (51071) zp        (1307)    16629 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/cli_examples.html
--rw-r--r--   0 barisits (51071) zp        (1307)     7763 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/client_examples.html
--rw-r--r--   0 barisits (51071) zp        (1307)    51571 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/client_howto.html
--rw-r--r--   0 barisits (51071) zp        (1307)    22174 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/client_tutorial.html
--rw-r--r--   0 barisits (51071) zp        (1307)    38831 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/core_constants.html
--rw-r--r--   0 barisits (51071) zp        (1307)    13195 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/developing.html
--rw-r--r--   0 barisits (51071) zp        (1307)    11262 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/development_guidelines.html
--rw-r--r--   0 barisits (51071) zp        (1307)    42116 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/did.html
--rw-r--r--   0 barisits (51071) zp        (1307)    64292 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/exception.html
--rw-r--r--   0 barisits (51071) zp        (1307)    54351 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/genindex.html
--rw-r--r--   0 barisits (51071) zp        (1307)    22008 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/http-routingtable.html
--rw-r--r--   0 barisits (51071) zp        (1307)    13231 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/identity.html
--rw-r--r--   0 barisits (51071) zp        (1307)    15245 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/index.html
--rw-r--r--   0 barisits (51071) zp        (1307)    10693 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/installing_atlas_clients.html
--rw-r--r--   0 barisits (51071) zp        (1307)     9658 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/installing_clients.html
--rw-r--r--   0 barisits (51071) zp        (1307)     8756 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/installing_server.html
--rw-r--r--   0 barisits (51071) zp        (1307)     9333 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/lock.html
--rw-r--r--   0 barisits (51071) zp        (1307)    13990 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/meta-data.html
--rw-r--r--   0 barisits (51071) zp        (1307)     8368 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/naming_convention_db.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4611 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/objects.inv
--rw-r--r--   0 barisits (51071) zp        (1307)     5892 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_Accounting_and_quota.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5729 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_Architecture.html
--rw-r--r--   0 barisits (51071) zp        (1307)     7965 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_Data_Deletion.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5828 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_Database_Schema.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5590 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_Deployment.html
--rw-r--r--   0 barisits (51071) zp        (1307)     7307 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_Exception_Handling.html
--rw-r--r--   0 barisits (51071) zp        (1307)    11254 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_File_Dataset_Container.html
--rw-r--r--   0 barisits (51071) zp        (1307)     6831 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_Meta-data_attributes.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5732 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_Notifications.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5700 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_Permission_model.html
--rw-r--r--   0 barisits (51071) zp        (1307)     8062 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_Replica_management.html
--rw-r--r--   0 barisits (51071) zp        (1307)     7173 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_Rucio_Storage_Element.html
--rw-r--r--   0 barisits (51071) zp        (1307)    46544 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_Rucio_Storage_Element_Manager.html
--rw-r--r--   0 barisits (51071) zp        (1307)     6701 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_Rucio_account.html
--rw-r--r--   0 barisits (51071) zp        (1307)    36223 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/overview_Rules.html
--rw-r--r--   0 barisits (51071) zp        (1307)     8997 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_Scheduled_Transfers.html
--rw-r--r--   0 barisits (51071) zp        (1307)    14110 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_Subscriptions.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4733 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_Traceability_and_logging.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5951 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/overview_flow.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5808 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/permission.html
--rw-r--r--   0 barisits (51071) zp        (1307)     7644 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/py-modindex.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5259 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/replica.html
--rw-r--r--   0 barisits (51071) zp        (1307)    11051 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/replication_rules_examples.html
--rw-r--r--   0 barisits (51071) zp        (1307)    22089 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/rest.html
--rw-r--r--   0 barisits (51071) zp        (1307)    47247 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/rse.html
--rw-r--r--   0 barisits (51071) zp        (1307)     6001 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/rucio_cli.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5824 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/rucio_clients.html
--rw-r--r--   0 barisits (51071) zp        (1307)    13860 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/rule.html
--rw-r--r--   0 barisits (51071) zp        (1307)     6962 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/rules_workflow.html
--rw-r--r--   0 barisits (51071) zp        (1307)    10313 2016-11-25 15:03:15.000000 rucio-clients-1.9.5/doc/build/html/scope.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4453 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/search.html
--rw-r--r--   0 barisits (51071) zp        (1307)    57160 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/searchindex.js
--rw-r--r--   0 barisits (51071) zp        (1307)    17589 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/setup.html
--rw-r--r--   0 barisits (51071) zp        (1307)    14675 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/subscription.html
--rw-r--r--   0 barisits (51071) zp        (1307)    10373 2016-11-25 15:03:16.000000 rucio-clients-1.9.5/doc/build/html/usecases.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/design/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/design/RSE/
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1996 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/design/RSE/meeting-2012-02-23.org
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/design/erd/
--rwxr-xr-x   0 barisits (51071) zp        (1307)    55942 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/design/erd/ERD.graffle
--rwxr-xr-x   0 barisits (51071) zp        (1307)    72676 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/design/erd/ERD.pdf
--rwxr-xr-x   0 barisits (51071) zp        (1307)    60363 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/design/rucio_schema.pdf
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/source/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/source/_static/
--rwxr-xr-x   0 barisits (51071) zp        (1307)     8270 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/_static/basic.css
--rw-r--r--   0 barisits (51071) zp        (1307)     4179 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/_static/classic.css
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4041 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/_static/default.css
--rwxr-xr-x   0 barisits (51071) zp        (1307)    19563 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/_static/rucio_logo.png
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/source/_templates/
--rwxr-xr-x   0 barisits (51071) zp        (1307)      777 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/_templates/layout.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/source/cli_examples/
--rw-r--r--   0 barisits (51071) zp        (1307)       14 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/cli_examples/ping.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)       12 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/cli_examples/ping.sh
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/source/curl_examples/
--rw-r--r--   0 barisits (51071) zp        (1307)      235 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/del_account.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      312 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/del_account.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/del_location.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      313 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/del_location.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      404 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_account.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      309 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_account.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      673 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_account_whoami.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      314 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_account_whoami.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      253 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_accounts.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      305 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_accounts.sh
--rw-r--r--   0 barisits (51071) zp        (1307)       29 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_api.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)       34 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_api.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_auth_gss.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      129 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_auth_gss.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_auth_userpass.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      168 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_auth_userpass.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      304 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_auth_validate.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      334 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_auth_validate.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_auth_x509.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      139 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_auth_x509.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_location.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      310 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_location.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      239 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_locations.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      306 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_locations.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      356 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_scopes.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      309 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/get_scopes.sh
--rwxr-xr-x   0 barisits (51071) zp        (1307)      380 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/post_account.sh
--rwxr-xr-x   0 barisits (51071) zp        (1307)      332 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/post_location.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      370 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/post_location_rse.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      257 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/put_account.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      331 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/put_account.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/put_location.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      309 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/put_location.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      257 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/put_scope.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      314 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/curl_examples/put_scope.sh
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/source/example_outputs/
--rw-r--r--   0 barisits (51071) zp        (1307)     3643 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/example_outputs/failure-rucio.tests.test_curl.TestCurlRucio.test_get_accounts_whoami.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      164 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/example_outputs/success-rucio.tests.test_bin_rucio.TestBinRucio.test_add_account.txt
--rw-r--r--   0 barisits (51071) zp        (1307)       43 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/example_outputs/success-rucio.tests.test_bin_rucio.TestBinRucio.test_rucio_ping.txt
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/example_outputs/success-rucio.tests.test_bin_rucio.TestBinRucio.test_rucio_version.txt
--rw-r--r--   0 barisits (51071) zp        (1307)       46 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/example_outputs/success-rucio.tests.test_clients.TestRucioClients.test_ping.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      804 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_accounts_whoami.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      429 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_GSS.txt
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_proxy.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      466 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_userpass.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      454 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_validate.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      442 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_x509.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      454 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_x509_proxy.txt
--rw-r--r--   0 barisits (51071) zp        (1307)       84 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_ping.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      440 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_post_account.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      398 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_post_rse.txt
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/source/images/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/source/images/deployment.graffle/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/source/images/deployment.graffle/QuickLook/
--rw-r--r--   0 barisits (51071) zp        (1307)    52757 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/deployment.graffle/QuickLook/Preview.pdf
--rw-r--r--   0 barisits (51071) zp        (1307)   124440 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/deployment.graffle/QuickLook/Thumbnail.tiff
--rw-r--r--   0 barisits (51071) zp        (1307)     3172 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/deployment.graffle/data.plist
--rw-r--r--   0 barisits (51071) zp        (1307)    26954 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/deployment.graffle/image2.tiff
--rw-r--r--   0 barisits (51071) zp        (1307)    10020 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/deployment.graffle/image3.tiff
--rwxr-xr-x   0 barisits (51071) zp        (1307)    71679 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/RSE_overview.png
--rwxr-xr-x   0 barisits (51071) zp        (1307)    45789 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/RSE_sequence_instantiation.png
--rwxr-xr-x   0 barisits (51071) zp        (1307)    32727 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/RSE_sequence_usage.png
--rwxr-xr-x   0 barisits (51071) zp        (1307)    56522 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/accounts.png
--rw-r--r--   0 barisits (51071) zp        (1307)   397841 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/architecture.graffle
--rw-r--r--   0 barisits (51071) zp        (1307)   136638 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/architecture.png
--rw-r--r--   0 barisits (51071) zp        (1307)    82950 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/deployment.png
--rwxr-xr-x   0 barisits (51071) zp        (1307)    70361 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/exception_handling.graffle
--rwxr-xr-x   0 barisits (51071) zp        (1307)   163115 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/exception_handling.png
--rwxr-xr-x   0 barisits (51071) zp        (1307)   127009 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/highLevelRoadmap.graffle
--rwxr-xr-x   0 barisits (51071) zp        (1307)   205501 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/rucio-get.graffle
--rwxr-xr-x   0 barisits (51071) zp        (1307)    45282 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/rucio-get.png
--rwxr-xr-x   0 barisits (51071) zp        (1307)   298526 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/rucio-put.graffle
--rwxr-xr-x   0 barisits (51071) zp        (1307)    73288 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/rucio-put.png
--rwxr-xr-x   0 barisits (51071) zp        (1307)   232239 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/rucio-register.graffle
--rwxr-xr-x   0 barisits (51071) zp        (1307)    55513 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/rucio-register.png
--rw-r--r--   0 barisits (51071) zp        (1307)    62543 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/rucio_schema.gml
--rwxr-xr-x   0 barisits (51071) zp        (1307)   226250 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/images/rucio_schema.pdf
--rwxr-xr-x   0 barisits (51071) zp        (1307)   230376 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/images/rucio_schema.png
--rw-r--r--   0 barisits (51071) zp        (1307)     2485 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/images/scheduled_transfers.dia
--rw-r--r--   0 barisits (51071) zp        (1307)    26628 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/images/scheduled_transfers.png
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/source/man/
--rwxr-xr-x   0 barisits (51071) zp        (1307)      770 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/man/rucio-admin.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1744 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/man/rucio.rst
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/source/rest/
--rw-r--r--   0 barisits (51071) zp        (1307)      350 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/rest/attach_dids_to_dids.rst
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/doc/source/usecases/
--rw-r--r--   0 barisits (51071) zp        (1307)      783 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/add_account_identity.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      708 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/add_metadata_dataset.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      691 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/add_metadata_file.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      655 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/add_scope_to_account.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1470 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/add_subscription.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1677 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/authentication.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      804 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/consistency_file_between_storage_and_rucio.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      902 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/delete_file_replica_from_storage.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      795 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/detect_site_reach_watermark.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      940 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      886 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/download_all_files_from_a_given_list_of_files_from_rucio.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      900 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/download_all_files_in_a_dataset_from_rucio.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      794 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/download_files_from_rucio.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      564 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/obsolete_dataset.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      652 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/register_account.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      916 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/register_file_already_on_storage_system.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      646 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/register_transfer_request_file_fts.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      563 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/remove_replication_rules_from_file.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1270 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/reupload_after_failure.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1102 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/search.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      409 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/select_unwanted_files_for_deletion.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      590 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/set_replication_rule_to_file.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      852 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/upload_file_with_replication_rule.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1106 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/usecase_upload_file_into_rucio.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      633 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases/where_are_the_replicas_for_a_file.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      325 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/Acronyms_and_Abbreviations.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)       39 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/Architecture.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2067 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/Comparison_matrix.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     7173 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/REST_Account.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1586 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/REST_Intro.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     2439 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/REST_authentication.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     7945 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/REST_did.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      611 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/REST_identity.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      637 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/REST_lock.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1444 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/REST_meta.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      349 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/REST_redirect.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     3702 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/REST_replica.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     7502 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/REST_rse.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     2509 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/REST_rule.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1034 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/REST_scope.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     2512 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/REST_subscription.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     6000 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/RSE_Expressions.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      662 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/Rucio_Project_Meeting.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      163 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/account.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      184 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/accountlimit.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)    19866 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/accounts.pdf
--rwxr-xr-x   0 barisits (51071) zp        (1307)    56522 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/accounts.png
--rw-r--r--   0 barisits (51071) zp        (1307)    16748 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/api_curl_examples.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     2265 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/atlas_integration_testbed.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/authentication_and_identity.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     4204 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/cli_admin_examples.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     4565 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/cli_examples.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1010 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/client_examples.rst
--rw-r--r--   0 barisits (51071) zp        (1307)    11591 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/client_tutorial.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     7556 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/conf.py
--rw-r--r--   0 barisits (51071) zp        (1307)      138 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/core_constants.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     7860 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/developing.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3281 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/development_guidelines.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      180 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/did.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      165 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/exception.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      162 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/source/identity.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3274 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/index.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     2167 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/installing_atlas_clients.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1601 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/installing_clients.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1693 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/installing_server.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      152 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/lock.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      162 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/meta-data.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1180 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/naming_convention_db.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      475 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Accounting_and_quota.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      157 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Architecture.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1905 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Data_Deletion.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      311 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Database_Schema.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      442 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Deployment.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1514 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Exception_Handling.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3882 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_File_Dataset_Container.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      894 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Meta-data_attributes.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      292 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Notifications.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      251 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Permission_model.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1911 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Replica_management.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1652 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Rucio_Storage_Element.rst
--rw-r--r--   0 barisits (51071) zp        (1307)    27901 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Rucio_Storage_Element_Manager.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1142 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Rucio_account.rst
--rw-r--r--   0 barisits (51071) zp        (1307)    23147 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Rules.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     2701 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Scheduled_Transfers.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4241 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Subscriptions.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      382 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_Traceability_and_logging.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      347 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/overview_flow.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      169 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/permission.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      155 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/replica.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1509 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/replication_rules_examples.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     7948 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/rest.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      453 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/rse.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      717 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/rucio_cli.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      814 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/rucio_clients.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      183 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/rule.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1414 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/rules_workflow.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      158 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/scope.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      189 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/service_avaibility.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      190 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/subscription.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2438 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/doc/source/usecases.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4590 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/Makefile
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4513 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/doc/make.bat
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/etc/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/etc/schemas/
--rw-r--r--   0 barisits (51071) zp        (1307)       97 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/etc/schemas/account.json
--rw-r--r--   0 barisits (51071) zp        (1307)       82 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/etc/schemas/account_type.json
--rw-r--r--   0 barisits (51071) zp        (1307)       82 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/etc/schemas/did_type.json
--rw-r--r--   0 barisits (51071) zp        (1307)      112 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/etc/schemas/mail.json
--rw-r--r--   0 barisits (51071) zp        (1307)      105 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/etc/schemas/rse.json
--rw-r--r--   0 barisits (51071) zp        (1307)      105 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/etc/schemas/scope.json
--rw-r--r--   0 barisits (51071) zp        (1307)      559 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/etc/schemas/sub_filter.json
--rwxr-xr-x   0 barisits (51071) zp        (1307)      543 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/etc/rse-accounts.cfg.template
--rw-r--r--   0 barisits (51071) zp        (1307)      570 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/etc/rucio.cfg.atlas.client.template
--rwxr-xr-x   0 barisits (51071) zp        (1307)     5165 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/etc/rucio.cfg.template
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/lib/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/lib/rucio/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/lib/rucio/client/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/lib/rucio/client/cli/
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/cli/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)      469 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/cli/download.py
--rw-r--r--   0 barisits (51071) zp        (1307)      581 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/cli/upload.py
--rw-r--r--   0 barisits (51071) zp        (1307)      325 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)    12651 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/accountclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2763 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/accountlimitclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)    21749 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/client/baseclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2381 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/client.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3523 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/configclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)    23023 2017-01-20 08:30:56.000000 rucio-clients-1.9.5/lib/rucio/client/didclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)    91449 2016-11-25 16:30:17.000000 rucio-clients-1.9.5/lib/rucio/client/dq2client.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1716 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/fileclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2594 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/lockclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4717 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/metaclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3915 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/objectstoreclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1356 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/pingclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9888 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/client/replicaclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)    19164 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/rseclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9768 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/client/ruleclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3292 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/scopeclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     7475 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/subscriptionclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4326 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/client/uploadclient.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/lib/rucio/common/
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/common/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1208 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/common/client.py
--rw-r--r--   0 barisits (51071) zp        (1307)     7763 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/common/closeness_sorter.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3883 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/common/config.py
--rw-r--r--   0 barisits (51071) zp        (1307)      938 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/common/constants.py
--rw-r--r--   0 barisits (51071) zp        (1307)      439 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/common/constraints.py
--rw-r--r--   0 barisits (51071) zp        (1307)    19606 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/common/exception.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3288 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/common/log.py
--rw-r--r--   0 barisits (51071) zp        (1307)    14068 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/common/objectstore.py
--rw-r--r--   0 barisits (51071) zp        (1307)     8188 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/common/policy.py
--rw-r--r--   0 barisits (51071) zp        (1307)     5461 2016-11-25 16:30:17.000000 rucio-clients-1.9.5/lib/rucio/common/replicas_selector.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1520 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/common/rse_attributes.py
--rw-r--r--   0 barisits (51071) zp        (1307)    14030 2017-01-20 08:30:56.000000 rucio-clients-1.9.5/lib/rucio/common/schema.py
--rw-r--r--   0 barisits (51071) zp        (1307)    14270 2016-11-25 16:30:17.000000 rucio-clients-1.9.5/lib/rucio/common/utils.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/lib/rucio/rse/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4165 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/cache.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3787 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/dummy.py
--rw-r--r--   0 barisits (51071) zp        (1307)    17585 2017-01-20 08:30:56.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/gfal.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1256 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/gfalv2.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4679 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/gsiftp.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2635 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/http_cache.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3741 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/mock.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6596 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/ngarc.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6199 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/posix.py
--rw-r--r--   0 barisits (51071) zp        (1307)    12783 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/protocol.py
--rw-r--r--   0 barisits (51071) zp        (1307)     5035 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/rfio.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9114 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/s3.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9915 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/s3boto.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6345 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/s3es.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6723 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/sftp.py
--rw-r--r--   0 barisits (51071) zp        (1307)    15403 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/signeds3.py
--rw-r--r--   0 barisits (51071) zp        (1307)    13829 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/srm.py
--rw-r--r--   0 barisits (51071) zp        (1307)    19999 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/webdav.py
--rw-r--r--   0 barisits (51071) zp        (1307)     8153 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/rse/protocols/xrootd.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1937 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/rse/__init__.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)    25214 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/rse/rsemanager.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/lib/rucio/tests/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/lib/rucio/tests/emulation/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/lib/rucio/tests/emulation/usecases/
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/emulation/usecases/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)      969 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/emulation/usecases/auth.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1476 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/emulation/usecases/dummy.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2208 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/emulation/usecases/dummy_template.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3716 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/emulation/usecases/jdoe.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)    65781 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/emulation/usecases/panda.py
--rw-r--r--   0 barisits (51071) zp        (1307)    56221 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/emulation/usecases/panda_new.py
--rw-r--r--   0 barisits (51071) zp        (1307)    21228 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/emulation/usecases/tzero.py
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/emulation/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9327 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/emulation/emulator.py
--rw-r--r--   0 barisits (51071) zp        (1307)    15903 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/emulation/ucemulator.py
--rw-r--r--   0 barisits (51071) zp        (1307)     8610 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/emulation/ucprocess.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3278 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/emulation/worker.py
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4684 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/common.py
--rw-r--r--   0 barisits (51071) zp        (1307)    22701 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/tests/rsemgr_api_test.py
--rw-r--r--   0 barisits (51071) zp        (1307)    14408 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_account.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4351 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_account_limits.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1245 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_alembic.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2723 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_auditor.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1719 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_auditor_hdfs.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2888 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_auditor_srmdumps.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2292 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_authentication.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3786 2017-01-20 09:22:58.000000 rucio-clients-1.9.5/lib/rucio/tests/test_bb8.py
--rw-r--r--   0 barisits (51071) zp        (1307)    27965 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/tests/test_bin_rucio.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3210 2016-11-25 16:30:17.000000 rucio-clients-1.9.5/lib/rucio/tests/test_clients.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3120 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_config.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1200 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/tests/test_conveyor.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4563 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_counter.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6716 2017-01-20 08:30:56.000000 rucio-clients-1.9.5/lib/rucio/tests/test_curl.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2091 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_dataset_replicas.py
--rw-r--r--   0 barisits (51071) zp        (1307)      707 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_db.py
--rw-r--r--   0 barisits (51071) zp        (1307)    37907 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/tests/test_did.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6392 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_dumper.py
--rw-r--r--   0 barisits (51071) zp        (1307)    16150 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_dumper_consistency.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9790 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_dumper_data_model.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3145 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_dumper_path_parsing.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3362 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_heartbeat.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1657 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_hermes.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2141 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_identity.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3274 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_judge_cleaner.py
--rw-r--r--   0 barisits (51071) zp        (1307)    11109 2017-01-20 08:30:56.000000 rucio-clients-1.9.5/lib/rucio/tests/test_judge_evaluator.py
--rw-r--r--   0 barisits (51071) zp        (1307)     8060 2017-01-24 09:05:38.000000 rucio-clients-1.9.5/lib/rucio/tests/test_judge_injector.py
--rw-r--r--   0 barisits (51071) zp        (1307)    16107 2016-11-28 15:43:52.000000 rucio-clients-1.9.5/lib/rucio/tests/test_judge_repairer.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2086 2016-11-25 16:30:17.000000 rucio-clients-1.9.5/lib/rucio/tests/test_message.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3149 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_meta.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2532 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_meta_did.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1510 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_monitor.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2756 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_naming_convention.py
--rw-r--r--   0 barisits (51071) zp        (1307)    12265 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_objectstore.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3185 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_permission.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1286 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_ping.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1358 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/tests/test_quarantined_replica.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1307 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/tests/test_reaper.py
--rw-r--r--   0 barisits (51071) zp        (1307)     5633 2017-01-20 08:30:56.000000 rucio-clients-1.9.5/lib/rucio/tests/test_redirect.py
--rw-r--r--   0 barisits (51071) zp        (1307)    27875 2017-01-20 08:30:56.000000 rucio-clients-1.9.5/lib/rucio/tests/test_replica.py
--rw-r--r--   0 barisits (51071) zp        (1307)    78040 2016-11-25 16:30:17.000000 rucio-clients-1.9.5/lib/rucio/tests/test_rse.py
--rw-r--r--   0 barisits (51071) zp        (1307)    10690 2017-01-20 08:30:56.000000 rucio-clients-1.9.5/lib/rucio/tests/test_rse_expression_parser.py
--rw-r--r--   0 barisits (51071) zp        (1307)    13237 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_gfal2.py
--rw-r--r--   0 barisits (51071) zp        (1307)     5173 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_mock.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9728 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_posix.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9813 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_s3.py
--rw-r--r--   0 barisits (51071) zp        (1307)    11909 2016-11-25 16:30:17.000000 rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_s3boto.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4845 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_s3es.py
--rw-r--r--   0 barisits (51071) zp        (1307)    10110 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_sftp.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9909 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_signeds3.py
--rw-r--r--   0 barisits (51071) zp        (1307)    12805 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_srm.py
--rw-r--r--   0 barisits (51071) zp        (1307)    11084 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_webdav.py
--rw-r--r--   0 barisits (51071) zp        (1307)    10967 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_xrootd.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6537 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_rucio_cache.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4792 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_rucio_server.py
--rw-r--r--   0 barisits (51071) zp        (1307)    51857 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/tests/test_rule.py
--rw-r--r--   0 barisits (51071) zp        (1307)    10288 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_scope.py
--rw-r--r--   0 barisits (51071) zp        (1307)    20485 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/tests/test_subscription.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2650 2016-11-28 16:40:28.000000 rucio-clients-1.9.5/lib/rucio/tests/test_temporary_did.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1345 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/tests/test_trace.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3258 2016-11-25 16:30:17.000000 rucio-clients-1.9.5/lib/rucio/tests/test_undertaker.py
--rw-r--r--   0 barisits (51071) zp        (1307)      337 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)      249 2017-01-24 09:13:56.000000 rucio-clients-1.9.5/lib/rucio/vcsversion.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1127 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/lib/rucio/version.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/tools/
--rw-r--r--   0 barisits (51071) zp        (1307)     1060 2017-01-20 08:30:56.000000 rucio-clients-1.9.5/tools/pip-requires-client
--rw-r--r--   0 barisits (51071) zp        (1307)      541 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/AUTHORS
--rw-r--r--   0 barisits (51071) zp        (1307)      273 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/ChangeLog
--rw-r--r--   0 barisits (51071) zp        (1307)      274 2016-11-25 15:17:13.000000 rucio-clients-1.9.5/LICENSE
--rw-r--r--   0 barisits (51071) zp        (1307)      737 2017-01-24 09:13:56.000000 rucio-clients-1.9.5/MANIFEST.in
--rw-r--r--   0 barisits (51071) zp        (1307)      298 2017-01-24 09:13:56.000000 rucio-clients-1.9.5/README.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     7396 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/pylintrc
--rw-r--r--   0 barisits (51071) zp        (1307)     1014 2016-11-25 15:17:14.000000 rucio-clients-1.9.5/setup.cfg
--rw-r--r--   0 barisits (51071) zp        (1307)     6401 2017-01-24 09:13:56.000000 rucio-clients-1.9.5/setup.py
--rw-r--r--   0 barisits (51071) zp        (1307)      759 2017-01-24 09:13:59.000000 rucio-clients-1.9.5/PKG-INFO
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/bin/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   121517 2017-01-31 11:31:28.000000 rucio-clients-1.9.6/bin/rucio
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    44207 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/bin/rucio-admin
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/atlasnote/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   164832 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/AN_atlaslogo.pdf
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    88058 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/AN_cernlogo.pdf
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2877 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/AtlasRucioNote.aux
+-rw-r--r--   0 barisits (51071) zp        (1307)   440060 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/AtlasRucioNote.pdf
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    23795 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/AtlasRucioNote.tex
+-rw-r--r--   0 barisits (51071) zp        (1307)    65762 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/accounts.graffle
+-rw-r--r--   0 barisits (51071) zp        (1307)    31807 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/accounts.pdf
+-rw-r--r--   0 barisits (51071) zp        (1307)    27065 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/accounts.png
+-rw-r--r--   0 barisits (51071) zp        (1307)   125132 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/aggregation_hierarchy.graffle
+-rw-r--r--   0 barisits (51071) zp        (1307)    44183 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/aggregation_hierarchy.pdf
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     6980 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/atlasnote.cls
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     6557 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/booktabs.sty
+-rw-r--r--   0 barisits (51071) zp        (1307)   132902 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/dataset_hierarchy.graffle
+-rw-r--r--   0 barisits (51071) zp        (1307)    44639 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/dataset_hierarchy.pdf
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    18775 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/fncychap.sty
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    14665 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/sphinx.sty
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2073 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/sphinxhowto.cls
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3421 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/atlasnote/sphinxmanual.cls
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/doctrees/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/doctrees/man/
+-rw-r--r--   0 barisits (51071) zp        (1307)    13923 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/man/rucio-admin.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    21710 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/man/rucio.doctree
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/doctrees/rest/
+-rw-r--r--   0 barisits (51071) zp        (1307)     6101 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/rest/attach_dids_to_dids.doctree
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/
+-rw-r--r--   0 barisits (51071) zp        (1307)     4822 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/add_account_identity.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4818 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/add_metadata_dataset.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4785 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/add_metadata_file.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5249 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/add_scope_to_account.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     8508 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/add_subscription.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    12024 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/authentication.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4960 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/consistency_file_between_storage_and_rucio.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5038 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/delete_file_replica_from_storage.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4927 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/detect_site_reach_watermark.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5230 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4988 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/download_all_files_from_a_given_list_of_files_from_rucio.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5030 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/download_all_files_in_a_dataset_from_rucio.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4835 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/download_files_from_rucio.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4400 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/obsolete_dataset.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5231 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/register_account.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5081 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/register_file_already_on_storage_system.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4524 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/register_transfer_request_file_fts.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4380 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/remove_replication_rules_from_file.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5772 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/reupload_after_failure.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     7617 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/search.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     3221 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/select_unwanted_files_for_deletion.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4412 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/set_replication_rule_to_file.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5464 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/upload_file_with_replication_rule.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     7457 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/usecase_upload_file_into_rucio.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5107 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases/where_are_the_replicas_for_a_file.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     7150 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/Acronyms_and_Abbreviations.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     2393 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/doctrees/Architecture.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    21792 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/Comparison_matrix.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    81561 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/REST_Account.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     8685 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/REST_Intro.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    28088 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/REST_authentication.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    90687 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/REST_did.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     8194 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/REST_identity.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     9921 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/REST_lock.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    19528 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/REST_meta.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     7204 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/REST_redirect.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    43167 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/REST_replica.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    93418 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/REST_rse.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    33047 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/REST_rule.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    14549 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/REST_scope.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    31270 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/REST_subscription.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     8088 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/doctrees/Rucio_Project_Meeting.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    78224 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/account.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    21746 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/accountlimit.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)   196168 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/api_curl_examples.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    27111 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/atlas_integration_testbed.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     2054 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/authentication_and_identity.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    27974 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/cli_admin_examples.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    21844 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/doctrees/cli_examples.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     8060 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/client_examples.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)   116795 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/client_howto.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    39959 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/doctrees/client_tutorial.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)   155605 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/core_constants.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    21418 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/developing.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    18604 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/development_guidelines.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)   153643 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/doctrees/did.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)   452979 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/environment.pickle
+-rw-r--r--   0 barisits (51071) zp        (1307)   224246 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/exception.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    37099 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/identity.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    18065 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/index.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    15084 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/installing_atlas_clients.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    11551 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/installing_clients.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    12786 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/installing_server.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    19939 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/lock.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    39479 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/meta-data.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     7248 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/naming_convention_db.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     3506 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Accounting_and_quota.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     2773 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Architecture.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     9766 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Data_Deletion.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     3278 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Database_Schema.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     3459 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Deployment.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     6135 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Exception_Handling.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    17155 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_File_Dataset_Container.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     6672 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Meta-data_attributes.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     3043 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Notifications.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     2956 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Permission_model.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     9183 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Replica_management.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     6869 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Rucio_Storage_Element.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)   117157 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Rucio_Storage_Element_Manager.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5437 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Rucio_account.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    95260 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Rules.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     9339 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Scheduled_Transfers.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    35789 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Subscriptions.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     3214 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_Traceability_and_logging.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     3326 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/overview_flow.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     9984 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/permission.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     3498 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/replica.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    23662 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/replication_rules_examples.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    94015 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/rest.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)   183082 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/rse.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     7070 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/rucio_cli.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5185 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/rucio_clients.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    41739 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/rule.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4903 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/rules_workflow.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    25243 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/doctrees/scope.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    40983 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/setup.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    48626 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/subscription.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    28243 2016-11-25 15:03:17.000000 rucio-clients-1.9.6/doc/build/doctrees/usecases.doctree
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/_images/
+-rw-r--r--   0 barisits (51071) zp        (1307)    71679 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_images/RSE_overview.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    45789 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_images/RSE_sequence_instantiation.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    32727 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_images/RSE_sequence_usage.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    56522 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_images/accounts.png
+-rw-r--r--   0 barisits (51071) zp        (1307)   136638 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_images/architecture.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    82950 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_images/deployment.png
+-rw-r--r--   0 barisits (51071) zp        (1307)   163115 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_images/exception_handling.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    45282 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_images/rucio-get.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    73288 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_images/rucio-put.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    55513 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_images/rucio-register.png
+-rw-r--r--   0 barisits (51071) zp        (1307)   230376 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_images/rucio_schema.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    26628 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_images/scheduled_transfers.png
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/_modules/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/api/
+-rw-r--r--   0 barisits (51071) zp        (1307)    16466 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/api/identity.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     6844 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/api/permission.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/
+-rw-r--r--   0 barisits (51071) zp        (1307)    59303 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/accountclient.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    14938 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/accountlimitclient.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    93774 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/didclient.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    14712 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/lockclient.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    23765 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/metaclient.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    77886 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/rseclient.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    29268 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/ruleclient.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    17486 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/scopeclient.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    29268 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/subscriptionclient.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/common/
+-rw-r--r--   0 barisits (51071) zp        (1307)   100322 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/common/exception.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/db/
+-rw-r--r--   0 barisits (51071) zp        (1307)    25179 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/db/constants.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    20480 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/db/enum.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/rse/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/rse/protocols/
+-rw-r--r--   0 barisits (51071) zp        (1307)    51488 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/rse/protocols/protocol.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/web/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/web/rest/
+-rw-r--r--   0 barisits (51071) zp        (1307)    11578 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/rucio/web/rest/ping.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5307 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_modules/index.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/_sources/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/_sources/man/
+-rw-r--r--   0 barisits (51071) zp        (1307)      770 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/man/rucio-admin.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1744 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/man/rucio.txt
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/_sources/rest/
+-rw-r--r--   0 barisits (51071) zp        (1307)      350 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/rest/attach_dids_to_dids.txt
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/
+-rw-r--r--   0 barisits (51071) zp        (1307)      783 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/add_account_identity.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      708 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/add_metadata_dataset.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      691 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/add_metadata_file.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      655 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/add_scope_to_account.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1470 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/add_subscription.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1677 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/authentication.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      804 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/consistency_file_between_storage_and_rucio.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      902 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/delete_file_replica_from_storage.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      795 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/detect_site_reach_watermark.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      940 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      886 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/download_all_files_from_a_given_list_of_files_from_rucio.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      900 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/download_all_files_in_a_dataset_from_rucio.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      794 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/download_files_from_rucio.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      564 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/obsolete_dataset.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      652 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/register_account.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      916 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/register_file_already_on_storage_system.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      646 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/register_transfer_request_file_fts.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      563 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/remove_replication_rules_from_file.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1270 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/reupload_after_failure.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1102 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/search.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      409 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/select_unwanted_files_for_deletion.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      590 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/set_replication_rule_to_file.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      852 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/upload_file_with_replication_rule.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1106 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/usecase_upload_file_into_rucio.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      633 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases/where_are_the_replicas_for_a_file.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      325 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/Acronyms_and_Abbreviations.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)       39 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/Architecture.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2067 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/Comparison_matrix.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     7173 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/REST_Account.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1586 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/REST_Intro.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2439 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/REST_authentication.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     7945 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/REST_did.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      611 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/REST_identity.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      637 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/REST_lock.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1444 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/REST_meta.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      349 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/REST_redirect.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     3702 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/REST_replica.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     7502 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/REST_rse.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2509 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/REST_rule.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1034 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/REST_scope.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2512 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/REST_subscription.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      662 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/Rucio_Project_Meeting.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      163 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/account.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      184 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/accountlimit.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)    16748 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/api_curl_examples.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2265 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/atlas_integration_testbed.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/authentication_and_identity.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     4204 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/cli_admin_examples.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     4565 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/cli_examples.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1010 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/client_examples.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)    24065 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/client_howto.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)    11591 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/client_tutorial.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      138 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/core_constants.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     4981 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/developing.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     3281 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/development_guidelines.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      180 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/did.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      165 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/exception.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      162 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/identity.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2917 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/index.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2167 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/installing_atlas_clients.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1601 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/installing_clients.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1693 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/installing_server.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      152 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/lock.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      162 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/meta-data.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1180 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/naming_convention_db.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      475 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Accounting_and_quota.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      157 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Architecture.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1905 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Data_Deletion.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      311 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Database_Schema.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      442 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Deployment.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1514 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Exception_Handling.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     3882 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_File_Dataset_Container.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      894 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Meta-data_attributes.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      292 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Notifications.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      251 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Permission_model.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1911 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Replica_management.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1652 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Rucio_Storage_Element.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)    27901 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Rucio_Storage_Element_Manager.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1142 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Rucio_account.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)    23147 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Rules.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2701 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Scheduled_Transfers.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     4241 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Subscriptions.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      382 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_Traceability_and_logging.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      347 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/overview_flow.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      169 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/permission.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      155 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/replica.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     3376 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/replication_rules_examples.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     7948 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/rest.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      453 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/rse.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      717 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/rucio_cli.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      814 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/rucio_clients.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      183 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/rule.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1414 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/rules_workflow.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      158 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/scope.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     6529 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/setup.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      190 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/subscription.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2438 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_sources/usecases.txt
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/_static/
+-rw-r--r--   0 barisits (51071) zp        (1307)      673 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/ajax-loader.gif
+-rw-r--r--   0 barisits (51071) zp        (1307)     8270 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/basic.css
+-rw-r--r--   0 barisits (51071) zp        (1307)     4125 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/classic.css
+-rw-r--r--   0 barisits (51071) zp        (1307)     3500 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/comment-bright.png
+-rw-r--r--   0 barisits (51071) zp        (1307)     3578 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/comment-close.png
+-rw-r--r--   0 barisits (51071) zp        (1307)     3445 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/comment.png
+-rw-r--r--   0 barisits (51071) zp        (1307)     4041 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/default.css
+-rw-r--r--   0 barisits (51071) zp        (1307)     7377 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/doctools.js
+-rw-r--r--   0 barisits (51071) zp        (1307)      347 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/down-pressed.png
+-rw-r--r--   0 barisits (51071) zp        (1307)      347 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/down.png
+-rw-r--r--   0 barisits (51071) zp        (1307)      358 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/file.png
+-rw-r--r--   0 barisits (51071) zp        (1307)   282766 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/jquery-1.11.1.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    95786 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/jquery.js
+-rw-r--r--   0 barisits (51071) zp        (1307)      173 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/minus.png
+-rw-r--r--   0 barisits (51071) zp        (1307)      173 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/plus.png
+-rw-r--r--   0 barisits (51071) zp        (1307)     3991 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/pygments.css
+-rw-r--r--   0 barisits (51071) zp        (1307)    19563 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/rucio_logo.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    17880 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/searchtools.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     4803 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/sidebar.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    35168 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    12140 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/underscore.js
+-rw-r--r--   0 barisits (51071) zp        (1307)      345 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/up-pressed.png
+-rw-r--r--   0 barisits (51071) zp        (1307)      345 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/up.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    25350 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/_static/websupport.js
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/man/
+-rw-r--r--   0 barisits (51071) zp        (1307)     7794 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/man/rucio-admin.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     9052 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/man/rucio.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/rest/
+-rw-r--r--   0 barisits (51071) zp        (1307)     5795 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/rest/attach_dids_to_dids.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/build/html/usecases/
+-rw-r--r--   0 barisits (51071) zp        (1307)     4477 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/add_account_identity.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4558 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/add_metadata_dataset.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4543 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/add_metadata_file.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4538 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/add_scope_to_account.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4872 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/add_subscription.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5938 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/authentication.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4716 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/consistency_file_between_storage_and_rucio.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4557 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/delete_file_replica_from_storage.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4701 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/detect_site_reach_watermark.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4745 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4665 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/download_all_files_from_a_given_list_of_files_from_rucio.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4595 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/download_all_files_in_a_dataset_from_rucio.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4510 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/download_files_from_rucio.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4433 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/obsolete_dataset.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4551 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/register_account.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4548 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/register_file_already_on_storage_system.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4567 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/register_transfer_request_file_fts.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4523 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/remove_replication_rules_from_file.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4531 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/reupload_after_failure.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4876 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/search.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4523 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/select_unwanted_files_for_deletion.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4549 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/set_replication_rule_to_file.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4671 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/upload_file_with_replication_rule.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5164 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/usecase_upload_file_into_rucio.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4518 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/usecases/where_are_the_replicas_for_a_file.html
+-rw-r--r--   0 barisits (51071) zp        (1307)      230 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/.buildinfo
+-rw-r--r--   0 barisits (51071) zp        (1307)     5302 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/Acronyms_and_Abbreviations.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4352 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/Architecture.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     6632 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/Comparison_matrix.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    33965 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/REST_Account.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     8155 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/REST_Intro.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    13611 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/REST_authentication.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    36870 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/REST_did.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     7178 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/REST_identity.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     8464 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/REST_lock.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    11196 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/REST_meta.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     6873 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/REST_redirect.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    19743 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/REST_replica.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    36294 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/REST_rse.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    15403 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/REST_rule.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     9564 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/REST_scope.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    15806 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/REST_subscription.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5982 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/Rucio_Project_Meeting.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    24371 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/account.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     9490 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/accountlimit.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    49271 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/api_curl_examples.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     8847 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/atlas_integration_testbed.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4218 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/authentication_and_identity.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    20697 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/cli_admin_examples.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    16629 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/cli_examples.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     7763 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/client_examples.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    51571 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/client_howto.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    22174 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/client_tutorial.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    38831 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/core_constants.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    13195 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/developing.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    11262 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/development_guidelines.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    42116 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/did.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    64292 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/exception.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    54351 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/genindex.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    22008 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/http-routingtable.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    13231 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/identity.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    15245 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/index.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    10693 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/installing_atlas_clients.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     9658 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/installing_clients.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     8756 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/installing_server.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     9333 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/lock.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    13990 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/meta-data.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     8368 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/naming_convention_db.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4611 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/objects.inv
+-rw-r--r--   0 barisits (51071) zp        (1307)     5892 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_Accounting_and_quota.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5729 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_Architecture.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     7965 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_Data_Deletion.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5828 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_Database_Schema.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5590 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_Deployment.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     7307 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_Exception_Handling.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    11254 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_File_Dataset_Container.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     6831 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_Meta-data_attributes.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5732 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_Notifications.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5700 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_Permission_model.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     8062 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_Replica_management.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     7173 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_Rucio_Storage_Element.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    46544 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_Rucio_Storage_Element_Manager.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     6701 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_Rucio_account.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    36223 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/overview_Rules.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     8997 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_Scheduled_Transfers.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    14110 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_Subscriptions.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4733 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_Traceability_and_logging.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5951 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/overview_flow.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5808 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/permission.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     7644 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/py-modindex.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5259 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/replica.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    11051 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/replication_rules_examples.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    22089 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/rest.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    47247 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/rse.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     6001 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/rucio_cli.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5824 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/rucio_clients.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    13860 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/rule.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     6962 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/rules_workflow.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    10313 2016-11-25 15:03:15.000000 rucio-clients-1.9.6/doc/build/html/scope.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4453 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/search.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    57160 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/searchindex.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    17589 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/setup.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    14675 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/subscription.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    10373 2016-11-25 15:03:16.000000 rucio-clients-1.9.6/doc/build/html/usecases.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/design/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/design/RSE/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1996 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/design/RSE/meeting-2012-02-23.org
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/design/erd/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    55942 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/design/erd/ERD.graffle
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    72676 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/design/erd/ERD.pdf
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    60363 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/design/rucio_schema.pdf
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/source/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/source/_static/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     8270 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/_static/basic.css
+-rw-r--r--   0 barisits (51071) zp        (1307)     4179 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/_static/classic.css
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4041 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/_static/default.css
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    19563 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/_static/rucio_logo.png
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/source/_templates/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      777 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/_templates/layout.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/source/cli_examples/
+-rw-r--r--   0 barisits (51071) zp        (1307)       14 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/cli_examples/ping.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)       12 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/cli_examples/ping.sh
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/source/curl_examples/
+-rw-r--r--   0 barisits (51071) zp        (1307)      235 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/del_account.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      312 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/del_account.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/del_location.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      313 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/del_location.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      404 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_account.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      309 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_account.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      673 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_account_whoami.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      314 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_account_whoami.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      253 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_accounts.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      305 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_accounts.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)       29 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_api.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)       34 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_api.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_auth_gss.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      129 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_auth_gss.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_auth_userpass.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      168 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_auth_userpass.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      304 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_auth_validate.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      334 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_auth_validate.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_auth_x509.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      139 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_auth_x509.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_location.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      310 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_location.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      239 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_locations.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      306 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_locations.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      356 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_scopes.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      309 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/get_scopes.sh
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      380 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/post_account.sh
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      332 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/post_location.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      370 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/post_location_rse.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      257 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/put_account.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      331 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/put_account.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/put_location.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      309 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/put_location.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      257 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/put_scope.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      314 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/curl_examples/put_scope.sh
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/source/example_outputs/
+-rw-r--r--   0 barisits (51071) zp        (1307)     3643 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/example_outputs/failure-rucio.tests.test_curl.TestCurlRucio.test_get_accounts_whoami.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      164 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/example_outputs/success-rucio.tests.test_bin_rucio.TestBinRucio.test_add_account.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)       43 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/example_outputs/success-rucio.tests.test_bin_rucio.TestBinRucio.test_rucio_ping.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/example_outputs/success-rucio.tests.test_bin_rucio.TestBinRucio.test_rucio_version.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)       46 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/example_outputs/success-rucio.tests.test_clients.TestRucioClients.test_ping.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      804 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_accounts_whoami.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      429 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_GSS.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_proxy.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      466 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_userpass.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      454 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_validate.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      442 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_x509.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      454 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_x509_proxy.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)       84 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_ping.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      440 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_post_account.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      398 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_post_rse.txt
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/source/images/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/source/images/deployment.graffle/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/source/images/deployment.graffle/QuickLook/
+-rw-r--r--   0 barisits (51071) zp        (1307)    52757 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/deployment.graffle/QuickLook/Preview.pdf
+-rw-r--r--   0 barisits (51071) zp        (1307)   124440 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/deployment.graffle/QuickLook/Thumbnail.tiff
+-rw-r--r--   0 barisits (51071) zp        (1307)     3172 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/deployment.graffle/data.plist
+-rw-r--r--   0 barisits (51071) zp        (1307)    26954 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/deployment.graffle/image2.tiff
+-rw-r--r--   0 barisits (51071) zp        (1307)    10020 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/deployment.graffle/image3.tiff
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    71679 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/RSE_overview.png
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    45789 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/RSE_sequence_instantiation.png
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    32727 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/RSE_sequence_usage.png
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    56522 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/accounts.png
+-rw-r--r--   0 barisits (51071) zp        (1307)   397841 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/architecture.graffle
+-rw-r--r--   0 barisits (51071) zp        (1307)   136638 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/architecture.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    82950 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/deployment.png
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    70361 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/exception_handling.graffle
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   163115 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/exception_handling.png
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   127009 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/highLevelRoadmap.graffle
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   205501 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/rucio-get.graffle
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    45282 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/rucio-get.png
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   298526 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/rucio-put.graffle
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    73288 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/rucio-put.png
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   232239 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/rucio-register.graffle
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    55513 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/rucio-register.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    62543 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/rucio_schema.gml
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   226250 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/images/rucio_schema.pdf
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   230376 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/images/rucio_schema.png
+-rw-r--r--   0 barisits (51071) zp        (1307)     2485 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/images/scheduled_transfers.dia
+-rw-r--r--   0 barisits (51071) zp        (1307)    26628 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/images/scheduled_transfers.png
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/source/man/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      770 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/man/rucio-admin.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1744 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/man/rucio.rst
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/source/rest/
+-rw-r--r--   0 barisits (51071) zp        (1307)      350 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/rest/attach_dids_to_dids.rst
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/doc/source/usecases/
+-rw-r--r--   0 barisits (51071) zp        (1307)      783 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/add_account_identity.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      708 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/add_metadata_dataset.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      691 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/add_metadata_file.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      655 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/add_scope_to_account.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1470 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/add_subscription.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1677 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/authentication.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      804 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/consistency_file_between_storage_and_rucio.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      902 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/delete_file_replica_from_storage.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      795 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/detect_site_reach_watermark.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      940 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      886 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/download_all_files_from_a_given_list_of_files_from_rucio.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      900 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/download_all_files_in_a_dataset_from_rucio.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      794 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/download_files_from_rucio.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      564 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/obsolete_dataset.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      652 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/register_account.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      916 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/register_file_already_on_storage_system.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      646 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/register_transfer_request_file_fts.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      563 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/remove_replication_rules_from_file.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1270 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/reupload_after_failure.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1102 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/search.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      409 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/select_unwanted_files_for_deletion.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      590 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/set_replication_rule_to_file.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      852 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/upload_file_with_replication_rule.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1106 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/usecase_upload_file_into_rucio.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      633 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases/where_are_the_replicas_for_a_file.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      325 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/Acronyms_and_Abbreviations.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)       39 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/Architecture.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2067 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/Comparison_matrix.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     7173 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/REST_Account.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1586 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/REST_Intro.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     2439 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/REST_authentication.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     7945 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/REST_did.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      611 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/REST_identity.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      637 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/REST_lock.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1444 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/REST_meta.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      349 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/REST_redirect.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     3702 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/REST_replica.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     7502 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/REST_rse.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     2509 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/REST_rule.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1034 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/REST_scope.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     2512 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/REST_subscription.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     6000 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/RSE_Expressions.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      662 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/Rucio_Project_Meeting.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      163 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/account.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      184 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/accountlimit.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    19866 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/accounts.pdf
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    56522 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/accounts.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    16748 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/api_curl_examples.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     2265 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/atlas_integration_testbed.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/authentication_and_identity.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     4204 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/cli_admin_examples.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     4565 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/cli_examples.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1010 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/client_examples.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)    11591 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/client_tutorial.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     7556 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/conf.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      138 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/core_constants.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     7860 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/developing.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3281 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/development_guidelines.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      180 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/did.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      165 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/exception.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      162 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/source/identity.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3274 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/index.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     2167 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/installing_atlas_clients.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1601 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/installing_clients.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1693 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/installing_server.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      152 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/lock.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      162 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/meta-data.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1180 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/naming_convention_db.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      475 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Accounting_and_quota.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      157 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Architecture.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1905 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Data_Deletion.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      311 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Database_Schema.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      442 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Deployment.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1514 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Exception_Handling.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3882 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_File_Dataset_Container.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      894 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Meta-data_attributes.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      292 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Notifications.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      251 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Permission_model.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1911 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Replica_management.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1652 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Rucio_Storage_Element.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)    27901 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Rucio_Storage_Element_Manager.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1142 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Rucio_account.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)    23147 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Rules.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     2701 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Scheduled_Transfers.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4241 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Subscriptions.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      382 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_Traceability_and_logging.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      347 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/overview_flow.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      169 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/permission.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      155 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/replica.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1509 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/replication_rules_examples.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     7948 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/rest.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      453 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/rse.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      717 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/rucio_cli.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      814 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/rucio_clients.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      183 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/rule.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1414 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/rules_workflow.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      158 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/scope.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      189 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/service_avaibility.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      190 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/subscription.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2438 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/doc/source/usecases.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4590 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/Makefile
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4513 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/doc/make.bat
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/etc/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/etc/schemas/
+-rw-r--r--   0 barisits (51071) zp        (1307)       97 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/etc/schemas/account.json
+-rw-r--r--   0 barisits (51071) zp        (1307)       82 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/etc/schemas/account_type.json
+-rw-r--r--   0 barisits (51071) zp        (1307)       82 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/etc/schemas/did_type.json
+-rw-r--r--   0 barisits (51071) zp        (1307)      112 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/etc/schemas/mail.json
+-rw-r--r--   0 barisits (51071) zp        (1307)      105 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/etc/schemas/rse.json
+-rw-r--r--   0 barisits (51071) zp        (1307)      105 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/etc/schemas/scope.json
+-rw-r--r--   0 barisits (51071) zp        (1307)      559 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/etc/schemas/sub_filter.json
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      543 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/etc/rse-accounts.cfg.template
+-rw-r--r--   0 barisits (51071) zp        (1307)      570 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/etc/rucio.cfg.atlas.client.template
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     5165 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/etc/rucio.cfg.template
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/lib/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/lib/rucio/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/lib/rucio/client/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/lib/rucio/client/cli/
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/cli/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      469 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/cli/download.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      581 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/cli/upload.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      325 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    12651 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/accountclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2763 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/accountlimitclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    21749 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/client/baseclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2381 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/client.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3523 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/configclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    23023 2017-01-20 08:30:56.000000 rucio-clients-1.9.6/lib/rucio/client/didclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    91449 2016-11-25 16:30:17.000000 rucio-clients-1.9.6/lib/rucio/client/dq2client.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1716 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/fileclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2594 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/lockclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4717 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/metaclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3915 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/objectstoreclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1356 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/pingclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9888 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/client/replicaclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    19164 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/rseclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9768 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/client/ruleclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3292 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/scopeclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     7475 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/subscriptionclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4326 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/client/uploadclient.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/lib/rucio/common/
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/common/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1208 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/common/client.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     7763 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/common/closeness_sorter.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3883 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/common/config.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      938 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/common/constants.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      439 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/common/constraints.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    19606 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/common/exception.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3288 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/common/log.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    14068 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/common/objectstore.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     8188 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/common/policy.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     5461 2016-11-25 16:30:17.000000 rucio-clients-1.9.6/lib/rucio/common/replicas_selector.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1520 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/common/rse_attributes.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    14030 2017-01-20 08:30:56.000000 rucio-clients-1.9.6/lib/rucio/common/schema.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    14270 2016-11-25 16:30:17.000000 rucio-clients-1.9.6/lib/rucio/common/utils.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/lib/rucio/rse/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4165 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/cache.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3787 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/dummy.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    17585 2017-01-20 08:30:56.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/gfal.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1256 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/gfalv2.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4680 2017-01-31 11:31:28.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/gsiftp.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2635 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/http_cache.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3741 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/mock.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6596 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/ngarc.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6199 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/posix.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    12783 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/protocol.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     5035 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/rfio.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9114 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/s3.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9915 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/s3boto.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6345 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/s3es.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6723 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/sftp.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    15403 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/signeds3.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    13829 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/srm.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    19999 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/webdav.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     8153 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/rse/protocols/xrootd.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1937 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/rse/__init__.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    25451 2017-01-31 11:31:28.000000 rucio-clients-1.9.6/lib/rucio/rse/rsemanager.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/lib/rucio/tests/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/lib/rucio/tests/emulation/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/lib/rucio/tests/emulation/usecases/
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/emulation/usecases/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      969 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/emulation/usecases/auth.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1476 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/emulation/usecases/dummy.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2208 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/emulation/usecases/dummy_template.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3716 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/emulation/usecases/jdoe.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    65781 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/emulation/usecases/panda.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    56221 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/emulation/usecases/panda_new.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    21228 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/emulation/usecases/tzero.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/emulation/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9327 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/emulation/emulator.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    15903 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/emulation/ucemulator.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     8610 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/emulation/ucprocess.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3278 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/emulation/worker.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4684 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/common.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    22701 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/tests/rsemgr_api_test.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    14408 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_account.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4351 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_account_limits.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1245 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_alembic.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2723 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_auditor.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1719 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_auditor_hdfs.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2888 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_auditor_srmdumps.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2292 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_authentication.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3786 2017-01-20 09:22:58.000000 rucio-clients-1.9.6/lib/rucio/tests/test_bb8.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    27965 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/tests/test_bin_rucio.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3210 2016-11-25 16:30:17.000000 rucio-clients-1.9.6/lib/rucio/tests/test_clients.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3120 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_config.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1200 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/tests/test_conveyor.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4563 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_counter.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6716 2017-01-20 08:30:56.000000 rucio-clients-1.9.6/lib/rucio/tests/test_curl.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2091 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_dataset_replicas.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      707 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_db.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    37907 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/tests/test_did.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6392 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_dumper.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    16150 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_dumper_consistency.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9790 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_dumper_data_model.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3145 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_dumper_path_parsing.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3362 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_heartbeat.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1657 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_hermes.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2141 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_identity.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3274 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_judge_cleaner.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    11109 2017-01-20 08:30:56.000000 rucio-clients-1.9.6/lib/rucio/tests/test_judge_evaluator.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     8060 2017-01-30 16:14:23.000000 rucio-clients-1.9.6/lib/rucio/tests/test_judge_injector.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    16107 2017-02-01 12:54:56.000000 rucio-clients-1.9.6/lib/rucio/tests/test_judge_repairer.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2086 2016-11-25 16:30:17.000000 rucio-clients-1.9.6/lib/rucio/tests/test_message.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3149 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_meta.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2532 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_meta_did.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1510 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_monitor.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2756 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_naming_convention.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    12265 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_objectstore.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3185 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_permission.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1286 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_ping.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1358 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/tests/test_quarantined_replica.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1307 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/tests/test_reaper.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     5633 2017-01-20 08:30:56.000000 rucio-clients-1.9.6/lib/rucio/tests/test_redirect.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    27875 2017-01-20 08:30:56.000000 rucio-clients-1.9.6/lib/rucio/tests/test_replica.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    78040 2016-11-25 16:30:17.000000 rucio-clients-1.9.6/lib/rucio/tests/test_rse.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    10690 2017-01-20 08:30:56.000000 rucio-clients-1.9.6/lib/rucio/tests/test_rse_expression_parser.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    13237 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_gfal2.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     5173 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_mock.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9728 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_posix.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9813 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_s3.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    11909 2016-11-25 16:30:17.000000 rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_s3boto.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4845 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_s3es.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    10110 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_sftp.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9909 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_signeds3.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    12805 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_srm.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    11084 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_webdav.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    10967 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_xrootd.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6537 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_rucio_cache.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4792 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_rucio_server.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    51857 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/tests/test_rule.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    10288 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_scope.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    20485 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/tests/test_subscription.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2650 2016-11-28 16:40:28.000000 rucio-clients-1.9.6/lib/rucio/tests/test_temporary_did.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1345 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/tests/test_trace.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3258 2016-11-25 16:30:17.000000 rucio-clients-1.9.6/lib/rucio/tests/test_undertaker.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      337 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      249 2017-02-07 09:03:41.000000 rucio-clients-1.9.6/lib/rucio/vcsversion.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1127 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/lib/rucio/version.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/tools/
+-rw-r--r--   0 barisits (51071) zp        (1307)     1060 2017-01-20 08:30:56.000000 rucio-clients-1.9.6/tools/pip-requires-client
+-rw-r--r--   0 barisits (51071) zp        (1307)      541 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/AUTHORS
+-rw-r--r--   0 barisits (51071) zp        (1307)      273 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/ChangeLog
+-rw-r--r--   0 barisits (51071) zp        (1307)      274 2016-11-25 15:17:13.000000 rucio-clients-1.9.6/LICENSE
+-rw-r--r--   0 barisits (51071) zp        (1307)      737 2017-02-07 09:03:41.000000 rucio-clients-1.9.6/MANIFEST.in
+-rw-r--r--   0 barisits (51071) zp        (1307)      298 2017-02-07 09:03:41.000000 rucio-clients-1.9.6/README.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     7396 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/pylintrc
+-rw-r--r--   0 barisits (51071) zp        (1307)     1014 2016-11-25 15:17:14.000000 rucio-clients-1.9.6/setup.cfg
+-rw-r--r--   0 barisits (51071) zp        (1307)     6401 2017-02-07 09:03:41.000000 rucio-clients-1.9.6/setup.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      759 2017-02-07 09:03:44.000000 rucio-clients-1.9.6/PKG-INFO
```

### Comparing `rucio-clients-1.9.5/bin/rucio` & `rucio-clients-1.9.6/bin/rucio`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright European Organization for Nuclear Research (CERN)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Authors:
-# - Mario Lassnig, <mario.lassnig@cern.ch>, 2012-2014, 2016
+# - Mario Lassnig, <mario.lassnig@cern.ch>, 2012-2014, 2016-2017
 # - Vincent Garonne, <vincent.garonne@cern.ch>, 2012-2016
 # - Thomas Beermann, <thomas.beermann@cern.ch>, 2012
 # - Yun-Pin Sun, <yun-pin.sun@cern.ch>, 2013
 # - Cedric Serfon <cedric.serfon@cern.ch>, 2013-2016
 # - Martin Barisits <martin.barisits@cern.ch>, 2013-2016
 # - Joaquin Bogado <joaquin.bogado@cern.ch>, 2014, 2015
 # - Evangelia Liotiri <evangelia.liotiri@cern.ch>, 2015
@@ -1201,19 +1201,28 @@
                 if rse_dict[rse]['availability_read']:
                     trace.update({'remoteSite': rse_dict[rse]['rse'], 'protocol': rse_dict[rse]['protocols'][0]['scheme'], 'transferStart': time.time(), 'clientState': 'DOWNLOAD_ATTEMPT'})
                     success = False
                     retries = 5
                     for attempt in xrange(0, retries):
                         try:
                             logger.info('Thread %s/%s : File %s:%s trying from %s' % (threadnb, total_threads, file['scope'], file['name'], rse))
-                            rsemgr.download(rse_dict[rse],
-                                            files=[{'name': file['name'],
-                                                    'scope': file['scope'],
-                                                    'adler32': file['adler32']}, ],
-                                            dest_dir=dest_dir)
+                            if args.pfn:
+                                rsemgr.download(rse_dict[rse],
+                                                files=[{'name': file['name'],
+                                                        'scope': file['scope'],
+                                                        'adler32': file['adler32'],
+                                                        'pfn': args.pfn}, ],
+                                                dest_dir=dest_dir,
+                                                force_scheme=args.pfn.split(':')[0])
+                            else:
+                                rsemgr.download(rse_dict[rse],
+                                                files=[{'name': file['name'],
+                                                        'scope': file['scope'],
+                                                        'adler32': file['adler32']}, ],
+                                                dest_dir=dest_dir)
                             logger.info('Thread %s/%s : File %s:%s successfully downloaded from %s' % (threadnb,
                                                                                                        total_threads,
                                                                                                        file['scope'],
                                                                                                        file['name'],
                                                                                                        rse))
                             download_ok = 1
                             success = True
@@ -1354,15 +1363,16 @@
         try:
             summary['%s:%s' % (scope, name)] = {}
             logger.debug('Checking validity of DID')
             did_info = client.get_did(scope, name)
             did_type = did_info['type']
             dataset_scope = '' if did_type == 'FILE' else scope
             dataset_name = '' if did_type == 'FILE' else name
-            logger.debug('Getting the list of replicas')
+
+            logger.debug('Getting the list of replicas from Rucio servers')
             replicas = [f for f in client.list_replicas([{'scope': scope, 'name': name}],
                                                         rse_expression=args.rse)]
 
             if args.nrandom:
                 files_to_download = replicas
                 random.shuffle(files_to_download)
                 files_to_download = files_to_download[0:args.nrandom]
@@ -2037,15 +2047,14 @@
     List the datasets in a site.
 
     """
     client = get_client(args)
     if args.long:
         table = []
         for dsn in client.list_datasets_per_rse(args.rse):
-            print dsn
             table.append(['%s:%s' % (dsn['scope'], dsn['name']), '%s/%s' % (str(dsn['available_length']), str(dsn['length'])), '%s/%s' % (str(dsn['available_bytes']), str(dsn['bytes']))])
         table.sort()
         print tabulate.tabulate(table, tablefmt=tablefmt, headers=['DID', 'LOCAL FILES/TOTAL FILES', 'LOCAL BYTES/TOTAL BYTES'])
     else:
         dsns = list(set(['%s:%s' % (dsn['scope'], dsn['name']) for dsn in client.list_datasets_per_rse(args.rse)]))
         dsns.sort()
         print "SCOPE:NAME"
@@ -2075,15 +2084,14 @@
     for input in inputs:
         try:
             uuid.UUID(input)
             guids.append(input)
         except ValueError:
             pfns.append(input)
 
-    print pfns, guids
     dict_datasets = {}
     if pfns:
         for res in client.get_did_from_pfns(pfns):
             for key in res:
                 if key not in dict_datasets:
                     dict_datasets[key] = []
                 for rule in client.list_associated_rules_for_file(res[key]['scope'], res[key]['name']):
@@ -2292,32 +2300,34 @@
     upload_parser.add_argument('--protocol', action='store', help='Force the protocol to use')
     upload_parser.add_argument(dest='args', action='store', nargs='+', help='files and datasets.')
 
     # The download subparser
     get_parser = subparsers.add_parser('get', help='Download method (synonym for download)')
     get_parser.set_defaults(which='download')
     get_parser.add_argument('--dir', dest='dir', default='.', action='store', help='The directory to store the downloaded file.')
-    get_parser.add_argument(dest='dids', nargs='+', action='store', help='List of space separated data identifiers')
-    get_parser.add_argument('--rse', action='store', help='RSE Expression to specify allowed sources')
-    get_parser.add_argument('--protocol', action='store', help='Force the protocol to use')
-    get_parser.add_argument('--nrandom', type=int, action='store', help='Download N random files from the DID')
-    get_parser.add_argument('--ndownloader', type=int, default=3, action='store', help='Choose the number of parallel processes for download')
+    get_parser.add_argument(dest='dids', nargs='+', action='store', help='List of space separated data identifiers.')
+    get_parser.add_argument('--rse', action='store', help='RSE Expression to specify allowed sources.')
+    get_parser.add_argument('--protocol', action='store', help='Force the protocol to use.')
+    get_parser.add_argument('--nrandom', type=int, action='store', help='Download N random files from the DID.')
+    get_parser.add_argument('--ndownloader', type=int, default=3, action='store', help='Choose the number of parallel processes for download.')
     get_parser.add_argument('--no-subdir', action='store_true', default=False, help="Don't create a subdirectory for the scope of the files. Existing files in the directory will be overwritten.")
     get_parser.add_argument('--old', action='store_true', default=False, help="Choose the old download thread model.")
+    get_parser.add_argument('--pfn', dest='pfn', action='store', help="Specify the exact PFN for the download.")
 
     download_parser = subparsers.add_parser('download', help='Download method (synonym for get)')
     download_parser.set_defaults(which='download')
     download_parser.add_argument('--dir', dest='dir', default='.', action='store', help='The directory to store the downloaded file.')
     download_parser.add_argument(dest='dids', nargs='+', action='store', help='List of space separated data identifiers.')
     download_parser.add_argument('--rse', action='store', help='RSE Expression to specify allowed sources')
     download_parser.add_argument('--protocol', action='store', help='Force the protocol to use.')
     download_parser.add_argument('--nrandom', type=int, action='store', help='Download N random files from the DID.')
     download_parser.add_argument('--ndownloader', type=int, default=3, action='store', help='Choose the number of parallel processes for download.')
     download_parser.add_argument('--no-subdir', action='store_true', default=False, help="Don't create a subdirectory for the scope of the files. Existing files in the directory will be overwritten.")
     download_parser.add_argument('--old', action='store_true', default=False, help="Choose the old download thread model.")
+    download_parser.add_argument('--pfn', dest='pfn', action='store', help="Specify the exact PFN for the download.")
 
     # The get-metadata subparser
     get_metadata_parser = subparsers.add_parser('get-metadata', help='Get metadata for DIDs.')
     get_metadata_parser.set_defaults(which='get_metadata')
     get_metadata_parser.add_argument(dest='dids', nargs='+', action='store', help='List of space separated data identifiers.')
 
     # The set-metadata subparser
```

### Comparing `rucio-clients-1.9.5/bin/rucio-admin` & `rucio-clients-1.9.6/bin/rucio-admin`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/AN_atlaslogo.pdf` & `rucio-clients-1.9.6/doc/atlasnote/AN_atlaslogo.pdf`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/AN_cernlogo.pdf` & `rucio-clients-1.9.6/doc/atlasnote/AN_cernlogo.pdf`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/AtlasRucioNote.aux` & `rucio-clients-1.9.6/doc/atlasnote/AtlasRucioNote.aux`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/AtlasRucioNote.pdf` & `rucio-clients-1.9.6/doc/atlasnote/AtlasRucioNote.pdf`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/AtlasRucioNote.tex` & `rucio-clients-1.9.6/doc/atlasnote/AtlasRucioNote.tex`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/accounts.graffle` & `rucio-clients-1.9.6/doc/atlasnote/accounts.graffle`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/accounts.pdf` & `rucio-clients-1.9.6/doc/atlasnote/accounts.pdf`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/accounts.png` & `rucio-clients-1.9.6/doc/atlasnote/accounts.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/aggregation_hierarchy.graffle` & `rucio-clients-1.9.6/doc/atlasnote/aggregation_hierarchy.graffle`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/aggregation_hierarchy.pdf` & `rucio-clients-1.9.6/doc/atlasnote/aggregation_hierarchy.pdf`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/atlasnote.cls` & `rucio-clients-1.9.6/doc/atlasnote/atlasnote.cls`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/booktabs.sty` & `rucio-clients-1.9.6/doc/atlasnote/booktabs.sty`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/dataset_hierarchy.graffle` & `rucio-clients-1.9.6/doc/atlasnote/dataset_hierarchy.graffle`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/dataset_hierarchy.pdf` & `rucio-clients-1.9.6/doc/atlasnote/dataset_hierarchy.pdf`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/fncychap.sty` & `rucio-clients-1.9.6/doc/atlasnote/fncychap.sty`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/sphinx.sty` & `rucio-clients-1.9.6/doc/atlasnote/sphinx.sty`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/sphinxhowto.cls` & `rucio-clients-1.9.6/doc/atlasnote/sphinxhowto.cls`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/atlasnote/sphinxmanual.cls` & `rucio-clients-1.9.6/doc/atlasnote/sphinxmanual.cls`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/man/rucio-admin.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/man/rucio-admin.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/man/rucio.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/man/rucio.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/rest/attach_dids_to_dids.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/rest/attach_dids_to_dids.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/add_account_identity.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/add_account_identity.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/add_metadata_dataset.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/add_metadata_dataset.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/add_metadata_file.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/add_metadata_file.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/add_scope_to_account.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/add_scope_to_account.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/add_subscription.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/add_subscription.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/authentication.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/authentication.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/consistency_file_between_storage_and_rucio.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/consistency_file_between_storage_and_rucio.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/delete_file_replica_from_storage.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/delete_file_replica_from_storage.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/detect_site_reach_watermark.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/detect_site_reach_watermark.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/download_all_files_from_a_given_list_of_files_from_rucio.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/download_all_files_from_a_given_list_of_files_from_rucio.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/download_all_files_in_a_dataset_from_rucio.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/download_all_files_in_a_dataset_from_rucio.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/download_files_from_rucio.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/download_files_from_rucio.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/obsolete_dataset.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/obsolete_dataset.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/register_account.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/register_account.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/register_file_already_on_storage_system.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/register_file_already_on_storage_system.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/register_transfer_request_file_fts.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/register_transfer_request_file_fts.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/remove_replication_rules_from_file.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/remove_replication_rules_from_file.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/reupload_after_failure.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/reupload_after_failure.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/search.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/search.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/select_unwanted_files_for_deletion.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/select_unwanted_files_for_deletion.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/set_replication_rule_to_file.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/set_replication_rule_to_file.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/upload_file_with_replication_rule.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/upload_file_with_replication_rule.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/usecase_upload_file_into_rucio.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/usecase_upload_file_into_rucio.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases/where_are_the_replicas_for_a_file.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases/where_are_the_replicas_for_a_file.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/Acronyms_and_Abbreviations.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/Acronyms_and_Abbreviations.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/Architecture.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/Architecture.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/Comparison_matrix.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/Comparison_matrix.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/REST_Account.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/REST_Account.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/REST_Intro.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/REST_Intro.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/REST_authentication.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/REST_authentication.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/REST_did.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/REST_did.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/REST_identity.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/REST_identity.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/REST_lock.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/REST_lock.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/REST_meta.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/REST_meta.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/REST_redirect.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/REST_redirect.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/REST_replica.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/REST_replica.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/REST_rse.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/REST_rse.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/REST_rule.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/REST_rule.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/REST_scope.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/REST_scope.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/REST_subscription.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/REST_subscription.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/Rucio_Project_Meeting.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/Rucio_Project_Meeting.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/account.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/account.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/accountlimit.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/accountlimit.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/api_curl_examples.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/api_curl_examples.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/atlas_integration_testbed.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/atlas_integration_testbed.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/authentication_and_identity.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/authentication_and_identity.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/cli_admin_examples.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/cli_admin_examples.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/cli_examples.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/cli_examples.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/client_examples.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/client_examples.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/client_howto.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/client_howto.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/client_tutorial.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/client_tutorial.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/core_constants.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/core_constants.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/developing.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/developing.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/development_guidelines.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/development_guidelines.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/did.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/did.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/environment.pickle` & `rucio-clients-1.9.6/doc/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/exception.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/exception.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/identity.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/identity.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/index.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/installing_atlas_clients.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/installing_atlas_clients.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/installing_clients.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/installing_clients.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/installing_server.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/installing_server.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/lock.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/lock.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/meta-data.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/meta-data.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/naming_convention_db.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/naming_convention_db.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Accounting_and_quota.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Accounting_and_quota.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Architecture.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Architecture.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Data_Deletion.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Data_Deletion.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Database_Schema.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Database_Schema.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Deployment.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Deployment.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Exception_Handling.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Exception_Handling.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_File_Dataset_Container.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_File_Dataset_Container.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Meta-data_attributes.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Meta-data_attributes.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Notifications.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Notifications.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Permission_model.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Permission_model.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Replica_management.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Replica_management.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Rucio_Storage_Element.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Rucio_Storage_Element.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Rucio_Storage_Element_Manager.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Rucio_Storage_Element_Manager.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Rucio_account.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Rucio_account.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Rules.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Rules.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Scheduled_Transfers.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Scheduled_Transfers.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Subscriptions.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Subscriptions.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_Traceability_and_logging.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_Traceability_and_logging.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/overview_flow.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/overview_flow.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/permission.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/permission.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/replica.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/replica.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/replication_rules_examples.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/replication_rules_examples.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/rest.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/rest.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/rse.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/rse.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/rucio_cli.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/rucio_cli.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/rucio_clients.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/rucio_clients.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/rule.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/rule.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/rules_workflow.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/rules_workflow.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/scope.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/scope.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/setup.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/setup.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/subscription.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/subscription.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/doctrees/usecases.doctree` & `rucio-clients-1.9.6/doc/build/doctrees/usecases.doctree`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_images/RSE_overview.png` & `rucio-clients-1.9.6/doc/build/html/_images/RSE_overview.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_images/RSE_sequence_instantiation.png` & `rucio-clients-1.9.6/doc/build/html/_images/RSE_sequence_instantiation.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_images/RSE_sequence_usage.png` & `rucio-clients-1.9.6/doc/build/html/_images/RSE_sequence_usage.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_images/accounts.png` & `rucio-clients-1.9.6/doc/build/html/_images/accounts.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_images/architecture.png` & `rucio-clients-1.9.6/doc/build/html/_images/architecture.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_images/deployment.png` & `rucio-clients-1.9.6/doc/build/html/_images/deployment.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_images/exception_handling.png` & `rucio-clients-1.9.6/doc/build/html/_images/exception_handling.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_images/rucio-get.png` & `rucio-clients-1.9.6/doc/build/html/_images/rucio-get.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_images/rucio-put.png` & `rucio-clients-1.9.6/doc/build/html/_images/rucio-put.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_images/rucio-register.png` & `rucio-clients-1.9.6/doc/build/html/_images/rucio-register.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_images/rucio_schema.png` & `rucio-clients-1.9.6/doc/build/html/_images/rucio_schema.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_images/scheduled_transfers.png` & `rucio-clients-1.9.6/doc/build/html/_images/scheduled_transfers.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/rucio/api/identity.html` & `rucio-clients-1.9.6/doc/build/html/_modules/rucio/api/identity.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/rucio/api/permission.html` & `rucio-clients-1.9.6/doc/build/html/_modules/rucio/api/permission.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/accountclient.html` & `rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/accountclient.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/accountlimitclient.html` & `rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/accountlimitclient.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/didclient.html` & `rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/didclient.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/lockclient.html` & `rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/lockclient.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/metaclient.html` & `rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/metaclient.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/rseclient.html` & `rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/rseclient.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/ruleclient.html` & `rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/ruleclient.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/scopeclient.html` & `rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/scopeclient.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/rucio/client/subscriptionclient.html` & `rucio-clients-1.9.6/doc/build/html/_modules/rucio/client/subscriptionclient.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/rucio/common/exception.html` & `rucio-clients-1.9.6/doc/build/html/_modules/rucio/common/exception.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/rucio/db/constants.html` & `rucio-clients-1.9.6/doc/build/html/_modules/rucio/db/constants.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/rucio/db/enum.html` & `rucio-clients-1.9.6/doc/build/html/_modules/rucio/db/enum.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/rucio/rse/protocols/protocol.html` & `rucio-clients-1.9.6/doc/build/html/_modules/rucio/rse/protocols/protocol.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/rucio/web/rest/ping.html` & `rucio-clients-1.9.6/doc/build/html/_modules/rucio/web/rest/ping.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_modules/index.html` & `rucio-clients-1.9.6/doc/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/man/rucio-admin.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/man/rucio-admin.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/man/rucio.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/man/rucio.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/add_account_identity.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/add_account_identity.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/add_metadata_dataset.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/add_metadata_dataset.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/add_metadata_file.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/add_metadata_file.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/add_scope_to_account.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/add_scope_to_account.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/add_subscription.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/add_subscription.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/authentication.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/authentication.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/consistency_file_between_storage_and_rucio.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/consistency_file_between_storage_and_rucio.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/delete_file_replica_from_storage.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/delete_file_replica_from_storage.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/detect_site_reach_watermark.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/detect_site_reach_watermark.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/download_all_files_from_a_given_list_of_files_from_rucio.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/download_all_files_from_a_given_list_of_files_from_rucio.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/download_all_files_in_a_dataset_from_rucio.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/download_all_files_in_a_dataset_from_rucio.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/download_files_from_rucio.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/download_files_from_rucio.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/obsolete_dataset.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/obsolete_dataset.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/register_account.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/register_account.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/register_file_already_on_storage_system.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/register_file_already_on_storage_system.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/register_transfer_request_file_fts.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/register_transfer_request_file_fts.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/remove_replication_rules_from_file.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/remove_replication_rules_from_file.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/reupload_after_failure.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/reupload_after_failure.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/search.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/search.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/set_replication_rule_to_file.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/set_replication_rule_to_file.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/upload_file_with_replication_rule.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/upload_file_with_replication_rule.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/usecase_upload_file_into_rucio.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/usecase_upload_file_into_rucio.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases/where_are_the_replicas_for_a_file.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases/where_are_the_replicas_for_a_file.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/Comparison_matrix.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/Comparison_matrix.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/REST_Account.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/REST_Account.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/REST_Intro.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/REST_Intro.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/REST_authentication.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/REST_authentication.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/REST_did.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/REST_did.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/REST_identity.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/REST_identity.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/REST_lock.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/REST_lock.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/REST_meta.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/REST_meta.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/REST_replica.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/REST_replica.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/REST_rse.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/REST_rse.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/REST_rule.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/REST_rule.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/REST_scope.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/REST_scope.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/REST_subscription.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/REST_subscription.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/Rucio_Project_Meeting.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/Rucio_Project_Meeting.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/api_curl_examples.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/api_curl_examples.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/atlas_integration_testbed.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/atlas_integration_testbed.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/cli_admin_examples.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/cli_admin_examples.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/cli_examples.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/cli_examples.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/client_examples.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/client_examples.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/client_howto.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/client_howto.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/client_tutorial.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/client_tutorial.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/developing.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/developing.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/development_guidelines.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/development_guidelines.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/index.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/index.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/installing_atlas_clients.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/installing_atlas_clients.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/installing_clients.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/installing_clients.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/installing_server.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/installing_server.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/naming_convention_db.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/naming_convention_db.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/overview_Data_Deletion.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/overview_Data_Deletion.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/overview_Exception_Handling.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/overview_Exception_Handling.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/overview_File_Dataset_Container.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/overview_File_Dataset_Container.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/overview_Meta-data_attributes.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/overview_Meta-data_attributes.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/overview_Replica_management.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/overview_Replica_management.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/overview_Rucio_Storage_Element.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/overview_Rucio_Storage_Element.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/overview_Rucio_Storage_Element_Manager.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/overview_Rucio_Storage_Element_Manager.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/overview_Rucio_account.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/overview_Rucio_account.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/overview_Rules.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/overview_Rules.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/overview_Scheduled_Transfers.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/overview_Scheduled_Transfers.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/overview_Subscriptions.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/overview_Subscriptions.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/replication_rules_examples.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/replication_rules_examples.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/rest.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/rest.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/rucio_cli.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/rucio_cli.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/rucio_clients.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/rucio_clients.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/rules_workflow.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/rules_workflow.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/setup.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/setup.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_sources/usecases.txt` & `rucio-clients-1.9.6/doc/build/html/_sources/usecases.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/ajax-loader.gif` & `rucio-clients-1.9.6/doc/build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/basic.css` & `rucio-clients-1.9.6/doc/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/classic.css` & `rucio-clients-1.9.6/doc/build/html/_static/classic.css`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/comment-bright.png` & `rucio-clients-1.9.6/doc/build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/comment-close.png` & `rucio-clients-1.9.6/doc/build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/comment.png` & `rucio-clients-1.9.6/doc/build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/default.css` & `rucio-clients-1.9.6/doc/build/html/_static/default.css`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/doctools.js` & `rucio-clients-1.9.6/doc/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/jquery-1.11.1.js` & `rucio-clients-1.9.6/doc/build/html/_static/jquery-1.11.1.js`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/jquery.js` & `rucio-clients-1.9.6/doc/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/pygments.css` & `rucio-clients-1.9.6/doc/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/rucio_logo.png` & `rucio-clients-1.9.6/doc/build/html/_static/rucio_logo.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/searchtools.js` & `rucio-clients-1.9.6/doc/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/sidebar.js` & `rucio-clients-1.9.6/doc/build/html/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/underscore-1.3.1.js` & `rucio-clients-1.9.6/doc/build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/underscore.js` & `rucio-clients-1.9.6/doc/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/_static/websupport.js` & `rucio-clients-1.9.6/doc/build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/man/rucio-admin.html` & `rucio-clients-1.9.6/doc/build/html/man/rucio-admin.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/man/rucio.html` & `rucio-clients-1.9.6/doc/build/html/man/rucio.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/rest/attach_dids_to_dids.html` & `rucio-clients-1.9.6/doc/build/html/rest/attach_dids_to_dids.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/add_account_identity.html` & `rucio-clients-1.9.6/doc/build/html/usecases/add_account_identity.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/add_metadata_dataset.html` & `rucio-clients-1.9.6/doc/build/html/usecases/add_metadata_dataset.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/add_metadata_file.html` & `rucio-clients-1.9.6/doc/build/html/usecases/add_metadata_file.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/add_scope_to_account.html` & `rucio-clients-1.9.6/doc/build/html/usecases/add_scope_to_account.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/add_subscription.html` & `rucio-clients-1.9.6/doc/build/html/usecases/add_subscription.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/authentication.html` & `rucio-clients-1.9.6/doc/build/html/usecases/authentication.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/consistency_file_between_storage_and_rucio.html` & `rucio-clients-1.9.6/doc/build/html/usecases/consistency_file_between_storage_and_rucio.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/delete_file_replica_from_storage.html` & `rucio-clients-1.9.6/doc/build/html/usecases/delete_file_replica_from_storage.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/detect_site_reach_watermark.html` & `rucio-clients-1.9.6/doc/build/html/usecases/detect_site_reach_watermark.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.html` & `rucio-clients-1.9.6/doc/build/html/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/download_all_files_from_a_given_list_of_files_from_rucio.html` & `rucio-clients-1.9.6/doc/build/html/usecases/download_all_files_from_a_given_list_of_files_from_rucio.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/download_all_files_in_a_dataset_from_rucio.html` & `rucio-clients-1.9.6/doc/build/html/usecases/download_all_files_in_a_dataset_from_rucio.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/download_files_from_rucio.html` & `rucio-clients-1.9.6/doc/build/html/usecases/download_files_from_rucio.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/obsolete_dataset.html` & `rucio-clients-1.9.6/doc/build/html/usecases/obsolete_dataset.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/register_account.html` & `rucio-clients-1.9.6/doc/build/html/usecases/register_account.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/register_file_already_on_storage_system.html` & `rucio-clients-1.9.6/doc/build/html/usecases/register_file_already_on_storage_system.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/register_transfer_request_file_fts.html` & `rucio-clients-1.9.6/doc/build/html/usecases/register_transfer_request_file_fts.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/remove_replication_rules_from_file.html` & `rucio-clients-1.9.6/doc/build/html/usecases/remove_replication_rules_from_file.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/reupload_after_failure.html` & `rucio-clients-1.9.6/doc/build/html/usecases/reupload_after_failure.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/search.html` & `rucio-clients-1.9.6/doc/build/html/usecases/search.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/select_unwanted_files_for_deletion.html` & `rucio-clients-1.9.6/doc/build/html/usecases/select_unwanted_files_for_deletion.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/set_replication_rule_to_file.html` & `rucio-clients-1.9.6/doc/build/html/usecases/set_replication_rule_to_file.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/upload_file_with_replication_rule.html` & `rucio-clients-1.9.6/doc/build/html/usecases/upload_file_with_replication_rule.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/usecase_upload_file_into_rucio.html` & `rucio-clients-1.9.6/doc/build/html/usecases/usecase_upload_file_into_rucio.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases/where_are_the_replicas_for_a_file.html` & `rucio-clients-1.9.6/doc/build/html/usecases/where_are_the_replicas_for_a_file.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/Acronyms_and_Abbreviations.html` & `rucio-clients-1.9.6/doc/build/html/Acronyms_and_Abbreviations.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/Architecture.html` & `rucio-clients-1.9.6/doc/build/html/Architecture.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/Comparison_matrix.html` & `rucio-clients-1.9.6/doc/build/html/Comparison_matrix.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/REST_Account.html` & `rucio-clients-1.9.6/doc/build/html/REST_Account.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/REST_Intro.html` & `rucio-clients-1.9.6/doc/build/html/REST_Intro.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/REST_authentication.html` & `rucio-clients-1.9.6/doc/build/html/REST_authentication.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/REST_did.html` & `rucio-clients-1.9.6/doc/build/html/REST_did.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/REST_identity.html` & `rucio-clients-1.9.6/doc/build/html/REST_identity.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/REST_lock.html` & `rucio-clients-1.9.6/doc/build/html/REST_lock.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/REST_meta.html` & `rucio-clients-1.9.6/doc/build/html/REST_meta.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/REST_redirect.html` & `rucio-clients-1.9.6/doc/build/html/REST_redirect.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/REST_replica.html` & `rucio-clients-1.9.6/doc/build/html/REST_replica.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/REST_rse.html` & `rucio-clients-1.9.6/doc/build/html/REST_rse.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/REST_rule.html` & `rucio-clients-1.9.6/doc/build/html/REST_rule.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/REST_scope.html` & `rucio-clients-1.9.6/doc/build/html/REST_scope.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/REST_subscription.html` & `rucio-clients-1.9.6/doc/build/html/REST_subscription.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/Rucio_Project_Meeting.html` & `rucio-clients-1.9.6/doc/build/html/Rucio_Project_Meeting.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/account.html` & `rucio-clients-1.9.6/doc/build/html/account.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/accountlimit.html` & `rucio-clients-1.9.6/doc/build/html/accountlimit.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/api_curl_examples.html` & `rucio-clients-1.9.6/doc/build/html/api_curl_examples.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/atlas_integration_testbed.html` & `rucio-clients-1.9.6/doc/build/html/atlas_integration_testbed.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/authentication_and_identity.html` & `rucio-clients-1.9.6/doc/build/html/authentication_and_identity.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/cli_admin_examples.html` & `rucio-clients-1.9.6/doc/build/html/cli_admin_examples.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/cli_examples.html` & `rucio-clients-1.9.6/doc/build/html/cli_examples.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/client_examples.html` & `rucio-clients-1.9.6/doc/build/html/client_examples.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/client_howto.html` & `rucio-clients-1.9.6/doc/build/html/client_howto.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/client_tutorial.html` & `rucio-clients-1.9.6/doc/build/html/client_tutorial.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/core_constants.html` & `rucio-clients-1.9.6/doc/build/html/core_constants.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/developing.html` & `rucio-clients-1.9.6/doc/build/html/developing.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/development_guidelines.html` & `rucio-clients-1.9.6/doc/build/html/development_guidelines.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/did.html` & `rucio-clients-1.9.6/doc/build/html/did.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/exception.html` & `rucio-clients-1.9.6/doc/build/html/exception.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/genindex.html` & `rucio-clients-1.9.6/doc/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/http-routingtable.html` & `rucio-clients-1.9.6/doc/build/html/http-routingtable.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/identity.html` & `rucio-clients-1.9.6/doc/build/html/identity.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/index.html` & `rucio-clients-1.9.6/doc/build/html/index.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/installing_atlas_clients.html` & `rucio-clients-1.9.6/doc/build/html/installing_atlas_clients.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/installing_clients.html` & `rucio-clients-1.9.6/doc/build/html/installing_clients.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/installing_server.html` & `rucio-clients-1.9.6/doc/build/html/installing_server.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/lock.html` & `rucio-clients-1.9.6/doc/build/html/lock.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/meta-data.html` & `rucio-clients-1.9.6/doc/build/html/meta-data.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/naming_convention_db.html` & `rucio-clients-1.9.6/doc/build/html/naming_convention_db.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/objects.inv` & `rucio-clients-1.9.6/doc/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Accounting_and_quota.html` & `rucio-clients-1.9.6/doc/build/html/overview_Accounting_and_quota.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Architecture.html` & `rucio-clients-1.9.6/doc/build/html/overview_Architecture.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Data_Deletion.html` & `rucio-clients-1.9.6/doc/build/html/overview_Data_Deletion.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Database_Schema.html` & `rucio-clients-1.9.6/doc/build/html/overview_Database_Schema.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Deployment.html` & `rucio-clients-1.9.6/doc/build/html/overview_Deployment.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Exception_Handling.html` & `rucio-clients-1.9.6/doc/build/html/overview_Exception_Handling.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_File_Dataset_Container.html` & `rucio-clients-1.9.6/doc/build/html/overview_File_Dataset_Container.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Meta-data_attributes.html` & `rucio-clients-1.9.6/doc/build/html/overview_Meta-data_attributes.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Notifications.html` & `rucio-clients-1.9.6/doc/build/html/overview_Notifications.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Permission_model.html` & `rucio-clients-1.9.6/doc/build/html/overview_Permission_model.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Replica_management.html` & `rucio-clients-1.9.6/doc/build/html/overview_Replica_management.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Rucio_Storage_Element.html` & `rucio-clients-1.9.6/doc/build/html/overview_Rucio_Storage_Element.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Rucio_Storage_Element_Manager.html` & `rucio-clients-1.9.6/doc/build/html/overview_Rucio_Storage_Element_Manager.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Rucio_account.html` & `rucio-clients-1.9.6/doc/build/html/overview_Rucio_account.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Rules.html` & `rucio-clients-1.9.6/doc/build/html/overview_Rules.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Scheduled_Transfers.html` & `rucio-clients-1.9.6/doc/build/html/overview_Scheduled_Transfers.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Subscriptions.html` & `rucio-clients-1.9.6/doc/build/html/overview_Subscriptions.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_Traceability_and_logging.html` & `rucio-clients-1.9.6/doc/build/html/overview_Traceability_and_logging.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/overview_flow.html` & `rucio-clients-1.9.6/doc/build/html/overview_flow.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/permission.html` & `rucio-clients-1.9.6/doc/build/html/permission.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/py-modindex.html` & `rucio-clients-1.9.6/doc/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/replica.html` & `rucio-clients-1.9.6/doc/build/html/replica.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/replication_rules_examples.html` & `rucio-clients-1.9.6/doc/build/html/replication_rules_examples.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/rest.html` & `rucio-clients-1.9.6/doc/build/html/rest.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/rse.html` & `rucio-clients-1.9.6/doc/build/html/rse.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/rucio_cli.html` & `rucio-clients-1.9.6/doc/build/html/rucio_cli.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/rucio_clients.html` & `rucio-clients-1.9.6/doc/build/html/rucio_clients.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/rule.html` & `rucio-clients-1.9.6/doc/build/html/rule.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/rules_workflow.html` & `rucio-clients-1.9.6/doc/build/html/rules_workflow.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/scope.html` & `rucio-clients-1.9.6/doc/build/html/scope.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/search.html` & `rucio-clients-1.9.6/doc/build/html/search.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/searchindex.js` & `rucio-clients-1.9.6/doc/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/setup.html` & `rucio-clients-1.9.6/doc/build/html/setup.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/subscription.html` & `rucio-clients-1.9.6/doc/build/html/subscription.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/build/html/usecases.html` & `rucio-clients-1.9.6/doc/build/html/usecases.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/design/RSE/meeting-2012-02-23.org` & `rucio-clients-1.9.6/doc/design/RSE/meeting-2012-02-23.org`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/design/erd/ERD.graffle` & `rucio-clients-1.9.6/doc/design/erd/ERD.graffle`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/design/erd/ERD.pdf` & `rucio-clients-1.9.6/doc/design/erd/ERD.pdf`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/design/rucio_schema.pdf` & `rucio-clients-1.9.6/doc/design/rucio_schema.pdf`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/_static/basic.css` & `rucio-clients-1.9.6/doc/source/_static/basic.css`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/_static/classic.css` & `rucio-clients-1.9.6/doc/source/_static/classic.css`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/_static/default.css` & `rucio-clients-1.9.6/doc/source/_static/default.css`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/_static/rucio_logo.png` & `rucio-clients-1.9.6/doc/source/_static/rucio_logo.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/_templates/layout.html` & `rucio-clients-1.9.6/doc/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/curl_examples/get_account_whoami.out` & `rucio-clients-1.9.6/doc/source/curl_examples/get_account_whoami.out`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/example_outputs/failure-rucio.tests.test_curl.TestCurlRucio.test_get_accounts_whoami.txt` & `rucio-clients-1.9.6/doc/source/example_outputs/failure-rucio.tests.test_curl.TestCurlRucio.test_get_accounts_whoami.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_accounts_whoami.txt` & `rucio-clients-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_accounts_whoami.txt`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/deployment.graffle/QuickLook/Preview.pdf` & `rucio-clients-1.9.6/doc/source/images/deployment.graffle/QuickLook/Preview.pdf`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/deployment.graffle/QuickLook/Thumbnail.tiff` & `rucio-clients-1.9.6/doc/source/images/deployment.graffle/QuickLook/Thumbnail.tiff`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/deployment.graffle/data.plist` & `rucio-clients-1.9.6/doc/source/images/deployment.graffle/data.plist`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/deployment.graffle/image2.tiff` & `rucio-clients-1.9.6/doc/source/images/deployment.graffle/image2.tiff`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/deployment.graffle/image3.tiff` & `rucio-clients-1.9.6/doc/source/images/deployment.graffle/image3.tiff`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/RSE_overview.png` & `rucio-clients-1.9.6/doc/source/images/RSE_overview.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/RSE_sequence_instantiation.png` & `rucio-clients-1.9.6/doc/source/images/RSE_sequence_instantiation.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/RSE_sequence_usage.png` & `rucio-clients-1.9.6/doc/source/images/RSE_sequence_usage.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/accounts.png` & `rucio-clients-1.9.6/doc/source/images/accounts.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/architecture.graffle` & `rucio-clients-1.9.6/doc/source/images/architecture.graffle`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/architecture.png` & `rucio-clients-1.9.6/doc/source/images/architecture.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/deployment.png` & `rucio-clients-1.9.6/doc/source/images/deployment.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/exception_handling.graffle` & `rucio-clients-1.9.6/doc/source/images/exception_handling.graffle`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/exception_handling.png` & `rucio-clients-1.9.6/doc/source/images/exception_handling.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/highLevelRoadmap.graffle` & `rucio-clients-1.9.6/doc/source/images/highLevelRoadmap.graffle`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/rucio-get.graffle` & `rucio-clients-1.9.6/doc/source/images/rucio-get.graffle`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/rucio-get.png` & `rucio-clients-1.9.6/doc/source/images/rucio-get.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/rucio-put.graffle` & `rucio-clients-1.9.6/doc/source/images/rucio-put.graffle`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/rucio-put.png` & `rucio-clients-1.9.6/doc/source/images/rucio-put.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/rucio-register.graffle` & `rucio-clients-1.9.6/doc/source/images/rucio-register.graffle`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/rucio-register.png` & `rucio-clients-1.9.6/doc/source/images/rucio-register.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/rucio_schema.gml` & `rucio-clients-1.9.6/doc/source/images/rucio_schema.gml`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/rucio_schema.pdf` & `rucio-clients-1.9.6/doc/source/images/rucio_schema.pdf`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/rucio_schema.png` & `rucio-clients-1.9.6/doc/source/images/rucio_schema.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/scheduled_transfers.dia` & `rucio-clients-1.9.6/doc/source/images/scheduled_transfers.dia`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/images/scheduled_transfers.png` & `rucio-clients-1.9.6/doc/source/images/scheduled_transfers.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/man/rucio-admin.rst` & `rucio-clients-1.9.6/doc/source/man/rucio-admin.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/man/rucio.rst` & `rucio-clients-1.9.6/doc/source/man/rucio.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/add_account_identity.rst` & `rucio-clients-1.9.6/doc/source/usecases/add_account_identity.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/add_metadata_dataset.rst` & `rucio-clients-1.9.6/doc/source/usecases/add_metadata_dataset.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/add_metadata_file.rst` & `rucio-clients-1.9.6/doc/source/usecases/add_metadata_file.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/add_scope_to_account.rst` & `rucio-clients-1.9.6/doc/source/usecases/add_scope_to_account.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/add_subscription.rst` & `rucio-clients-1.9.6/doc/source/usecases/add_subscription.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/authentication.rst` & `rucio-clients-1.9.6/doc/source/usecases/authentication.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/consistency_file_between_storage_and_rucio.rst` & `rucio-clients-1.9.6/doc/source/usecases/consistency_file_between_storage_and_rucio.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/delete_file_replica_from_storage.rst` & `rucio-clients-1.9.6/doc/source/usecases/delete_file_replica_from_storage.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/detect_site_reach_watermark.rst` & `rucio-clients-1.9.6/doc/source/usecases/detect_site_reach_watermark.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.rst` & `rucio-clients-1.9.6/doc/source/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/download_all_files_from_a_given_list_of_files_from_rucio.rst` & `rucio-clients-1.9.6/doc/source/usecases/download_all_files_from_a_given_list_of_files_from_rucio.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/download_all_files_in_a_dataset_from_rucio.rst` & `rucio-clients-1.9.6/doc/source/usecases/download_all_files_in_a_dataset_from_rucio.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/download_files_from_rucio.rst` & `rucio-clients-1.9.6/doc/source/usecases/download_files_from_rucio.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/obsolete_dataset.rst` & `rucio-clients-1.9.6/doc/source/usecases/obsolete_dataset.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/register_account.rst` & `rucio-clients-1.9.6/doc/source/usecases/register_account.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/register_file_already_on_storage_system.rst` & `rucio-clients-1.9.6/doc/source/usecases/register_file_already_on_storage_system.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/register_transfer_request_file_fts.rst` & `rucio-clients-1.9.6/doc/source/usecases/register_transfer_request_file_fts.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/remove_replication_rules_from_file.rst` & `rucio-clients-1.9.6/doc/source/usecases/remove_replication_rules_from_file.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/reupload_after_failure.rst` & `rucio-clients-1.9.6/doc/source/usecases/reupload_after_failure.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/search.rst` & `rucio-clients-1.9.6/doc/source/usecases/search.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/set_replication_rule_to_file.rst` & `rucio-clients-1.9.6/doc/source/usecases/set_replication_rule_to_file.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/upload_file_with_replication_rule.rst` & `rucio-clients-1.9.6/doc/source/usecases/upload_file_with_replication_rule.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/usecase_upload_file_into_rucio.rst` & `rucio-clients-1.9.6/doc/source/usecases/usecase_upload_file_into_rucio.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases/where_are_the_replicas_for_a_file.rst` & `rucio-clients-1.9.6/doc/source/usecases/where_are_the_replicas_for_a_file.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/Comparison_matrix.rst` & `rucio-clients-1.9.6/doc/source/Comparison_matrix.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/REST_Account.rst` & `rucio-clients-1.9.6/doc/source/REST_Account.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/REST_Intro.rst` & `rucio-clients-1.9.6/doc/source/REST_Intro.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/REST_authentication.rst` & `rucio-clients-1.9.6/doc/source/REST_authentication.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/REST_did.rst` & `rucio-clients-1.9.6/doc/source/REST_did.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/REST_identity.rst` & `rucio-clients-1.9.6/doc/source/REST_identity.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/REST_lock.rst` & `rucio-clients-1.9.6/doc/source/REST_lock.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/REST_meta.rst` & `rucio-clients-1.9.6/doc/source/REST_meta.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/REST_replica.rst` & `rucio-clients-1.9.6/doc/source/REST_replica.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/REST_rse.rst` & `rucio-clients-1.9.6/doc/source/REST_rse.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/REST_rule.rst` & `rucio-clients-1.9.6/doc/source/REST_rule.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/REST_scope.rst` & `rucio-clients-1.9.6/doc/source/REST_scope.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/REST_subscription.rst` & `rucio-clients-1.9.6/doc/source/REST_subscription.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/RSE_Expressions.rst` & `rucio-clients-1.9.6/doc/source/RSE_Expressions.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/Rucio_Project_Meeting.rst` & `rucio-clients-1.9.6/doc/source/Rucio_Project_Meeting.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/accounts.pdf` & `rucio-clients-1.9.6/doc/source/accounts.pdf`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/accounts.png` & `rucio-clients-1.9.6/doc/source/accounts.png`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/api_curl_examples.rst` & `rucio-clients-1.9.6/doc/source/api_curl_examples.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/atlas_integration_testbed.rst` & `rucio-clients-1.9.6/doc/source/atlas_integration_testbed.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/cli_admin_examples.rst` & `rucio-clients-1.9.6/doc/source/cli_admin_examples.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/cli_examples.rst` & `rucio-clients-1.9.6/doc/source/cli_examples.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/client_examples.rst` & `rucio-clients-1.9.6/doc/source/client_examples.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/client_tutorial.rst` & `rucio-clients-1.9.6/doc/source/client_tutorial.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/conf.py` & `rucio-clients-1.9.6/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/developing.rst` & `rucio-clients-1.9.6/doc/source/developing.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/development_guidelines.rst` & `rucio-clients-1.9.6/doc/source/development_guidelines.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/index.rst` & `rucio-clients-1.9.6/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/installing_atlas_clients.rst` & `rucio-clients-1.9.6/doc/source/installing_atlas_clients.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/installing_clients.rst` & `rucio-clients-1.9.6/doc/source/installing_clients.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/installing_server.rst` & `rucio-clients-1.9.6/doc/source/installing_server.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/naming_convention_db.rst` & `rucio-clients-1.9.6/doc/source/naming_convention_db.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/overview_Data_Deletion.rst` & `rucio-clients-1.9.6/doc/source/overview_Data_Deletion.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/overview_Exception_Handling.rst` & `rucio-clients-1.9.6/doc/source/overview_Exception_Handling.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/overview_File_Dataset_Container.rst` & `rucio-clients-1.9.6/doc/source/overview_File_Dataset_Container.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/overview_Meta-data_attributes.rst` & `rucio-clients-1.9.6/doc/source/overview_Meta-data_attributes.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/overview_Replica_management.rst` & `rucio-clients-1.9.6/doc/source/overview_Replica_management.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/overview_Rucio_Storage_Element.rst` & `rucio-clients-1.9.6/doc/source/overview_Rucio_Storage_Element.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/overview_Rucio_Storage_Element_Manager.rst` & `rucio-clients-1.9.6/doc/source/overview_Rucio_Storage_Element_Manager.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/overview_Rucio_account.rst` & `rucio-clients-1.9.6/doc/source/overview_Rucio_account.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/overview_Rules.rst` & `rucio-clients-1.9.6/doc/source/overview_Rules.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/overview_Scheduled_Transfers.rst` & `rucio-clients-1.9.6/doc/source/overview_Scheduled_Transfers.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/overview_Subscriptions.rst` & `rucio-clients-1.9.6/doc/source/overview_Subscriptions.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/replication_rules_examples.rst` & `rucio-clients-1.9.6/doc/source/replication_rules_examples.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/rest.rst` & `rucio-clients-1.9.6/doc/source/rest.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/rucio_cli.rst` & `rucio-clients-1.9.6/doc/source/rucio_cli.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/rucio_clients.rst` & `rucio-clients-1.9.6/doc/source/rucio_clients.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/rules_workflow.rst` & `rucio-clients-1.9.6/doc/source/rules_workflow.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/source/usecases.rst` & `rucio-clients-1.9.6/doc/source/usecases.rst`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/Makefile` & `rucio-clients-1.9.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/doc/make.bat` & `rucio-clients-1.9.6/doc/make.bat`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/etc/schemas/sub_filter.json` & `rucio-clients-1.9.6/etc/schemas/sub_filter.json`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/etc/rse-accounts.cfg.template` & `rucio-clients-1.9.6/etc/rse-accounts.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/etc/rucio.cfg.atlas.client.template` & `rucio-clients-1.9.6/etc/rucio.cfg.atlas.client.template`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/etc/rucio.cfg.template` & `rucio-clients-1.9.6/etc/rucio.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/cli/upload.py` & `rucio-clients-1.9.6/lib/rucio/client/cli/upload.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/accountclient.py` & `rucio-clients-1.9.6/lib/rucio/client/accountclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/accountlimitclient.py` & `rucio-clients-1.9.6/lib/rucio/client/accountlimitclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/baseclient.py` & `rucio-clients-1.9.6/lib/rucio/client/baseclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/client.py` & `rucio-clients-1.9.6/lib/rucio/client/client.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/configclient.py` & `rucio-clients-1.9.6/lib/rucio/client/configclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/didclient.py` & `rucio-clients-1.9.6/lib/rucio/client/didclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/dq2client.py` & `rucio-clients-1.9.6/lib/rucio/client/dq2client.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/fileclient.py` & `rucio-clients-1.9.6/lib/rucio/client/fileclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/lockclient.py` & `rucio-clients-1.9.6/lib/rucio/client/lockclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/metaclient.py` & `rucio-clients-1.9.6/lib/rucio/client/metaclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/objectstoreclient.py` & `rucio-clients-1.9.6/lib/rucio/client/objectstoreclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/pingclient.py` & `rucio-clients-1.9.6/lib/rucio/client/pingclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/replicaclient.py` & `rucio-clients-1.9.6/lib/rucio/client/replicaclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/rseclient.py` & `rucio-clients-1.9.6/lib/rucio/client/rseclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/ruleclient.py` & `rucio-clients-1.9.6/lib/rucio/client/ruleclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/scopeclient.py` & `rucio-clients-1.9.6/lib/rucio/client/scopeclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/subscriptionclient.py` & `rucio-clients-1.9.6/lib/rucio/client/subscriptionclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/client/uploadclient.py` & `rucio-clients-1.9.6/lib/rucio/client/uploadclient.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/common/client.py` & `rucio-clients-1.9.6/lib/rucio/common/client.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/common/closeness_sorter.py` & `rucio-clients-1.9.6/lib/rucio/common/closeness_sorter.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/common/config.py` & `rucio-clients-1.9.6/lib/rucio/common/config.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/common/constants.py` & `rucio-clients-1.9.6/lib/rucio/common/constants.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/common/exception.py` & `rucio-clients-1.9.6/lib/rucio/common/exception.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/common/log.py` & `rucio-clients-1.9.6/lib/rucio/common/log.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/common/objectstore.py` & `rucio-clients-1.9.6/lib/rucio/common/objectstore.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/common/policy.py` & `rucio-clients-1.9.6/lib/rucio/common/policy.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/common/replicas_selector.py` & `rucio-clients-1.9.6/lib/rucio/common/replicas_selector.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/common/rse_attributes.py` & `rucio-clients-1.9.6/lib/rucio/common/rse_attributes.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/common/schema.py` & `rucio-clients-1.9.6/lib/rucio/common/schema.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/common/utils.py` & `rucio-clients-1.9.6/lib/rucio/common/utils.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/cache.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/cache.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/dummy.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/dummy.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/gfal.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/gfal.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/gfalv2.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/gfalv2.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/gsiftp.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/gsiftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             params.timeout = 3600
             ret = ctx.filecopy(params, str(space_usage_url), str('file://' + dest))
 
             if ret == 0:
                 data_file = open(dest)
                 data = json.load(data_file)
                 data_file.close()
-                if data.keys()[0] != agis_token:
+                if agis_token not in data.keys():
                     print 'ERROR: space usage json has different token as key'
                 else:
                     totalsize = data[agis_token]['total_space']
                     used = data[agis_token]['used_space']
                     unusedsize = totalsize - used
                     return totalsize, unusedsize
         except Exception as e:
```

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/http_cache.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/http_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/mock.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/mock.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/ngarc.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/ngarc.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/posix.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/posix.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/protocol.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/protocol.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/rfio.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/rfio.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/s3.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/s3.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/s3boto.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/s3boto.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/s3es.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/s3es.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/sftp.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/sftp.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/signeds3.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/signeds3.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/srm.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/srm.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/webdav.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/protocols/xrootd.py` & `rucio-clients-1.9.6/lib/rucio/rse/protocols/xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/__init__.py` & `rucio-clients-1.9.6/lib/rucio/rse/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/rse/rsemanager.py` & `rucio-clients-1.9.6/lib/rucio/rse/rsemanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Authors:
 # - Ralph Vigne, <ralph.vigne@cern.ch>, 2013-2015
-# - Mario Lassnig, <mario.lassnig@cern.ch>, 2012-2014
+# - Mario Lassnig, <mario.lassnig@cern.ch>, 2012-2014, 2017
 # - Vincent Garonne, <vincent.garonne@cern.ch>, 2013-2014
 # - Cedric Serfon, <cedric.serfon@cern.ch>, 2013-2014
 # - Wen Guan, <wen.guan@cern.ch>, 2014-2015
 
 import copy
 import os
 
@@ -170,38 +170,40 @@
         :raises RSEOperationNotSupported: If no matching protocol was found for the requested operation
     """
     if len(set([urlparse(pfn).scheme for pfn in pfns])) != 1:
         raise ValueError('All PFNs must provide the same protocol scheme')
     return create_protocol(rse_settings, operation, urlparse(pfns[0]).scheme).parse_pfns(pfns)
 
 
-def download(rse_settings, files, dest_dir=None, printstatements=False):
+def download(rse_settings, files, dest_dir=None, force_scheme=None, printstatements=False):
     """
         Copy a file from the connected storage to the local file system.
         Providing a list indicates the bulk mode.
 
 
         :param rse_settings:    RSE to use
         :param files:           a single dict or a list with dicts containing 'scope' and 'name'
                                 if LFNs are provided and additional 'pfn' if PFNs are provided.
                                 E.g.  [{'name': '2_rse_remote_get.raw', 'scope': 'user.jdoe'},
                                        {'name':'3_rse_remote_get.raw', 'scope': 'user.jdoe', 'pfn': 'user/jdoe/5a/98/3_rse_remote_get.raw'}]
         :param dest_dir:        path to the directory where the downloaded files will be stored. If not given, each scope is represented by its own directory.
+        :param force_scheme:    normally the scheme is dictated by the RSE object, when specifying the PFN it must be forced to the one specified in the PFN, overruling the RSE description.
 
         :returns: True/False for a single file or a dict object with 'scope:name' for LFNs or 'name' for PFNs as keys and True or the exception as value for each file in bulk mode
 
         :raises SourceNotFound: remote source file can not be found on storage
         :raises DestinationNotAccessible: local destination directory is not accessible
         :raises FileConsistencyMismatch: the checksum of the downloaded file does not match the provided one
         :raises ServiceUnavailable: for any other reason
 
     """
     ret = {}
     gs = True  # gs represents the global status which inidcates if every operation workd in bulk mode
-    protocol = create_protocol(rse_settings, 'read')
+
+    protocol = create_protocol(rse_settings, 'read', scheme=force_scheme)
     protocol.connect()
 
     files = [files] if not type(files) is list else files
     for f in files:
         pfn = f['pfn'] if 'pfn' in f else protocol.lfns2pfns(f).values()[0]
         target_dir = "./%s" % f['scope'] if dest_dir is None else dest_dir
         try:
```

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/emulation/usecases/auth.py` & `rucio-clients-1.9.6/lib/rucio/tests/emulation/usecases/auth.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/emulation/usecases/dummy.py` & `rucio-clients-1.9.6/lib/rucio/tests/emulation/usecases/dummy.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/emulation/usecases/dummy_template.py` & `rucio-clients-1.9.6/lib/rucio/tests/emulation/usecases/dummy_template.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/emulation/usecases/jdoe.py` & `rucio-clients-1.9.6/lib/rucio/tests/emulation/usecases/jdoe.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/emulation/usecases/panda.py` & `rucio-clients-1.9.6/lib/rucio/tests/emulation/usecases/panda.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/emulation/usecases/panda_new.py` & `rucio-clients-1.9.6/lib/rucio/tests/emulation/usecases/panda_new.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/emulation/usecases/tzero.py` & `rucio-clients-1.9.6/lib/rucio/tests/emulation/usecases/tzero.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/emulation/emulator.py` & `rucio-clients-1.9.6/lib/rucio/tests/emulation/emulator.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/emulation/ucemulator.py` & `rucio-clients-1.9.6/lib/rucio/tests/emulation/ucemulator.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/emulation/ucprocess.py` & `rucio-clients-1.9.6/lib/rucio/tests/emulation/ucprocess.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/emulation/worker.py` & `rucio-clients-1.9.6/lib/rucio/tests/emulation/worker.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/common.py` & `rucio-clients-1.9.6/lib/rucio/tests/common.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/rsemgr_api_test.py` & `rucio-clients-1.9.6/lib/rucio/tests/rsemgr_api_test.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_account.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_account_limits.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_account_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_alembic.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_auditor.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_auditor.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_auditor_hdfs.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_auditor_hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_auditor_srmdumps.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_auditor_srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_authentication.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_bb8.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_bin_rucio.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_bin_rucio.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_clients.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_config.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_conveyor.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_conveyor.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_counter.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_curl.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_curl.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_dataset_replicas.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_dataset_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_db.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_did.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_did.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_dumper.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_dumper.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_dumper_consistency.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_dumper_consistency.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_dumper_data_model.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_dumper_data_model.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_dumper_path_parsing.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_dumper_path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_heartbeat.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_hermes.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_hermes.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_identity.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_judge_cleaner.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_judge_cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_judge_evaluator.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_judge_evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_judge_injector.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_judge_injector.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_judge_repairer.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_judge_repairer.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_message.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_meta.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_meta_did.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_meta_did.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_monitor.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_naming_convention.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_objectstore.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_objectstore.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_permission.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_ping.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_quarantined_replica.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_reaper.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_redirect.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_replica.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_rse.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_rse_expression_parser.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_gfal2.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_gfal2.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_mock.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_mock.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_posix.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_posix.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_s3.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_s3.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_s3boto.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_s3boto.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_s3es.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_s3es.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_sftp.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_sftp.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_signeds3.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_signeds3.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_srm.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_srm.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_webdav.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_rse_protocol_xrootd.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_rse_protocol_xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_rucio_cache.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_rucio_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_rucio_server.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_rule.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_scope.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_subscription.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_temporary_did.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_temporary_did.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_trace.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/tests/test_undertaker.py` & `rucio-clients-1.9.6/lib/rucio/tests/test_undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/lib/rucio/version.py` & `rucio-clients-1.9.6/lib/rucio/version.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/tools/pip-requires-client` & `rucio-clients-1.9.6/tools/pip-requires-client`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/AUTHORS` & `rucio-clients-1.9.6/AUTHORS`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/MANIFEST.in` & `rucio-clients-1.9.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/pylintrc` & `rucio-clients-1.9.6/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/setup.cfg` & `rucio-clients-1.9.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/setup.py` & `rucio-clients-1.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `rucio-clients-1.9.5/PKG-INFO` & `rucio-clients-1.9.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rucio-clients
-Version: 1.9.5
+Version: 1.9.6
 Summary: Rucio Client Lite Package
 Home-page: http://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

