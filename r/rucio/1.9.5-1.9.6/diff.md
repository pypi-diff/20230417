# Comparing `tmp/rucio-1.9.5.tar.gz` & `tmp/rucio-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rucio-1.9.5.tar", last modified: Tue Jan 24 09:13:46 2017, max compression
+gzip compressed data, was "dist/rucio-1.9.6.tar", last modified: Tue Feb  7 09:03:32 2017, max compression
```

## Comparing `rucio-1.9.5.tar` & `rucio-1.9.6.tar`

### file list

```diff
@@ -1,1169 +1,1170 @@
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/bin/
--rwxr-xr-x   0 barisits (51071) zp        (1307)   120671 2017-01-24 09:05:38.000000 rucio-1.9.5/bin/rucio
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1367 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-abacus-account
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1355 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-abacus-rse
--rwxr-xr-x   0 barisits (51071) zp        (1307)    44207 2016-11-28 16:40:28.000000 rucio-1.9.5/bin/rucio-admin
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1697 2016-11-28 16:40:28.000000 rucio-1.9.5/bin/rucio-atropos
--rwxr-xr-x   0 barisits (51071) zp        (1307)     5298 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-auditor
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1257 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-automatix
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2366 2017-01-20 09:22:58.000000 rucio-1.9.5/bin/rucio-bb8
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3427 2016-11-28 16:40:28.000000 rucio-1.9.5/bin/rucio-c3po
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4661 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-cache-client
--rwxr-xr-x   0 barisits (51071) zp        (1307)      873 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-cache-consumer
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2174 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-conveyor-finisher
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2772 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-conveyor-poller
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1798 2016-11-25 16:30:17.000000 rucio-1.9.5/bin/rucio-conveyor-poller-latest
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1206 2016-11-28 16:40:28.000000 rucio-1.9.5/bin/rucio-conveyor-receiver
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3600 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-conveyor-stager
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3791 2016-11-28 16:40:28.000000 rucio-1.9.5/bin/rucio-conveyor-submitter
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1028 2016-11-28 16:40:28.000000 rucio-1.9.5/bin/rucio-conveyor-throttler
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3791 2016-11-28 16:40:28.000000 rucio-1.9.5/bin/rucio-conveyor-transfer-submitter
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1545 2016-11-28 16:40:28.000000 rucio-1.9.5/bin/rucio-dark-reaper
--rwxr-xr-x   0 barisits (51071) zp        (1307)     5505 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-dumper
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1315 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-hermes
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1021 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-judge-cleaner
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1024 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-judge-evaluator
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1027 2016-11-28 16:40:28.000000 rucio-1.9.5/bin/rucio-judge-injector
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1023 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-judge-repairer
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1071 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-kronos
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1546 2016-11-28 16:40:28.000000 rucio-1.9.5/bin/rucio-light-reaper
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1244 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-necromancer
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2162 2016-11-28 16:40:28.000000 rucio-1.9.5/bin/rucio-reaper
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1299 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-transmogrifier
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1101 2016-11-25 15:17:13.000000 rucio-1.9.5/bin/rucio-undertaker
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/atlasnote/
--rwxr-xr-x   0 barisits (51071) zp        (1307)   164832 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/AN_atlaslogo.pdf
--rwxr-xr-x   0 barisits (51071) zp        (1307)    88058 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/AN_cernlogo.pdf
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2877 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/AtlasRucioNote.aux
--rw-r--r--   0 barisits (51071) zp        (1307)   440060 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/AtlasRucioNote.pdf
--rwxr-xr-x   0 barisits (51071) zp        (1307)    23795 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/AtlasRucioNote.tex
--rw-r--r--   0 barisits (51071) zp        (1307)    65762 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/accounts.graffle
--rw-r--r--   0 barisits (51071) zp        (1307)    31807 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/accounts.pdf
--rw-r--r--   0 barisits (51071) zp        (1307)    27065 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/accounts.png
--rw-r--r--   0 barisits (51071) zp        (1307)   125132 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/aggregation_hierarchy.graffle
--rw-r--r--   0 barisits (51071) zp        (1307)    44183 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/aggregation_hierarchy.pdf
--rwxr-xr-x   0 barisits (51071) zp        (1307)     6980 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/atlasnote.cls
--rwxr-xr-x   0 barisits (51071) zp        (1307)     6557 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/booktabs.sty
--rw-r--r--   0 barisits (51071) zp        (1307)   132902 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/dataset_hierarchy.graffle
--rw-r--r--   0 barisits (51071) zp        (1307)    44639 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/dataset_hierarchy.pdf
--rwxr-xr-x   0 barisits (51071) zp        (1307)    18775 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/fncychap.sty
--rwxr-xr-x   0 barisits (51071) zp        (1307)    14665 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/sphinx.sty
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2073 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/sphinxhowto.cls
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3421 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/atlasnote/sphinxmanual.cls
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/doctrees/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/doctrees/man/
--rw-r--r--   0 barisits (51071) zp        (1307)    13923 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/man/rucio-admin.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    21710 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/man/rucio.doctree
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/doctrees/rest/
--rw-r--r--   0 barisits (51071) zp        (1307)     6101 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/rest/attach_dids_to_dids.doctree
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/doctrees/usecases/
--rw-r--r--   0 barisits (51071) zp        (1307)     4822 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/add_account_identity.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4818 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/add_metadata_dataset.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4785 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/add_metadata_file.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5249 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/add_scope_to_account.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     8508 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/add_subscription.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    12024 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/authentication.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4960 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/consistency_file_between_storage_and_rucio.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5038 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/delete_file_replica_from_storage.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4927 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/detect_site_reach_watermark.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5230 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4988 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/download_all_files_from_a_given_list_of_files_from_rucio.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5030 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/download_all_files_in_a_dataset_from_rucio.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4835 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/download_files_from_rucio.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4400 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/obsolete_dataset.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5231 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/register_account.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5081 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/register_file_already_on_storage_system.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4524 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/register_transfer_request_file_fts.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4380 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/remove_replication_rules_from_file.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5772 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/reupload_after_failure.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     7617 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/search.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     3221 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/select_unwanted_files_for_deletion.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4412 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/set_replication_rule_to_file.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5464 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/upload_file_with_replication_rule.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     7457 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/usecase_upload_file_into_rucio.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5107 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases/where_are_the_replicas_for_a_file.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     7150 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/Acronyms_and_Abbreviations.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     2393 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/doctrees/Architecture.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    21792 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/Comparison_matrix.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    81561 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/REST_Account.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     8685 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/REST_Intro.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    28088 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/REST_authentication.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    90687 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/REST_did.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     8194 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/REST_identity.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     9921 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/REST_lock.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    19528 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/REST_meta.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     7204 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/REST_redirect.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    43167 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/REST_replica.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    93418 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/REST_rse.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    33047 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/REST_rule.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    14549 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/REST_scope.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    31270 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/REST_subscription.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     8088 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/doctrees/Rucio_Project_Meeting.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    78224 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/account.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    21746 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/accountlimit.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)   196168 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/api_curl_examples.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    27111 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/atlas_integration_testbed.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     2054 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/authentication_and_identity.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    27974 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/cli_admin_examples.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    21844 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/doctrees/cli_examples.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     8060 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/client_examples.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)   116795 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/client_howto.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    39959 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/doctrees/client_tutorial.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)   155605 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/core_constants.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    21418 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/developing.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    18604 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/development_guidelines.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)   153643 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/doctrees/did.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)   452979 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/environment.pickle
--rw-r--r--   0 barisits (51071) zp        (1307)   224246 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/exception.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    37099 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/identity.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    18065 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/index.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    15084 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/installing_atlas_clients.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    11551 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/installing_clients.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    12786 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/installing_server.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    19939 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/lock.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    39479 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/meta-data.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     7248 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/naming_convention_db.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     3506 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Accounting_and_quota.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     2773 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Architecture.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     9766 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Data_Deletion.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     3278 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Database_Schema.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     3459 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Deployment.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     6135 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Exception_Handling.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    17155 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_File_Dataset_Container.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     6672 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Meta-data_attributes.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     3043 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Notifications.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     2956 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Permission_model.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     9183 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Replica_management.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     6869 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Rucio_Storage_Element.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)   117157 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Rucio_Storage_Element_Manager.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5437 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Rucio_account.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    95260 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Rules.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     9339 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Scheduled_Transfers.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    35789 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Subscriptions.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     3214 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_Traceability_and_logging.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     3326 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/overview_flow.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     9984 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/permission.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     3498 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/replica.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    23662 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/replication_rules_examples.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    94015 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/rest.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)   183082 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/rse.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     7070 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/rucio_cli.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     5185 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/rucio_clients.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    41739 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/rule.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)     4903 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/rules_workflow.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    25243 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/doctrees/scope.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    40983 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/setup.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    48626 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/subscription.doctree
--rw-r--r--   0 barisits (51071) zp        (1307)    28243 2016-11-25 15:03:17.000000 rucio-1.9.5/doc/build/doctrees/usecases.doctree
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/_images/
--rw-r--r--   0 barisits (51071) zp        (1307)    71679 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_images/RSE_overview.png
--rw-r--r--   0 barisits (51071) zp        (1307)    45789 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_images/RSE_sequence_instantiation.png
--rw-r--r--   0 barisits (51071) zp        (1307)    32727 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_images/RSE_sequence_usage.png
--rw-r--r--   0 barisits (51071) zp        (1307)    56522 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_images/accounts.png
--rw-r--r--   0 barisits (51071) zp        (1307)   136638 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_images/architecture.png
--rw-r--r--   0 barisits (51071) zp        (1307)    82950 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_images/deployment.png
--rw-r--r--   0 barisits (51071) zp        (1307)   163115 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_images/exception_handling.png
--rw-r--r--   0 barisits (51071) zp        (1307)    45282 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_images/rucio-get.png
--rw-r--r--   0 barisits (51071) zp        (1307)    73288 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_images/rucio-put.png
--rw-r--r--   0 barisits (51071) zp        (1307)    55513 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_images/rucio-register.png
--rw-r--r--   0 barisits (51071) zp        (1307)   230376 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_images/rucio_schema.png
--rw-r--r--   0 barisits (51071) zp        (1307)    26628 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_images/scheduled_transfers.png
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/_modules/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/_modules/rucio/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/_modules/rucio/api/
--rw-r--r--   0 barisits (51071) zp        (1307)    16466 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/rucio/api/identity.html
--rw-r--r--   0 barisits (51071) zp        (1307)     6844 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/rucio/api/permission.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/_modules/rucio/client/
--rw-r--r--   0 barisits (51071) zp        (1307)    59303 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/rucio/client/accountclient.html
--rw-r--r--   0 barisits (51071) zp        (1307)    14938 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/rucio/client/accountlimitclient.html
--rw-r--r--   0 barisits (51071) zp        (1307)    93774 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/rucio/client/didclient.html
--rw-r--r--   0 barisits (51071) zp        (1307)    14712 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/rucio/client/lockclient.html
--rw-r--r--   0 barisits (51071) zp        (1307)    23765 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/rucio/client/metaclient.html
--rw-r--r--   0 barisits (51071) zp        (1307)    77886 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/rucio/client/rseclient.html
--rw-r--r--   0 barisits (51071) zp        (1307)    29268 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/rucio/client/ruleclient.html
--rw-r--r--   0 barisits (51071) zp        (1307)    17486 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/rucio/client/scopeclient.html
--rw-r--r--   0 barisits (51071) zp        (1307)    29268 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/rucio/client/subscriptionclient.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/_modules/rucio/common/
--rw-r--r--   0 barisits (51071) zp        (1307)   100322 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/rucio/common/exception.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/_modules/rucio/db/
--rw-r--r--   0 barisits (51071) zp        (1307)    25179 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/rucio/db/constants.html
--rw-r--r--   0 barisits (51071) zp        (1307)    20480 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/rucio/db/enum.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/_modules/rucio/rse/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/_modules/rucio/rse/protocols/
--rw-r--r--   0 barisits (51071) zp        (1307)    51488 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/rucio/rse/protocols/protocol.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/_modules/rucio/web/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/_modules/rucio/web/rest/
--rw-r--r--   0 barisits (51071) zp        (1307)    11578 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/rucio/web/rest/ping.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5307 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_modules/index.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/_sources/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/_sources/man/
--rw-r--r--   0 barisits (51071) zp        (1307)      770 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/man/rucio-admin.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1744 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/man/rucio.txt
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/_sources/rest/
--rw-r--r--   0 barisits (51071) zp        (1307)      350 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/rest/attach_dids_to_dids.txt
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/_sources/usecases/
--rw-r--r--   0 barisits (51071) zp        (1307)      783 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/add_account_identity.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      708 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/add_metadata_dataset.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      691 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/add_metadata_file.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      655 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/add_scope_to_account.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1470 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/add_subscription.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1677 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/authentication.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      804 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/consistency_file_between_storage_and_rucio.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      902 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/delete_file_replica_from_storage.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      795 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/detect_site_reach_watermark.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      940 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      886 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/download_all_files_from_a_given_list_of_files_from_rucio.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      900 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/download_all_files_in_a_dataset_from_rucio.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      794 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/download_files_from_rucio.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      564 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/obsolete_dataset.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      652 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/register_account.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      916 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/register_file_already_on_storage_system.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      646 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/register_transfer_request_file_fts.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      563 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/remove_replication_rules_from_file.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1270 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/reupload_after_failure.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1102 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/search.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      409 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/select_unwanted_files_for_deletion.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      590 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/set_replication_rule_to_file.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      852 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/upload_file_with_replication_rule.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1106 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/usecase_upload_file_into_rucio.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      633 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases/where_are_the_replicas_for_a_file.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      325 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/Acronyms_and_Abbreviations.txt
--rw-r--r--   0 barisits (51071) zp        (1307)       39 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/Architecture.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2067 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/Comparison_matrix.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     7173 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/REST_Account.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1586 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/REST_Intro.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2439 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/REST_authentication.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     7945 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/REST_did.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      611 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/REST_identity.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      637 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/REST_lock.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1444 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/REST_meta.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      349 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/REST_redirect.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     3702 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/REST_replica.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     7502 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/REST_rse.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2509 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/REST_rule.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1034 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/REST_scope.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2512 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/REST_subscription.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      662 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/Rucio_Project_Meeting.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      163 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/account.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      184 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/accountlimit.txt
--rw-r--r--   0 barisits (51071) zp        (1307)    16748 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/api_curl_examples.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2265 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/atlas_integration_testbed.txt
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/authentication_and_identity.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     4204 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/cli_admin_examples.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     4565 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/cli_examples.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1010 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/client_examples.txt
--rw-r--r--   0 barisits (51071) zp        (1307)    24065 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/client_howto.txt
--rw-r--r--   0 barisits (51071) zp        (1307)    11591 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/client_tutorial.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      138 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/core_constants.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     4981 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/developing.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     3281 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/development_guidelines.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      180 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/did.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      165 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/exception.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      162 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/identity.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2917 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/index.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2167 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/installing_atlas_clients.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1601 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/installing_clients.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1693 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/installing_server.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      152 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/lock.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      162 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/meta-data.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1180 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/naming_convention_db.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      475 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Accounting_and_quota.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      157 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Architecture.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1905 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Data_Deletion.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      311 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Database_Schema.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      442 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Deployment.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1514 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Exception_Handling.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     3882 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_File_Dataset_Container.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      894 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Meta-data_attributes.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      292 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Notifications.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      251 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Permission_model.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1911 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Replica_management.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1652 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Rucio_Storage_Element.txt
--rw-r--r--   0 barisits (51071) zp        (1307)    27901 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Rucio_Storage_Element_Manager.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1142 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Rucio_account.txt
--rw-r--r--   0 barisits (51071) zp        (1307)    23147 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Rules.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2701 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Scheduled_Transfers.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     4241 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Subscriptions.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      382 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_Traceability_and_logging.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      347 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/overview_flow.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      169 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/permission.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      155 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/replica.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     3376 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/replication_rules_examples.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     7948 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/rest.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      453 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/rse.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      717 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/rucio_cli.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      814 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/rucio_clients.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      183 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/rule.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     1414 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/rules_workflow.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      158 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/scope.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     6529 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/setup.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      190 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/subscription.txt
--rw-r--r--   0 barisits (51071) zp        (1307)     2438 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_sources/usecases.txt
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/_static/
--rw-r--r--   0 barisits (51071) zp        (1307)      673 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/ajax-loader.gif
--rw-r--r--   0 barisits (51071) zp        (1307)     8270 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/basic.css
--rw-r--r--   0 barisits (51071) zp        (1307)     4125 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/classic.css
--rw-r--r--   0 barisits (51071) zp        (1307)     3500 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/comment-bright.png
--rw-r--r--   0 barisits (51071) zp        (1307)     3578 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/comment-close.png
--rw-r--r--   0 barisits (51071) zp        (1307)     3445 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/comment.png
--rw-r--r--   0 barisits (51071) zp        (1307)     4041 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/default.css
--rw-r--r--   0 barisits (51071) zp        (1307)     7377 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/doctools.js
--rw-r--r--   0 barisits (51071) zp        (1307)      347 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/down-pressed.png
--rw-r--r--   0 barisits (51071) zp        (1307)      347 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/down.png
--rw-r--r--   0 barisits (51071) zp        (1307)      358 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/file.png
--rw-r--r--   0 barisits (51071) zp        (1307)   282766 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/jquery-1.11.1.js
--rw-r--r--   0 barisits (51071) zp        (1307)    95786 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/jquery.js
--rw-r--r--   0 barisits (51071) zp        (1307)      173 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/minus.png
--rw-r--r--   0 barisits (51071) zp        (1307)      173 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/plus.png
--rw-r--r--   0 barisits (51071) zp        (1307)     3991 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/pygments.css
--rw-r--r--   0 barisits (51071) zp        (1307)    19563 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/rucio_logo.png
--rw-r--r--   0 barisits (51071) zp        (1307)    17880 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/searchtools.js
--rw-r--r--   0 barisits (51071) zp        (1307)     4803 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/sidebar.js
--rw-r--r--   0 barisits (51071) zp        (1307)    35168 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/underscore-1.3.1.js
--rw-r--r--   0 barisits (51071) zp        (1307)    12140 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/underscore.js
--rw-r--r--   0 barisits (51071) zp        (1307)      345 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/up-pressed.png
--rw-r--r--   0 barisits (51071) zp        (1307)      345 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/up.png
--rw-r--r--   0 barisits (51071) zp        (1307)    25350 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/_static/websupport.js
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/man/
--rw-r--r--   0 barisits (51071) zp        (1307)     7794 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/man/rucio-admin.html
--rw-r--r--   0 barisits (51071) zp        (1307)     9052 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/man/rucio.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/rest/
--rw-r--r--   0 barisits (51071) zp        (1307)     5795 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/rest/attach_dids_to_dids.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/build/html/usecases/
--rw-r--r--   0 barisits (51071) zp        (1307)     4477 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/add_account_identity.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4558 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/add_metadata_dataset.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4543 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/add_metadata_file.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4538 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/add_scope_to_account.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4872 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/add_subscription.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5938 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/authentication.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4716 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/consistency_file_between_storage_and_rucio.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4557 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/delete_file_replica_from_storage.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4701 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/detect_site_reach_watermark.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4745 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4665 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/download_all_files_from_a_given_list_of_files_from_rucio.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4595 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/download_all_files_in_a_dataset_from_rucio.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4510 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/download_files_from_rucio.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4433 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/obsolete_dataset.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4551 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/register_account.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4548 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/register_file_already_on_storage_system.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4567 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/register_transfer_request_file_fts.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4523 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/remove_replication_rules_from_file.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4531 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/reupload_after_failure.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4876 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/search.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4523 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/select_unwanted_files_for_deletion.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4549 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/set_replication_rule_to_file.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4671 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/upload_file_with_replication_rule.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5164 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/usecase_upload_file_into_rucio.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4518 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/usecases/where_are_the_replicas_for_a_file.html
--rw-r--r--   0 barisits (51071) zp        (1307)      230 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/.buildinfo
--rw-r--r--   0 barisits (51071) zp        (1307)     5302 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/Acronyms_and_Abbreviations.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4352 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/Architecture.html
--rw-r--r--   0 barisits (51071) zp        (1307)     6632 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/Comparison_matrix.html
--rw-r--r--   0 barisits (51071) zp        (1307)    33965 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/REST_Account.html
--rw-r--r--   0 barisits (51071) zp        (1307)     8155 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/REST_Intro.html
--rw-r--r--   0 barisits (51071) zp        (1307)    13611 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/REST_authentication.html
--rw-r--r--   0 barisits (51071) zp        (1307)    36870 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/REST_did.html
--rw-r--r--   0 barisits (51071) zp        (1307)     7178 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/REST_identity.html
--rw-r--r--   0 barisits (51071) zp        (1307)     8464 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/REST_lock.html
--rw-r--r--   0 barisits (51071) zp        (1307)    11196 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/REST_meta.html
--rw-r--r--   0 barisits (51071) zp        (1307)     6873 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/REST_redirect.html
--rw-r--r--   0 barisits (51071) zp        (1307)    19743 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/REST_replica.html
--rw-r--r--   0 barisits (51071) zp        (1307)    36294 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/REST_rse.html
--rw-r--r--   0 barisits (51071) zp        (1307)    15403 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/REST_rule.html
--rw-r--r--   0 barisits (51071) zp        (1307)     9564 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/REST_scope.html
--rw-r--r--   0 barisits (51071) zp        (1307)    15806 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/REST_subscription.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5982 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/Rucio_Project_Meeting.html
--rw-r--r--   0 barisits (51071) zp        (1307)    24371 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/account.html
--rw-r--r--   0 barisits (51071) zp        (1307)     9490 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/accountlimit.html
--rw-r--r--   0 barisits (51071) zp        (1307)    49271 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/api_curl_examples.html
--rw-r--r--   0 barisits (51071) zp        (1307)     8847 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/atlas_integration_testbed.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4218 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/authentication_and_identity.html
--rw-r--r--   0 barisits (51071) zp        (1307)    20697 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/cli_admin_examples.html
--rw-r--r--   0 barisits (51071) zp        (1307)    16629 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/cli_examples.html
--rw-r--r--   0 barisits (51071) zp        (1307)     7763 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/client_examples.html
--rw-r--r--   0 barisits (51071) zp        (1307)    51571 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/client_howto.html
--rw-r--r--   0 barisits (51071) zp        (1307)    22174 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/client_tutorial.html
--rw-r--r--   0 barisits (51071) zp        (1307)    38831 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/core_constants.html
--rw-r--r--   0 barisits (51071) zp        (1307)    13195 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/developing.html
--rw-r--r--   0 barisits (51071) zp        (1307)    11262 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/development_guidelines.html
--rw-r--r--   0 barisits (51071) zp        (1307)    42116 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/did.html
--rw-r--r--   0 barisits (51071) zp        (1307)    64292 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/exception.html
--rw-r--r--   0 barisits (51071) zp        (1307)    54351 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/genindex.html
--rw-r--r--   0 barisits (51071) zp        (1307)    22008 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/http-routingtable.html
--rw-r--r--   0 barisits (51071) zp        (1307)    13231 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/identity.html
--rw-r--r--   0 barisits (51071) zp        (1307)    15245 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/index.html
--rw-r--r--   0 barisits (51071) zp        (1307)    10693 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/installing_atlas_clients.html
--rw-r--r--   0 barisits (51071) zp        (1307)     9658 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/installing_clients.html
--rw-r--r--   0 barisits (51071) zp        (1307)     8756 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/installing_server.html
--rw-r--r--   0 barisits (51071) zp        (1307)     9333 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/lock.html
--rw-r--r--   0 barisits (51071) zp        (1307)    13990 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/meta-data.html
--rw-r--r--   0 barisits (51071) zp        (1307)     8368 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/naming_convention_db.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4611 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/objects.inv
--rw-r--r--   0 barisits (51071) zp        (1307)     5892 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_Accounting_and_quota.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5729 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_Architecture.html
--rw-r--r--   0 barisits (51071) zp        (1307)     7965 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_Data_Deletion.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5828 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_Database_Schema.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5590 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_Deployment.html
--rw-r--r--   0 barisits (51071) zp        (1307)     7307 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_Exception_Handling.html
--rw-r--r--   0 barisits (51071) zp        (1307)    11254 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_File_Dataset_Container.html
--rw-r--r--   0 barisits (51071) zp        (1307)     6831 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_Meta-data_attributes.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5732 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_Notifications.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5700 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_Permission_model.html
--rw-r--r--   0 barisits (51071) zp        (1307)     8062 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_Replica_management.html
--rw-r--r--   0 barisits (51071) zp        (1307)     7173 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_Rucio_Storage_Element.html
--rw-r--r--   0 barisits (51071) zp        (1307)    46544 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_Rucio_Storage_Element_Manager.html
--rw-r--r--   0 barisits (51071) zp        (1307)     6701 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_Rucio_account.html
--rw-r--r--   0 barisits (51071) zp        (1307)    36223 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/overview_Rules.html
--rw-r--r--   0 barisits (51071) zp        (1307)     8997 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_Scheduled_Transfers.html
--rw-r--r--   0 barisits (51071) zp        (1307)    14110 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_Subscriptions.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4733 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_Traceability_and_logging.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5951 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/overview_flow.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5808 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/permission.html
--rw-r--r--   0 barisits (51071) zp        (1307)     7644 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/py-modindex.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5259 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/replica.html
--rw-r--r--   0 barisits (51071) zp        (1307)    11051 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/replication_rules_examples.html
--rw-r--r--   0 barisits (51071) zp        (1307)    22089 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/rest.html
--rw-r--r--   0 barisits (51071) zp        (1307)    47247 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/rse.html
--rw-r--r--   0 barisits (51071) zp        (1307)     6001 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/rucio_cli.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5824 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/rucio_clients.html
--rw-r--r--   0 barisits (51071) zp        (1307)    13860 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/rule.html
--rw-r--r--   0 barisits (51071) zp        (1307)     6962 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/rules_workflow.html
--rw-r--r--   0 barisits (51071) zp        (1307)    10313 2016-11-25 15:03:15.000000 rucio-1.9.5/doc/build/html/scope.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4453 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/search.html
--rw-r--r--   0 barisits (51071) zp        (1307)    57160 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/searchindex.js
--rw-r--r--   0 barisits (51071) zp        (1307)    17589 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/setup.html
--rw-r--r--   0 barisits (51071) zp        (1307)    14675 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/subscription.html
--rw-r--r--   0 barisits (51071) zp        (1307)    10373 2016-11-25 15:03:16.000000 rucio-1.9.5/doc/build/html/usecases.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/design/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/design/RSE/
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1996 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/design/RSE/meeting-2012-02-23.org
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/design/erd/
--rwxr-xr-x   0 barisits (51071) zp        (1307)    55942 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/design/erd/ERD.graffle
--rwxr-xr-x   0 barisits (51071) zp        (1307)    72676 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/design/erd/ERD.pdf
--rwxr-xr-x   0 barisits (51071) zp        (1307)    60363 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/design/rucio_schema.pdf
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/source/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/source/_static/
--rwxr-xr-x   0 barisits (51071) zp        (1307)     8270 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/_static/basic.css
--rw-r--r--   0 barisits (51071) zp        (1307)     4179 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/_static/classic.css
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4041 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/_static/default.css
--rwxr-xr-x   0 barisits (51071) zp        (1307)    19563 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/_static/rucio_logo.png
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/source/_templates/
--rwxr-xr-x   0 barisits (51071) zp        (1307)      777 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/_templates/layout.html
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/source/cli_examples/
--rw-r--r--   0 barisits (51071) zp        (1307)       14 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/cli_examples/ping.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)       12 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/cli_examples/ping.sh
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/source/curl_examples/
--rw-r--r--   0 barisits (51071) zp        (1307)      235 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/del_account.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      312 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/del_account.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/del_location.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      313 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/del_location.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      404 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_account.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      309 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_account.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      673 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_account_whoami.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      314 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_account_whoami.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      253 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_accounts.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      305 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_accounts.sh
--rw-r--r--   0 barisits (51071) zp        (1307)       29 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_api.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)       34 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_api.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_auth_gss.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      129 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_auth_gss.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_auth_userpass.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      168 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_auth_userpass.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      304 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_auth_validate.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      334 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_auth_validate.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_auth_x509.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      139 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_auth_x509.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_location.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      310 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_location.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      239 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_locations.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      306 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_locations.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      356 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_scopes.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      309 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/get_scopes.sh
--rwxr-xr-x   0 barisits (51071) zp        (1307)      380 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/post_account.sh
--rwxr-xr-x   0 barisits (51071) zp        (1307)      332 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/post_location.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      370 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/post_location_rse.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      257 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/put_account.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      331 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/put_account.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/put_location.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      309 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/put_location.sh
--rw-r--r--   0 barisits (51071) zp        (1307)      257 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/put_scope.out
--rwxr-xr-x   0 barisits (51071) zp        (1307)      314 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/curl_examples/put_scope.sh
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/source/example_outputs/
--rw-r--r--   0 barisits (51071) zp        (1307)     3643 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/example_outputs/failure-rucio.tests.test_curl.TestCurlRucio.test_get_accounts_whoami.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      164 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/example_outputs/success-rucio.tests.test_bin_rucio.TestBinRucio.test_add_account.txt
--rw-r--r--   0 barisits (51071) zp        (1307)       43 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/example_outputs/success-rucio.tests.test_bin_rucio.TestBinRucio.test_rucio_ping.txt
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/example_outputs/success-rucio.tests.test_bin_rucio.TestBinRucio.test_rucio_version.txt
--rw-r--r--   0 barisits (51071) zp        (1307)       46 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/example_outputs/success-rucio.tests.test_clients.TestRucioClients.test_ping.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      804 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_accounts_whoami.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      429 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_GSS.txt
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_proxy.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      466 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_userpass.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      454 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_validate.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      442 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_x509.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      454 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_x509_proxy.txt
--rw-r--r--   0 barisits (51071) zp        (1307)       84 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_ping.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      440 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_post_account.txt
--rw-r--r--   0 barisits (51071) zp        (1307)      398 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_post_rse.txt
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/source/images/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/source/images/deployment.graffle/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/source/images/deployment.graffle/QuickLook/
--rw-r--r--   0 barisits (51071) zp        (1307)    52757 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/deployment.graffle/QuickLook/Preview.pdf
--rw-r--r--   0 barisits (51071) zp        (1307)   124440 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/deployment.graffle/QuickLook/Thumbnail.tiff
--rw-r--r--   0 barisits (51071) zp        (1307)     3172 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/deployment.graffle/data.plist
--rw-r--r--   0 barisits (51071) zp        (1307)    26954 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/deployment.graffle/image2.tiff
--rw-r--r--   0 barisits (51071) zp        (1307)    10020 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/deployment.graffle/image3.tiff
--rwxr-xr-x   0 barisits (51071) zp        (1307)    71679 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/RSE_overview.png
--rwxr-xr-x   0 barisits (51071) zp        (1307)    45789 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/RSE_sequence_instantiation.png
--rwxr-xr-x   0 barisits (51071) zp        (1307)    32727 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/RSE_sequence_usage.png
--rwxr-xr-x   0 barisits (51071) zp        (1307)    56522 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/accounts.png
--rw-r--r--   0 barisits (51071) zp        (1307)   397841 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/architecture.graffle
--rw-r--r--   0 barisits (51071) zp        (1307)   136638 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/architecture.png
--rw-r--r--   0 barisits (51071) zp        (1307)    82950 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/deployment.png
--rwxr-xr-x   0 barisits (51071) zp        (1307)    70361 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/exception_handling.graffle
--rwxr-xr-x   0 barisits (51071) zp        (1307)   163115 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/exception_handling.png
--rwxr-xr-x   0 barisits (51071) zp        (1307)   127009 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/highLevelRoadmap.graffle
--rwxr-xr-x   0 barisits (51071) zp        (1307)   205501 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/rucio-get.graffle
--rwxr-xr-x   0 barisits (51071) zp        (1307)    45282 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/rucio-get.png
--rwxr-xr-x   0 barisits (51071) zp        (1307)   298526 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/rucio-put.graffle
--rwxr-xr-x   0 barisits (51071) zp        (1307)    73288 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/rucio-put.png
--rwxr-xr-x   0 barisits (51071) zp        (1307)   232239 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/rucio-register.graffle
--rwxr-xr-x   0 barisits (51071) zp        (1307)    55513 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/rucio-register.png
--rw-r--r--   0 barisits (51071) zp        (1307)    62543 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/rucio_schema.gml
--rwxr-xr-x   0 barisits (51071) zp        (1307)   226250 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/images/rucio_schema.pdf
--rwxr-xr-x   0 barisits (51071) zp        (1307)   230376 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/images/rucio_schema.png
--rw-r--r--   0 barisits (51071) zp        (1307)     2485 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/images/scheduled_transfers.dia
--rw-r--r--   0 barisits (51071) zp        (1307)    26628 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/images/scheduled_transfers.png
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/source/man/
--rwxr-xr-x   0 barisits (51071) zp        (1307)      770 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/man/rucio-admin.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1744 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/man/rucio.rst
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/source/rest/
--rw-r--r--   0 barisits (51071) zp        (1307)      350 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/rest/attach_dids_to_dids.rst
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/doc/source/usecases/
--rw-r--r--   0 barisits (51071) zp        (1307)      783 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/add_account_identity.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      708 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/add_metadata_dataset.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      691 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/add_metadata_file.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      655 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/add_scope_to_account.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1470 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/add_subscription.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1677 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/authentication.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      804 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/consistency_file_between_storage_and_rucio.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      902 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/delete_file_replica_from_storage.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      795 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/detect_site_reach_watermark.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      940 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      886 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/download_all_files_from_a_given_list_of_files_from_rucio.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      900 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/download_all_files_in_a_dataset_from_rucio.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      794 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/download_files_from_rucio.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      564 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/obsolete_dataset.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      652 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/register_account.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      916 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/register_file_already_on_storage_system.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      646 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/register_transfer_request_file_fts.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      563 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/remove_replication_rules_from_file.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1270 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/reupload_after_failure.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1102 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/search.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      409 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/select_unwanted_files_for_deletion.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      590 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/set_replication_rule_to_file.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      852 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/upload_file_with_replication_rule.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1106 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/usecase_upload_file_into_rucio.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      633 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases/where_are_the_replicas_for_a_file.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      325 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/Acronyms_and_Abbreviations.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)       39 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/Architecture.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2067 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/Comparison_matrix.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     7173 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/REST_Account.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1586 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/REST_Intro.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     2439 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/REST_authentication.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     7945 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/REST_did.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      611 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/REST_identity.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      637 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/REST_lock.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1444 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/REST_meta.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      349 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/REST_redirect.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     3702 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/REST_replica.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     7502 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/REST_rse.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     2509 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/REST_rule.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1034 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/REST_scope.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     2512 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/REST_subscription.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     6000 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/RSE_Expressions.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      662 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/Rucio_Project_Meeting.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      163 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/account.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      184 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/accountlimit.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)    19866 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/accounts.pdf
--rwxr-xr-x   0 barisits (51071) zp        (1307)    56522 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/accounts.png
--rw-r--r--   0 barisits (51071) zp        (1307)    16748 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/api_curl_examples.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     2265 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/atlas_integration_testbed.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/authentication_and_identity.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     4204 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/cli_admin_examples.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     4565 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/cli_examples.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1010 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/client_examples.rst
--rw-r--r--   0 barisits (51071) zp        (1307)    11591 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/client_tutorial.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     7556 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/conf.py
--rw-r--r--   0 barisits (51071) zp        (1307)      138 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/core_constants.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     7860 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/developing.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3281 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/development_guidelines.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      180 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/did.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      165 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/exception.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      162 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/source/identity.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3274 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/index.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     2167 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/installing_atlas_clients.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1601 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/installing_clients.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1693 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/installing_server.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      152 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/lock.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      162 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/meta-data.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1180 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/naming_convention_db.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      475 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Accounting_and_quota.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      157 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Architecture.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1905 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Data_Deletion.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      311 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Database_Schema.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      442 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Deployment.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1514 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Exception_Handling.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3882 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_File_Dataset_Container.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      894 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Meta-data_attributes.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      292 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Notifications.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      251 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Permission_model.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1911 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Replica_management.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1652 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Rucio_Storage_Element.rst
--rw-r--r--   0 barisits (51071) zp        (1307)    27901 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Rucio_Storage_Element_Manager.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1142 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Rucio_account.rst
--rw-r--r--   0 barisits (51071) zp        (1307)    23147 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Rules.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     2701 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Scheduled_Transfers.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4241 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Subscriptions.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      382 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_Traceability_and_logging.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      347 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/overview_flow.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      169 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/permission.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      155 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/replica.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1509 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/replication_rules_examples.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     7948 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/rest.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      453 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/rse.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      717 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/rucio_cli.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      814 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/rucio_clients.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      183 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/rule.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     1414 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/rules_workflow.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      158 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/scope.rst
--rw-r--r--   0 barisits (51071) zp        (1307)      189 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/service_avaibility.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)      190 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/subscription.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2438 2016-11-25 15:17:14.000000 rucio-1.9.5/doc/source/usecases.rst
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4590 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/Makefile
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4513 2016-11-25 15:17:13.000000 rucio-1.9.5/doc/make.bat
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/etc/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/etc/mail_templates/
--rw-r--r--   0 barisits (51071) zp        (1307)     1078 2016-11-28 16:40:28.000000 rucio-1.9.5/etc/mail_templates/rule_approval_request.tmpl
--rw-r--r--   0 barisits (51071) zp        (1307)      105 2016-11-28 16:40:28.000000 rucio-1.9.5/etc/mail_templates/rule_approved_admin.tmpl
--rw-r--r--   0 barisits (51071) zp        (1307)      498 2016-11-28 16:40:28.000000 rucio-1.9.5/etc/mail_templates/rule_approved_user.tmpl
--rw-r--r--   0 barisits (51071) zp        (1307)      103 2016-11-28 16:40:28.000000 rucio-1.9.5/etc/mail_templates/rule_denied_admin.tmpl
--rw-r--r--   0 barisits (51071) zp        (1307)      460 2016-11-28 16:40:28.000000 rucio-1.9.5/etc/mail_templates/rule_denied_user.tmpl
--rw-r--r--   0 barisits (51071) zp        (1307)      545 2016-11-28 16:40:28.000000 rucio-1.9.5/etc/mail_templates/rule_ok_notification.tmpl
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/etc/schemas/
--rw-r--r--   0 barisits (51071) zp        (1307)       97 2016-11-25 15:17:14.000000 rucio-1.9.5/etc/schemas/account.json
--rw-r--r--   0 barisits (51071) zp        (1307)       82 2016-11-25 15:17:14.000000 rucio-1.9.5/etc/schemas/account_type.json
--rw-r--r--   0 barisits (51071) zp        (1307)       82 2016-11-25 15:17:14.000000 rucio-1.9.5/etc/schemas/did_type.json
--rw-r--r--   0 barisits (51071) zp        (1307)      112 2016-11-25 15:17:14.000000 rucio-1.9.5/etc/schemas/mail.json
--rw-r--r--   0 barisits (51071) zp        (1307)      105 2016-11-25 15:17:14.000000 rucio-1.9.5/etc/schemas/rse.json
--rw-r--r--   0 barisits (51071) zp        (1307)      105 2016-11-25 15:17:14.000000 rucio-1.9.5/etc/schemas/scope.json
--rw-r--r--   0 barisits (51071) zp        (1307)      559 2016-11-25 15:17:14.000000 rucio-1.9.5/etc/schemas/sub_filter.json
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/etc/web/
--rw-r--r--   0 barisits (51071) zp        (1307)     2551 2016-11-25 15:17:14.000000 rucio-1.9.5/etc/web/httpd-rucio-443-py26-slc6.conf.template
--rw-r--r--   0 barisits (51071) zp        (1307)     2557 2017-01-20 08:30:56.000000 rucio-1.9.5/etc/web/httpd-rucio-443-py27-cc7.conf.template
--rw-r--r--   0 barisits (51071) zp        (1307)     1690 2016-11-25 15:17:14.000000 rucio-1.9.5/etc/web/httpd-rucio-443-py27-debian.conf.template
--rw-r--r--   0 barisits (51071) zp        (1307)     2055 2016-11-25 15:17:14.000000 rucio-1.9.5/etc/web/httpd-rucio-443-py27-osx.conf.template
--rw-r--r--   0 barisits (51071) zp        (1307)     1665 2016-11-25 15:17:14.000000 rucio-1.9.5/etc/web/httpd-rucio-443-py27-ubuntu.conf.template
--rw-r--r--   0 barisits (51071) zp        (1307)     1358 2016-11-25 15:17:14.000000 rucio-1.9.5/etc/alembic.ini.template
--rw-r--r--   0 barisits (51071) zp        (1307)      807 2016-11-25 15:17:14.000000 rucio-1.9.5/etc/ldap.cfg.template
--rwxr-xr-x   0 barisits (51071) zp        (1307)      543 2016-11-25 15:17:14.000000 rucio-1.9.5/etc/rse-accounts.cfg.template
--rw-r--r--   0 barisits (51071) zp        (1307)      570 2016-11-25 15:17:14.000000 rucio-1.9.5/etc/rucio.cfg.atlas.client.template
--rwxr-xr-x   0 barisits (51071) zp        (1307)     5165 2016-11-28 16:40:28.000000 rucio-1.9.5/etc/rucio.cfg.template
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/api/
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/api/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     5257 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/api/account.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4277 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/api/account_limit.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3541 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/api/authentication.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1839 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/api/availability.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6358 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/api/config.py
--rw-r--r--   0 barisits (51071) zp        (1307)    11944 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/api/did.py
--rw-r--r--   0 barisits (51071) zp        (1307)      896 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/api/heartbeat.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3812 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/api/identity.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1269 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/api/lock.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2121 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/api/meta.py
--rw-r--r--   0 barisits (51071) zp        (1307)      983 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/api/permission.py
--rw-r--r--   0 barisits (51071) zp        (1307)     7451 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/api/replica.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4641 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/api/request.py
--rw-r--r--   0 barisits (51071) zp        (1307)    10182 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/api/rse.py
--rw-r--r--   0 barisits (51071) zp        (1307)     8596 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/api/rule.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1532 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/api/scope.py
--rw-r--r--   0 barisits (51071) zp        (1307)     7330 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/api/subscription.py
--rw-r--r--   0 barisits (51071) zp        (1307)      816 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/api/temporary_did.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/client/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/client/cli/
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/cli/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)      469 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/cli/download.py
--rw-r--r--   0 barisits (51071) zp        (1307)      581 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/cli/upload.py
--rw-r--r--   0 barisits (51071) zp        (1307)      325 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)    12651 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/accountclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2763 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/accountlimitclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)    21749 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/client/baseclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2381 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/client.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3523 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/configclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)    23023 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/client/didclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)    91449 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/client/dq2client.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1716 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/fileclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2594 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/lockclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4717 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/metaclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3915 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/objectstoreclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1356 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/pingclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9888 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/client/replicaclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)    19164 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/rseclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9768 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/client/ruleclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3292 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/scopeclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     7475 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/subscriptionclient.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4326 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/client/uploadclient.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/common/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/common/dumper/
--rw-r--r--   0 barisits (51071) zp        (1307)    10166 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/common/dumper/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)    15801 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/common/dumper/consistency.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9062 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/common/dumper/data_models.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1637 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/common/dumper/path_parsing.py
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/common/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1208 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/common/client.py
--rw-r--r--   0 barisits (51071) zp        (1307)     7763 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/common/closeness_sorter.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3883 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/common/config.py
--rw-r--r--   0 barisits (51071) zp        (1307)      938 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/common/constants.py
--rw-r--r--   0 barisits (51071) zp        (1307)      439 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/common/constraints.py
--rw-r--r--   0 barisits (51071) zp        (1307)    19606 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/common/exception.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3288 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/common/log.py
--rw-r--r--   0 barisits (51071) zp        (1307)    14068 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/common/objectstore.py
--rw-r--r--   0 barisits (51071) zp        (1307)     8188 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/common/policy.py
--rw-r--r--   0 barisits (51071) zp        (1307)     5461 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/common/replicas_selector.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1520 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/common/rse_attributes.py
--rw-r--r--   0 barisits (51071) zp        (1307)    14030 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/common/schema.py
--rw-r--r--   0 barisits (51071) zp        (1307)    14270 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/common/utils.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/core/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/core/permission/
--rw-r--r--   0 barisits (51071) zp        (1307)      954 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/core/permission/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)    33084 2017-01-24 09:05:38.000000 rucio-1.9.5/lib/rucio/core/permission/atlas.py
--rw-r--r--   0 barisits (51071) zp        (1307)    27320 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/core/permission/generic.py
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/core/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9768 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/core/account.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6664 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/core/account_counter.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6506 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/core/account_limit.py
--rw-r--r--   0 barisits (51071) zp        (1307)     7133 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/core/authentication.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6879 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/core/config.py
--rw-r--r--   0 barisits (51071) zp        (1307)    70393 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/core/did.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6526 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/core/distance.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6533 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/core/heartbeat.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6453 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/core/identity.py
--rw-r--r--   0 barisits (51071) zp        (1307)    17559 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/core/lock.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4812 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/core/message.py
--rw-r--r--   0 barisits (51071) zp        (1307)     5715 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/core/meta.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2501 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/core/monitor.py
--rw-r--r--   0 barisits (51071) zp        (1307)     5252 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/core/naming_convention.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2621 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/core/nongrid_trace.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6092 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/core/quarantined_replica.py
--rw-r--r--   0 barisits (51071) zp        (1307)    90233 2017-01-20 09:22:58.000000 rucio-1.9.5/lib/rucio/core/replica.py
--rw-r--r--   0 barisits (51071) zp        (1307)    77757 2017-01-20 09:22:58.000000 rucio-1.9.5/lib/rucio/core/request.py
--rw-r--r--   0 barisits (51071) zp        (1307)    37244 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/core/rse.py
--rw-r--r--   0 barisits (51071) zp        (1307)     5046 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/core/rse_counter.py
--rw-r--r--   0 barisits (51071) zp        (1307)    14410 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/core/rse_expression_parser.py
--rw-r--r--   0 barisits (51071) zp        (1307)     7258 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/core/rse_selector.py
--rw-r--r--   0 barisits (51071) zp        (1307)   159902 2017-01-24 09:05:38.000000 rucio-1.9.5/lib/rucio/core/rule.py
--rw-r--r--   0 barisits (51071) zp        (1307)    71602 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/core/rule_grouping.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4386 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/core/scope.py
--rw-r--r--   0 barisits (51071) zp        (1307)    10826 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/core/subscription.py
--rw-r--r--   0 barisits (51071) zp        (1307)     7249 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/core/temporary_did.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2618 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/core/trace.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4351 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/core/volatile_replica.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/daemons/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/daemons/abacus/
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/daemons/abacus/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3549 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/daemons/abacus/account.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3337 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/daemons/abacus/rse.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/daemons/auditor/
--rw-r--r--   0 barisits (51071) zp        (1307)     4485 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/daemons/auditor/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2258 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/daemons/auditor/hdfs.py
--rw-r--r--   0 barisits (51071) zp        (1307)     7680 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/daemons/auditor/srmdumps.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/daemons/bb8/
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/bb8/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2186 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/bb8/bb8.py
--rw-r--r--   0 barisits (51071) zp        (1307)    11937 2017-01-20 09:22:58.000000 rucio-1.9.5/lib/rucio/daemons/bb8/common.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4367 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/daemons/bb8/t1_background_rebalance.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/daemons/c3po/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/daemons/c3po/algorithms/
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/algorithms/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4266 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/algorithms/simple.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4125 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/algorithms/t2_free_space.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4388 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py
--rw-r--r--   0 barisits (51071) zp        (1307)    11732 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/daemons/c3po/collectors/
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/collectors/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2533 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/collectors/agis.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1536 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/collectors/free_space.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1379 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/collectors/jedi_did.py
--rw-r--r--   0 barisits (51071) zp        (1307)      946 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/collectors/mock_did.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1800 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/collectors/network_metrics.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3435 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/collectors/workload.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/daemons/c3po/utils/
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/utils/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1066 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/utils/dataset_cache.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1100 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1361 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/utils/expiring_list.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2109 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/utils/popularity.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1458 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/utils/timeseries.py
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)    12253 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/c3po/c3po.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/daemons/cache/
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/daemons/cache/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     5201 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/cache/consumer.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/daemons/conveyor/
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/daemons/conveyor/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)    35293 2017-01-20 09:22:58.000000 rucio-1.9.5/lib/rucio/daemons/conveyor/common.py
--rw-r--r--   0 barisits (51071) zp        (1307)     7392 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/conveyor/finisher.py
--rw-r--r--   0 barisits (51071) zp        (1307)     8949 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/daemons/conveyor/poller.py
--rw-r--r--   0 barisits (51071) zp        (1307)     5004 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/daemons/conveyor/poller_latest.py
--rw-r--r--   0 barisits (51071) zp        (1307)    12691 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/conveyor/receiver.py
--rw-r--r--   0 barisits (51071) zp        (1307)    10002 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/conveyor/stager.py
--rw-r--r--   0 barisits (51071) zp        (1307)    10532 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/conveyor/submitter.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3586 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/conveyor/throttler.py
--rw-r--r--   0 barisits (51071) zp        (1307)    79138 2017-01-20 09:22:58.000000 rucio-1.9.5/lib/rucio/daemons/conveyor/utils.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/daemons/hermes/
--rw-r--r--   0 barisits (51071) zp        (1307)      304 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/daemons/hermes/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)    16283 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/hermes/hermes.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/daemons/judge/
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/daemons/judge/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6840 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/judge/cleaner.py
--rw-r--r--   0 barisits (51071) zp        (1307)     8227 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/judge/evaluator.py
--rw-r--r--   0 barisits (51071) zp        (1307)     7265 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/judge/injector.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6446 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/judge/repairer.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/daemons/mock/
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/daemons/mock/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     7146 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/daemons/mock/conveyorinjector.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/daemons/reaper/
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/reaper/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     8793 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/reaper/dark_reaper.py
--rw-r--r--   0 barisits (51071) zp        (1307)     8771 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/reaper/light_reaper.py
--rw-r--r--   0 barisits (51071) zp        (1307)    22608 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/daemons/reaper/reaper.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/daemons/tracer/
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/daemons/tracer/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)    17432 2017-01-20 09:22:58.000000 rucio-1.9.5/lib/rucio/daemons/tracer/kronos.py
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/daemons/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     8726 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/atropos.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     6006 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/necromancer.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)    22173 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/daemons/transmogrifier.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3903 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/daemons/undertaker.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/db/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/db/elasticsearch/
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/db/elasticsearch/__init__.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/db/sqla/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/
--rw-r--r--   0 barisits (51071) zp        (1307)     1198 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py
--rw-r--r--   0 barisits (51071) zp        (1307)      762 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py
--rw-r--r--   0 barisits (51071) zp        (1307)      773 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1978 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py
--rw-r--r--   0 barisits (51071) zp        (1307)      738 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1059 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1118 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py
--rw-r--r--   0 barisits (51071) zp        (1307)      799 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2224 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1385 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1049 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1254 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py
--rw-r--r--   0 barisits (51071) zp        (1307)      893 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2147 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1984 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py
--rw-r--r--   0 barisits (51071) zp        (1307)      934 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py
--rw-r--r--   0 barisits (51071) zp        (1307)      903 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py
--rw-r--r--   0 barisits (51071) zp        (1307)      983 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1565 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py
--rw-r--r--   0 barisits (51071) zp        (1307)      979 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1839 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2253 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py
--rw-r--r--   0 barisits (51071) zp        (1307)      922 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1018 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1364 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py
--rw-r--r--   0 barisits (51071) zp        (1307)      843 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1986 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1501 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1928 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py
--rw-r--r--   0 barisits (51071) zp        (1307)      954 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2160 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4355 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2560 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1233 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1063 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py
--rw-r--r--   0 barisits (51071) zp        (1307)      928 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1056 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py
--rw-r--r--   0 barisits (51071) zp        (1307)      773 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py
--rw-r--r--   0 barisits (51071) zp        (1307)      848 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1112 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2966 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py
--rw-r--r--   0 barisits (51071) zp        (1307)      934 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1772 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1255 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py
--rw-r--r--   0 barisits (51071) zp        (1307)      881 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1291 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py
--rw-r--r--   0 barisits (51071) zp        (1307)      743 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2141 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py
--rw-r--r--   0 barisits (51071) zp        (1307)      992 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py
--rw-r--r--   0 barisits (51071) zp        (1307)      823 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1713 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1045 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2776 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1502 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1254 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py
--rw-r--r--   0 barisits (51071) zp        (1307)      904 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2111 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3451 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1723 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2090 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1190 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1465 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py
--rw-r--r--   0 barisits (51071) zp        (1307)      880 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py
--rw-r--r--   0 barisits (51071) zp        (1307)      942 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3398 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py
--rw-r--r--   0 barisits (51071) zp        (1307)      975 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2606 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/env.py
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/db/sqla/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4652 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/db/sqla/constants.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3389 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/db/sqla/enum.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6109 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/db/sqla/history.py
--rw-r--r--   0 barisits (51071) zp        (1307)    60735 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/db/sqla/models.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1407 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/db/sqla/sautils.py
--rw-r--r--   0 barisits (51071) zp        (1307)    11324 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/db/sqla/session.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2907 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/db/sqla/types.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6086 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/db/sqla/util.py
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/db/__init__.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/rse/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/rse/protocols/
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/rse/protocols/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4165 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/rse/protocols/cache.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3787 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/rse/protocols/dummy.py
--rw-r--r--   0 barisits (51071) zp        (1307)    17585 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/rse/protocols/gfal.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1256 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/rse/protocols/gfalv2.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4679 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/rse/protocols/gsiftp.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2635 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/rse/protocols/http_cache.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3741 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/rse/protocols/mock.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6596 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/rse/protocols/ngarc.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6199 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/rse/protocols/posix.py
--rw-r--r--   0 barisits (51071) zp        (1307)    12783 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/rse/protocols/protocol.py
--rw-r--r--   0 barisits (51071) zp        (1307)     5035 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/rse/protocols/rfio.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9114 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/rse/protocols/s3.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9915 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/rse/protocols/s3boto.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6345 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/rse/protocols/s3es.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6723 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/rse/protocols/sftp.py
--rw-r--r--   0 barisits (51071) zp        (1307)    15403 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/rse/protocols/signeds3.py
--rw-r--r--   0 barisits (51071) zp        (1307)    13829 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/rse/protocols/srm.py
--rw-r--r--   0 barisits (51071) zp        (1307)    19999 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/rse/protocols/webdav.py
--rw-r--r--   0 barisits (51071) zp        (1307)     8153 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/rse/protocols/xrootd.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1937 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/rse/__init__.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)    25214 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/rse/rsemanager.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/tests/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/tests/daemons/
--rwxr-xr-x   0 barisits (51071) zp        (1307)    11714 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/tests/daemons/Automatix.py
--rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/daemons/__init__.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/tests/emulation/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/tests/emulation/usecases/
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/emulation/usecases/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)      969 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/emulation/usecases/auth.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1476 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/emulation/usecases/dummy.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2208 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/emulation/usecases/dummy_template.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3716 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/emulation/usecases/jdoe.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)    65781 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/emulation/usecases/panda.py
--rw-r--r--   0 barisits (51071) zp        (1307)    56221 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/emulation/usecases/panda_new.py
--rw-r--r--   0 barisits (51071) zp        (1307)    21228 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/emulation/usecases/tzero.py
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/emulation/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9327 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/emulation/emulator.py
--rw-r--r--   0 barisits (51071) zp        (1307)    15903 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/emulation/ucemulator.py
--rw-r--r--   0 barisits (51071) zp        (1307)     8610 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/emulation/ucprocess.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3278 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/emulation/worker.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/tests/functional/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/tests/functional/blocks/
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/functional/blocks/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)      577 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/functional/blocks/block1.py
--rw-r--r--   0 barisits (51071) zp        (1307)     8354 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/tests/functional/blocks/block2.py
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/functional/__init__.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     5986 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/tests/functional/run.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/tests/mock/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/tests/mock/web/
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/mock/web/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2271 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/mock/web/fts3.py
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/mock/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3707 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/tests/mock/fts3.py
--rw-r--r--   0 barisits (51071) zp        (1307)      532 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/mock/gfal2.py
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4684 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/common.py
--rw-r--r--   0 barisits (51071) zp        (1307)    22701 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/tests/rsemgr_api_test.py
--rw-r--r--   0 barisits (51071) zp        (1307)    14408 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_account.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4351 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_account_limits.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1245 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_alembic.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2723 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_auditor.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1719 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_auditor_hdfs.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2888 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_auditor_srmdumps.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2292 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_authentication.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3786 2017-01-20 09:22:58.000000 rucio-1.9.5/lib/rucio/tests/test_bb8.py
--rw-r--r--   0 barisits (51071) zp        (1307)    27965 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/tests/test_bin_rucio.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3210 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/tests/test_clients.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3120 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_config.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1200 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/tests/test_conveyor.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4563 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_counter.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6716 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/tests/test_curl.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2091 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_dataset_replicas.py
--rw-r--r--   0 barisits (51071) zp        (1307)      707 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_db.py
--rw-r--r--   0 barisits (51071) zp        (1307)    37907 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/tests/test_did.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6392 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_dumper.py
--rw-r--r--   0 barisits (51071) zp        (1307)    16150 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_dumper_consistency.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9790 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_dumper_data_model.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3145 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_dumper_path_parsing.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3362 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_heartbeat.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1657 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_hermes.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2141 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_identity.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3274 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_judge_cleaner.py
--rw-r--r--   0 barisits (51071) zp        (1307)    11109 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/tests/test_judge_evaluator.py
--rw-r--r--   0 barisits (51071) zp        (1307)     8060 2017-01-24 09:05:38.000000 rucio-1.9.5/lib/rucio/tests/test_judge_injector.py
--rw-r--r--   0 barisits (51071) zp        (1307)    16107 2016-11-28 15:43:52.000000 rucio-1.9.5/lib/rucio/tests/test_judge_repairer.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2086 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/tests/test_message.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3149 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_meta.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2532 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_meta_did.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1510 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_monitor.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2756 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_naming_convention.py
--rw-r--r--   0 barisits (51071) zp        (1307)    12265 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_objectstore.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3185 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_permission.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1286 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_ping.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1358 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/tests/test_quarantined_replica.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1307 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/tests/test_reaper.py
--rw-r--r--   0 barisits (51071) zp        (1307)     5633 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/tests/test_redirect.py
--rw-r--r--   0 barisits (51071) zp        (1307)    27875 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/tests/test_replica.py
--rw-r--r--   0 barisits (51071) zp        (1307)    78040 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/tests/test_rse.py
--rw-r--r--   0 barisits (51071) zp        (1307)    10690 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/tests/test_rse_expression_parser.py
--rw-r--r--   0 barisits (51071) zp        (1307)    13237 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_rse_protocol_gfal2.py
--rw-r--r--   0 barisits (51071) zp        (1307)     5173 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_rse_protocol_mock.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9728 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_rse_protocol_posix.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9813 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_rse_protocol_s3.py
--rw-r--r--   0 barisits (51071) zp        (1307)    11909 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/tests/test_rse_protocol_s3boto.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4845 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/tests/test_rse_protocol_s3es.py
--rw-r--r--   0 barisits (51071) zp        (1307)    10110 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_rse_protocol_sftp.py
--rw-r--r--   0 barisits (51071) zp        (1307)     9909 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_rse_protocol_signeds3.py
--rw-r--r--   0 barisits (51071) zp        (1307)    12805 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_rse_protocol_srm.py
--rw-r--r--   0 barisits (51071) zp        (1307)    11084 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_rse_protocol_webdav.py
--rw-r--r--   0 barisits (51071) zp        (1307)    10967 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_rse_protocol_xrootd.py
--rw-r--r--   0 barisits (51071) zp        (1307)     6537 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_rucio_cache.py
--rw-r--r--   0 barisits (51071) zp        (1307)     4792 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_rucio_server.py
--rw-r--r--   0 barisits (51071) zp        (1307)    51857 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/tests/test_rule.py
--rw-r--r--   0 barisits (51071) zp        (1307)    10288 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_scope.py
--rw-r--r--   0 barisits (51071) zp        (1307)    20485 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/tests/test_subscription.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2650 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/tests/test_temporary_did.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1345 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/tests/test_trace.py
--rw-r--r--   0 barisits (51071) zp        (1307)     3258 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/tests/test_undertaker.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/transfertool/
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/transfertool/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)    39426 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/transfertool/fts3.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/web/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/lib/rucio/web/rest/
--rwxr-xr-x   0 barisits (51071) zp        (1307)      346 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/web/rest/__init__.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)    21464 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/web/rest/account.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3914 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/web/rest/account_limit.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)    11929 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/web/rest/authentication.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4112 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/web/rest/common.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4332 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/web/rest/config.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)    27806 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/web/rest/did.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1402 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/web/rest/heartbeat.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4706 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/web/rest/identity.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3112 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/web/rest/lock.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4904 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/web/rest/meta.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1846 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/web/rest/nongrid_trace.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     5430 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/web/rest/objectstore.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2170 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/web/rest/ping.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)    10189 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/web/rest/redirect.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)    26431 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/web/rest/replica.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2102 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/web/rest/request.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)    22664 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/web/rest/rse.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)    16478 2017-01-20 08:30:56.000000 rucio-1.9.5/lib/rucio/web/rest/rule.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3538 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/web/rest/scope.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     9331 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/web/rest/subscription.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1588 2016-11-28 16:40:28.000000 rucio-1.9.5/lib/rucio/web/rest/temporary_did.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2209 2016-11-25 16:30:17.000000 rucio-1.9.5/lib/rucio/web/rest/trace.py
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/web/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)      337 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)      249 2017-01-24 09:13:43.000000 rucio-1.9.5/lib/rucio/vcsversion.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1127 2016-11-25 15:17:14.000000 rucio-1.9.5/lib/rucio/version.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/tools/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/tools/probes/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:13:46.000000 rucio-1.9.5/tools/probes/common/
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1578 2016-11-28 16:40:29.000000 rucio-1.9.5/tools/probes/common/boost_long_fts_jobs
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1570 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_WebDAV_ping
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1071 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_activemq_queue
--rwxr-xr-x   0 barisits (51071) zp        (1307)      441 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_always_ok
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3727 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_ami
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2358 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_clean_staging_areas
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3114 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_cloud_srm_space
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1973 2016-11-28 16:40:29.000000 rucio-1.9.5/tools/probes/common/check_deletable_replicas
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1855 2016-11-28 16:40:29.000000 rucio-1.9.5/tools/probes/common/check_disabled_rses
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1110 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_expired_dids
--rwxr-xr-x   0 barisits (51071) zp        (1307)     5626 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/check_expired_es_indices
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1940 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_expired_locked_rules
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1202 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_expired_rules
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1066 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_free_space
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4186 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/check_fts_backlog
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2478 2016-11-28 16:40:29.000000 rucio-1.9.5/tools/probes/common/check_gridftp_space
--rwxr-xr-x   0 barisits (51071) zp        (1307)      960 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/check_injecting_rules
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2010 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/check_log
--rwxr-xr-x   0 barisits (51071) zp        (1307)    10685 2016-11-28 16:40:29.000000 rucio-1.9.5/tools/probes/common/check_lost_files
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4239 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_map_voms_roles
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1118 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_messages_to_submit
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1003 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_new_dids
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2068 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_obsolete_replicas
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1845 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_oracle
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1393 2016-11-28 16:40:29.000000 rucio-1.9.5/tools/probes/common/check_oracle_partitions
--rwxr-xr-x   0 barisits (51071) zp        (1307)      607 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_ping_rucio_servers
--rwxr-xr-x   0 barisits (51071) zp        (1307)    11296 2017-01-20 08:30:56.000000 rucio-1.9.5/tools/probes/common/check_quotas
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3784 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/check_redis
--rwxr-xr-x   0 barisits (51071) zp        (1307)     3651 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/check_requests_to_rses
--rwxr-xr-x   0 barisits (51071) zp        (1307)     5274 2016-11-28 16:40:29.000000 rucio-1.9.5/tools/probes/common/check_rse_attributes
--rwxr-xr-x   0 barisits (51071) zp        (1307)    12587 2016-11-28 16:40:29.000000 rucio-1.9.5/tools/probes/common/check_rses_distance
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1712 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_rule_health
--rwxr-xr-x   0 barisits (51071) zp        (1307)     5237 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/check_rules
--rwxr-xr-x   0 barisits (51071) zp        (1307)     6706 2016-11-28 16:40:29.000000 rucio-1.9.5/tools/probes/common/check_set_rse_space_limits
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2315 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_site_status
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2224 2016-11-28 16:40:29.000000 rucio-1.9.5/tools/probes/common/check_srm_space
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4099 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_stalled_fts_connections
--rwxr-xr-x   0 barisits (51071) zp        (1307)     6843 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/check_stresstest_dids_requests_replicas_daily
--rwxr-xr-x   0 barisits (51071) zp        (1307)     6891 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/check_stresstest_dids_requests_replicas_hourly
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2180 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/check_stresstest_replicas_replicating_time_hourly
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2133 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/check_stresstest_replicas_replicating_time_statistics_2hours
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2126 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/check_stresstest_replicas_replicating_time_statistics_daily
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1260 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_stuck_rules
--rwxr-xr-x   0 barisits (51071) zp        (1307)    11753 2016-11-28 16:40:29.000000 rucio-1.9.5/tools/probes/common/check_sync_rses_with_agis
--rwxr-xr-x   0 barisits (51071) zp        (1307)     2228 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_transfer_queues_status
--rwxr-xr-x   0 barisits (51071) zp        (1307)      910 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_unevaluated_dids
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1724 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/check_unlocked_replicas
--rwxr-xr-x   0 barisits (51071) zp        (1307)      960 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_updated_account_counters
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1701 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_updated_dids
--rwxr-xr-x   0 barisits (51071) zp        (1307)      948 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_updated_rse_counters
--rwxr-xr-x   0 barisits (51071) zp        (1307)      928 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_used_space
--rwxr-xr-x   0 barisits (51071) zp        (1307)     8471 2017-01-20 09:22:58.000000 rucio-1.9.5/tools/probes/common/check_voms
--rwxr-xr-x   0 barisits (51071) zp        (1307)     6882 2016-11-28 16:40:29.000000 rucio-1.9.5/tools/probes/common/check_voms_admin
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1128 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/check_webDAV_service
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1905 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/check_webdav_space
--rwxr-xr-x   0 barisits (51071) zp        (1307)     6881 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/daemon_activity_reports
--rwxr-xr-x   0 barisits (51071) zp        (1307)     5110 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/graphite2nagios
--rwxr-xr-x   0 barisits (51071) zp        (1307)     7517 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/monitor_apache
--rwxr-xr-x   0 barisits (51071) zp        (1307)     4430 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/monitor_client
--rwxr-xr-x   0 barisits (51071) zp        (1307)     5014 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/monitor_flume
--rwxr-xr-x   0 barisits (51071) zp        (1307)     5887 2016-11-25 16:30:17.000000 rucio-1.9.5/tools/probes/common/monitor_haproxy_local
--rw-r--r--   0 barisits (51071) zp        (1307)     5519 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/service_monitoring.cfg
--rw-r--r--   0 barisits (51071) zp        (1307)     4200 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/probes/common/service_monitoring.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)      841 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/bootstrap.py
--rw-r--r--   0 barisits (51071) zp        (1307)     2549 2017-01-20 08:30:56.000000 rucio-1.9.5/tools/pip-requires
--rw-r--r--   0 barisits (51071) zp        (1307)     1060 2017-01-20 08:30:56.000000 rucio-1.9.5/tools/pip-requires-client
--rwxr-xr-x   0 barisits (51071) zp        (1307)     1819 2017-01-20 08:30:56.000000 rucio-1.9.5/tools/pip-requires-test
--rwxr-xr-x   0 barisits (51071) zp        (1307)      928 2016-11-25 15:17:14.000000 rucio-1.9.5/tools/reset_database.py
--rw-r--r--   0 barisits (51071) zp        (1307)      541 2016-11-25 15:17:13.000000 rucio-1.9.5/AUTHORS
--rw-r--r--   0 barisits (51071) zp        (1307)      273 2016-11-25 15:17:13.000000 rucio-1.9.5/ChangeLog
--rw-r--r--   0 barisits (51071) zp        (1307)      274 2016-11-25 15:17:13.000000 rucio-1.9.5/LICENSE
--rw-r--r--   0 barisits (51071) zp        (1307)      919 2017-01-24 09:13:42.000000 rucio-1.9.5/MANIFEST.in
--rw-r--r--   0 barisits (51071) zp        (1307)      274 2017-01-24 09:13:42.000000 rucio-1.9.5/README.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     7396 2016-11-25 15:17:14.000000 rucio-1.9.5/pylintrc
--rw-r--r--   0 barisits (51071) zp        (1307)     1014 2016-11-25 15:17:14.000000 rucio-1.9.5/setup.cfg
--rw-r--r--   0 barisits (51071) zp        (1307)     6459 2017-01-24 09:13:42.000000 rucio-1.9.5/setup.py
--rw-r--r--   0 barisits (51071) zp        (1307)      739 2017-01-24 09:13:46.000000 rucio-1.9.5/PKG-INFO
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/bin/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   121517 2017-01-31 11:31:28.000000 rucio-1.9.6/bin/rucio
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1367 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-abacus-account
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1355 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-abacus-rse
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    44207 2016-11-28 16:40:28.000000 rucio-1.9.6/bin/rucio-admin
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1697 2016-11-28 16:40:28.000000 rucio-1.9.6/bin/rucio-atropos
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     5298 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-auditor
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1257 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-automatix
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2366 2017-01-20 09:22:58.000000 rucio-1.9.6/bin/rucio-bb8
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3427 2016-11-28 16:40:28.000000 rucio-1.9.6/bin/rucio-c3po
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4661 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-cache-client
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      873 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-cache-consumer
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2174 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-conveyor-finisher
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2772 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-conveyor-poller
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1798 2016-11-25 16:30:17.000000 rucio-1.9.6/bin/rucio-conveyor-poller-latest
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1206 2016-11-28 16:40:28.000000 rucio-1.9.6/bin/rucio-conveyor-receiver
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3600 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-conveyor-stager
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3791 2016-11-28 16:40:28.000000 rucio-1.9.6/bin/rucio-conveyor-submitter
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1028 2016-11-28 16:40:28.000000 rucio-1.9.6/bin/rucio-conveyor-throttler
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3791 2016-11-28 16:40:28.000000 rucio-1.9.6/bin/rucio-conveyor-transfer-submitter
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1545 2016-11-28 16:40:28.000000 rucio-1.9.6/bin/rucio-dark-reaper
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     5505 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-dumper
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1315 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-hermes
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1021 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-judge-cleaner
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1024 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-judge-evaluator
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1027 2016-11-28 16:40:28.000000 rucio-1.9.6/bin/rucio-judge-injector
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1023 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-judge-repairer
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1071 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-kronos
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1546 2016-11-28 16:40:28.000000 rucio-1.9.6/bin/rucio-light-reaper
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1244 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-necromancer
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2162 2016-11-28 16:40:28.000000 rucio-1.9.6/bin/rucio-reaper
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1299 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-transmogrifier
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1101 2016-11-25 15:17:13.000000 rucio-1.9.6/bin/rucio-undertaker
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/atlasnote/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   164832 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/AN_atlaslogo.pdf
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    88058 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/AN_cernlogo.pdf
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2877 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/AtlasRucioNote.aux
+-rw-r--r--   0 barisits (51071) zp        (1307)   440060 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/AtlasRucioNote.pdf
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    23795 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/AtlasRucioNote.tex
+-rw-r--r--   0 barisits (51071) zp        (1307)    65762 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/accounts.graffle
+-rw-r--r--   0 barisits (51071) zp        (1307)    31807 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/accounts.pdf
+-rw-r--r--   0 barisits (51071) zp        (1307)    27065 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/accounts.png
+-rw-r--r--   0 barisits (51071) zp        (1307)   125132 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/aggregation_hierarchy.graffle
+-rw-r--r--   0 barisits (51071) zp        (1307)    44183 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/aggregation_hierarchy.pdf
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     6980 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/atlasnote.cls
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     6557 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/booktabs.sty
+-rw-r--r--   0 barisits (51071) zp        (1307)   132902 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/dataset_hierarchy.graffle
+-rw-r--r--   0 barisits (51071) zp        (1307)    44639 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/dataset_hierarchy.pdf
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    18775 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/fncychap.sty
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    14665 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/sphinx.sty
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2073 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/sphinxhowto.cls
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3421 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/atlasnote/sphinxmanual.cls
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/doctrees/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/doctrees/man/
+-rw-r--r--   0 barisits (51071) zp        (1307)    13923 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/man/rucio-admin.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    21710 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/man/rucio.doctree
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/doctrees/rest/
+-rw-r--r--   0 barisits (51071) zp        (1307)     6101 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/rest/attach_dids_to_dids.doctree
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/doctrees/usecases/
+-rw-r--r--   0 barisits (51071) zp        (1307)     4822 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/add_account_identity.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4818 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/add_metadata_dataset.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4785 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/add_metadata_file.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5249 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/add_scope_to_account.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     8508 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/add_subscription.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    12024 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/authentication.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4960 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/consistency_file_between_storage_and_rucio.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5038 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/delete_file_replica_from_storage.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4927 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/detect_site_reach_watermark.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5230 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4988 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/download_all_files_from_a_given_list_of_files_from_rucio.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5030 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/download_all_files_in_a_dataset_from_rucio.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4835 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/download_files_from_rucio.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4400 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/obsolete_dataset.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5231 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/register_account.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5081 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/register_file_already_on_storage_system.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4524 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/register_transfer_request_file_fts.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4380 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/remove_replication_rules_from_file.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5772 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/reupload_after_failure.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     7617 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/search.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     3221 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/select_unwanted_files_for_deletion.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4412 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/set_replication_rule_to_file.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5464 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/upload_file_with_replication_rule.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     7457 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/usecase_upload_file_into_rucio.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5107 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases/where_are_the_replicas_for_a_file.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     7150 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/Acronyms_and_Abbreviations.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     2393 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/doctrees/Architecture.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    21792 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/Comparison_matrix.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    81561 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/REST_Account.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     8685 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/REST_Intro.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    28088 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/REST_authentication.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    90687 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/REST_did.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     8194 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/REST_identity.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     9921 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/REST_lock.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    19528 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/REST_meta.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     7204 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/REST_redirect.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    43167 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/REST_replica.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    93418 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/REST_rse.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    33047 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/REST_rule.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    14549 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/REST_scope.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    31270 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/REST_subscription.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     8088 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/doctrees/Rucio_Project_Meeting.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    78224 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/account.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    21746 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/accountlimit.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)   196168 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/api_curl_examples.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    27111 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/atlas_integration_testbed.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     2054 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/authentication_and_identity.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    27974 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/cli_admin_examples.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    21844 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/doctrees/cli_examples.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     8060 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/client_examples.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)   116795 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/client_howto.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    39959 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/doctrees/client_tutorial.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)   155605 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/core_constants.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    21418 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/developing.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    18604 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/development_guidelines.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)   153643 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/doctrees/did.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)   452979 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/environment.pickle
+-rw-r--r--   0 barisits (51071) zp        (1307)   224246 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/exception.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    37099 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/identity.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    18065 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/index.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    15084 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/installing_atlas_clients.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    11551 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/installing_clients.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    12786 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/installing_server.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    19939 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/lock.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    39479 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/meta-data.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     7248 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/naming_convention_db.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     3506 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Accounting_and_quota.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     2773 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Architecture.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     9766 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Data_Deletion.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     3278 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Database_Schema.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     3459 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Deployment.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     6135 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Exception_Handling.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    17155 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_File_Dataset_Container.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     6672 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Meta-data_attributes.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     3043 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Notifications.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     2956 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Permission_model.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     9183 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Replica_management.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     6869 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Rucio_Storage_Element.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)   117157 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Rucio_Storage_Element_Manager.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5437 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Rucio_account.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    95260 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Rules.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     9339 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Scheduled_Transfers.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    35789 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Subscriptions.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     3214 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_Traceability_and_logging.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     3326 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/overview_flow.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     9984 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/permission.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     3498 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/replica.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    23662 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/replication_rules_examples.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    94015 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/rest.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)   183082 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/rse.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     7070 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/rucio_cli.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     5185 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/rucio_clients.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    41739 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/rule.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)     4903 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/rules_workflow.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    25243 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/doctrees/scope.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    40983 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/setup.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    48626 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/subscription.doctree
+-rw-r--r--   0 barisits (51071) zp        (1307)    28243 2016-11-25 15:03:17.000000 rucio-1.9.6/doc/build/doctrees/usecases.doctree
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/_images/
+-rw-r--r--   0 barisits (51071) zp        (1307)    71679 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_images/RSE_overview.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    45789 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_images/RSE_sequence_instantiation.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    32727 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_images/RSE_sequence_usage.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    56522 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_images/accounts.png
+-rw-r--r--   0 barisits (51071) zp        (1307)   136638 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_images/architecture.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    82950 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_images/deployment.png
+-rw-r--r--   0 barisits (51071) zp        (1307)   163115 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_images/exception_handling.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    45282 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_images/rucio-get.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    73288 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_images/rucio-put.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    55513 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_images/rucio-register.png
+-rw-r--r--   0 barisits (51071) zp        (1307)   230376 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_images/rucio_schema.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    26628 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_images/scheduled_transfers.png
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/_modules/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/_modules/rucio/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/_modules/rucio/api/
+-rw-r--r--   0 barisits (51071) zp        (1307)    16466 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/rucio/api/identity.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     6844 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/rucio/api/permission.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/_modules/rucio/client/
+-rw-r--r--   0 barisits (51071) zp        (1307)    59303 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/rucio/client/accountclient.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    14938 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/rucio/client/accountlimitclient.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    93774 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/rucio/client/didclient.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    14712 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/rucio/client/lockclient.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    23765 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/rucio/client/metaclient.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    77886 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/rucio/client/rseclient.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    29268 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/rucio/client/ruleclient.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    17486 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/rucio/client/scopeclient.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    29268 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/rucio/client/subscriptionclient.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/_modules/rucio/common/
+-rw-r--r--   0 barisits (51071) zp        (1307)   100322 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/rucio/common/exception.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/_modules/rucio/db/
+-rw-r--r--   0 barisits (51071) zp        (1307)    25179 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/rucio/db/constants.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    20480 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/rucio/db/enum.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/_modules/rucio/rse/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/_modules/rucio/rse/protocols/
+-rw-r--r--   0 barisits (51071) zp        (1307)    51488 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/rucio/rse/protocols/protocol.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/_modules/rucio/web/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/_modules/rucio/web/rest/
+-rw-r--r--   0 barisits (51071) zp        (1307)    11578 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/rucio/web/rest/ping.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5307 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_modules/index.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/_sources/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/_sources/man/
+-rw-r--r--   0 barisits (51071) zp        (1307)      770 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/man/rucio-admin.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1744 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/man/rucio.txt
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/_sources/rest/
+-rw-r--r--   0 barisits (51071) zp        (1307)      350 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/rest/attach_dids_to_dids.txt
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/_sources/usecases/
+-rw-r--r--   0 barisits (51071) zp        (1307)      783 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/add_account_identity.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      708 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/add_metadata_dataset.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      691 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/add_metadata_file.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      655 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/add_scope_to_account.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1470 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/add_subscription.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1677 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/authentication.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      804 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/consistency_file_between_storage_and_rucio.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      902 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/delete_file_replica_from_storage.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      795 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/detect_site_reach_watermark.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      940 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      886 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/download_all_files_from_a_given_list_of_files_from_rucio.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      900 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/download_all_files_in_a_dataset_from_rucio.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      794 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/download_files_from_rucio.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      564 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/obsolete_dataset.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      652 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/register_account.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      916 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/register_file_already_on_storage_system.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      646 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/register_transfer_request_file_fts.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      563 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/remove_replication_rules_from_file.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1270 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/reupload_after_failure.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1102 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/search.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      409 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/select_unwanted_files_for_deletion.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      590 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/set_replication_rule_to_file.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      852 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/upload_file_with_replication_rule.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1106 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/usecase_upload_file_into_rucio.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      633 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases/where_are_the_replicas_for_a_file.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      325 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/Acronyms_and_Abbreviations.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)       39 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/Architecture.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2067 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/Comparison_matrix.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     7173 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/REST_Account.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1586 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/REST_Intro.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2439 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/REST_authentication.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     7945 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/REST_did.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      611 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/REST_identity.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      637 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/REST_lock.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1444 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/REST_meta.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      349 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/REST_redirect.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     3702 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/REST_replica.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     7502 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/REST_rse.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2509 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/REST_rule.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1034 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/REST_scope.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2512 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/REST_subscription.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      662 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/Rucio_Project_Meeting.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      163 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/account.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      184 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/accountlimit.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)    16748 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/api_curl_examples.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2265 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/atlas_integration_testbed.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/authentication_and_identity.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     4204 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/cli_admin_examples.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     4565 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/cli_examples.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1010 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/client_examples.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)    24065 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/client_howto.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)    11591 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/client_tutorial.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      138 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/core_constants.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     4981 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/developing.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     3281 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/development_guidelines.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      180 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/did.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      165 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/exception.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      162 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/identity.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2917 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/index.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2167 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/installing_atlas_clients.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1601 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/installing_clients.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1693 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/installing_server.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      152 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/lock.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      162 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/meta-data.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1180 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/naming_convention_db.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      475 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Accounting_and_quota.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      157 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Architecture.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1905 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Data_Deletion.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      311 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Database_Schema.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      442 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Deployment.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1514 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Exception_Handling.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     3882 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_File_Dataset_Container.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      894 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Meta-data_attributes.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      292 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Notifications.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      251 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Permission_model.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1911 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Replica_management.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1652 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Rucio_Storage_Element.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)    27901 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Rucio_Storage_Element_Manager.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1142 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Rucio_account.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)    23147 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Rules.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2701 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Scheduled_Transfers.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     4241 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Subscriptions.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      382 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_Traceability_and_logging.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      347 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/overview_flow.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      169 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/permission.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      155 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/replica.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     3376 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/replication_rules_examples.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     7948 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/rest.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      453 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/rse.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      717 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/rucio_cli.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      814 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/rucio_clients.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      183 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/rule.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     1414 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/rules_workflow.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      158 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/scope.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     6529 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/setup.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      190 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/subscription.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)     2438 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_sources/usecases.txt
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/_static/
+-rw-r--r--   0 barisits (51071) zp        (1307)      673 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/ajax-loader.gif
+-rw-r--r--   0 barisits (51071) zp        (1307)     8270 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/basic.css
+-rw-r--r--   0 barisits (51071) zp        (1307)     4125 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/classic.css
+-rw-r--r--   0 barisits (51071) zp        (1307)     3500 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/comment-bright.png
+-rw-r--r--   0 barisits (51071) zp        (1307)     3578 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/comment-close.png
+-rw-r--r--   0 barisits (51071) zp        (1307)     3445 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/comment.png
+-rw-r--r--   0 barisits (51071) zp        (1307)     4041 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/default.css
+-rw-r--r--   0 barisits (51071) zp        (1307)     7377 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/doctools.js
+-rw-r--r--   0 barisits (51071) zp        (1307)      347 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/down-pressed.png
+-rw-r--r--   0 barisits (51071) zp        (1307)      347 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/down.png
+-rw-r--r--   0 barisits (51071) zp        (1307)      358 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/file.png
+-rw-r--r--   0 barisits (51071) zp        (1307)   282766 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/jquery-1.11.1.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    95786 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/jquery.js
+-rw-r--r--   0 barisits (51071) zp        (1307)      173 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/minus.png
+-rw-r--r--   0 barisits (51071) zp        (1307)      173 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/plus.png
+-rw-r--r--   0 barisits (51071) zp        (1307)     3991 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/pygments.css
+-rw-r--r--   0 barisits (51071) zp        (1307)    19563 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/rucio_logo.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    17880 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/searchtools.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     4803 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/sidebar.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    35168 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    12140 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/underscore.js
+-rw-r--r--   0 barisits (51071) zp        (1307)      345 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/up-pressed.png
+-rw-r--r--   0 barisits (51071) zp        (1307)      345 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/up.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    25350 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/_static/websupport.js
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/man/
+-rw-r--r--   0 barisits (51071) zp        (1307)     7794 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/man/rucio-admin.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     9052 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/man/rucio.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/rest/
+-rw-r--r--   0 barisits (51071) zp        (1307)     5795 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/rest/attach_dids_to_dids.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/build/html/usecases/
+-rw-r--r--   0 barisits (51071) zp        (1307)     4477 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/add_account_identity.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4558 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/add_metadata_dataset.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4543 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/add_metadata_file.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4538 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/add_scope_to_account.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4872 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/add_subscription.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5938 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/authentication.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4716 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/consistency_file_between_storage_and_rucio.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4557 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/delete_file_replica_from_storage.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4701 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/detect_site_reach_watermark.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4745 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4665 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/download_all_files_from_a_given_list_of_files_from_rucio.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4595 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/download_all_files_in_a_dataset_from_rucio.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4510 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/download_files_from_rucio.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4433 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/obsolete_dataset.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4551 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/register_account.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4548 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/register_file_already_on_storage_system.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4567 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/register_transfer_request_file_fts.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4523 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/remove_replication_rules_from_file.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4531 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/reupload_after_failure.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4876 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/search.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4523 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/select_unwanted_files_for_deletion.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4549 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/set_replication_rule_to_file.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4671 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/upload_file_with_replication_rule.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5164 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/usecase_upload_file_into_rucio.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4518 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/usecases/where_are_the_replicas_for_a_file.html
+-rw-r--r--   0 barisits (51071) zp        (1307)      230 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/.buildinfo
+-rw-r--r--   0 barisits (51071) zp        (1307)     5302 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/Acronyms_and_Abbreviations.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4352 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/Architecture.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     6632 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/Comparison_matrix.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    33965 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/REST_Account.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     8155 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/REST_Intro.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    13611 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/REST_authentication.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    36870 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/REST_did.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     7178 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/REST_identity.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     8464 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/REST_lock.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    11196 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/REST_meta.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     6873 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/REST_redirect.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    19743 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/REST_replica.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    36294 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/REST_rse.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    15403 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/REST_rule.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     9564 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/REST_scope.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    15806 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/REST_subscription.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5982 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/Rucio_Project_Meeting.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    24371 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/account.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     9490 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/accountlimit.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    49271 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/api_curl_examples.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     8847 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/atlas_integration_testbed.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4218 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/authentication_and_identity.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    20697 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/cli_admin_examples.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    16629 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/cli_examples.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     7763 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/client_examples.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    51571 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/client_howto.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    22174 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/client_tutorial.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    38831 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/core_constants.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    13195 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/developing.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    11262 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/development_guidelines.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    42116 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/did.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    64292 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/exception.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    54351 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/genindex.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    22008 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/http-routingtable.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    13231 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/identity.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    15245 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/index.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    10693 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/installing_atlas_clients.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     9658 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/installing_clients.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     8756 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/installing_server.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     9333 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/lock.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    13990 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/meta-data.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     8368 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/naming_convention_db.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4611 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/objects.inv
+-rw-r--r--   0 barisits (51071) zp        (1307)     5892 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_Accounting_and_quota.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5729 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_Architecture.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     7965 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_Data_Deletion.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5828 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_Database_Schema.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5590 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_Deployment.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     7307 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_Exception_Handling.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    11254 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_File_Dataset_Container.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     6831 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_Meta-data_attributes.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5732 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_Notifications.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5700 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_Permission_model.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     8062 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_Replica_management.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     7173 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_Rucio_Storage_Element.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    46544 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_Rucio_Storage_Element_Manager.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     6701 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_Rucio_account.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    36223 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/overview_Rules.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     8997 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_Scheduled_Transfers.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    14110 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_Subscriptions.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4733 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_Traceability_and_logging.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5951 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/overview_flow.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5808 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/permission.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     7644 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/py-modindex.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5259 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/replica.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    11051 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/replication_rules_examples.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    22089 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/rest.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    47247 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/rse.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     6001 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/rucio_cli.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5824 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/rucio_clients.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    13860 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/rule.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     6962 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/rules_workflow.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    10313 2016-11-25 15:03:15.000000 rucio-1.9.6/doc/build/html/scope.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4453 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/search.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    57160 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/searchindex.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    17589 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/setup.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    14675 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/subscription.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    10373 2016-11-25 15:03:16.000000 rucio-1.9.6/doc/build/html/usecases.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/design/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/design/RSE/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1996 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/design/RSE/meeting-2012-02-23.org
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/design/erd/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    55942 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/design/erd/ERD.graffle
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    72676 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/design/erd/ERD.pdf
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    60363 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/design/rucio_schema.pdf
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/source/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/source/_static/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     8270 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/_static/basic.css
+-rw-r--r--   0 barisits (51071) zp        (1307)     4179 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/_static/classic.css
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4041 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/_static/default.css
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    19563 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/_static/rucio_logo.png
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/source/_templates/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      777 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/_templates/layout.html
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/source/cli_examples/
+-rw-r--r--   0 barisits (51071) zp        (1307)       14 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/cli_examples/ping.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)       12 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/cli_examples/ping.sh
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/source/curl_examples/
+-rw-r--r--   0 barisits (51071) zp        (1307)      235 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/del_account.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      312 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/del_account.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/del_location.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      313 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/del_location.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      404 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_account.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      309 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_account.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      673 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_account_whoami.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      314 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_account_whoami.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      253 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_accounts.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      305 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_accounts.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)       29 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_api.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)       34 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_api.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_auth_gss.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      129 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_auth_gss.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_auth_userpass.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      168 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_auth_userpass.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      304 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_auth_validate.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      334 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_auth_validate.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_auth_x509.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      139 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_auth_x509.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_location.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      310 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_location.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      239 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_locations.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      306 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_locations.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      356 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_scopes.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      309 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/get_scopes.sh
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      380 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/post_account.sh
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      332 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/post_location.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      370 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/post_location_rse.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      257 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/put_account.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      331 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/put_account.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      289 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/put_location.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      309 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/put_location.sh
+-rw-r--r--   0 barisits (51071) zp        (1307)      257 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/put_scope.out
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      314 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/curl_examples/put_scope.sh
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/source/example_outputs/
+-rw-r--r--   0 barisits (51071) zp        (1307)     3643 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/example_outputs/failure-rucio.tests.test_curl.TestCurlRucio.test_get_accounts_whoami.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      164 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/example_outputs/success-rucio.tests.test_bin_rucio.TestBinRucio.test_add_account.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)       43 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/example_outputs/success-rucio.tests.test_bin_rucio.TestBinRucio.test_rucio_ping.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/example_outputs/success-rucio.tests.test_bin_rucio.TestBinRucio.test_rucio_version.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)       46 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/example_outputs/success-rucio.tests.test_clients.TestRucioClients.test_ping.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      804 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_accounts_whoami.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      429 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_GSS.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_proxy.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      466 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_userpass.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      454 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_validate.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      442 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_x509.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      454 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_auth_x509_proxy.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)       84 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_ping.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      440 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_post_account.txt
+-rw-r--r--   0 barisits (51071) zp        (1307)      398 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_post_rse.txt
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/source/images/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/source/images/deployment.graffle/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/source/images/deployment.graffle/QuickLook/
+-rw-r--r--   0 barisits (51071) zp        (1307)    52757 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/deployment.graffle/QuickLook/Preview.pdf
+-rw-r--r--   0 barisits (51071) zp        (1307)   124440 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/deployment.graffle/QuickLook/Thumbnail.tiff
+-rw-r--r--   0 barisits (51071) zp        (1307)     3172 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/deployment.graffle/data.plist
+-rw-r--r--   0 barisits (51071) zp        (1307)    26954 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/deployment.graffle/image2.tiff
+-rw-r--r--   0 barisits (51071) zp        (1307)    10020 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/deployment.graffle/image3.tiff
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    71679 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/RSE_overview.png
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    45789 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/RSE_sequence_instantiation.png
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    32727 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/RSE_sequence_usage.png
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    56522 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/accounts.png
+-rw-r--r--   0 barisits (51071) zp        (1307)   397841 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/architecture.graffle
+-rw-r--r--   0 barisits (51071) zp        (1307)   136638 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/architecture.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    82950 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/deployment.png
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    70361 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/exception_handling.graffle
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   163115 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/exception_handling.png
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   127009 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/highLevelRoadmap.graffle
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   205501 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/rucio-get.graffle
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    45282 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/rucio-get.png
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   298526 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/rucio-put.graffle
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    73288 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/rucio-put.png
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   232239 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/rucio-register.graffle
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    55513 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/rucio-register.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    62543 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/rucio_schema.gml
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   226250 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/images/rucio_schema.pdf
+-rwxr-xr-x   0 barisits (51071) zp        (1307)   230376 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/images/rucio_schema.png
+-rw-r--r--   0 barisits (51071) zp        (1307)     2485 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/images/scheduled_transfers.dia
+-rw-r--r--   0 barisits (51071) zp        (1307)    26628 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/images/scheduled_transfers.png
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/source/man/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      770 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/man/rucio-admin.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1744 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/man/rucio.rst
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/source/rest/
+-rw-r--r--   0 barisits (51071) zp        (1307)      350 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/rest/attach_dids_to_dids.rst
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/doc/source/usecases/
+-rw-r--r--   0 barisits (51071) zp        (1307)      783 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/add_account_identity.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      708 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/add_metadata_dataset.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      691 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/add_metadata_file.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      655 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/add_scope_to_account.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1470 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/add_subscription.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1677 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/authentication.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      804 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/consistency_file_between_storage_and_rucio.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      902 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/delete_file_replica_from_storage.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      795 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/detect_site_reach_watermark.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      940 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      886 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/download_all_files_from_a_given_list_of_files_from_rucio.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      900 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/download_all_files_in_a_dataset_from_rucio.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      794 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/download_files_from_rucio.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      564 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/obsolete_dataset.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      652 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/register_account.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      916 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/register_file_already_on_storage_system.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      646 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/register_transfer_request_file_fts.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      563 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/remove_replication_rules_from_file.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1270 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/reupload_after_failure.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1102 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/search.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      409 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/select_unwanted_files_for_deletion.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      590 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/set_replication_rule_to_file.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      852 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/upload_file_with_replication_rule.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1106 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/usecase_upload_file_into_rucio.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      633 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases/where_are_the_replicas_for_a_file.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      325 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/Acronyms_and_Abbreviations.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)       39 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/Architecture.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2067 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/Comparison_matrix.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     7173 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/REST_Account.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1586 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/REST_Intro.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     2439 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/REST_authentication.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     7945 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/REST_did.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      611 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/REST_identity.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      637 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/REST_lock.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1444 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/REST_meta.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      349 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/REST_redirect.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     3702 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/REST_replica.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     7502 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/REST_rse.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     2509 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/REST_rule.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1034 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/REST_scope.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     2512 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/REST_subscription.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     6000 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/RSE_Expressions.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      662 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/Rucio_Project_Meeting.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      163 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/account.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      184 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/accountlimit.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    19866 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/accounts.pdf
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    56522 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/accounts.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    16748 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/api_curl_examples.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     2265 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/atlas_integration_testbed.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/authentication_and_identity.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     4204 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/cli_admin_examples.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     4565 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/cli_examples.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1010 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/client_examples.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)    11591 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/client_tutorial.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     7556 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/conf.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      138 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/core_constants.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     7860 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/developing.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3281 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/development_guidelines.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      180 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/did.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      165 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/exception.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      162 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/source/identity.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3274 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/index.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     2167 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/installing_atlas_clients.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1601 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/installing_clients.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1693 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/installing_server.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      152 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/lock.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      162 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/meta-data.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1180 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/naming_convention_db.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      475 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Accounting_and_quota.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      157 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Architecture.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1905 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Data_Deletion.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      311 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Database_Schema.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      442 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Deployment.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1514 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Exception_Handling.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3882 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_File_Dataset_Container.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      894 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Meta-data_attributes.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      292 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Notifications.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      251 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Permission_model.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1911 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Replica_management.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1652 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Rucio_Storage_Element.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)    27901 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Rucio_Storage_Element_Manager.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1142 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Rucio_account.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)    23147 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Rules.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     2701 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Scheduled_Transfers.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4241 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Subscriptions.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      382 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_Traceability_and_logging.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      347 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/overview_flow.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      169 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/permission.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      155 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/replica.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1509 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/replication_rules_examples.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     7948 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/rest.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      453 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/rse.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      717 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/rucio_cli.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      814 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/rucio_clients.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      183 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/rule.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     1414 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/rules_workflow.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      158 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/scope.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)      189 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/service_avaibility.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      190 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/subscription.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2438 2016-11-25 15:17:14.000000 rucio-1.9.6/doc/source/usecases.rst
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4590 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/Makefile
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4513 2016-11-25 15:17:13.000000 rucio-1.9.6/doc/make.bat
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/etc/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/etc/mail_templates/
+-rw-r--r--   0 barisits (51071) zp        (1307)     1078 2016-11-28 16:40:28.000000 rucio-1.9.6/etc/mail_templates/rule_approval_request.tmpl
+-rw-r--r--   0 barisits (51071) zp        (1307)      105 2016-11-28 16:40:28.000000 rucio-1.9.6/etc/mail_templates/rule_approved_admin.tmpl
+-rw-r--r--   0 barisits (51071) zp        (1307)      498 2016-11-28 16:40:28.000000 rucio-1.9.6/etc/mail_templates/rule_approved_user.tmpl
+-rw-r--r--   0 barisits (51071) zp        (1307)      103 2016-11-28 16:40:28.000000 rucio-1.9.6/etc/mail_templates/rule_denied_admin.tmpl
+-rw-r--r--   0 barisits (51071) zp        (1307)      460 2016-11-28 16:40:28.000000 rucio-1.9.6/etc/mail_templates/rule_denied_user.tmpl
+-rw-r--r--   0 barisits (51071) zp        (1307)      545 2016-11-28 16:40:28.000000 rucio-1.9.6/etc/mail_templates/rule_ok_notification.tmpl
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/etc/schemas/
+-rw-r--r--   0 barisits (51071) zp        (1307)       97 2016-11-25 15:17:14.000000 rucio-1.9.6/etc/schemas/account.json
+-rw-r--r--   0 barisits (51071) zp        (1307)       82 2016-11-25 15:17:14.000000 rucio-1.9.6/etc/schemas/account_type.json
+-rw-r--r--   0 barisits (51071) zp        (1307)       82 2016-11-25 15:17:14.000000 rucio-1.9.6/etc/schemas/did_type.json
+-rw-r--r--   0 barisits (51071) zp        (1307)      112 2016-11-25 15:17:14.000000 rucio-1.9.6/etc/schemas/mail.json
+-rw-r--r--   0 barisits (51071) zp        (1307)      105 2016-11-25 15:17:14.000000 rucio-1.9.6/etc/schemas/rse.json
+-rw-r--r--   0 barisits (51071) zp        (1307)      105 2016-11-25 15:17:14.000000 rucio-1.9.6/etc/schemas/scope.json
+-rw-r--r--   0 barisits (51071) zp        (1307)      559 2016-11-25 15:17:14.000000 rucio-1.9.6/etc/schemas/sub_filter.json
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/etc/web/
+-rw-r--r--   0 barisits (51071) zp        (1307)     2551 2016-11-25 15:17:14.000000 rucio-1.9.6/etc/web/httpd-rucio-443-py26-slc6.conf.template
+-rw-r--r--   0 barisits (51071) zp        (1307)     2557 2017-01-20 08:30:56.000000 rucio-1.9.6/etc/web/httpd-rucio-443-py27-cc7.conf.template
+-rw-r--r--   0 barisits (51071) zp        (1307)     1690 2016-11-25 15:17:14.000000 rucio-1.9.6/etc/web/httpd-rucio-443-py27-debian.conf.template
+-rw-r--r--   0 barisits (51071) zp        (1307)     2055 2016-11-25 15:17:14.000000 rucio-1.9.6/etc/web/httpd-rucio-443-py27-osx.conf.template
+-rw-r--r--   0 barisits (51071) zp        (1307)     1665 2016-11-25 15:17:14.000000 rucio-1.9.6/etc/web/httpd-rucio-443-py27-ubuntu.conf.template
+-rw-r--r--   0 barisits (51071) zp        (1307)     1358 2016-11-25 15:17:14.000000 rucio-1.9.6/etc/alembic.ini.template
+-rw-r--r--   0 barisits (51071) zp        (1307)      807 2016-11-25 15:17:14.000000 rucio-1.9.6/etc/ldap.cfg.template
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      543 2016-11-25 15:17:14.000000 rucio-1.9.6/etc/rse-accounts.cfg.template
+-rw-r--r--   0 barisits (51071) zp        (1307)      570 2016-11-25 15:17:14.000000 rucio-1.9.6/etc/rucio.cfg.atlas.client.template
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     5165 2016-11-28 16:40:28.000000 rucio-1.9.6/etc/rucio.cfg.template
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/api/
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/api/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     5257 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/api/account.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4277 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/api/account_limit.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3541 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/api/authentication.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1839 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/api/availability.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6358 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/api/config.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    11944 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/api/did.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      896 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/api/heartbeat.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3812 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/api/identity.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1269 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/api/lock.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2121 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/api/meta.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      983 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/api/permission.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     7451 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/api/replica.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4641 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/api/request.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    10182 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/api/rse.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     8596 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/api/rule.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1532 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/api/scope.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     7330 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/api/subscription.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      816 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/api/temporary_did.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/client/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/client/cli/
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/cli/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      469 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/cli/download.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      581 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/cli/upload.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      325 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    12651 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/accountclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2763 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/accountlimitclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    21749 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/client/baseclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2381 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/client.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3523 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/configclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    23023 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/client/didclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    91449 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/client/dq2client.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1716 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/fileclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2594 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/lockclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4717 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/metaclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3915 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/objectstoreclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1356 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/pingclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9888 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/client/replicaclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    19164 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/rseclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9768 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/client/ruleclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3292 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/scopeclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     7475 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/subscriptionclient.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4326 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/client/uploadclient.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/common/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/common/dumper/
+-rw-r--r--   0 barisits (51071) zp        (1307)    10166 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/common/dumper/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    15801 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/common/dumper/consistency.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9062 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/common/dumper/data_models.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1637 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/common/dumper/path_parsing.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/common/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1208 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/common/client.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     7763 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/common/closeness_sorter.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3883 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/common/config.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      938 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/common/constants.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      439 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/common/constraints.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    19606 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/common/exception.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3288 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/common/log.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    14068 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/common/objectstore.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     8188 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/common/policy.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     5461 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/common/replicas_selector.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1520 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/common/rse_attributes.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    14030 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/common/schema.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    14270 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/common/utils.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/core/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/core/permission/
+-rw-r--r--   0 barisits (51071) zp        (1307)      954 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/core/permission/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    33084 2017-01-30 16:14:23.000000 rucio-1.9.6/lib/rucio/core/permission/atlas.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    27320 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/core/permission/generic.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/core/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9768 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/core/account.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6664 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/core/account_counter.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6506 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/core/account_limit.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     7133 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/core/authentication.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6879 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/core/config.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    70609 2017-02-07 08:58:02.000000 rucio-1.9.6/lib/rucio/core/did.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6526 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/core/distance.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     7114 2017-01-30 16:14:23.000000 rucio-1.9.6/lib/rucio/core/heartbeat.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6453 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/core/identity.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    17559 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/core/lock.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4812 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/core/message.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     5715 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/core/meta.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2501 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/core/monitor.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     5252 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/core/naming_convention.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2621 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/core/nongrid_trace.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6082 2017-02-07 08:58:02.000000 rucio-1.9.6/lib/rucio/core/quarantined_replica.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    90603 2017-02-07 08:58:02.000000 rucio-1.9.6/lib/rucio/core/replica.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    77839 2017-02-07 08:58:02.000000 rucio-1.9.6/lib/rucio/core/request.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    37244 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/core/rse.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     5046 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/core/rse_counter.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    14410 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/core/rse_expression_parser.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     7258 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/core/rse_selector.py
+-rw-r--r--   0 barisits (51071) zp        (1307)   159876 2017-02-07 08:58:02.000000 rucio-1.9.6/lib/rucio/core/rule.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    71608 2017-02-02 12:35:27.000000 rucio-1.9.6/lib/rucio/core/rule_grouping.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4386 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/core/scope.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    10826 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/core/subscription.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     7249 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/core/temporary_did.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2618 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/core/trace.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4351 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/core/volatile_replica.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/daemons/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/daemons/abacus/
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/daemons/abacus/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3549 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/daemons/abacus/account.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3337 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/daemons/abacus/rse.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/daemons/auditor/
+-rw-r--r--   0 barisits (51071) zp        (1307)     4485 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/daemons/auditor/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2258 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/daemons/auditor/hdfs.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     7680 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/daemons/auditor/srmdumps.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/daemons/bb8/
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/bb8/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2186 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/bb8/bb8.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    12237 2017-02-07 08:58:02.000000 rucio-1.9.6/lib/rucio/daemons/bb8/common.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4367 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/daemons/bb8/t1_background_rebalance.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/daemons/c3po/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/daemons/c3po/algorithms/
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/algorithms/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4266 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/algorithms/simple.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4125 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/algorithms/t2_free_space.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4388 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    11732 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/daemons/c3po/collectors/
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/collectors/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2533 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/collectors/agis.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1536 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/collectors/free_space.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1379 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/collectors/jedi_did.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      946 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/collectors/mock_did.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1800 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/collectors/network_metrics.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3435 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/collectors/workload.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/daemons/c3po/utils/
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/utils/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1066 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/utils/dataset_cache.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1100 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1361 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/utils/expiring_list.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2109 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/utils/popularity.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1458 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/utils/timeseries.py
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    12253 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/c3po/c3po.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/daemons/cache/
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/daemons/cache/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     5201 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/cache/consumer.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/daemons/conveyor/
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/daemons/conveyor/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    35293 2017-01-20 09:22:58.000000 rucio-1.9.6/lib/rucio/daemons/conveyor/common.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     7392 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/conveyor/finisher.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     8949 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/daemons/conveyor/poller.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     5004 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/daemons/conveyor/poller_latest.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    12691 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/conveyor/receiver.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    10002 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/conveyor/stager.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    10532 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/conveyor/submitter.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3586 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/conveyor/throttler.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    79138 2017-01-20 09:22:58.000000 rucio-1.9.6/lib/rucio/daemons/conveyor/utils.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/daemons/hermes/
+-rw-r--r--   0 barisits (51071) zp        (1307)      304 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/daemons/hermes/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    16283 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/hermes/hermes.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/daemons/judge/
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/daemons/judge/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6840 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/judge/cleaner.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     8227 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/judge/evaluator.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     7265 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/judge/injector.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6446 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/judge/repairer.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/daemons/mock/
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/daemons/mock/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     7146 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/daemons/mock/conveyorinjector.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/daemons/reaper/
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/reaper/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     8793 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/reaper/dark_reaper.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     8771 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/reaper/light_reaper.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    23652 2017-02-07 08:58:02.000000 rucio-1.9.6/lib/rucio/daemons/reaper/reaper.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/daemons/tracer/
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/daemons/tracer/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    17432 2017-01-20 09:22:58.000000 rucio-1.9.6/lib/rucio/daemons/tracer/kronos.py
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/daemons/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     8726 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/atropos.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     6006 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/necromancer.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    22173 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/daemons/transmogrifier.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3903 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/daemons/undertaker.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/db/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/db/elasticsearch/
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/db/elasticsearch/__init__.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/db/sqla/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/
+-rw-r--r--   0 barisits (51071) zp        (1307)     1198 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      762 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      773 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1978 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      738 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1059 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1118 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      799 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2224 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1385 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1049 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1254 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      893 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2147 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1984 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      934 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      903 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      983 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1565 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      979 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1839 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2253 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      922 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1018 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1364 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      843 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1986 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1501 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1928 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      954 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2160 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4355 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2560 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1233 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1063 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      928 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1056 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      773 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      848 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1112 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2966 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      934 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1772 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1255 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      881 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1291 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      743 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2141 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      992 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      823 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1713 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1045 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2776 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1502 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1254 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      904 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2111 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3451 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1723 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2090 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1190 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1465 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      880 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      942 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3398 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      975 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2606 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/env.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/db/sqla/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4652 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/db/sqla/constants.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3389 2017-02-07 08:57:43.000000 rucio-1.9.6/lib/rucio/db/sqla/enum.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6109 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/db/sqla/history.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    60735 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/db/sqla/models.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1407 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/db/sqla/sautils.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    11324 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/db/sqla/session.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2907 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/db/sqla/types.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6086 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/db/sqla/util.py
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/db/__init__.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/rse/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/rse/protocols/
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/rse/protocols/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4165 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/rse/protocols/cache.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3787 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/rse/protocols/dummy.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    17585 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/rse/protocols/gfal.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1256 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/rse/protocols/gfalv2.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4680 2017-01-31 11:31:28.000000 rucio-1.9.6/lib/rucio/rse/protocols/gsiftp.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2635 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/rse/protocols/http_cache.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3741 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/rse/protocols/mock.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6596 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/rse/protocols/ngarc.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6199 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/rse/protocols/posix.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    12783 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/rse/protocols/protocol.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     5035 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/rse/protocols/rfio.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9114 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/rse/protocols/s3.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9915 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/rse/protocols/s3boto.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6345 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/rse/protocols/s3es.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6723 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/rse/protocols/sftp.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    15403 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/rse/protocols/signeds3.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    13829 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/rse/protocols/srm.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    19999 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/rse/protocols/webdav.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     8153 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/rse/protocols/xrootd.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1937 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/rse/__init__.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    25451 2017-01-31 11:31:28.000000 rucio-1.9.6/lib/rucio/rse/rsemanager.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/tests/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/tests/daemons/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    11714 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/tests/daemons/Automatix.py
+-rw-r--r--   0 barisits (51071) zp        (1307)        0 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/daemons/__init__.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/tests/emulation/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/tests/emulation/usecases/
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/emulation/usecases/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      969 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/emulation/usecases/auth.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1476 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/emulation/usecases/dummy.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2208 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/emulation/usecases/dummy_template.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3716 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/emulation/usecases/jdoe.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    65781 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/emulation/usecases/panda.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    56221 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/emulation/usecases/panda_new.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    21228 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/emulation/usecases/tzero.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/emulation/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9327 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/emulation/emulator.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    15903 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/emulation/ucemulator.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     8610 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/emulation/ucprocess.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3278 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/emulation/worker.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/tests/functional/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/tests/functional/blocks/
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/functional/blocks/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      577 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/functional/blocks/block1.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     8354 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/tests/functional/blocks/block2.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/functional/__init__.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     5986 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/tests/functional/run.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/tests/mock/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/tests/mock/web/
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/mock/web/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2271 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/mock/web/fts3.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/mock/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3707 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/tests/mock/fts3.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      532 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/mock/gfal2.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4684 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/common.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    22701 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/tests/rsemgr_api_test.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    14408 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_account.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4351 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_account_limits.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1245 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_alembic.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2723 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_auditor.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1719 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_auditor_hdfs.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2888 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_auditor_srmdumps.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2292 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_authentication.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3786 2017-01-20 09:22:58.000000 rucio-1.9.6/lib/rucio/tests/test_bb8.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    27965 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/tests/test_bin_rucio.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3210 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/tests/test_clients.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3120 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_config.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1200 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/tests/test_conveyor.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4563 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_counter.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6716 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/tests/test_curl.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2091 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_dataset_replicas.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      707 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_db.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    37907 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/tests/test_did.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6392 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_dumper.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    16150 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_dumper_consistency.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9790 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_dumper_data_model.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3145 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_dumper_path_parsing.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3362 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_heartbeat.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1657 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_hermes.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2141 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_identity.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3274 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_judge_cleaner.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    11109 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/tests/test_judge_evaluator.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     8060 2017-01-30 16:14:23.000000 rucio-1.9.6/lib/rucio/tests/test_judge_injector.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    16107 2017-02-01 12:54:56.000000 rucio-1.9.6/lib/rucio/tests/test_judge_repairer.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2086 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/tests/test_message.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3149 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_meta.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2532 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_meta_did.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1510 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_monitor.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2756 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_naming_convention.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    12265 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_objectstore.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3185 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_permission.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1286 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_ping.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1358 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/tests/test_quarantined_replica.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1307 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/tests/test_reaper.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     5633 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/tests/test_redirect.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    27875 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/tests/test_replica.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    78040 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/tests/test_rse.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    10690 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/tests/test_rse_expression_parser.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    13237 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_rse_protocol_gfal2.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     5173 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_rse_protocol_mock.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9728 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_rse_protocol_posix.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9813 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_rse_protocol_s3.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    11909 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/tests/test_rse_protocol_s3boto.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4845 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/tests/test_rse_protocol_s3es.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    10110 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_rse_protocol_sftp.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     9909 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_rse_protocol_signeds3.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    12805 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_rse_protocol_srm.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    11084 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_rse_protocol_webdav.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    10967 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_rse_protocol_xrootd.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     6537 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_rucio_cache.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     4792 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_rucio_server.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    51857 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/tests/test_rule.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    10288 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_scope.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    20485 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/tests/test_subscription.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2650 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/tests/test_temporary_did.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1345 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/tests/test_trace.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     3258 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/tests/test_undertaker.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/transfertool/
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/transfertool/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)    39426 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/transfertool/fts3.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/web/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/lib/rucio/web/rest/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      346 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/web/rest/__init__.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    21464 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/web/rest/account.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3914 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/web/rest/account_limit.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    11929 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/web/rest/authentication.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4112 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/web/rest/common.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4332 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/web/rest/config.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    27806 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/web/rest/did.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1402 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/web/rest/heartbeat.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4706 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/web/rest/identity.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3112 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/web/rest/lock.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4904 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/web/rest/meta.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1846 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/web/rest/nongrid_trace.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     5430 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/web/rest/objectstore.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2170 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/web/rest/ping.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    10189 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/web/rest/redirect.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    26431 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/web/rest/replica.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2102 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/web/rest/request.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    22664 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/web/rest/rse.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    16478 2017-01-20 08:30:56.000000 rucio-1.9.6/lib/rucio/web/rest/rule.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3538 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/web/rest/scope.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     9331 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/web/rest/subscription.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1588 2016-11-28 16:40:28.000000 rucio-1.9.6/lib/rucio/web/rest/temporary_did.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2209 2016-11-25 16:30:17.000000 rucio-1.9.6/lib/rucio/web/rest/trace.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/web/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      337 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      249 2017-02-07 09:03:29.000000 rucio-1.9.6/lib/rucio/vcsversion.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1127 2016-11-25 15:17:14.000000 rucio-1.9.6/lib/rucio/version.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/tools/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/tools/probes/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:32.000000 rucio-1.9.6/tools/probes/common/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1578 2016-11-28 16:40:29.000000 rucio-1.9.6/tools/probes/common/boost_long_fts_jobs
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1570 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_WebDAV_ping
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1071 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_activemq_queue
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      441 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_always_ok
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3727 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_ami
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2358 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_clean_staging_areas
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3114 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_cloud_srm_space
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1973 2016-11-28 16:40:29.000000 rucio-1.9.6/tools/probes/common/check_deletable_replicas
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1855 2016-11-28 16:40:29.000000 rucio-1.9.6/tools/probes/common/check_disabled_rses
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1110 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_expired_dids
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     5626 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/check_expired_es_indices
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1940 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_expired_locked_rules
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1202 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_expired_rules
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1066 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_free_space
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4186 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/check_fts_backlog
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2478 2016-11-28 16:40:29.000000 rucio-1.9.6/tools/probes/common/check_gridftp_space
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      960 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/check_injecting_rules
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2010 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/check_log
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    10685 2016-11-28 16:40:29.000000 rucio-1.9.6/tools/probes/common/check_lost_files
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4239 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_map_voms_roles
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1118 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_messages_to_submit
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1003 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_new_dids
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2068 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_obsolete_replicas
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1845 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_oracle
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1393 2016-11-28 16:40:29.000000 rucio-1.9.6/tools/probes/common/check_oracle_partitions
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      607 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_ping_rucio_servers
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    11296 2017-01-20 08:30:56.000000 rucio-1.9.6/tools/probes/common/check_quotas
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3784 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/check_redis
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     3651 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/check_requests_to_rses
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     5429 2017-01-30 16:14:23.000000 rucio-1.9.6/tools/probes/common/check_rse_attributes
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    12587 2016-11-28 16:40:29.000000 rucio-1.9.6/tools/probes/common/check_rses_distance
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1712 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_rule_health
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     5237 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/check_rules
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     6923 2017-02-02 12:35:27.000000 rucio-1.9.6/tools/probes/common/check_set_rse_space_limits
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2315 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_site_status
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2224 2016-11-28 16:40:29.000000 rucio-1.9.6/tools/probes/common/check_srm_space
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4099 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_stalled_fts_connections
+-rw-r--r--   0 barisits (51071) zp        (1307)     2815 2017-01-30 16:14:23.000000 rucio-1.9.6/tools/probes/common/check_storage_space
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     6843 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/check_stresstest_dids_requests_replicas_daily
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     6891 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/check_stresstest_dids_requests_replicas_hourly
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2180 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/check_stresstest_replicas_replicating_time_hourly
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2133 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/check_stresstest_replicas_replicating_time_statistics_2hours
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2126 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/check_stresstest_replicas_replicating_time_statistics_daily
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1260 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_stuck_rules
+-rwxr-xr-x   0 barisits (51071) zp        (1307)    11753 2016-11-28 16:40:29.000000 rucio-1.9.6/tools/probes/common/check_sync_rses_with_agis
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     2228 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_transfer_queues_status
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      910 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_unevaluated_dids
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1724 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/check_unlocked_replicas
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      960 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_updated_account_counters
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1701 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_updated_dids
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      948 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_updated_rse_counters
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      928 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_used_space
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     8471 2017-01-20 09:22:58.000000 rucio-1.9.6/tools/probes/common/check_voms
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     6882 2016-11-28 16:40:29.000000 rucio-1.9.6/tools/probes/common/check_voms_admin
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1128 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/check_webDAV_service
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1905 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/check_webdav_space
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     6881 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/daemon_activity_reports
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     5110 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/graphite2nagios
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     7517 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/monitor_apache
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     4430 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/monitor_client
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     5014 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/monitor_flume
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     5887 2016-11-25 16:30:17.000000 rucio-1.9.6/tools/probes/common/monitor_haproxy_local
+-rw-r--r--   0 barisits (51071) zp        (1307)     5519 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/service_monitoring.cfg
+-rw-r--r--   0 barisits (51071) zp        (1307)     4200 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/probes/common/service_monitoring.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      841 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/bootstrap.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     2549 2017-02-07 08:57:43.000000 rucio-1.9.6/tools/pip-requires
+-rw-r--r--   0 barisits (51071) zp        (1307)     1060 2017-01-20 08:30:56.000000 rucio-1.9.6/tools/pip-requires-client
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     1819 2017-01-20 08:30:56.000000 rucio-1.9.6/tools/pip-requires-test
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      928 2016-11-25 15:17:14.000000 rucio-1.9.6/tools/reset_database.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      541 2016-11-25 15:17:13.000000 rucio-1.9.6/AUTHORS
+-rw-r--r--   0 barisits (51071) zp        (1307)      273 2016-11-25 15:17:13.000000 rucio-1.9.6/ChangeLog
+-rw-r--r--   0 barisits (51071) zp        (1307)      274 2016-11-25 15:17:13.000000 rucio-1.9.6/LICENSE
+-rw-r--r--   0 barisits (51071) zp        (1307)      919 2017-02-07 09:03:28.000000 rucio-1.9.6/MANIFEST.in
+-rw-r--r--   0 barisits (51071) zp        (1307)      274 2017-02-07 09:03:28.000000 rucio-1.9.6/README.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     7396 2016-11-25 15:17:14.000000 rucio-1.9.6/pylintrc
+-rw-r--r--   0 barisits (51071) zp        (1307)     1014 2016-11-25 15:17:14.000000 rucio-1.9.6/setup.cfg
+-rw-r--r--   0 barisits (51071) zp        (1307)     6459 2017-02-07 09:03:28.000000 rucio-1.9.6/setup.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      739 2017-02-07 09:03:32.000000 rucio-1.9.6/PKG-INFO
```

### Comparing `rucio-1.9.5/bin/rucio` & `rucio-1.9.6/bin/rucio`

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

### Comparing `rucio-1.9.5/bin/rucio-abacus-account` & `rucio-1.9.6/bin/rucio-abacus-account`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-abacus-rse` & `rucio-1.9.6/bin/rucio-abacus-rse`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-admin` & `rucio-1.9.6/bin/rucio-admin`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-atropos` & `rucio-1.9.6/bin/rucio-atropos`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-auditor` & `rucio-1.9.6/bin/rucio-auditor`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-automatix` & `rucio-1.9.6/bin/rucio-automatix`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-bb8` & `rucio-1.9.6/bin/rucio-bb8`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-c3po` & `rucio-1.9.6/bin/rucio-c3po`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-cache-client` & `rucio-1.9.6/bin/rucio-cache-client`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-cache-consumer` & `rucio-1.9.6/bin/rucio-cache-consumer`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-conveyor-finisher` & `rucio-1.9.6/bin/rucio-conveyor-finisher`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-conveyor-poller` & `rucio-1.9.6/bin/rucio-conveyor-poller`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-conveyor-poller-latest` & `rucio-1.9.6/bin/rucio-conveyor-poller-latest`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-conveyor-receiver` & `rucio-1.9.6/bin/rucio-conveyor-receiver`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-conveyor-stager` & `rucio-1.9.6/bin/rucio-conveyor-stager`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-conveyor-submitter` & `rucio-1.9.6/bin/rucio-conveyor-submitter`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-conveyor-throttler` & `rucio-1.9.6/bin/rucio-conveyor-throttler`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-conveyor-transfer-submitter` & `rucio-1.9.6/bin/rucio-conveyor-transfer-submitter`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-dark-reaper` & `rucio-1.9.6/bin/rucio-dark-reaper`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-dumper` & `rucio-1.9.6/bin/rucio-dumper`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-hermes` & `rucio-1.9.6/bin/rucio-hermes`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-judge-cleaner` & `rucio-1.9.6/bin/rucio-judge-cleaner`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-judge-evaluator` & `rucio-1.9.6/bin/rucio-judge-evaluator`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-judge-injector` & `rucio-1.9.6/bin/rucio-judge-injector`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-judge-repairer` & `rucio-1.9.6/bin/rucio-judge-repairer`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-kronos` & `rucio-1.9.6/bin/rucio-kronos`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-light-reaper` & `rucio-1.9.6/bin/rucio-light-reaper`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-necromancer` & `rucio-1.9.6/bin/rucio-necromancer`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-reaper` & `rucio-1.9.6/bin/rucio-reaper`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-transmogrifier` & `rucio-1.9.6/bin/rucio-transmogrifier`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/bin/rucio-undertaker` & `rucio-1.9.6/bin/rucio-undertaker`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/AN_atlaslogo.pdf` & `rucio-1.9.6/doc/atlasnote/AN_atlaslogo.pdf`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/AN_cernlogo.pdf` & `rucio-1.9.6/doc/atlasnote/AN_cernlogo.pdf`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/AtlasRucioNote.aux` & `rucio-1.9.6/doc/atlasnote/AtlasRucioNote.aux`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/AtlasRucioNote.pdf` & `rucio-1.9.6/doc/atlasnote/AtlasRucioNote.pdf`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/AtlasRucioNote.tex` & `rucio-1.9.6/doc/atlasnote/AtlasRucioNote.tex`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/accounts.graffle` & `rucio-1.9.6/doc/atlasnote/accounts.graffle`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/accounts.pdf` & `rucio-1.9.6/doc/atlasnote/accounts.pdf`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/accounts.png` & `rucio-1.9.6/doc/atlasnote/accounts.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/aggregation_hierarchy.graffle` & `rucio-1.9.6/doc/atlasnote/aggregation_hierarchy.graffle`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/aggregation_hierarchy.pdf` & `rucio-1.9.6/doc/atlasnote/aggregation_hierarchy.pdf`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/atlasnote.cls` & `rucio-1.9.6/doc/atlasnote/atlasnote.cls`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/booktabs.sty` & `rucio-1.9.6/doc/atlasnote/booktabs.sty`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/dataset_hierarchy.graffle` & `rucio-1.9.6/doc/atlasnote/dataset_hierarchy.graffle`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/dataset_hierarchy.pdf` & `rucio-1.9.6/doc/atlasnote/dataset_hierarchy.pdf`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/fncychap.sty` & `rucio-1.9.6/doc/atlasnote/fncychap.sty`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/sphinx.sty` & `rucio-1.9.6/doc/atlasnote/sphinx.sty`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/sphinxhowto.cls` & `rucio-1.9.6/doc/atlasnote/sphinxhowto.cls`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/atlasnote/sphinxmanual.cls` & `rucio-1.9.6/doc/atlasnote/sphinxmanual.cls`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/man/rucio-admin.doctree` & `rucio-1.9.6/doc/build/doctrees/man/rucio-admin.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/man/rucio.doctree` & `rucio-1.9.6/doc/build/doctrees/man/rucio.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/rest/attach_dids_to_dids.doctree` & `rucio-1.9.6/doc/build/doctrees/rest/attach_dids_to_dids.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/add_account_identity.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/add_account_identity.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/add_metadata_dataset.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/add_metadata_dataset.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/add_metadata_file.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/add_metadata_file.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/add_scope_to_account.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/add_scope_to_account.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/add_subscription.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/add_subscription.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/authentication.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/authentication.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/consistency_file_between_storage_and_rucio.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/consistency_file_between_storage_and_rucio.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/delete_file_replica_from_storage.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/delete_file_replica_from_storage.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/detect_site_reach_watermark.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/detect_site_reach_watermark.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/download_all_files_from_a_given_list_of_files_from_rucio.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/download_all_files_from_a_given_list_of_files_from_rucio.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/download_all_files_in_a_dataset_from_rucio.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/download_all_files_in_a_dataset_from_rucio.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/download_files_from_rucio.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/download_files_from_rucio.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/obsolete_dataset.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/obsolete_dataset.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/register_account.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/register_account.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/register_file_already_on_storage_system.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/register_file_already_on_storage_system.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/register_transfer_request_file_fts.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/register_transfer_request_file_fts.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/remove_replication_rules_from_file.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/remove_replication_rules_from_file.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/reupload_after_failure.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/reupload_after_failure.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/search.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/search.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/select_unwanted_files_for_deletion.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/select_unwanted_files_for_deletion.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/set_replication_rule_to_file.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/set_replication_rule_to_file.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/upload_file_with_replication_rule.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/upload_file_with_replication_rule.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/usecase_upload_file_into_rucio.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/usecase_upload_file_into_rucio.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases/where_are_the_replicas_for_a_file.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases/where_are_the_replicas_for_a_file.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/Acronyms_and_Abbreviations.doctree` & `rucio-1.9.6/doc/build/doctrees/Acronyms_and_Abbreviations.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/Architecture.doctree` & `rucio-1.9.6/doc/build/doctrees/Architecture.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/Comparison_matrix.doctree` & `rucio-1.9.6/doc/build/doctrees/Comparison_matrix.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/REST_Account.doctree` & `rucio-1.9.6/doc/build/doctrees/REST_Account.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/REST_Intro.doctree` & `rucio-1.9.6/doc/build/doctrees/REST_Intro.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/REST_authentication.doctree` & `rucio-1.9.6/doc/build/doctrees/REST_authentication.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/REST_did.doctree` & `rucio-1.9.6/doc/build/doctrees/REST_did.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/REST_identity.doctree` & `rucio-1.9.6/doc/build/doctrees/REST_identity.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/REST_lock.doctree` & `rucio-1.9.6/doc/build/doctrees/REST_lock.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/REST_meta.doctree` & `rucio-1.9.6/doc/build/doctrees/REST_meta.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/REST_redirect.doctree` & `rucio-1.9.6/doc/build/doctrees/REST_redirect.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/REST_replica.doctree` & `rucio-1.9.6/doc/build/doctrees/REST_replica.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/REST_rse.doctree` & `rucio-1.9.6/doc/build/doctrees/REST_rse.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/REST_rule.doctree` & `rucio-1.9.6/doc/build/doctrees/REST_rule.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/REST_scope.doctree` & `rucio-1.9.6/doc/build/doctrees/REST_scope.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/REST_subscription.doctree` & `rucio-1.9.6/doc/build/doctrees/REST_subscription.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/Rucio_Project_Meeting.doctree` & `rucio-1.9.6/doc/build/doctrees/Rucio_Project_Meeting.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/account.doctree` & `rucio-1.9.6/doc/build/doctrees/account.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/accountlimit.doctree` & `rucio-1.9.6/doc/build/doctrees/accountlimit.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/api_curl_examples.doctree` & `rucio-1.9.6/doc/build/doctrees/api_curl_examples.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/atlas_integration_testbed.doctree` & `rucio-1.9.6/doc/build/doctrees/atlas_integration_testbed.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/authentication_and_identity.doctree` & `rucio-1.9.6/doc/build/doctrees/authentication_and_identity.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/cli_admin_examples.doctree` & `rucio-1.9.6/doc/build/doctrees/cli_admin_examples.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/cli_examples.doctree` & `rucio-1.9.6/doc/build/doctrees/cli_examples.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/client_examples.doctree` & `rucio-1.9.6/doc/build/doctrees/client_examples.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/client_howto.doctree` & `rucio-1.9.6/doc/build/doctrees/client_howto.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/client_tutorial.doctree` & `rucio-1.9.6/doc/build/doctrees/client_tutorial.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/core_constants.doctree` & `rucio-1.9.6/doc/build/doctrees/core_constants.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/developing.doctree` & `rucio-1.9.6/doc/build/doctrees/developing.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/development_guidelines.doctree` & `rucio-1.9.6/doc/build/doctrees/development_guidelines.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/did.doctree` & `rucio-1.9.6/doc/build/doctrees/did.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/environment.pickle` & `rucio-1.9.6/doc/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/exception.doctree` & `rucio-1.9.6/doc/build/doctrees/exception.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/identity.doctree` & `rucio-1.9.6/doc/build/doctrees/identity.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/index.doctree` & `rucio-1.9.6/doc/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/installing_atlas_clients.doctree` & `rucio-1.9.6/doc/build/doctrees/installing_atlas_clients.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/installing_clients.doctree` & `rucio-1.9.6/doc/build/doctrees/installing_clients.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/installing_server.doctree` & `rucio-1.9.6/doc/build/doctrees/installing_server.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/lock.doctree` & `rucio-1.9.6/doc/build/doctrees/lock.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/meta-data.doctree` & `rucio-1.9.6/doc/build/doctrees/meta-data.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/naming_convention_db.doctree` & `rucio-1.9.6/doc/build/doctrees/naming_convention_db.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Accounting_and_quota.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Accounting_and_quota.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Architecture.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Architecture.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Data_Deletion.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Data_Deletion.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Database_Schema.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Database_Schema.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Deployment.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Deployment.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Exception_Handling.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Exception_Handling.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_File_Dataset_Container.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_File_Dataset_Container.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Meta-data_attributes.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Meta-data_attributes.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Notifications.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Notifications.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Permission_model.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Permission_model.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Replica_management.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Replica_management.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Rucio_Storage_Element.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Rucio_Storage_Element.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Rucio_Storage_Element_Manager.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Rucio_Storage_Element_Manager.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Rucio_account.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Rucio_account.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Rules.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Rules.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Scheduled_Transfers.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Scheduled_Transfers.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Subscriptions.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Subscriptions.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_Traceability_and_logging.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_Traceability_and_logging.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/overview_flow.doctree` & `rucio-1.9.6/doc/build/doctrees/overview_flow.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/permission.doctree` & `rucio-1.9.6/doc/build/doctrees/permission.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/replica.doctree` & `rucio-1.9.6/doc/build/doctrees/replica.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/replication_rules_examples.doctree` & `rucio-1.9.6/doc/build/doctrees/replication_rules_examples.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/rest.doctree` & `rucio-1.9.6/doc/build/doctrees/rest.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/rse.doctree` & `rucio-1.9.6/doc/build/doctrees/rse.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/rucio_cli.doctree` & `rucio-1.9.6/doc/build/doctrees/rucio_cli.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/rucio_clients.doctree` & `rucio-1.9.6/doc/build/doctrees/rucio_clients.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/rule.doctree` & `rucio-1.9.6/doc/build/doctrees/rule.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/rules_workflow.doctree` & `rucio-1.9.6/doc/build/doctrees/rules_workflow.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/scope.doctree` & `rucio-1.9.6/doc/build/doctrees/scope.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/setup.doctree` & `rucio-1.9.6/doc/build/doctrees/setup.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/subscription.doctree` & `rucio-1.9.6/doc/build/doctrees/subscription.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/doctrees/usecases.doctree` & `rucio-1.9.6/doc/build/doctrees/usecases.doctree`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_images/RSE_overview.png` & `rucio-1.9.6/doc/build/html/_images/RSE_overview.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_images/RSE_sequence_instantiation.png` & `rucio-1.9.6/doc/build/html/_images/RSE_sequence_instantiation.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_images/RSE_sequence_usage.png` & `rucio-1.9.6/doc/build/html/_images/RSE_sequence_usage.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_images/accounts.png` & `rucio-1.9.6/doc/build/html/_images/accounts.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_images/architecture.png` & `rucio-1.9.6/doc/build/html/_images/architecture.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_images/deployment.png` & `rucio-1.9.6/doc/build/html/_images/deployment.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_images/exception_handling.png` & `rucio-1.9.6/doc/build/html/_images/exception_handling.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_images/rucio-get.png` & `rucio-1.9.6/doc/build/html/_images/rucio-get.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_images/rucio-put.png` & `rucio-1.9.6/doc/build/html/_images/rucio-put.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_images/rucio-register.png` & `rucio-1.9.6/doc/build/html/_images/rucio-register.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_images/rucio_schema.png` & `rucio-1.9.6/doc/build/html/_images/rucio_schema.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_images/scheduled_transfers.png` & `rucio-1.9.6/doc/build/html/_images/scheduled_transfers.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/rucio/api/identity.html` & `rucio-1.9.6/doc/build/html/_modules/rucio/api/identity.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/rucio/api/permission.html` & `rucio-1.9.6/doc/build/html/_modules/rucio/api/permission.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/rucio/client/accountclient.html` & `rucio-1.9.6/doc/build/html/_modules/rucio/client/accountclient.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/rucio/client/accountlimitclient.html` & `rucio-1.9.6/doc/build/html/_modules/rucio/client/accountlimitclient.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/rucio/client/didclient.html` & `rucio-1.9.6/doc/build/html/_modules/rucio/client/didclient.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/rucio/client/lockclient.html` & `rucio-1.9.6/doc/build/html/_modules/rucio/client/lockclient.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/rucio/client/metaclient.html` & `rucio-1.9.6/doc/build/html/_modules/rucio/client/metaclient.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/rucio/client/rseclient.html` & `rucio-1.9.6/doc/build/html/_modules/rucio/client/rseclient.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/rucio/client/ruleclient.html` & `rucio-1.9.6/doc/build/html/_modules/rucio/client/ruleclient.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/rucio/client/scopeclient.html` & `rucio-1.9.6/doc/build/html/_modules/rucio/client/scopeclient.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/rucio/client/subscriptionclient.html` & `rucio-1.9.6/doc/build/html/_modules/rucio/client/subscriptionclient.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/rucio/common/exception.html` & `rucio-1.9.6/doc/build/html/_modules/rucio/common/exception.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/rucio/db/constants.html` & `rucio-1.9.6/doc/build/html/_modules/rucio/db/constants.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/rucio/db/enum.html` & `rucio-1.9.6/doc/build/html/_modules/rucio/db/enum.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/rucio/rse/protocols/protocol.html` & `rucio-1.9.6/doc/build/html/_modules/rucio/rse/protocols/protocol.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/rucio/web/rest/ping.html` & `rucio-1.9.6/doc/build/html/_modules/rucio/web/rest/ping.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_modules/index.html` & `rucio-1.9.6/doc/build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/man/rucio-admin.txt` & `rucio-1.9.6/doc/build/html/_sources/man/rucio-admin.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/man/rucio.txt` & `rucio-1.9.6/doc/build/html/_sources/man/rucio.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/add_account_identity.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/add_account_identity.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/add_metadata_dataset.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/add_metadata_dataset.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/add_metadata_file.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/add_metadata_file.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/add_scope_to_account.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/add_scope_to_account.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/add_subscription.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/add_subscription.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/authentication.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/authentication.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/consistency_file_between_storage_and_rucio.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/consistency_file_between_storage_and_rucio.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/delete_file_replica_from_storage.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/delete_file_replica_from_storage.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/detect_site_reach_watermark.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/detect_site_reach_watermark.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/download_all_files_from_a_given_list_of_files_from_rucio.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/download_all_files_from_a_given_list_of_files_from_rucio.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/download_all_files_in_a_dataset_from_rucio.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/download_all_files_in_a_dataset_from_rucio.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/download_files_from_rucio.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/download_files_from_rucio.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/obsolete_dataset.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/obsolete_dataset.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/register_account.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/register_account.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/register_file_already_on_storage_system.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/register_file_already_on_storage_system.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/register_transfer_request_file_fts.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/register_transfer_request_file_fts.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/remove_replication_rules_from_file.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/remove_replication_rules_from_file.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/reupload_after_failure.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/reupload_after_failure.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/search.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/search.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/set_replication_rule_to_file.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/set_replication_rule_to_file.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/upload_file_with_replication_rule.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/upload_file_with_replication_rule.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/usecase_upload_file_into_rucio.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/usecase_upload_file_into_rucio.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases/where_are_the_replicas_for_a_file.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases/where_are_the_replicas_for_a_file.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/Comparison_matrix.txt` & `rucio-1.9.6/doc/build/html/_sources/Comparison_matrix.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/REST_Account.txt` & `rucio-1.9.6/doc/build/html/_sources/REST_Account.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/REST_Intro.txt` & `rucio-1.9.6/doc/build/html/_sources/REST_Intro.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/REST_authentication.txt` & `rucio-1.9.6/doc/build/html/_sources/REST_authentication.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/REST_did.txt` & `rucio-1.9.6/doc/build/html/_sources/REST_did.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/REST_identity.txt` & `rucio-1.9.6/doc/build/html/_sources/REST_identity.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/REST_lock.txt` & `rucio-1.9.6/doc/build/html/_sources/REST_lock.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/REST_meta.txt` & `rucio-1.9.6/doc/build/html/_sources/REST_meta.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/REST_replica.txt` & `rucio-1.9.6/doc/build/html/_sources/REST_replica.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/REST_rse.txt` & `rucio-1.9.6/doc/build/html/_sources/REST_rse.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/REST_rule.txt` & `rucio-1.9.6/doc/build/html/_sources/REST_rule.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/REST_scope.txt` & `rucio-1.9.6/doc/build/html/_sources/REST_scope.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/REST_subscription.txt` & `rucio-1.9.6/doc/build/html/_sources/REST_subscription.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/Rucio_Project_Meeting.txt` & `rucio-1.9.6/doc/build/html/_sources/Rucio_Project_Meeting.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/api_curl_examples.txt` & `rucio-1.9.6/doc/build/html/_sources/api_curl_examples.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/atlas_integration_testbed.txt` & `rucio-1.9.6/doc/build/html/_sources/atlas_integration_testbed.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/cli_admin_examples.txt` & `rucio-1.9.6/doc/build/html/_sources/cli_admin_examples.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/cli_examples.txt` & `rucio-1.9.6/doc/build/html/_sources/cli_examples.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/client_examples.txt` & `rucio-1.9.6/doc/build/html/_sources/client_examples.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/client_howto.txt` & `rucio-1.9.6/doc/build/html/_sources/client_howto.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/client_tutorial.txt` & `rucio-1.9.6/doc/build/html/_sources/client_tutorial.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/developing.txt` & `rucio-1.9.6/doc/build/html/_sources/developing.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/development_guidelines.txt` & `rucio-1.9.6/doc/build/html/_sources/development_guidelines.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/index.txt` & `rucio-1.9.6/doc/build/html/_sources/index.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/installing_atlas_clients.txt` & `rucio-1.9.6/doc/build/html/_sources/installing_atlas_clients.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/installing_clients.txt` & `rucio-1.9.6/doc/build/html/_sources/installing_clients.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/installing_server.txt` & `rucio-1.9.6/doc/build/html/_sources/installing_server.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/naming_convention_db.txt` & `rucio-1.9.6/doc/build/html/_sources/naming_convention_db.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/overview_Data_Deletion.txt` & `rucio-1.9.6/doc/build/html/_sources/overview_Data_Deletion.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/overview_Exception_Handling.txt` & `rucio-1.9.6/doc/build/html/_sources/overview_Exception_Handling.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/overview_File_Dataset_Container.txt` & `rucio-1.9.6/doc/build/html/_sources/overview_File_Dataset_Container.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/overview_Meta-data_attributes.txt` & `rucio-1.9.6/doc/build/html/_sources/overview_Meta-data_attributes.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/overview_Replica_management.txt` & `rucio-1.9.6/doc/build/html/_sources/overview_Replica_management.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/overview_Rucio_Storage_Element.txt` & `rucio-1.9.6/doc/build/html/_sources/overview_Rucio_Storage_Element.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/overview_Rucio_Storage_Element_Manager.txt` & `rucio-1.9.6/doc/build/html/_sources/overview_Rucio_Storage_Element_Manager.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/overview_Rucio_account.txt` & `rucio-1.9.6/doc/build/html/_sources/overview_Rucio_account.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/overview_Rules.txt` & `rucio-1.9.6/doc/build/html/_sources/overview_Rules.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/overview_Scheduled_Transfers.txt` & `rucio-1.9.6/doc/build/html/_sources/overview_Scheduled_Transfers.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/overview_Subscriptions.txt` & `rucio-1.9.6/doc/build/html/_sources/overview_Subscriptions.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/replication_rules_examples.txt` & `rucio-1.9.6/doc/build/html/_sources/replication_rules_examples.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/rest.txt` & `rucio-1.9.6/doc/build/html/_sources/rest.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/rucio_cli.txt` & `rucio-1.9.6/doc/build/html/_sources/rucio_cli.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/rucio_clients.txt` & `rucio-1.9.6/doc/build/html/_sources/rucio_clients.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/rules_workflow.txt` & `rucio-1.9.6/doc/build/html/_sources/rules_workflow.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/setup.txt` & `rucio-1.9.6/doc/build/html/_sources/setup.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_sources/usecases.txt` & `rucio-1.9.6/doc/build/html/_sources/usecases.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/ajax-loader.gif` & `rucio-1.9.6/doc/build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/basic.css` & `rucio-1.9.6/doc/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/classic.css` & `rucio-1.9.6/doc/build/html/_static/classic.css`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/comment-bright.png` & `rucio-1.9.6/doc/build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/comment-close.png` & `rucio-1.9.6/doc/build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/comment.png` & `rucio-1.9.6/doc/build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/default.css` & `rucio-1.9.6/doc/build/html/_static/default.css`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/doctools.js` & `rucio-1.9.6/doc/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/jquery-1.11.1.js` & `rucio-1.9.6/doc/build/html/_static/jquery-1.11.1.js`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/jquery.js` & `rucio-1.9.6/doc/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/pygments.css` & `rucio-1.9.6/doc/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/rucio_logo.png` & `rucio-1.9.6/doc/build/html/_static/rucio_logo.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/searchtools.js` & `rucio-1.9.6/doc/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/sidebar.js` & `rucio-1.9.6/doc/build/html/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/underscore-1.3.1.js` & `rucio-1.9.6/doc/build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/underscore.js` & `rucio-1.9.6/doc/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/_static/websupport.js` & `rucio-1.9.6/doc/build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/man/rucio-admin.html` & `rucio-1.9.6/doc/build/html/man/rucio-admin.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/man/rucio.html` & `rucio-1.9.6/doc/build/html/man/rucio.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/rest/attach_dids_to_dids.html` & `rucio-1.9.6/doc/build/html/rest/attach_dids_to_dids.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/add_account_identity.html` & `rucio-1.9.6/doc/build/html/usecases/add_account_identity.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/add_metadata_dataset.html` & `rucio-1.9.6/doc/build/html/usecases/add_metadata_dataset.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/add_metadata_file.html` & `rucio-1.9.6/doc/build/html/usecases/add_metadata_file.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/add_scope_to_account.html` & `rucio-1.9.6/doc/build/html/usecases/add_scope_to_account.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/add_subscription.html` & `rucio-1.9.6/doc/build/html/usecases/add_subscription.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/authentication.html` & `rucio-1.9.6/doc/build/html/usecases/authentication.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/consistency_file_between_storage_and_rucio.html` & `rucio-1.9.6/doc/build/html/usecases/consistency_file_between_storage_and_rucio.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/delete_file_replica_from_storage.html` & `rucio-1.9.6/doc/build/html/usecases/delete_file_replica_from_storage.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/detect_site_reach_watermark.html` & `rucio-1.9.6/doc/build/html/usecases/detect_site_reach_watermark.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.html` & `rucio-1.9.6/doc/build/html/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/download_all_files_from_a_given_list_of_files_from_rucio.html` & `rucio-1.9.6/doc/build/html/usecases/download_all_files_from_a_given_list_of_files_from_rucio.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/download_all_files_in_a_dataset_from_rucio.html` & `rucio-1.9.6/doc/build/html/usecases/download_all_files_in_a_dataset_from_rucio.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/download_files_from_rucio.html` & `rucio-1.9.6/doc/build/html/usecases/download_files_from_rucio.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/obsolete_dataset.html` & `rucio-1.9.6/doc/build/html/usecases/obsolete_dataset.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/register_account.html` & `rucio-1.9.6/doc/build/html/usecases/register_account.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/register_file_already_on_storage_system.html` & `rucio-1.9.6/doc/build/html/usecases/register_file_already_on_storage_system.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/register_transfer_request_file_fts.html` & `rucio-1.9.6/doc/build/html/usecases/register_transfer_request_file_fts.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/remove_replication_rules_from_file.html` & `rucio-1.9.6/doc/build/html/usecases/remove_replication_rules_from_file.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/reupload_after_failure.html` & `rucio-1.9.6/doc/build/html/usecases/reupload_after_failure.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/search.html` & `rucio-1.9.6/doc/build/html/usecases/search.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/select_unwanted_files_for_deletion.html` & `rucio-1.9.6/doc/build/html/usecases/select_unwanted_files_for_deletion.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/set_replication_rule_to_file.html` & `rucio-1.9.6/doc/build/html/usecases/set_replication_rule_to_file.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/upload_file_with_replication_rule.html` & `rucio-1.9.6/doc/build/html/usecases/upload_file_with_replication_rule.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/usecase_upload_file_into_rucio.html` & `rucio-1.9.6/doc/build/html/usecases/usecase_upload_file_into_rucio.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases/where_are_the_replicas_for_a_file.html` & `rucio-1.9.6/doc/build/html/usecases/where_are_the_replicas_for_a_file.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/Acronyms_and_Abbreviations.html` & `rucio-1.9.6/doc/build/html/Acronyms_and_Abbreviations.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/Architecture.html` & `rucio-1.9.6/doc/build/html/Architecture.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/Comparison_matrix.html` & `rucio-1.9.6/doc/build/html/Comparison_matrix.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/REST_Account.html` & `rucio-1.9.6/doc/build/html/REST_Account.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/REST_Intro.html` & `rucio-1.9.6/doc/build/html/REST_Intro.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/REST_authentication.html` & `rucio-1.9.6/doc/build/html/REST_authentication.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/REST_did.html` & `rucio-1.9.6/doc/build/html/REST_did.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/REST_identity.html` & `rucio-1.9.6/doc/build/html/REST_identity.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/REST_lock.html` & `rucio-1.9.6/doc/build/html/REST_lock.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/REST_meta.html` & `rucio-1.9.6/doc/build/html/REST_meta.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/REST_redirect.html` & `rucio-1.9.6/doc/build/html/REST_redirect.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/REST_replica.html` & `rucio-1.9.6/doc/build/html/REST_replica.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/REST_rse.html` & `rucio-1.9.6/doc/build/html/REST_rse.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/REST_rule.html` & `rucio-1.9.6/doc/build/html/REST_rule.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/REST_scope.html` & `rucio-1.9.6/doc/build/html/REST_scope.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/REST_subscription.html` & `rucio-1.9.6/doc/build/html/REST_subscription.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/Rucio_Project_Meeting.html` & `rucio-1.9.6/doc/build/html/Rucio_Project_Meeting.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/account.html` & `rucio-1.9.6/doc/build/html/account.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/accountlimit.html` & `rucio-1.9.6/doc/build/html/accountlimit.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/api_curl_examples.html` & `rucio-1.9.6/doc/build/html/api_curl_examples.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/atlas_integration_testbed.html` & `rucio-1.9.6/doc/build/html/atlas_integration_testbed.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/authentication_and_identity.html` & `rucio-1.9.6/doc/build/html/authentication_and_identity.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/cli_admin_examples.html` & `rucio-1.9.6/doc/build/html/cli_admin_examples.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/cli_examples.html` & `rucio-1.9.6/doc/build/html/cli_examples.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/client_examples.html` & `rucio-1.9.6/doc/build/html/client_examples.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/client_howto.html` & `rucio-1.9.6/doc/build/html/client_howto.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/client_tutorial.html` & `rucio-1.9.6/doc/build/html/client_tutorial.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/core_constants.html` & `rucio-1.9.6/doc/build/html/core_constants.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/developing.html` & `rucio-1.9.6/doc/build/html/developing.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/development_guidelines.html` & `rucio-1.9.6/doc/build/html/development_guidelines.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/did.html` & `rucio-1.9.6/doc/build/html/did.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/exception.html` & `rucio-1.9.6/doc/build/html/exception.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/genindex.html` & `rucio-1.9.6/doc/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/http-routingtable.html` & `rucio-1.9.6/doc/build/html/http-routingtable.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/identity.html` & `rucio-1.9.6/doc/build/html/identity.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/index.html` & `rucio-1.9.6/doc/build/html/index.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/installing_atlas_clients.html` & `rucio-1.9.6/doc/build/html/installing_atlas_clients.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/installing_clients.html` & `rucio-1.9.6/doc/build/html/installing_clients.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/installing_server.html` & `rucio-1.9.6/doc/build/html/installing_server.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/lock.html` & `rucio-1.9.6/doc/build/html/lock.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/meta-data.html` & `rucio-1.9.6/doc/build/html/meta-data.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/naming_convention_db.html` & `rucio-1.9.6/doc/build/html/naming_convention_db.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/objects.inv` & `rucio-1.9.6/doc/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Accounting_and_quota.html` & `rucio-1.9.6/doc/build/html/overview_Accounting_and_quota.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Architecture.html` & `rucio-1.9.6/doc/build/html/overview_Architecture.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Data_Deletion.html` & `rucio-1.9.6/doc/build/html/overview_Data_Deletion.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Database_Schema.html` & `rucio-1.9.6/doc/build/html/overview_Database_Schema.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Deployment.html` & `rucio-1.9.6/doc/build/html/overview_Deployment.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Exception_Handling.html` & `rucio-1.9.6/doc/build/html/overview_Exception_Handling.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_File_Dataset_Container.html` & `rucio-1.9.6/doc/build/html/overview_File_Dataset_Container.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Meta-data_attributes.html` & `rucio-1.9.6/doc/build/html/overview_Meta-data_attributes.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Notifications.html` & `rucio-1.9.6/doc/build/html/overview_Notifications.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Permission_model.html` & `rucio-1.9.6/doc/build/html/overview_Permission_model.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Replica_management.html` & `rucio-1.9.6/doc/build/html/overview_Replica_management.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Rucio_Storage_Element.html` & `rucio-1.9.6/doc/build/html/overview_Rucio_Storage_Element.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Rucio_Storage_Element_Manager.html` & `rucio-1.9.6/doc/build/html/overview_Rucio_Storage_Element_Manager.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Rucio_account.html` & `rucio-1.9.6/doc/build/html/overview_Rucio_account.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Rules.html` & `rucio-1.9.6/doc/build/html/overview_Rules.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Scheduled_Transfers.html` & `rucio-1.9.6/doc/build/html/overview_Scheduled_Transfers.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Subscriptions.html` & `rucio-1.9.6/doc/build/html/overview_Subscriptions.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_Traceability_and_logging.html` & `rucio-1.9.6/doc/build/html/overview_Traceability_and_logging.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/overview_flow.html` & `rucio-1.9.6/doc/build/html/overview_flow.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/permission.html` & `rucio-1.9.6/doc/build/html/permission.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/py-modindex.html` & `rucio-1.9.6/doc/build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/replica.html` & `rucio-1.9.6/doc/build/html/replica.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/replication_rules_examples.html` & `rucio-1.9.6/doc/build/html/replication_rules_examples.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/rest.html` & `rucio-1.9.6/doc/build/html/rest.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/rse.html` & `rucio-1.9.6/doc/build/html/rse.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/rucio_cli.html` & `rucio-1.9.6/doc/build/html/rucio_cli.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/rucio_clients.html` & `rucio-1.9.6/doc/build/html/rucio_clients.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/rule.html` & `rucio-1.9.6/doc/build/html/rule.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/rules_workflow.html` & `rucio-1.9.6/doc/build/html/rules_workflow.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/scope.html` & `rucio-1.9.6/doc/build/html/scope.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/search.html` & `rucio-1.9.6/doc/build/html/search.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/searchindex.js` & `rucio-1.9.6/doc/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/setup.html` & `rucio-1.9.6/doc/build/html/setup.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/subscription.html` & `rucio-1.9.6/doc/build/html/subscription.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/build/html/usecases.html` & `rucio-1.9.6/doc/build/html/usecases.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/design/RSE/meeting-2012-02-23.org` & `rucio-1.9.6/doc/design/RSE/meeting-2012-02-23.org`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/design/erd/ERD.graffle` & `rucio-1.9.6/doc/design/erd/ERD.graffle`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/design/erd/ERD.pdf` & `rucio-1.9.6/doc/design/erd/ERD.pdf`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/design/rucio_schema.pdf` & `rucio-1.9.6/doc/design/rucio_schema.pdf`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/_static/basic.css` & `rucio-1.9.6/doc/source/_static/basic.css`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/_static/classic.css` & `rucio-1.9.6/doc/source/_static/classic.css`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/_static/default.css` & `rucio-1.9.6/doc/source/_static/default.css`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/_static/rucio_logo.png` & `rucio-1.9.6/doc/source/_static/rucio_logo.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/_templates/layout.html` & `rucio-1.9.6/doc/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/curl_examples/get_account_whoami.out` & `rucio-1.9.6/doc/source/curl_examples/get_account_whoami.out`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/example_outputs/failure-rucio.tests.test_curl.TestCurlRucio.test_get_accounts_whoami.txt` & `rucio-1.9.6/doc/source/example_outputs/failure-rucio.tests.test_curl.TestCurlRucio.test_get_accounts_whoami.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_accounts_whoami.txt` & `rucio-1.9.6/doc/source/example_outputs/success-rucio.tests.test_curl.TestCurlRucio.test_get_accounts_whoami.txt`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/deployment.graffle/QuickLook/Preview.pdf` & `rucio-1.9.6/doc/source/images/deployment.graffle/QuickLook/Preview.pdf`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/deployment.graffle/QuickLook/Thumbnail.tiff` & `rucio-1.9.6/doc/source/images/deployment.graffle/QuickLook/Thumbnail.tiff`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/deployment.graffle/data.plist` & `rucio-1.9.6/doc/source/images/deployment.graffle/data.plist`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/deployment.graffle/image2.tiff` & `rucio-1.9.6/doc/source/images/deployment.graffle/image2.tiff`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/deployment.graffle/image3.tiff` & `rucio-1.9.6/doc/source/images/deployment.graffle/image3.tiff`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/RSE_overview.png` & `rucio-1.9.6/doc/source/images/RSE_overview.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/RSE_sequence_instantiation.png` & `rucio-1.9.6/doc/source/images/RSE_sequence_instantiation.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/RSE_sequence_usage.png` & `rucio-1.9.6/doc/source/images/RSE_sequence_usage.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/accounts.png` & `rucio-1.9.6/doc/source/images/accounts.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/architecture.graffle` & `rucio-1.9.6/doc/source/images/architecture.graffle`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/architecture.png` & `rucio-1.9.6/doc/source/images/architecture.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/deployment.png` & `rucio-1.9.6/doc/source/images/deployment.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/exception_handling.graffle` & `rucio-1.9.6/doc/source/images/exception_handling.graffle`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/exception_handling.png` & `rucio-1.9.6/doc/source/images/exception_handling.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/highLevelRoadmap.graffle` & `rucio-1.9.6/doc/source/images/highLevelRoadmap.graffle`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/rucio-get.graffle` & `rucio-1.9.6/doc/source/images/rucio-get.graffle`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/rucio-get.png` & `rucio-1.9.6/doc/source/images/rucio-get.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/rucio-put.graffle` & `rucio-1.9.6/doc/source/images/rucio-put.graffle`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/rucio-put.png` & `rucio-1.9.6/doc/source/images/rucio-put.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/rucio-register.graffle` & `rucio-1.9.6/doc/source/images/rucio-register.graffle`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/rucio-register.png` & `rucio-1.9.6/doc/source/images/rucio-register.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/rucio_schema.gml` & `rucio-1.9.6/doc/source/images/rucio_schema.gml`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/rucio_schema.pdf` & `rucio-1.9.6/doc/source/images/rucio_schema.pdf`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/rucio_schema.png` & `rucio-1.9.6/doc/source/images/rucio_schema.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/scheduled_transfers.dia` & `rucio-1.9.6/doc/source/images/scheduled_transfers.dia`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/images/scheduled_transfers.png` & `rucio-1.9.6/doc/source/images/scheduled_transfers.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/man/rucio-admin.rst` & `rucio-1.9.6/doc/source/man/rucio-admin.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/man/rucio.rst` & `rucio-1.9.6/doc/source/man/rucio.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/add_account_identity.rst` & `rucio-1.9.6/doc/source/usecases/add_account_identity.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/add_metadata_dataset.rst` & `rucio-1.9.6/doc/source/usecases/add_metadata_dataset.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/add_metadata_file.rst` & `rucio-1.9.6/doc/source/usecases/add_metadata_file.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/add_scope_to_account.rst` & `rucio-1.9.6/doc/source/usecases/add_scope_to_account.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/add_subscription.rst` & `rucio-1.9.6/doc/source/usecases/add_subscription.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/authentication.rst` & `rucio-1.9.6/doc/source/usecases/authentication.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/consistency_file_between_storage_and_rucio.rst` & `rucio-1.9.6/doc/source/usecases/consistency_file_between_storage_and_rucio.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/delete_file_replica_from_storage.rst` & `rucio-1.9.6/doc/source/usecases/delete_file_replica_from_storage.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/detect_site_reach_watermark.rst` & `rucio-1.9.6/doc/source/usecases/detect_site_reach_watermark.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.rst` & `rucio-1.9.6/doc/source/usecases/download_all_files_from_a_given_list_of_file_replicas_from_rucio.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/download_all_files_from_a_given_list_of_files_from_rucio.rst` & `rucio-1.9.6/doc/source/usecases/download_all_files_from_a_given_list_of_files_from_rucio.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/download_all_files_in_a_dataset_from_rucio.rst` & `rucio-1.9.6/doc/source/usecases/download_all_files_in_a_dataset_from_rucio.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/download_files_from_rucio.rst` & `rucio-1.9.6/doc/source/usecases/download_files_from_rucio.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/obsolete_dataset.rst` & `rucio-1.9.6/doc/source/usecases/obsolete_dataset.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/register_account.rst` & `rucio-1.9.6/doc/source/usecases/register_account.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/register_file_already_on_storage_system.rst` & `rucio-1.9.6/doc/source/usecases/register_file_already_on_storage_system.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/register_transfer_request_file_fts.rst` & `rucio-1.9.6/doc/source/usecases/register_transfer_request_file_fts.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/remove_replication_rules_from_file.rst` & `rucio-1.9.6/doc/source/usecases/remove_replication_rules_from_file.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/reupload_after_failure.rst` & `rucio-1.9.6/doc/source/usecases/reupload_after_failure.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/search.rst` & `rucio-1.9.6/doc/source/usecases/search.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/set_replication_rule_to_file.rst` & `rucio-1.9.6/doc/source/usecases/set_replication_rule_to_file.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/upload_file_with_replication_rule.rst` & `rucio-1.9.6/doc/source/usecases/upload_file_with_replication_rule.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/usecase_upload_file_into_rucio.rst` & `rucio-1.9.6/doc/source/usecases/usecase_upload_file_into_rucio.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases/where_are_the_replicas_for_a_file.rst` & `rucio-1.9.6/doc/source/usecases/where_are_the_replicas_for_a_file.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/Comparison_matrix.rst` & `rucio-1.9.6/doc/source/Comparison_matrix.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/REST_Account.rst` & `rucio-1.9.6/doc/source/REST_Account.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/REST_Intro.rst` & `rucio-1.9.6/doc/source/REST_Intro.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/REST_authentication.rst` & `rucio-1.9.6/doc/source/REST_authentication.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/REST_did.rst` & `rucio-1.9.6/doc/source/REST_did.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/REST_identity.rst` & `rucio-1.9.6/doc/source/REST_identity.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/REST_lock.rst` & `rucio-1.9.6/doc/source/REST_lock.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/REST_meta.rst` & `rucio-1.9.6/doc/source/REST_meta.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/REST_replica.rst` & `rucio-1.9.6/doc/source/REST_replica.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/REST_rse.rst` & `rucio-1.9.6/doc/source/REST_rse.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/REST_rule.rst` & `rucio-1.9.6/doc/source/REST_rule.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/REST_scope.rst` & `rucio-1.9.6/doc/source/REST_scope.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/REST_subscription.rst` & `rucio-1.9.6/doc/source/REST_subscription.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/RSE_Expressions.rst` & `rucio-1.9.6/doc/source/RSE_Expressions.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/Rucio_Project_Meeting.rst` & `rucio-1.9.6/doc/source/Rucio_Project_Meeting.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/accounts.pdf` & `rucio-1.9.6/doc/source/accounts.pdf`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/accounts.png` & `rucio-1.9.6/doc/source/accounts.png`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/api_curl_examples.rst` & `rucio-1.9.6/doc/source/api_curl_examples.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/atlas_integration_testbed.rst` & `rucio-1.9.6/doc/source/atlas_integration_testbed.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/cli_admin_examples.rst` & `rucio-1.9.6/doc/source/cli_admin_examples.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/cli_examples.rst` & `rucio-1.9.6/doc/source/cli_examples.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/client_examples.rst` & `rucio-1.9.6/doc/source/client_examples.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/client_tutorial.rst` & `rucio-1.9.6/doc/source/client_tutorial.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/conf.py` & `rucio-1.9.6/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/developing.rst` & `rucio-1.9.6/doc/source/developing.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/development_guidelines.rst` & `rucio-1.9.6/doc/source/development_guidelines.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/index.rst` & `rucio-1.9.6/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/installing_atlas_clients.rst` & `rucio-1.9.6/doc/source/installing_atlas_clients.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/installing_clients.rst` & `rucio-1.9.6/doc/source/installing_clients.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/installing_server.rst` & `rucio-1.9.6/doc/source/installing_server.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/naming_convention_db.rst` & `rucio-1.9.6/doc/source/naming_convention_db.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/overview_Data_Deletion.rst` & `rucio-1.9.6/doc/source/overview_Data_Deletion.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/overview_Exception_Handling.rst` & `rucio-1.9.6/doc/source/overview_Exception_Handling.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/overview_File_Dataset_Container.rst` & `rucio-1.9.6/doc/source/overview_File_Dataset_Container.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/overview_Meta-data_attributes.rst` & `rucio-1.9.6/doc/source/overview_Meta-data_attributes.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/overview_Replica_management.rst` & `rucio-1.9.6/doc/source/overview_Replica_management.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/overview_Rucio_Storage_Element.rst` & `rucio-1.9.6/doc/source/overview_Rucio_Storage_Element.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/overview_Rucio_Storage_Element_Manager.rst` & `rucio-1.9.6/doc/source/overview_Rucio_Storage_Element_Manager.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/overview_Rucio_account.rst` & `rucio-1.9.6/doc/source/overview_Rucio_account.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/overview_Rules.rst` & `rucio-1.9.6/doc/source/overview_Rules.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/overview_Scheduled_Transfers.rst` & `rucio-1.9.6/doc/source/overview_Scheduled_Transfers.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/overview_Subscriptions.rst` & `rucio-1.9.6/doc/source/overview_Subscriptions.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/replication_rules_examples.rst` & `rucio-1.9.6/doc/source/replication_rules_examples.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/rest.rst` & `rucio-1.9.6/doc/source/rest.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/rucio_cli.rst` & `rucio-1.9.6/doc/source/rucio_cli.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/rucio_clients.rst` & `rucio-1.9.6/doc/source/rucio_clients.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/rules_workflow.rst` & `rucio-1.9.6/doc/source/rules_workflow.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/source/usecases.rst` & `rucio-1.9.6/doc/source/usecases.rst`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/Makefile` & `rucio-1.9.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/doc/make.bat` & `rucio-1.9.6/doc/make.bat`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/etc/mail_templates/rule_approval_request.tmpl` & `rucio-1.9.6/etc/mail_templates/rule_approval_request.tmpl`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/etc/mail_templates/rule_ok_notification.tmpl` & `rucio-1.9.6/etc/mail_templates/rule_ok_notification.tmpl`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/etc/schemas/sub_filter.json` & `rucio-1.9.6/etc/schemas/sub_filter.json`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/etc/web/httpd-rucio-443-py26-slc6.conf.template` & `rucio-1.9.6/etc/web/httpd-rucio-443-py26-slc6.conf.template`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/etc/web/httpd-rucio-443-py27-cc7.conf.template` & `rucio-1.9.6/etc/web/httpd-rucio-443-py27-cc7.conf.template`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/etc/web/httpd-rucio-443-py27-debian.conf.template` & `rucio-1.9.6/etc/web/httpd-rucio-443-py27-debian.conf.template`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/etc/web/httpd-rucio-443-py27-osx.conf.template` & `rucio-1.9.6/etc/web/httpd-rucio-443-py27-osx.conf.template`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/etc/web/httpd-rucio-443-py27-ubuntu.conf.template` & `rucio-1.9.6/etc/web/httpd-rucio-443-py27-ubuntu.conf.template`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/etc/alembic.ini.template` & `rucio-1.9.6/etc/alembic.ini.template`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/etc/ldap.cfg.template` & `rucio-1.9.6/etc/ldap.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/etc/rse-accounts.cfg.template` & `rucio-1.9.6/etc/rse-accounts.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/etc/rucio.cfg.atlas.client.template` & `rucio-1.9.6/etc/rucio.cfg.atlas.client.template`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/etc/rucio.cfg.template` & `rucio-1.9.6/etc/rucio.cfg.template`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/account.py` & `rucio-1.9.6/lib/rucio/api/account.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/account_limit.py` & `rucio-1.9.6/lib/rucio/api/account_limit.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/authentication.py` & `rucio-1.9.6/lib/rucio/api/authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/availability.py` & `rucio-1.9.6/lib/rucio/api/availability.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/config.py` & `rucio-1.9.6/lib/rucio/api/config.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/did.py` & `rucio-1.9.6/lib/rucio/api/did.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/heartbeat.py` & `rucio-1.9.6/lib/rucio/api/heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/identity.py` & `rucio-1.9.6/lib/rucio/api/identity.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/lock.py` & `rucio-1.9.6/lib/rucio/api/lock.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/meta.py` & `rucio-1.9.6/lib/rucio/api/meta.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/permission.py` & `rucio-1.9.6/lib/rucio/api/permission.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/replica.py` & `rucio-1.9.6/lib/rucio/api/replica.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/request.py` & `rucio-1.9.6/lib/rucio/api/request.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/rse.py` & `rucio-1.9.6/lib/rucio/api/rse.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/rule.py` & `rucio-1.9.6/lib/rucio/api/rule.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/scope.py` & `rucio-1.9.6/lib/rucio/api/scope.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/subscription.py` & `rucio-1.9.6/lib/rucio/api/subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/api/temporary_did.py` & `rucio-1.9.6/lib/rucio/api/temporary_did.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/cli/upload.py` & `rucio-1.9.6/lib/rucio/client/cli/upload.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/accountclient.py` & `rucio-1.9.6/lib/rucio/client/accountclient.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/accountlimitclient.py` & `rucio-1.9.6/lib/rucio/client/accountlimitclient.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/baseclient.py` & `rucio-1.9.6/lib/rucio/client/baseclient.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/client.py` & `rucio-1.9.6/lib/rucio/client/client.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/configclient.py` & `rucio-1.9.6/lib/rucio/client/configclient.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/didclient.py` & `rucio-1.9.6/lib/rucio/client/didclient.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/dq2client.py` & `rucio-1.9.6/lib/rucio/client/dq2client.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/fileclient.py` & `rucio-1.9.6/lib/rucio/client/fileclient.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/lockclient.py` & `rucio-1.9.6/lib/rucio/client/lockclient.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/metaclient.py` & `rucio-1.9.6/lib/rucio/client/metaclient.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/objectstoreclient.py` & `rucio-1.9.6/lib/rucio/client/objectstoreclient.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/pingclient.py` & `rucio-1.9.6/lib/rucio/client/pingclient.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/replicaclient.py` & `rucio-1.9.6/lib/rucio/client/replicaclient.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/rseclient.py` & `rucio-1.9.6/lib/rucio/client/rseclient.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/ruleclient.py` & `rucio-1.9.6/lib/rucio/client/ruleclient.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/scopeclient.py` & `rucio-1.9.6/lib/rucio/client/scopeclient.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/subscriptionclient.py` & `rucio-1.9.6/lib/rucio/client/subscriptionclient.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/client/uploadclient.py` & `rucio-1.9.6/lib/rucio/client/uploadclient.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/common/dumper/__init__.py` & `rucio-1.9.6/lib/rucio/common/dumper/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/common/dumper/consistency.py` & `rucio-1.9.6/lib/rucio/common/dumper/consistency.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/common/dumper/data_models.py` & `rucio-1.9.6/lib/rucio/common/dumper/data_models.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/common/dumper/path_parsing.py` & `rucio-1.9.6/lib/rucio/common/dumper/path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/common/client.py` & `rucio-1.9.6/lib/rucio/common/client.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/common/closeness_sorter.py` & `rucio-1.9.6/lib/rucio/common/closeness_sorter.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/common/config.py` & `rucio-1.9.6/lib/rucio/common/config.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/common/constants.py` & `rucio-1.9.6/lib/rucio/common/constants.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/common/exception.py` & `rucio-1.9.6/lib/rucio/common/exception.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/common/log.py` & `rucio-1.9.6/lib/rucio/common/log.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/common/objectstore.py` & `rucio-1.9.6/lib/rucio/common/objectstore.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/common/policy.py` & `rucio-1.9.6/lib/rucio/common/policy.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/common/replicas_selector.py` & `rucio-1.9.6/lib/rucio/common/replicas_selector.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/common/rse_attributes.py` & `rucio-1.9.6/lib/rucio/common/rse_attributes.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/common/schema.py` & `rucio-1.9.6/lib/rucio/common/schema.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/common/utils.py` & `rucio-1.9.6/lib/rucio/common/utils.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/permission/__init__.py` & `rucio-1.9.6/lib/rucio/core/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/permission/atlas.py` & `rucio-1.9.6/lib/rucio/core/permission/atlas.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/permission/generic.py` & `rucio-1.9.6/lib/rucio/core/permission/generic.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/account.py` & `rucio-1.9.6/lib/rucio/core/account.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/account_counter.py` & `rucio-1.9.6/lib/rucio/core/account_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/account_limit.py` & `rucio-1.9.6/lib/rucio/core/account_limit.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/authentication.py` & `rucio-1.9.6/lib/rucio/core/authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/config.py` & `rucio-1.9.6/lib/rucio/core/config.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/did.py` & `rucio-1.9.6/lib/rucio/core/did.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
   Licensed under the Apache License, Version 2.0 (the "License");
   You may not use this file except in compliance with the License.
   You may obtain a copy of the License at
   http://www.apache.org/licenses/LICENSE-2.0
 
   Authors:
-  - Vincent Garonne, <vincent.garonne@cern.ch>, 2012-2016
+  - Vincent Garonne, <vincent.garonne@cern.ch>, 2012-2017
   - Mario Lassnig, <mario.lassnig@cern.ch>, 2012-2015
   - Yun-Pin Sun, <yun-pin.sun@cern.ch>, 2013
   - Cedric Serfon, <cedric.serfon@cern.ch>, 2013-2015
   - Martin Barisits, <martin.barisits@cern.ch>, 2013-2015
   - Ralph Vigne, <ralph.vigne@cern.ch>, 2013
   - Thomas Beermann, <thomas.beermann@cern.ch>, 2014, 2016
   - Joaquin Bogado, <joaquin.bogado@cern.ch>, 2014-2015
@@ -26,15 +26,15 @@
 from hashlib import md5
 from re import match
 
 from sqlalchemy import and_, or_, exists
 from sqlalchemy.exc import DatabaseError, IntegrityError, CompileError
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql import not_, func
-from sqlalchemy.sql.expression import bindparam, text, Insert, select
+from sqlalchemy.sql.expression import bindparam, text, Insert, select, true
 
 import rucio.core.rule
 import rucio.core.replica  # import add_replicas
 
 from rucio.common import exception
 from rucio.common.config import config_get
 from rucio.common.utils import str_to_date
@@ -60,15 +60,15 @@
 
     :param limit: limit number.
     :param session: The database session in use.
     """
 
     stmt = exists().where(and_(models.ReplicationRule.scope == models.DataIdentifier.scope,
                                models.ReplicationRule.name == models.DataIdentifier.name,
-                               models.ReplicationRule.locked == True))  # NOQA
+                               models.ReplicationRule.locked == true()))
     query = session.query(models.DataIdentifier.scope, models.DataIdentifier.name,
                           models.DataIdentifier.did_type,
                           models.DataIdentifier.created_at,
                           models.DataIdentifier.purge_replicas).\
         filter(models.DataIdentifier.expired_at < datetime.utcnow(), not_(stmt)).\
         order_by(models.DataIdentifier.expired_at).\
         with_hint(models.DataIdentifier, "index(DIDS DIDS_EXPIRED_AT_IDX)", 'oracle')
@@ -95,19 +95,21 @@
                 if limit and row_count >= limit:
                     return dids
             return dids
 
     if limit:
         query = query.limit(limit)
 
-    return [{'scope': scope, 'name': name, 'did_type': did_type, 'created_at': created_at, 'purge_replicas': purge_replicas} for scope, name, did_type, created_at, purge_replicas in query]
+    return [{'scope': scope, 'name': name, 'did_type': did_type, 'created_at': created_at,
+             'purge_replicas': purge_replicas} for scope, name, did_type, created_at, purge_replicas in query]
 
 
 @transactional_session
-def add_did(scope, name, type, account, statuses=None, meta=None, rules=None, lifetime=None, dids=None, rse=None, session=None):
+def add_did(scope, name, type, account, statuses=None, meta=None, rules=None,
+            lifetime=None, dids=None, rse=None, session=None):
     """
     Add data identifier.
 
     :param scope: The scope name.
     :param name: The data identifier name.
     :param type: The data identifier type.
     :param account: The account owner.
@@ -1184,16 +1186,17 @@
         if not values['is_open']:
             rules_on_ds = session.query(models.ReplicationRule).filter_by(scope=scope, name=name).all()
             for rule in rules_on_ds:
                 rucio.core.rule.generate_message_for_dataset_ok_callback(rule=rule, session=session)
 
 
 @stream_session
-def list_dids(scope, filters, type='collection', ignore_case=False, limit=None, offset=None, long=False, session=None):
-    """
+def list_dids(scope, filters, type='collection', ignore_case=False, limit=None,
+              offset=None, long=False, session=None):
+    """0
     Search data identifiers
 
     :param scope: the scope name.
     :param filters: dictionary of attributes by which the results should be filtered.
     :param type: the type of the did: all(container, dataset, file), collection(dataset or container), dataset, container, file.
     :param ignore_case: ignore case distinctions.
     :param limit: limit number.
@@ -1208,14 +1211,17 @@
     query = session.query(models.DataIdentifier.scope,
                           models.DataIdentifier.name,
                           models.DataIdentifier.did_type,
                           models.DataIdentifier.bytes,
                           models.DataIdentifier.length).\
         filter(models.DataIdentifier.scope == scope)
 
+    # Exclude suppressed dids
+    query = query.filter(models.DataIdentifier.suppressed != true())
+
     if type == 'all':
         query = query.filter(or_(models.DataIdentifier.did_type == DIDType.CONTAINER,
                                  models.DataIdentifier.did_type == DIDType.DATASET,
                                  models.DataIdentifier.did_type == DIDType.FILE))
     elif type.lower() == 'collection':
         query = query.filter(or_(models.DataIdentifier.did_type == DIDType.CONTAINER,
                                  models.DataIdentifier.did_type == DIDType.DATASET))
@@ -1232,17 +1238,19 @@
            and not hasattr(models.DataIdentifier, k):
             raise exception.KeyNotFound(k)
 
         if (isinstance(v, unicode) or isinstance(v, str)) and ('*' in v or '%' in v):
             if v in ('*', '%', u'*', u'%'):
                 continue
             if session.bind.dialect.name == 'postgresql':  # PostgreSQL escapes automatically
-                query = query.filter(getattr(models.DataIdentifier, k).like(v.replace('*', '%')))
+                query = query.filter(getattr(models.DataIdentifier, k).
+                                     like(v.replace('*', '%')))
             else:
-                query = query.filter(getattr(models.DataIdentifier, k).like(v.replace('*', '%'), escape='\\'))
+                query = query.filter(getattr(models.DataIdentifier, k).
+                                     like(v.replace('*', '%'), escape='\\'))
         elif k == 'created_before':
             created_before = str_to_date(v)
             query = query.filter(models.DataIdentifier.created_at <= created_before)
         elif k == 'created_after':
             created_after = str_to_date(v)
             query = query.filter(models.DataIdentifier.created_at >= created_after)
         elif k == 'guid':
```

### Comparing `rucio-1.9.5/lib/rucio/core/distance.py` & `rucio-1.9.6/lib/rucio/core/distance.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/heartbeat.py` & `rucio-1.9.6/lib/rucio/core/heartbeat.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,44 @@
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Authors:
 # - Mario Lassnig, <mario.lassnig@cern.ch>, 2015
-# - Vincent Garonne, <vincent.garonne@cern.ch>, 2015
+# - Vincent Garonne, <vincent.garonne@cern.ch>, 2015-2017
 
 import datetime
 import hashlib
 
 from sqlalchemy.sql import distinct
 
 from rucio.db.sqla.models import Heartbeats
 from rucio.db.sqla.session import read_session, transactional_session
+from rucio.common.exception import DatabaseException
 from rucio.common.utils import pid_exists
 
 
+def sanity_check(executable, hostname, hash_executable=None):
+    """
+    sanity_check wrapper to ignore DatabaseException errors.
+
+    :param executable: Executable name as a string, e.g., conveyor-submitter.
+    :param hostname: Hostname as a string, e.g., rucio-daemon-prod-01.cern.ch.
+    :param hash_executable: Hash of the executable.
+    """
+    try:
+        _sanity_check(executable=executable, hostname=hostname,
+                      hash_executable=hash_executable)
+    except DatabaseException:
+        pass
+
+
 @transactional_session
-def sanity_check(executable, hostname, hash_executable=None, session=None):
+def _sanity_check(executable, hostname, hash_executable=None, session=None):
     """
     Check if processes on the host are still running.
 
     :param executable: Executable name as a string, e.g., conveyor-submitter.
     :param hostname: Hostname as a string, e.g., rucio-daemon-prod-01.cern.ch.
     :param hash_executable: Hash of the executable.
     """
```

### Comparing `rucio-1.9.5/lib/rucio/core/identity.py` & `rucio-1.9.6/lib/rucio/core/identity.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/lock.py` & `rucio-1.9.6/lib/rucio/core/lock.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/message.py` & `rucio-1.9.6/lib/rucio/core/message.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/meta.py` & `rucio-1.9.6/lib/rucio/core/meta.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/monitor.py` & `rucio-1.9.6/lib/rucio/core/monitor.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/naming_convention.py` & `rucio-1.9.6/lib/rucio/core/naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/nongrid_trace.py` & `rucio-1.9.6/lib/rucio/core/nongrid_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/quarantined_replica.py` & `rucio-1.9.6/lib/rucio/core/quarantined_replica.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
   Licensed under the Apache License, Version 2.0 (the "License");
   You may not use this file except in compliance with the License.
   You may obtain a copy of the License at
   http://www.apache.org/licenses/LICENSE-2.0
 
   Authors:
-  - Vincent Garonne, <vincent.garonne@cern.ch>, 2016
+  - Vincent Garonne, <vincent.garonne@cern.ch>, 2016-2017
 """
 
 import datetime
 
 from sqlalchemy import and_, or_, exists, not_
-from sqlalchemy.sql.expression import bindparam, text, select
+from sqlalchemy.sql.expression import bindparam, text, select, false
 
 from rucio.common.utils import chunks
 from rucio.core.rse import get_rse_id
 from rucio.db.sqla import models
 from rucio.db.sqla.session import read_session, transactional_session
 
 
@@ -143,12 +143,11 @@
     """
     List RSEs in the Quarantined Queues.
 
     :param session: The database session in use.
 
     :returns: a list of RSEs.
     """
-    is_false = False
     query = session.query(models.RSE.rse).distinct(models.RSE.rse).\
         filter(models.QuarantinedReplica.rse_id == models.RSE.id).\
-        filter(models.RSE.deleted == is_false)
+        filter(models.RSE.deleted == false())
     return [rse for (rse,) in query]
```

### Comparing `rucio-1.9.5/lib/rucio/core/replica.py` & `rucio-1.9.6/lib/rucio/core/replica.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
   Licensed under the Apache License, Version 2.0 (the "License");
   You may not use this file except in compliance with the License.
   You may obtain a copy of the License at
   http://www.apache.org/licenses/LICENSE-2.0
 
   Authors:
-  - Vincent Garonne, <vincent.garonne@cern.ch>, 2013-2016
+  - Vincent Garonne, <vincent.garonne@cern.ch>, 2013-2017
   - Martin Barisits, <martin.barisits@cern.ch>, 2014
-  - Cedric Serfon, <cedric.serfon@cern.ch>, 2014-2016
+  - Cedric Serfon, <cedric.serfon@cern.ch>, 2014-2017
   - Mario Lassnig, <mario.lassnig@cern.ch>, 2014-2015
   - Ralph Vigne, <ralph.vigne@cern.ch>, 2014
   - Thomas Beermann, <thomas.beermann@cern.ch>, 2014-2016
   - Wen Guan, <wen.guan@cern.ch>, 2015
 """
 
 from collections import defaultdict
@@ -21,15 +21,15 @@
 from datetime import datetime, timedelta
 from re import match
 from traceback import format_exc
 
 from sqlalchemy import func, and_, or_, exists, not_
 from sqlalchemy.exc import DatabaseError, IntegrityError
 from sqlalchemy.orm.exc import FlushError, NoResultFound
-from sqlalchemy.sql.expression import case, bindparam, select, text
+from sqlalchemy.sql.expression import case, bindparam, select, text, false
 
 import rucio.core.lock
 
 from rucio.common import exception
 from rucio.common.utils import chunks, clean_surls, str_to_date
 from rucio.core.rse import get_rse, get_rse_id, get_rse_name
 from rucio.core.rse_counter import decrease, increase
@@ -94,17 +94,22 @@
     :param name: The name of the file.
     :param path: The path of the replica.
     :param session: The database session in use.
     """
 
     already_declared = False
     if path:
+        path_clause = [models.RSEFileAssociation.path == path]
+        if path.startswith('/'):
+            path_clause.append(models.RSEFileAssociation.path == path[1:])
+        else:
+            path_clause.append(models.RSEFileAssociation.path == '/%s' % path)
         query = session.query(models.RSEFileAssociation.path, models.RSEFileAssociation.scope, models.RSEFileAssociation.name, models.RSEFileAssociation.rse_id).\
             with_hint(models.RSEFileAssociation, "+ index(replicas REPLICAS_PATH_IDX", 'oracle').\
-            filter(models.RSEFileAssociation.rse_id == rse_id).filter(models.RSEFileAssociation.path == path)
+            filter(models.RSEFileAssociation.rse_id == rse_id).filter(or_(*path_clause))
     else:
         query = session.query(models.RSEFileAssociation.path, models.RSEFileAssociation.scope, models.RSEFileAssociation.name, models.RSEFileAssociation.rse_id).\
             filter_by(rse_id=rse_id, scope=scope, name=name)
     if query.count():
         result = query.first()
         path, scope, name, rse_id = result[0], result[1], result[2], result[3]
         # Now we check that the replica is not already declared bad
@@ -331,14 +336,19 @@
                         if not isprint(char):
                             unknown_replicas.append('%s %s' % (pfn, 'PFN contains hidden chars'))
                             no_hidden_char = False
                             break
                     if no_hidden_char:
                         unknown_replicas.append('%s %s' % (pfn, 'Unknown replica'))
             path_clause.append(models.RSEFileAssociation.path == path)
+            if path.startswith('/'):
+                path_clause.append(models.RSEFileAssociation.path == path[1:])
+            else:
+                path_clause.append(models.RSEFileAssociation.path == '/%s' % path)
+
         if status == BadFilesStatus.BAD:
             # For BAD file, we modify the replica state, not for suspicious
             query = session.query(models.RSEFileAssociation.path, models.RSEFileAssociation.scope, models.RSEFileAssociation.name, models.RSEFileAssociation.rse_id).\
                 with_hint(models.RSEFileAssociation, "+ index(replicas REPLICAS_PATH_IDX", 'oracle').\
                 filter(models.RSEFileAssociation.rse_id == rse_id).filter(or_(*path_clause))
             rowcount = query.update({'state': ReplicaState.BAD})
             if rowcount != len(declared_replicas):
@@ -573,15 +583,15 @@
                                                        models.DataIdentifierAssociation.name == tmp_did.child_name))
 
                         else:
                             child_dids.append((tmp_did.child_scope, tmp_did.child_name))
 
     state_clause = None
     if not all_states:
-        # models.RSE.volatile == is_false
+        # models.RSE.volatile == false()
         if not unavailable:
             state_clause = and_(models.RSEFileAssociation.state == ReplicaState.AVAILABLE)
 
         else:
             state_clause = or_(models.RSEFileAssociation.state == ReplicaState.AVAILABLE,
                                models.RSEFileAssociation.state == ReplicaState.UNAVAILABLE,
                                models.RSEFileAssociation.state == ReplicaState.COPYING)
@@ -591,15 +601,14 @@
 
 def _list_replicas_for_datasets(dataset_clause, state_clause, rse_clause, session):
     """
     List file replicas for a list of datasets.
 
     :param session: The database session in use.
     """
-    is_false = False
     replica_query = session.query(models.DataIdentifierAssociation.child_scope,
                                   models.DataIdentifierAssociation.child_name,
                                   models.DataIdentifierAssociation.bytes,
                                   models.DataIdentifierAssociation.md5,
                                   models.DataIdentifierAssociation.adler32,
                                   models.RSEFileAssociation.path,
                                   models.RSEFileAssociation.state,
@@ -609,16 +618,16 @@
         with_hint(models.RSEFileAssociation,
                   text="INDEX_RS_ASC(CONTENTS CONTENTS_PK) INDEX_RS_ASC(REPLICAS REPLICAS_PK) NO_INDEX_FFS(CONTENTS CONTENTS_PK)",
                   dialect_name='oracle').\
         outerjoin(models.RSEFileAssociation,
                   and_(models.DataIdentifierAssociation.child_scope == models.RSEFileAssociation.scope,
                        models.DataIdentifierAssociation.child_name == models.RSEFileAssociation.name)).\
         join(models.RSE, models.RSE.id == models.RSEFileAssociation.rse_id).\
-        filter(models.RSE.deleted == is_false).\
-        filter(models.RSE.staging_area == is_false).\
+        filter(models.RSE.deleted == false()).\
+        filter(models.RSE.staging_area == false()).\
         filter(or_(*dataset_clause)).\
         order_by(models.DataIdentifierAssociation.child_scope,
                  models.DataIdentifierAssociation.child_name)
 
     if state_clause is not None:
         replica_query = replica_query.filter(and_(state_clause))
 
@@ -631,40 +640,39 @@
 
 def _list_replicas_for_files(file_clause, state_clause, files, rse_clause, session):
     """
     List file replicas for a list of files.
 
     :param session: The database session in use.
     """
-    is_false = False
     for replica_condition in chunks(file_clause, 50):
 
         if state_clause is None:
             if rse_clause is None:
                 whereclause = and_(models.RSEFileAssociation.rse_id == models.RSE.id,
-                                   models.RSE.deleted == is_false,
-                                   models.RSE.staging_area == is_false,
+                                   models.RSE.deleted == false(),
+                                   models.RSE.staging_area == false(),
                                    or_(*replica_condition))
             else:
                 whereclause = and_(models.RSEFileAssociation.rse_id == models.RSE.id,
-                                   models.RSE.deleted == is_false,
-                                   models.RSE.staging_area == is_false,
+                                   models.RSE.deleted == false(),
+                                   models.RSE.staging_area == false(),
                                    or_(*replica_condition),
                                    or_(*rse_clause))
         else:
             if rse_clause is None:
                 whereclause = and_(models.RSEFileAssociation.rse_id == models.RSE.id,
-                                   models.RSE.deleted == is_false,
-                                   models.RSE.staging_area == is_false,
+                                   models.RSE.deleted == false(),
+                                   models.RSE.staging_area == false(),
                                    state_clause,
                                    or_(*replica_condition))
             else:
                 whereclause = and_(models.RSEFileAssociation.rse_id == models.RSE.id,
-                                   models.RSE.deleted == is_false,
-                                   models.RSE.staging_area == is_false,
+                                   models.RSE.deleted == false(),
+                                   models.RSE.staging_area == false(),
                                    state_clause,
                                    or_(*replica_condition),
                                    or_(*rse_clause))
 
         replica_query = select(columns=(models.RSEFileAssociation.scope,
                                         models.RSEFileAssociation.name,
                                         models.RSEFileAssociation.bytes,
@@ -1649,15 +1657,14 @@
     :param scope: The scope of the dataset.
     :param name: The name of the dataset.
     :param deep: Lookup at the file level.
     :param session: Database session to use.
 
     :returns: A list of dict dataset replicas
     """
-    is_false = False
     if not deep:
         query = session.query(models.CollectionReplica.scope,
                               models.CollectionReplica.name,
                               models.RSE.rse,
                               models.CollectionReplica.rse_id,
                               models.CollectionReplica.bytes,
                               models.CollectionReplica.length,
@@ -1665,15 +1672,15 @@
                               models.CollectionReplica.available_replicas_cnt.label("available_length"),
                               models.CollectionReplica.state,
                               models.CollectionReplica.created_at,
                               models.CollectionReplica.updated_at,
                               models.CollectionReplica.accessed_at)\
             .filter_by(scope=scope, name=name, did_type=DIDType.DATASET)\
             .filter(models.CollectionReplica.rse_id == models.RSE.id)\
-            .filter(models.RSE.deleted == is_false)
+            .filter(models.RSE.deleted == false())
 
         for row in query:
             yield row._asdict()
 
     else:
         content_query = session.\
             query(func.sum(models.DataIdentifierAssociation.bytes).label("bytes"),
@@ -1712,15 +1719,15 @@
                               models.RSE.rse,
                               sub_query.c.available_bytes,
                               sub_query.c.available_length,
                               sub_query.c.created_at,
                               sub_query.c.updated_at,
                               sub_query.c.accessed_at)\
             .filter(models.RSE.id == sub_query.c.rse_id)\
-            .filter(models.RSE.deleted == is_false)
+            .filter(models.RSE.deleted == false())
 
         for row in query:
             replica = row._asdict()
             replica['length'], replica['bytes'] = length, bytes
             if replica['length'] == row.available_length:
                 replica['state'] = ReplicaState.AVAILABLE
             else:
@@ -1736,30 +1743,29 @@
     :param rse: the rse name.
     :param filters: dictionary of attributes by which the results should be filtered.
     :param limit: limit number.
     :param session: Database session to use.
 
     :returns: A list of dict dataset replicas
     """
-    is_false = False
     query = session.query(models.CollectionReplica.scope,
                           models.CollectionReplica.name,
                           models.RSE.rse,
                           models.CollectionReplica.bytes,
                           models.CollectionReplica.length,
                           models.CollectionReplica.available_bytes,
                           models.CollectionReplica.available_replicas_cnt.label("available_length"),
                           models.CollectionReplica.state,
                           models.CollectionReplica.created_at,
                           models.CollectionReplica.updated_at,
                           models.CollectionReplica.accessed_at)\
         .filter_by(did_type=DIDType.DATASET)\
         .filter(models.CollectionReplica.rse_id == models.RSE.id)\
         .filter(models.RSE.rse == rse)\
-        .filter(models.RSE.deleted == is_false)
+        .filter(models.RSE.deleted == false())
 
     for (k, v) in filters and filters.items() or []:
         if k == 'name' or k == 'scope':
             if '*' in v or '%' in v:
                 if session.bind.dialect.name == 'postgresql':  # PostgreSQL escapes automatically
                     query = query.filter(getattr(models.CollectionReplica, k).like(v.replace('*', '%')))
                 else:
```

### Comparing `rucio-1.9.5/lib/rucio/core/request.py` & `rucio-1.9.6/lib/rucio/core/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Authors:
 # - Mario Lassnig, <mario.lassnig@cern.ch>, 2013-2015
-# - Vincent Garonne, <vincent.garonne@cern.ch>, 2015-2016
+# - Vincent Garonne, <vincent.garonne@cern.ch>, 2015-2017
 # - Martin Barisits, <martin.barisits@cern.ch>, 2014
 # - Wen Guan, <wen.guan@cern.ch>, 2014-2016
 # - Joaquin Bogado, <jbogadog@cern.ch>, 2016
 # - Thomas Beermann, <thomas.beermann@cern.ch>, 2016
 
 import datetime
 import json
@@ -22,15 +22,15 @@
 from ConfigParser import NoOptionError
 from dogpile.cache import make_region
 from dogpile.cache.api import NoValue
 
 from sqlalchemy import and_, or_, func
 from sqlalchemy.orm import aliased
 from sqlalchemy.exc import IntegrityError
-from sqlalchemy.sql.expression import asc, bindparam, text
+from sqlalchemy.sql.expression import asc, bindparam, text, false, true
 
 from rucio.common.config import config_get
 from rucio.common.exception import RequestNotFound, RucioException, UnsupportedOperation
 from rucio.common.utils import generate_uuid, chunks
 from rucio.core import config as config_core, message as message_core
 from rucio.core.monitor import record_counter, record_timer
 from rucio.core.rse import get_rse_id, get_rse_name, get_rse_transfer_limits
@@ -304,22 +304,24 @@
             new_requests.append({'id': request['request_id'],
                                  'request_type': request['request_type'],
                                  'scope': request['scope'],
                                  'name': request['name'],
                                  'dest_rse_id': request['dest_rse_id'],
                                  'attributes': json.dumps(request['attributes']),
                                  'state': request['state'],
-                                 'previous_attempt_id': request['previous_attempt_id'],
-                                 'retry_count': request['retry_count'],
                                  'rule_id': request['rule_id'],
                                  'activity': request['attributes']['activity'],
                                  'bytes': request['attributes']['bytes'],
                                  'md5': request['attributes']['md5'],
                                  'adler32': request['attributes']['adler32'],
-                                 'account': request.get('account', None)})
+                                 'account': request.get('account', None),
+                                 'priority': request['attributes'].get('priority', None),
+                                 'requested_at': request.get('requested_at', None),
+                                 'retry_count': request['retry_count'],
+                                 'previous_attempt_id': request['previous_attempt_id']})
         else:
             request['request_id'] = generate_uuid()
             new_requests.append({'id': request['request_id'],
                                  'request_type': request['request_type'],
                                  'scope': request['scope'],
                                  'name': request['name'],
                                  'dest_rse_id': request['dest_rse_id'],
@@ -328,15 +330,15 @@
                                  'rule_id': request['rule_id'],
                                  'activity': request['attributes']['activity'],
                                  'bytes': request['attributes']['bytes'],
                                  'md5': request['attributes']['md5'],
                                  'adler32': request['attributes']['adler32'],
                                  'account': request.get('account', None),
                                  'priority': request['attributes'].get('priority', None),
-                                 'requested_at': request['attributes'].get('requested_at', None),
+                                 'requested_at': request.get('requested_at', None),
                                  'retry_count': request['retry_count']})
 
         if 'sources' in request and request['sources']:
             for source in request['sources']:
                 sources.append({'request_id': request['request_id'],
                                 'scope': request['scope'],
                                 'name': request['name'],
@@ -1344,15 +1346,14 @@
     :param rses: List of rse_id to select requests.
     :param session: Database session to use.
     :returns: List.
     """
     if total_processes > 1 and total_processes == total_threads:
         raise RucioException("Total process %s is the same with total threads %s, will create potential same hash" % (total_processes, total_threads))
 
-    is_false = False  # For PEP8
     sub_requests = session.query(models.Request.id,
                                  models.Request.rule_id,
                                  models.Request.scope,
                                  models.Request.name,
                                  models.Request.md5,
                                  models.Request.adler32,
                                  models.Request.bytes,
@@ -1416,16 +1417,16 @@
                           models.Distance.ranking)\
         .outerjoin(models.RSEFileAssociation, and_(sub_requests.c.scope == models.RSEFileAssociation.scope,
                                                    sub_requests.c.name == models.RSEFileAssociation.name,
                                                    models.RSEFileAssociation.state == ReplicaState.AVAILABLE,
                                                    sub_requests.c.dest_rse_id != models.RSEFileAssociation.rse_id))\
         .with_hint(models.RSEFileAssociation, "+ index(replicas REPLICAS_PK)", 'oracle')\
         .outerjoin(models.RSE, and_(models.RSE.id == models.RSEFileAssociation.rse_id,
-                                    models.RSE.staging_area == is_false,
-                                    models.RSE.deleted == is_false))\
+                                    models.RSE.staging_area == false(),
+                                    models.RSE.deleted == false()))\
         .outerjoin(models.Source, and_(sub_requests.c.id == models.Source.request_id,
                                        models.RSE.id == models.Source.rse_id))\
         .with_hint(models.Source, "+ index(sources SOURCES_PK)", 'oracle')\
         .outerjoin(models.Distance, and_(sub_requests.c.dest_rse_id == models.Distance.dest_rse_id,
                                          models.RSEFileAssociation.rse_id == models.Distance.src_rse_id))\
         .with_hint(models.Distance, "+ index(distances DISTANCES_PK)", 'oracle')
 
@@ -1453,15 +1454,14 @@
     :param limit: Integer of requests to retrieve.
     :param activity: Activity to be selected.
     :param older_than: Only select requests older than this DateTime.
     :param rses: List of rse_id to select requests.
     :param session: Database session to use.
     :returns: List.
     """
-    is_false = False  # For PEP8
     sub_requests = session.query(models.Request.id,
                                  models.Request.rule_id,
                                  models.Request.scope,
                                  models.Request.name,
                                  models.Request.md5,
                                  models.Request.adler32,
                                  models.Request.bytes,
@@ -1525,16 +1525,16 @@
                           models.Source.ranking)\
         .outerjoin(models.RSEFileAssociation, and_(sub_requests.c.scope == models.RSEFileAssociation.scope,
                                                    sub_requests.c.name == models.RSEFileAssociation.name,
                                                    models.RSEFileAssociation.state == ReplicaState.AVAILABLE,
                                                    sub_requests.c.dest_rse_id != models.RSEFileAssociation.rse_id))\
         .with_hint(models.RSEFileAssociation, "+ index(replicas REPLICAS_PK)", 'oracle')\
         .outerjoin(models.RSE, and_(models.RSE.id == models.RSEFileAssociation.rse_id,
-                                    models.RSE.staging_area == is_false,
-                                    models.RSE.deleted == is_false))\
+                                    models.RSE.staging_area == false(),
+                                    models.RSE.deleted == false()))\
         .outerjoin(models.RSEAttrAssociation, and_(models.RSEAttrAssociation.rse_id == models.RSE.id,
                                                    models.RSEAttrAssociation.key == 'staging_buffer'))\
         .outerjoin(models.Source, and_(sub_requests.c.id == models.Source.request_id,
                                        models.RSE.id == models.Source.rse_id))\
         .with_hint(models.Source, "+ index(sources SOURCES_PK)", 'oracle')
 
     if rses:
@@ -1602,19 +1602,17 @@
     """
     Retrieve heavy load rses.
 
     :param threshold: threshold as an int.
     :param session: Database session to use.
     :returns: .
     """
-
-    is_true = True
     try:
         results = session.query(models.Source.rse_id, func.count(models.Source.rse_id).label('load'))\
-                         .filter(models.Source.is_using == is_true)\
+                         .filter(models.Source.is_using == true())\
                          .group_by(models.Source.rse_id)\
                          .all()
 
         if not results:
             return
 
         result = []
```

### Comparing `rucio-1.9.5/lib/rucio/core/rse.py` & `rucio-1.9.6/lib/rucio/core/rse.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/rse_counter.py` & `rucio-1.9.6/lib/rucio/core/rse_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/rse_expression_parser.py` & `rucio-1.9.6/lib/rucio/core/rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/rse_selector.py` & `rucio-1.9.6/lib/rucio/core/rse_selector.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/rule.py` & `rucio-1.9.6/lib/rucio/core/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Authors:
-# - Vincent Garonne, <vincent.garonne@cern.ch>, 2012-2015
+# - Vincent Garonne, <vincent.garonne@cern.ch>, 2012-2017
 # - Martin Barisits, <martin.barisits@cern.ch>, 2013-2016
 # - Mario Lassnig, <mario.lassnig@cern.ch>, 2013-2015
 # - Cedric Serfon, <cedric.serfon@cern.ch>, 2014-2016
 
 import logging
 import sys
 
@@ -19,15 +19,15 @@
 from datetime import datetime, timedelta
 from re import match
 from string import Template
 
 from sqlalchemy.exc import IntegrityError, StatementError
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql import func
-from sqlalchemy.sql.expression import and_, or_, bindparam, text
+from sqlalchemy.sql.expression import and_, or_, bindparam, text, true, null
 
 import rucio.core.did
 import rucio.core.lock  # import get_replica_locks, get_files_and_replica_locks_of_dataset
 import rucio.core.replica  # import get_and_lock_file_replicas, get_and_lock_file_replicas_for_dataset
 
 from rucio.common.config import config_get
 from rucio.common.exception import (InvalidRSEExpression, InvalidReplicationRule, InsufficientAccountLimit,
@@ -1502,33 +1502,32 @@
     :param total_workers:      Number of total workers.
     :param worker_number:      id of the executing worker.
     :param delta:              Delta in seconds to select rules in.
     :param limit:              Maximum number of rules to select.
     :param blacklisted_rules:  Blacklisted rules to filter out.
     :param session:            Database session in use.
     """
-    is_none, is_true = None, True
     if session.bind.dialect.name == 'oracle':
         query = session.query(models.ReplicationRule.id).\
             with_hint(models.ReplicationRule, "index(rules RULES_STUCKSTATE_IDX)", 'oracle').\
             filter(text("(CASE when rules.state='S' THEN rules.state ELSE null END)= 'S' ")).\
             filter(models.ReplicationRule.state == RuleState.STUCK).\
             filter(models.ReplicationRule.updated_at < datetime.utcnow() - timedelta(seconds=delta)).\
-            filter(or_(models.ReplicationRule.expires_at == is_none,
+            filter(or_(models.ReplicationRule.expires_at == null(),
                        models.ReplicationRule.expires_at > datetime.utcnow(),
-                       models.ReplicationRule.locked == is_true)).\
+                       models.ReplicationRule.locked == true())).\
             order_by(models.ReplicationRule.updated_at)  # NOQA
     else:
         query = session.query(models.ReplicationRule.id).\
             with_hint(models.ReplicationRule, "index(rules RULES_STUCKSTATE_IDX)", 'oracle').\
             filter(models.ReplicationRule.state == RuleState.STUCK).\
             filter(models.ReplicationRule.updated_at < datetime.utcnow() - timedelta(seconds=delta)).\
-            filter(or_(models.ReplicationRule.expires_at == is_none,
+            filter(or_(models.ReplicationRule.expires_at == null(),
                        models.ReplicationRule.expires_at > datetime.utcnow(),
-                       models.ReplicationRule.locked == is_true)).\
+                       models.ReplicationRule.locked == true())).\
             order_by(models.ReplicationRule.updated_at)
 
     if session.bind.dialect.name == 'oracle':
         bindparams = [bindparam('worker_number', worker_number),
                       bindparam('total_workers', total_workers)]
         query = query.filter(text('ORA_HASH(name, :total_workers) = :worker_number', bindparams=bindparams))
     elif session.bind.dialect.name == 'mysql':
```

### Comparing `rucio-1.9.5/lib/rucio/core/rule_grouping.py` & `rucio-1.9.6/lib/rucio/core/rule_grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,27 +171,27 @@
                   'source_replica_expression': rule.source_replica_expression,
                   'lifetime': lifetime,
                   'ds_scope': ds_scope,
                   'ds_name': ds_name,
                   'bytes': bytes,
                   'md5': md5,
                   'adler32': adler32,
+                  'priority': rule.priority,
                   # 'allow_tape_source': has_account_attribute(account=rule.account, key='admin', session=session)}
                   'allow_tape_source': True}
 
     return {'dest_rse_id': dest_rse_id,
             'scope': scope,
             'name': name,
             'rule_id': rule.id,
             'attributes': attributes,
             'request_type': request_type,
             'retry_count': retry_count,
-            'generated_at': lock.created_at if lock else rule.created_at,
             'account': rule.account,
-            'priority': rule.priority}
+            'requested_at': lock.created_at if lock else rule.created_at}
 
 
 @transactional_session
 def __apply_rule_to_files_none_grouping(datasetfiles, locks, replicas, source_replicas, rseselector, rule, preferred_rse_ids=[], source_rses=[], session=None):
     """
     Apply a rule to files with NONE grouping.
```

### Comparing `rucio-1.9.5/lib/rucio/core/scope.py` & `rucio-1.9.6/lib/rucio/core/scope.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/subscription.py` & `rucio-1.9.6/lib/rucio/core/subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/temporary_did.py` & `rucio-1.9.6/lib/rucio/core/temporary_did.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/trace.py` & `rucio-1.9.6/lib/rucio/core/trace.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/core/volatile_replica.py` & `rucio-1.9.6/lib/rucio/core/volatile_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/abacus/account.py` & `rucio-1.9.6/lib/rucio/daemons/abacus/account.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/abacus/rse.py` & `rucio-1.9.6/lib/rucio/daemons/abacus/rse.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/auditor/__init__.py` & `rucio-1.9.6/lib/rucio/daemons/auditor/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/auditor/hdfs.py` & `rucio-1.9.6/lib/rucio/daemons/auditor/hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/auditor/srmdumps.py` & `rucio-1.9.6/lib/rucio/daemons/auditor/srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/bb8/bb8.py` & `rucio-1.9.6/lib/rucio/daemons/bb8/bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/bb8/common.py` & `rucio-1.9.6/lib/rucio/daemons/bb8/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # Copyright European Organization for Nuclear Research (CERN)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Authors:
-# - Martin Barisits, <martin.barisits@cern.ch>, 2016
+# - Martin Barisits, <martin.barisits@cern.ch>, 2016-2017
 
 import logging
 import sys
 
 from datetime import datetime
 
 from rucio.core.lock import get_dataset_locks
 from rucio.core.rule import get_rule, add_rule, update_rule
 from rucio.core.rse_expression_parser import parse_expression
 from rucio.core.rse import list_rse_attributes, get_rse_name
 from rucio.core.rse_selector import RSESelector
 # from rucio.core.subscription import get_subscription_by_id
 from rucio.common.config import config_get
-from rucio.common.exception import InsufficientTargetRSEs
+from rucio.common.exception import InsufficientTargetRSEs, RuleNotFound, DuplicateRule
+from rucio.db.sqla.constants import RuleGrouping
 from rucio.db.sqla.session import transactional_session
 
+
 logging.basicConfig(stream=sys.stdout,
                     level=getattr(logging, config_get('common', 'loglevel').upper()),
                     format='%(asctime)s\t%(process)d\t%(levelname)s\t%(message)s')
 
 
 def rebalance_rule(parent_rule_id, activity, rse_expression, priority, source_replica_expression=None, comment=None):
     """
@@ -42,20 +44,27 @@
     parent_rule = get_rule(rule_id=parent_rule_id)
 
     if parent_rule['expires_at'] is None:
         lifetime = None
     else:
         lifetime = (parent_rule['expires_at'] - datetime.utcnow()).days * 24 * 3600 + (parent_rule['expires_at'] - datetime.utcnow()).seconds
 
+    if parent_rule['grouping'] == RuleGrouping.ALL:
+        grouping = 'ALL'
+    elif parent_rule['grouping'] == RuleGrouping.NONE:
+        grouping = 'NONE'
+    else:
+        grouping = 'DATASET'
+
     child_rule = add_rule(dids=[{'scope': parent_rule['scope'],
                                  'name': parent_rule['name']}],
                           account=parent_rule['account'],
                           copies=parent_rule['copies'],
                           rse_expression=rse_expression,
-                          grouping=parent_rule['grouping'],
+                          grouping=grouping,
                           weight=parent_rule['weight'],
                           lifetime=lifetime,
                           locked=parent_rule['locked'],
                           subscription_id=parent_rule['subscription_id'],
                           source_replica_expression=source_replica_expression,
                           activity=activity,
                           notify=parent_rule['notification'],
@@ -215,15 +224,15 @@
                                                    activity='Data Rebalancing',
                                                    rse_expression=target_rse_exp,
                                                    priority=priority,
                                                    source_replica_expression=source_replica_expression,
                                                    comment=comment)
                 else:
                     child_rule_id = ''
-            except InsufficientTargetRSEs, e:
+            except (InsufficientTargetRSEs, DuplicateRule, RuleNotFound) as e:
                 continue
             print ('%s:%s %s %d %s %s' % (scope, name, str(rule_id), int(bytes / 1E9), target_rse_exp, child_rule_id))
             rebalanced_bytes += bytes
             rebalanced_files += length
             rebalanced_datasets.append((scope, name, bytes, length, target_rse_exp, rule_id, child_rule_id))
         except Exception, e:
             print 'Exception %s occured while rebalancing %s:%s, rule_id: %s!' % (str(e), scope, name, str(rule_id))
```

### Comparing `rucio-1.9.5/lib/rucio/daemons/bb8/t1_background_rebalance.py` & `rucio-1.9.6/lib/rucio/daemons/bb8/t1_background_rebalance.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/c3po/algorithms/simple.py` & `rucio-1.9.6/lib/rucio/daemons/c3po/algorithms/simple.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/c3po/algorithms/t2_free_space.py` & `rucio-1.9.6/lib/rucio/daemons/c3po/algorithms/t2_free_space.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py` & `rucio-1.9.6/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py` & `rucio-1.9.6/lib/rucio/daemons/c3po/algorithms/t2_free_space_only_pop_with_network.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/c3po/collectors/agis.py` & `rucio-1.9.6/lib/rucio/daemons/c3po/collectors/agis.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/c3po/collectors/free_space.py` & `rucio-1.9.6/lib/rucio/daemons/c3po/collectors/free_space.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/c3po/collectors/jedi_did.py` & `rucio-1.9.6/lib/rucio/daemons/c3po/collectors/jedi_did.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/c3po/collectors/mock_did.py` & `rucio-1.9.6/lib/rucio/daemons/c3po/collectors/mock_did.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/c3po/collectors/network_metrics.py` & `rucio-1.9.6/lib/rucio/daemons/c3po/collectors/network_metrics.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/c3po/collectors/workload.py` & `rucio-1.9.6/lib/rucio/daemons/c3po/collectors/workload.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/c3po/utils/dataset_cache.py` & `rucio-1.9.6/lib/rucio/daemons/c3po/utils/dataset_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py` & `rucio-1.9.6/lib/rucio/daemons/c3po/utils/expiring_dataset_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/c3po/utils/expiring_list.py` & `rucio-1.9.6/lib/rucio/daemons/c3po/utils/expiring_list.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/c3po/utils/popularity.py` & `rucio-1.9.6/lib/rucio/daemons/c3po/utils/popularity.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/c3po/utils/timeseries.py` & `rucio-1.9.6/lib/rucio/daemons/c3po/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/c3po/c3po.py` & `rucio-1.9.6/lib/rucio/daemons/c3po/c3po.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/cache/consumer.py` & `rucio-1.9.6/lib/rucio/daemons/cache/consumer.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/conveyor/common.py` & `rucio-1.9.6/lib/rucio/daemons/conveyor/common.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/conveyor/finisher.py` & `rucio-1.9.6/lib/rucio/daemons/conveyor/finisher.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/conveyor/poller.py` & `rucio-1.9.6/lib/rucio/daemons/conveyor/poller.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/conveyor/poller_latest.py` & `rucio-1.9.6/lib/rucio/daemons/conveyor/poller_latest.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/conveyor/receiver.py` & `rucio-1.9.6/lib/rucio/daemons/conveyor/receiver.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/conveyor/stager.py` & `rucio-1.9.6/lib/rucio/daemons/conveyor/stager.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/conveyor/submitter.py` & `rucio-1.9.6/lib/rucio/daemons/conveyor/submitter.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/conveyor/throttler.py` & `rucio-1.9.6/lib/rucio/daemons/conveyor/throttler.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/conveyor/utils.py` & `rucio-1.9.6/lib/rucio/daemons/conveyor/utils.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/hermes/hermes.py` & `rucio-1.9.6/lib/rucio/daemons/hermes/hermes.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/judge/cleaner.py` & `rucio-1.9.6/lib/rucio/daemons/judge/cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/judge/evaluator.py` & `rucio-1.9.6/lib/rucio/daemons/judge/evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/judge/injector.py` & `rucio-1.9.6/lib/rucio/daemons/judge/injector.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/judge/repairer.py` & `rucio-1.9.6/lib/rucio/daemons/judge/repairer.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/mock/conveyorinjector.py` & `rucio-1.9.6/lib/rucio/daemons/mock/conveyorinjector.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/reaper/dark_reaper.py` & `rucio-1.9.6/lib/rucio/daemons/reaper/dark_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/reaper/light_reaper.py` & `rucio-1.9.6/lib/rucio/daemons/reaper/light_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/reaper/reaper.py` & `rucio-1.9.6/lib/rucio/daemons/reaper/reaper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright European Organization for Nuclear Research (CERN)
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Authors:
-# - Vincent Garonne, <vincent.garonne@cern.ch>, 2012-2016
+# - Vincent Garonne, <vincent.garonne@cern.ch>, 2012-2017
 # - Cedric Serfon, <cedric.serfon@cern.ch>, 2013-2015
 # - Mario Lassnig, <mario.lassnig@cern.ch>, 2014
 # - Wen Guan, <wen.guan@cern.ch>, 2014-2016
 # - Thomas Beermann <thomas.beermann@cern.ch>, 2016
 
 '''
 Reaper is a daemon to manage file deletion.
@@ -34,16 +34,17 @@
                                     DatabaseException, UnsupportedOperation,
                                     ReplicaNotFound, RSENotFound)
 from rucio.common.utils import chunks
 from rucio.core import monitor
 from rucio.core import rse as rse_core
 from rucio.core.heartbeat import live, die, sanity_check
 from rucio.core.message import add_message
-from rucio.core.replica import list_unlocked_replicas, update_replicas_states, delete_replicas
-from rucio.core.rse import sort_rses
+from rucio.core.replica import (list_unlocked_replicas, update_replicas_states,
+                                delete_replicas)
+from rucio.core.rse import get_rse_attribute, sort_rses
 from rucio.core.rse_expression_parser import parse_expression
 from rucio.rse import rsemanager as rsemgr
 
 
 logging.getLogger("requests").setLevel(logging.CRITICAL)
 
 logging.basicConfig(stream=sys.stdout,
@@ -68,45 +69,67 @@
     limits = rse_core.get_rse_limits(rse=rse, rse_id=rse_id)
     if not limits and 'MinFreeSpace' not in limits and 'MaxBeingDeletedFiles' not in limits:
         return max_being_deleted_files, needed_free_space, used, free
 
     min_free_space = limits.get('MinFreeSpace')
     max_being_deleted_files = limits.get('MaxBeingDeletedFiles')
 
-    # Get total space available
-    usage = rse_core.get_rse_usage(rse=rse, rse_id=rse_id, source='srm')
+    # Check from which sources to get used and total spaces
+    # Default is storage
+    source_for_total_space, source_for_used_space = 'storage', 'storage'
+    values = get_rse_attribute(rse_id=rse_id, key='sourceForTotalSpace')
+    if values:
+        source_for_total_space = values[0]
+    values = get_rse_attribute(rse_id=rse_id, key='sourceForUsedSpace')
+    if values:
+        source_for_used_space = values[0]
+
+    logging.debug('RSE: %(rse)s, sourceForTotalSpace: %(source_for_total_space)s, '
+                  'sourceForUsedSpace: %(source_for_used_space)s' % locals())
+
+    # Get total and used space
+    usage = rse_core.get_rse_usage(rse=rse, rse_id=rse_id, source=source_for_total_space)
     if not usage:
         return max_being_deleted_files, needed_free_space, used, free
-
     for var in usage:
         total, used = var['total'], var['used']
         break
 
+    if source_for_total_space != source_for_used_space:
+        usage = rse_core.get_rse_usage(rse=rse, rse_id=rse_id, source=source_for_used_space)
+        if not usage:
+            return max_being_deleted_files, needed_free_space, None, free
+        for var in usage:
+            used = var['used']
+            break
+
     free = total - used
     if min_free_space:
         needed_free_space = min_free_space - free
 
     return max_being_deleted_files, needed_free_space, used, free
 
 
-def reaper(rses, worker_number=1, child_number=1, total_children=1, chunk_size=100, once=False, greedy=False, scheme=None, delay_seconds=0):
+def reaper(rses, worker_number=1, child_number=1, total_children=1, chunk_size=100,
+           once=False, greedy=False, scheme=None, delay_seconds=0):
     """
     Main loop to select and delete files.
 
     :param rses: List of RSEs the reaper should work against. If empty, it considers all RSEs.
     :param worker_number: The worker number.
     :param child_number: The child number.
     :param total_children: The total number of children created per worker.
     :param chunk_size: the size of chunk for deletion.
     :param once: If True, only runs one iteration of the main loop.
     :param greedy: If True, delete right away replicas with tombstone.
     :param scheme: Force the reaper to use a particular protocol, e.g., mock.
     :param exclude_rses: RSE expression to exclude RSEs from the Reaper.
     """
-    logging.info('Starting Reaper: Worker %(worker_number)s, child %(child_number)s will work on RSEs: ' % locals() + ', '.join([rse['rse'] for rse in rses]))
+    logging.info('Starting Reaper: Worker %(worker_number)s, '
+                 'child %(child_number)s will work on RSEs: ' % locals() + ', '.join([rse['rse'] for rse in rses]))
 
     pid = os.getpid()
     thread = threading.current_thread()
     hostname = socket.gethostname()
     executable = ' '.join(sys.argv)
     # Generate a hash just for the subset of RSEs
     rse_names = [rse['rse'] for rse in rses]
@@ -269,14 +292,15 @@
                                     add_message('deletion-failed', {'scope': replica['scope'],
                                                                     'name': replica['name'],
                                                                     'rse': rse_info['rse'],
                                                                     'file-size': replica['bytes'],
                                                                     'bytes': replica['bytes'],
                                                                     'url': replica['pfn'],
                                                                     'reason': str(error)})
+                                    break
                             finally:
                                 prot.close()
                             start = time.time()
                             with monitor.record_timer_block('reaper.delete_replicas'):
                                 delete_replicas(rse=rse['rse'], files=deleted_files)
                             logging.debug('Reaper %s-%s: delete_replicas successes %s %s %s', worker_number, child_number, rse['rse'], len(deleted_files), time.time() - start)
                             monitor.record_counter(counters='reaper.deletion.done', delta=len(deleted_files))
```

### Comparing `rucio-1.9.5/lib/rucio/daemons/tracer/kronos.py` & `rucio-1.9.6/lib/rucio/daemons/tracer/kronos.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/atropos.py` & `rucio-1.9.6/lib/rucio/daemons/atropos.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/necromancer.py` & `rucio-1.9.6/lib/rucio/daemons/necromancer.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/transmogrifier.py` & `rucio-1.9.6/lib/rucio/daemons/transmogrifier.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/daemons/undertaker.py` & `rucio-1.9.6/lib/rucio/daemons/undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/0437a40dbfd1_add_eol_at_in_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/102efcf145f4_added_stuck_at_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/14ec5aeb64cf_add_request_external_host.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/156fb5b5a14_add_request_type_to_requests_idx.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/16a0aca82e12_create_index_on_table_replicas_path.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/1803333ac20f_adding_provenance_and_phys_group.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/1a29d6a9504c_add_didtype_chck_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/1a80adff031a_create_index_on_rules_hist_recent.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/1d1215494e95_add_quarantined_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/1d96f484df21_asynchronous_rules_and_rule_approval.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/1fc15ab60d43_add_message_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/21d6b9dc9961_add_mismatch_scheme_state_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/22cf51430c78_add_availability_column_to_table_rses.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/22d887e4ec0a_create_sources_table.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/25821a8a45a3_remove_unique_constraint_on_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/25fc855625cf_added_unique_constraint_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/269fee20dee9_add_repair_cnt_to_locks.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/271a46ea6244_add_ignore_availability_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/277b5fbb41d3_switch_heartbeats_executable.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/2854cd9e168_added_rule_id_column.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/2af3291ec4c_added_replicas_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/2b8e7bcb4783_add_config_table.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/2ba5229cb54c_add_submitted_at_to_requests_table.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/2edee4a83846_add_source_to_requests_and_requests_.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/2eef46be23d4_change_tokens_pk.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/2f648fc909f3_index_in_rule_history_on_scope_name.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/3082b8cef557_add_naming_convention_table_and_closed_.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/3152492b110b_added_staging_area_column.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/32c7d2783f7e_create_bad_replicas_table.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/35ef10d1e11b_change_index_on_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/379a19b5332d_create_rse_limits_table.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/384b96aa0f60_created_rule_history_tables.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/3ad36e2268b0_create_collection_replicas_updates_table.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/3c9df354071b_extend_waiting_request_state.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/3d9813fab443_add_a_new_state_lost_in_badfilesstatus.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/40ad39ce3160_add_transferred_at_to_requests_table.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/4207be2fd914_add_notification_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/42db2617c364_create_index_on_requests_external_id.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/436827b13f82_added_column_activity_to_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/44278720f774_update_requests_typ_sta_upd_idx_index.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/45378a1e76a8_create_collection_replica_table.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/469d262be19_removing_created_at_index.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/4783c1f49cb4_create_distance_table.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/49a21b4d4357_create_index_on_table_tokens.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/4a2cbedda8b9_add_source_replica_expression_column_to_.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/4a7182d9578b_added_bytes_length_accessed_at_columns.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/4bab9edd01fc_create_index_on_requests_rule_id.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/4c3a4acfe006_new_attr_account_table.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/4cf0a2e127d4_adding_transient_metadata.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/52fd9f4916fa_added_activity_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/575767d9f89_added_source_history_table.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/58bff7008037_add_started_at_to_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/58c8b78301ab_rename_callback_to_message.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/5f139f77382a_added_child_rule_id_column.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/6e572a9bfbf3_add_new_split_container_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/70587619328_add_comment_column_for_subscriptions.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/914b8f02df38_new_table_for_lifetime_model_exceptions.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/a5f6f6e928a7_1_7_0.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/a616581ee47_added_columns_to_table_requests.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/a93e4e47bda_heartbeats.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/ae2a56fcc89_added_comment_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/bb695f45c04_extend_request_state.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/c129ccdb2d5_add_lumiblocknr_to_dids.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/d6dceb1de2d_added_purge_column_to_rules.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/d91002c5841_new_account_limits_table.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/versions/fe8ea2fa9788_added_third_party_copy_column_to_rse_.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/migrate_repo/env.py` & `rucio-1.9.6/lib/rucio/db/sqla/migrate_repo/env.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/constants.py` & `rucio-1.9.6/lib/rucio/db/sqla/constants.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/enum.py` & `rucio-1.9.6/lib/rucio/db/sqla/enum.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/history.py` & `rucio-1.9.6/lib/rucio/db/sqla/history.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/models.py` & `rucio-1.9.6/lib/rucio/db/sqla/models.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/sautils.py` & `rucio-1.9.6/lib/rucio/db/sqla/sautils.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/session.py` & `rucio-1.9.6/lib/rucio/db/sqla/session.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/types.py` & `rucio-1.9.6/lib/rucio/db/sqla/types.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/db/sqla/util.py` & `rucio-1.9.6/lib/rucio/db/sqla/util.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/cache.py` & `rucio-1.9.6/lib/rucio/rse/protocols/cache.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/dummy.py` & `rucio-1.9.6/lib/rucio/rse/protocols/dummy.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/gfal.py` & `rucio-1.9.6/lib/rucio/rse/protocols/gfal.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/gfalv2.py` & `rucio-1.9.6/lib/rucio/rse/protocols/gfalv2.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/gsiftp.py` & `rucio-1.9.6/lib/rucio/rse/protocols/gsiftp.py`

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

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/http_cache.py` & `rucio-1.9.6/lib/rucio/rse/protocols/http_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/mock.py` & `rucio-1.9.6/lib/rucio/rse/protocols/mock.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/ngarc.py` & `rucio-1.9.6/lib/rucio/rse/protocols/ngarc.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/posix.py` & `rucio-1.9.6/lib/rucio/rse/protocols/posix.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/protocol.py` & `rucio-1.9.6/lib/rucio/rse/protocols/protocol.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/rfio.py` & `rucio-1.9.6/lib/rucio/rse/protocols/rfio.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/s3.py` & `rucio-1.9.6/lib/rucio/rse/protocols/s3.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/s3boto.py` & `rucio-1.9.6/lib/rucio/rse/protocols/s3boto.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/s3es.py` & `rucio-1.9.6/lib/rucio/rse/protocols/s3es.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/sftp.py` & `rucio-1.9.6/lib/rucio/rse/protocols/sftp.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/signeds3.py` & `rucio-1.9.6/lib/rucio/rse/protocols/signeds3.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/srm.py` & `rucio-1.9.6/lib/rucio/rse/protocols/srm.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/webdav.py` & `rucio-1.9.6/lib/rucio/rse/protocols/webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/protocols/xrootd.py` & `rucio-1.9.6/lib/rucio/rse/protocols/xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/__init__.py` & `rucio-1.9.6/lib/rucio/rse/__init__.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/rse/rsemanager.py` & `rucio-1.9.6/lib/rucio/rse/rsemanager.py`

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

### Comparing `rucio-1.9.5/lib/rucio/tests/daemons/Automatix.py` & `rucio-1.9.6/lib/rucio/tests/daemons/Automatix.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/emulation/usecases/auth.py` & `rucio-1.9.6/lib/rucio/tests/emulation/usecases/auth.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/emulation/usecases/dummy.py` & `rucio-1.9.6/lib/rucio/tests/emulation/usecases/dummy.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/emulation/usecases/dummy_template.py` & `rucio-1.9.6/lib/rucio/tests/emulation/usecases/dummy_template.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/emulation/usecases/jdoe.py` & `rucio-1.9.6/lib/rucio/tests/emulation/usecases/jdoe.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/emulation/usecases/panda.py` & `rucio-1.9.6/lib/rucio/tests/emulation/usecases/panda.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/emulation/usecases/panda_new.py` & `rucio-1.9.6/lib/rucio/tests/emulation/usecases/panda_new.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/emulation/usecases/tzero.py` & `rucio-1.9.6/lib/rucio/tests/emulation/usecases/tzero.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/emulation/emulator.py` & `rucio-1.9.6/lib/rucio/tests/emulation/emulator.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/emulation/ucemulator.py` & `rucio-1.9.6/lib/rucio/tests/emulation/ucemulator.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/emulation/ucprocess.py` & `rucio-1.9.6/lib/rucio/tests/emulation/ucprocess.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/emulation/worker.py` & `rucio-1.9.6/lib/rucio/tests/emulation/worker.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/functional/blocks/block1.py` & `rucio-1.9.6/lib/rucio/tests/functional/blocks/block1.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/functional/blocks/block2.py` & `rucio-1.9.6/lib/rucio/tests/functional/blocks/block2.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/functional/run.py` & `rucio-1.9.6/lib/rucio/tests/functional/run.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/mock/web/fts3.py` & `rucio-1.9.6/lib/rucio/tests/mock/web/fts3.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/mock/fts3.py` & `rucio-1.9.6/lib/rucio/tests/mock/fts3.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/mock/gfal2.py` & `rucio-1.9.6/lib/rucio/tests/mock/gfal2.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/common.py` & `rucio-1.9.6/lib/rucio/tests/common.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/rsemgr_api_test.py` & `rucio-1.9.6/lib/rucio/tests/rsemgr_api_test.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_account.py` & `rucio-1.9.6/lib/rucio/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_account_limits.py` & `rucio-1.9.6/lib/rucio/tests/test_account_limits.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_alembic.py` & `rucio-1.9.6/lib/rucio/tests/test_alembic.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_auditor.py` & `rucio-1.9.6/lib/rucio/tests/test_auditor.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_auditor_hdfs.py` & `rucio-1.9.6/lib/rucio/tests/test_auditor_hdfs.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_auditor_srmdumps.py` & `rucio-1.9.6/lib/rucio/tests/test_auditor_srmdumps.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_authentication.py` & `rucio-1.9.6/lib/rucio/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_bb8.py` & `rucio-1.9.6/lib/rucio/tests/test_bb8.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_bin_rucio.py` & `rucio-1.9.6/lib/rucio/tests/test_bin_rucio.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_clients.py` & `rucio-1.9.6/lib/rucio/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_config.py` & `rucio-1.9.6/lib/rucio/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_conveyor.py` & `rucio-1.9.6/lib/rucio/tests/test_conveyor.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_counter.py` & `rucio-1.9.6/lib/rucio/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_curl.py` & `rucio-1.9.6/lib/rucio/tests/test_curl.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_dataset_replicas.py` & `rucio-1.9.6/lib/rucio/tests/test_dataset_replicas.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_db.py` & `rucio-1.9.6/lib/rucio/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_did.py` & `rucio-1.9.6/lib/rucio/tests/test_did.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_dumper.py` & `rucio-1.9.6/lib/rucio/tests/test_dumper.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_dumper_consistency.py` & `rucio-1.9.6/lib/rucio/tests/test_dumper_consistency.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_dumper_data_model.py` & `rucio-1.9.6/lib/rucio/tests/test_dumper_data_model.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_dumper_path_parsing.py` & `rucio-1.9.6/lib/rucio/tests/test_dumper_path_parsing.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_heartbeat.py` & `rucio-1.9.6/lib/rucio/tests/test_heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_hermes.py` & `rucio-1.9.6/lib/rucio/tests/test_hermes.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_identity.py` & `rucio-1.9.6/lib/rucio/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_judge_cleaner.py` & `rucio-1.9.6/lib/rucio/tests/test_judge_cleaner.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_judge_evaluator.py` & `rucio-1.9.6/lib/rucio/tests/test_judge_evaluator.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_judge_injector.py` & `rucio-1.9.6/lib/rucio/tests/test_judge_injector.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_judge_repairer.py` & `rucio-1.9.6/lib/rucio/tests/test_judge_repairer.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_message.py` & `rucio-1.9.6/lib/rucio/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_meta.py` & `rucio-1.9.6/lib/rucio/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_meta_did.py` & `rucio-1.9.6/lib/rucio/tests/test_meta_did.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_monitor.py` & `rucio-1.9.6/lib/rucio/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_naming_convention.py` & `rucio-1.9.6/lib/rucio/tests/test_naming_convention.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_objectstore.py` & `rucio-1.9.6/lib/rucio/tests/test_objectstore.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_permission.py` & `rucio-1.9.6/lib/rucio/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_ping.py` & `rucio-1.9.6/lib/rucio/tests/test_ping.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_quarantined_replica.py` & `rucio-1.9.6/lib/rucio/tests/test_quarantined_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_reaper.py` & `rucio-1.9.6/lib/rucio/tests/test_reaper.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_redirect.py` & `rucio-1.9.6/lib/rucio/tests/test_redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_replica.py` & `rucio-1.9.6/lib/rucio/tests/test_replica.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_rse.py` & `rucio-1.9.6/lib/rucio/tests/test_rse.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_rse_expression_parser.py` & `rucio-1.9.6/lib/rucio/tests/test_rse_expression_parser.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_rse_protocol_gfal2.py` & `rucio-1.9.6/lib/rucio/tests/test_rse_protocol_gfal2.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_rse_protocol_mock.py` & `rucio-1.9.6/lib/rucio/tests/test_rse_protocol_mock.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_rse_protocol_posix.py` & `rucio-1.9.6/lib/rucio/tests/test_rse_protocol_posix.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_rse_protocol_s3.py` & `rucio-1.9.6/lib/rucio/tests/test_rse_protocol_s3.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_rse_protocol_s3boto.py` & `rucio-1.9.6/lib/rucio/tests/test_rse_protocol_s3boto.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_rse_protocol_s3es.py` & `rucio-1.9.6/lib/rucio/tests/test_rse_protocol_s3es.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_rse_protocol_sftp.py` & `rucio-1.9.6/lib/rucio/tests/test_rse_protocol_sftp.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_rse_protocol_signeds3.py` & `rucio-1.9.6/lib/rucio/tests/test_rse_protocol_signeds3.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_rse_protocol_srm.py` & `rucio-1.9.6/lib/rucio/tests/test_rse_protocol_srm.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_rse_protocol_webdav.py` & `rucio-1.9.6/lib/rucio/tests/test_rse_protocol_webdav.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_rse_protocol_xrootd.py` & `rucio-1.9.6/lib/rucio/tests/test_rse_protocol_xrootd.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_rucio_cache.py` & `rucio-1.9.6/lib/rucio/tests/test_rucio_cache.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_rucio_server.py` & `rucio-1.9.6/lib/rucio/tests/test_rucio_server.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_rule.py` & `rucio-1.9.6/lib/rucio/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_scope.py` & `rucio-1.9.6/lib/rucio/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_subscription.py` & `rucio-1.9.6/lib/rucio/tests/test_subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_temporary_did.py` & `rucio-1.9.6/lib/rucio/tests/test_temporary_did.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_trace.py` & `rucio-1.9.6/lib/rucio/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/tests/test_undertaker.py` & `rucio-1.9.6/lib/rucio/tests/test_undertaker.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/transfertool/fts3.py` & `rucio-1.9.6/lib/rucio/transfertool/fts3.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/account.py` & `rucio-1.9.6/lib/rucio/web/rest/account.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/account_limit.py` & `rucio-1.9.6/lib/rucio/web/rest/account_limit.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/authentication.py` & `rucio-1.9.6/lib/rucio/web/rest/authentication.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/common.py` & `rucio-1.9.6/lib/rucio/web/rest/common.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/config.py` & `rucio-1.9.6/lib/rucio/web/rest/config.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/did.py` & `rucio-1.9.6/lib/rucio/web/rest/did.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/heartbeat.py` & `rucio-1.9.6/lib/rucio/web/rest/heartbeat.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/identity.py` & `rucio-1.9.6/lib/rucio/web/rest/identity.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/lock.py` & `rucio-1.9.6/lib/rucio/web/rest/lock.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/meta.py` & `rucio-1.9.6/lib/rucio/web/rest/meta.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/nongrid_trace.py` & `rucio-1.9.6/lib/rucio/web/rest/nongrid_trace.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/objectstore.py` & `rucio-1.9.6/lib/rucio/web/rest/objectstore.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/ping.py` & `rucio-1.9.6/lib/rucio/web/rest/ping.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/redirect.py` & `rucio-1.9.6/lib/rucio/web/rest/redirect.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/replica.py` & `rucio-1.9.6/lib/rucio/web/rest/replica.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/request.py` & `rucio-1.9.6/lib/rucio/web/rest/request.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/rse.py` & `rucio-1.9.6/lib/rucio/web/rest/rse.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/rule.py` & `rucio-1.9.6/lib/rucio/web/rest/rule.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/scope.py` & `rucio-1.9.6/lib/rucio/web/rest/scope.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/subscription.py` & `rucio-1.9.6/lib/rucio/web/rest/subscription.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/temporary_did.py` & `rucio-1.9.6/lib/rucio/web/rest/temporary_did.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/web/rest/trace.py` & `rucio-1.9.6/lib/rucio/web/rest/trace.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/lib/rucio/version.py` & `rucio-1.9.6/lib/rucio/version.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/boost_long_fts_jobs` & `rucio-1.9.6/tools/probes/common/boost_long_fts_jobs`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_WebDAV_ping` & `rucio-1.9.6/tools/probes/common/check_WebDAV_ping`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_activemq_queue` & `rucio-1.9.6/tools/probes/common/check_activemq_queue`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_ami` & `rucio-1.9.6/tools/probes/common/check_ami`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_clean_staging_areas` & `rucio-1.9.6/tools/probes/common/check_clean_staging_areas`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_cloud_srm_space` & `rucio-1.9.6/tools/probes/common/check_cloud_srm_space`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_deletable_replicas` & `rucio-1.9.6/tools/probes/common/check_deletable_replicas`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_disabled_rses` & `rucio-1.9.6/tools/probes/common/check_disabled_rses`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_expired_dids` & `rucio-1.9.6/tools/probes/common/check_expired_dids`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_expired_es_indices` & `rucio-1.9.6/tools/probes/common/check_expired_es_indices`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_expired_locked_rules` & `rucio-1.9.6/tools/probes/common/check_expired_locked_rules`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_expired_rules` & `rucio-1.9.6/tools/probes/common/check_expired_rules`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_free_space` & `rucio-1.9.6/tools/probes/common/check_free_space`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_fts_backlog` & `rucio-1.9.6/tools/probes/common/check_fts_backlog`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_gridftp_space` & `rucio-1.9.6/tools/probes/common/check_gridftp_space`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_injecting_rules` & `rucio-1.9.6/tools/probes/common/check_injecting_rules`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_log` & `rucio-1.9.6/tools/probes/common/check_log`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_lost_files` & `rucio-1.9.6/tools/probes/common/check_lost_files`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_map_voms_roles` & `rucio-1.9.6/tools/probes/common/check_map_voms_roles`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_messages_to_submit` & `rucio-1.9.6/tools/probes/common/check_messages_to_submit`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_new_dids` & `rucio-1.9.6/tools/probes/common/check_new_dids`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_obsolete_replicas` & `rucio-1.9.6/tools/probes/common/check_obsolete_replicas`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_oracle` & `rucio-1.9.6/tools/probes/common/check_oracle`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_oracle_partitions` & `rucio-1.9.6/tools/probes/common/check_oracle_partitions`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_ping_rucio_servers` & `rucio-1.9.6/tools/probes/common/check_ping_rucio_servers`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_quotas` & `rucio-1.9.6/tools/probes/common/check_quotas`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_redis` & `rucio-1.9.6/tools/probes/common/check_redis`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_requests_to_rses` & `rucio-1.9.6/tools/probes/common/check_requests_to_rses`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_rse_attributes` & `rucio-1.9.6/tools/probes/common/check_rse_attributes`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 # You may obtain a copy of the License at
 #                       http://www.apache.org/licenses/LICENSE-2.0
 #
 # Authors:
 # - Vincent Garonne, <vincent.garonne@cern.ch>, 2013-2014
 # - David Cameron, <david.cameron@cern.ch>, 2014-2015
 # - Tomas Kouba, <tomas.kouba@cern.ch>, 2014
-# - Cedric Serfon, <cedric.serfon@cern.ch>, 2016
+# - Cedric Serfon, <cedric.serfon@cern.ch>, 2016-2017
 
 import json
-import requests
 import sys
 import traceback
+import requests
 
 from rucio.common.exception import RucioException, RSENotFound
 from rucio.api import rse as r
 
 UNKNOWN = 3
 CRITICAL = 2
 WARNING = 1
@@ -42,16 +42,16 @@
 # Takes DDM endpoint information from AGIS and adds selected attributes to RSEs
 if __name__ == '__main__':
 
     url = 'http://atlas-agis-api.cern.ch/request/ddmendpoint/query/list/?json&state=ACTIVE&site_state=ACTIVE'
     try:
         resp = requests.get(url=url)
         data = json.loads(resp.content)
-    except Exception, e:
-        print "Failed to load info from AGIS: %s" % str(e)
+    except Exception as error:
+        print "Failed to load info from AGIS: %s" % str(error)
         sys.exit(WARNING)
 
     for rse in data:
 
         name = rse['name']
 
         # Check if RSE exists
@@ -66,14 +66,16 @@
             r.add_rse_attribute(name, 'ALL', '1', 'root')
             r.add_rse_attribute(name, 'tier', str(rse['tier_level']), 'root')
             r.add_rse_attribute(name, 'istape', str(rse['is_tape']), 'root')
             r.add_rse_attribute(name, 'cloud', str(rse['cloud']), 'root')
             r.add_rse_attribute(name, 'spacetoken', str(rse['token']), 'root')
             r.add_rse_attribute(name, 'site', str(rse['site']), 'root')
             r.add_rse_attribute(name, 'type', str(rse['type']), 'root')
+            if str(rse['space_method']) == 'other':
+                r.add_rse_attribute(name, 'space_usage_method', 'json', 'root')
             if rse['type'] == 'LOCALGROUPDISK' or rse['type'] == 'USERDISK':
                 country = countrycodes[str(rse['country'])]
                 if name.startswith('CERN'):
                     country = 'cern'
                 r.add_rse_attribute(name, 'country', country, 'root')
             if rse['phys_groups']:
                 r.add_rse_attribute(name, 'physgroup', str(rse['phys_groups'][0]), 'root')
@@ -104,16 +106,16 @@
                 freespace = float(freespace - unavailable_space) / 1000 / 1000 / 1000 / 1000
                 if freespace < 0:
                     freespace = 0
                 else:
                     freespace = int(freespace)
                 r.add_rse_attribute(name, 'freespace', freespace, 'root')
 
-        except RucioException as e:
-            print str(e)
+        except RucioException as error:
+            print str(error)
             sys.exit(CRITICAL)
         except:
             print traceback.format_exc()
             result = WARNING
 
         # TODO: set weights for data distribution here or in other collector
```

### Comparing `rucio-1.9.5/tools/probes/common/check_rses_distance` & `rucio-1.9.6/tools/probes/common/check_rses_distance`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_rule_health` & `rucio-1.9.6/tools/probes/common/check_rule_health`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_rules` & `rucio-1.9.6/tools/probes/common/check_rules`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_set_rse_space_limits` & `rucio-1.9.6/tools/probes/common/check_set_rse_space_limits`

 * *Files 16% similar despite different names*

```diff
@@ -4,97 +4,98 @@
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Authors:
 # - David Cameron, <david.cameron@cern.ch>, 2014-2016
 # - Mario Lassnig, <mario.lassnig@cern.ch>, 2015
+# - Cedric Serfon, <cedric.serfon@cern.ch>, 2017
 
 # Sets the minimum free space on RSEs according to the policy, which is set in
 # the configuration table of Rucio server. A relative and absolute limit are
 # set for the relevant endpoints, for example:
 #  Spacetoken  Free ratio  Free absolute
 #  PRODDISK      25%         10.0 TB
 #
 # The smaller of ratio and absolute is the threshold below which to clean.
 # Some tokens (tape, groupdisk, localgroupdisk) are not cleaned automatically.
 #
-# The capacity of each RSE is SRM used - Rucio used of other RSEs sharing the
+# The capacity of each RSE is Storage used - Rucio used of other RSEs sharing the
 # token. This allows RSEs to use space pledged but not used by other RSEs. The
 # minimum free space is evaluated based on this capacity. In the reaper Rucio
-# calculates the space to clean as MinFreeSpace limit - SRM free, where SRM
-# free is the total SRM capacity - Rucio used for this RSE. Therefore the
+# calculates the space to clean as MinFreeSpace limit - Storage free, where Storage
+# free is the total Storage capacity - Rucio used for this RSE. Therefore the
 # MinFreeSpace limit set here must include all the used space for all the other
 # RSEs in the token.
 
 import json
 import sys
-import requests
 from urlparse import urlparse
+import requests
 
 # Try to use server environment (direct database access). If that fails use
 # client.
 server = False
 try:
-    from rucio.api import rse as c
+    from rucio.api import rse as client
     from rucio.api import config
     server = True
 except:
     from rucio.client import Client
     from rucio.client.configclient import ConfigClient
-    c = Client()
+    client = Client()
     config = ConfigClient()
 
 UNKNOWN, OK, WARNING, CRITICAL = -1, 0, 1, 2
 
 # This is the limit of files to delete in each RSE in the reaper loop. To be
 # decided what is the ideal value and if it should be per RSE.
 max_files_to_delete = 100
 
 
 def TB(size):
     return size / 1000.0**4
 
 # Get endpoint info from AGIS to know the RSEs in each space token
 try:
-    url = 'http://atlas-agis-api.cern.ch/request/ddmendpoint/query/list/?json&state=ACTIVE&site_state=ACTIVE'
-    resp = requests.get(url=url)
+    URL = 'http://atlas-agis-api.cern.ch/request/ddmendpoint/query/list/?json&state=ACTIVE&site_state=ACTIVE'
+    resp = requests.get(url=URL)
     data = json.loads(resp.content)
-except Exception, e:
-    print "Failed to get information from AGIS: %s" % str(e)
+except Exception as error:
+    print "Failed to get information from AGIS: %s" % str(error)
     sys.exit(CRITICAL)
 
 # Map of RSE: hostname
 rse_host = {}
 for endpoint in data:
     host = urlparse(endpoint['se']).hostname
     if host:
         rse_host[endpoint['name']] = host
 
 try:
-    rses = [rse['rse'] for rse in c.list_rses()]
-except Exception, e:
-    print "Failed to get RSEs from Rucio: %s" % str(e)
+    rses = [rse['rse'] for rse in client.list_rses()]
+except Exception as error:
+    print "Failed to get RSEs from Rucio: %s" % str(error)
     sys.exit(CRITICAL)
 
 # Get policy defined in config. Each section is called limitstoken
 # {token: (relative limit in %, absolute limit in TB)}
 policy = {}
 try:
     if server:
-        sections = config.sections('root')
-        for section in [s for s in sections if s.startswith('limits')]:
+        SECTIONS = config.sections('root')
+        for section in [s for s in SECTIONS if s.startswith('limits')]:
             policy[section[6:].upper()] = (config.get(section, 'rellimit', 'root'), config.get(section, 'abslimit', 'root'))
     else:
-        sections = config.get_config()
-        for section in [s for s in sections if s.startswith('limits')]:
-            policy[section[6:].upper()] = (sections[section]['rellimit'], sections[section]['abslimit'])
+        SECTIONS = config.get_config()
+        for section in [s for s in SECTIONS if s.startswith('limits')]:
+            policy[section[6:].upper()] = (SECTIONS[section]['rellimit'], SECTIONS[section]['abslimit'])
 
-except Exception, e:
-    print "Failed to get configuration information from Rucio: %s" % str(e)
+except Exception as error:
+    print "Failed to get configuration information from Rucio: %s" % str(error)
     sys.exit(CRITICAL)
 
 for rse in rses:
 
     tokens = [token for token in policy if rse.endswith(token)]
     if not tokens:
         continue
@@ -105,55 +106,55 @@
 
     token = tokens[0]
 
     if not [r for r in data if r['name'] == rse]:
         print "RSE %s not defined in AGIS" % rse
         continue
     try:
-        spacetoken = c.list_rse_attributes(rse)['spacetoken']
+        spacetoken = client.list_rse_attributes(rse)['spacetoken']
     except:
         print "No space token info for %s" % rse
         continue
 
     # Client and server API are different for get_rse_usage
     try:
         if server:
-            spaceinfo = c.get_rse_usage(rse, None)
+            spaceinfo = client.get_rse_usage(rse, None)
         else:
-            spaceinfo = c.get_rse_usage(rse)
-    except Exception, e:
-        print "Could not get space information for %s: %s" % (rse, str(e))
+            spaceinfo = client.get_rse_usage(rse)
+    except Exception as error:
+        print "Could not get space information for %s: %s" % (rse, str(error))
         continue
 
     spaceinfo = [i for i in spaceinfo]  # Generator can only be used once
 
-    capacity = [source['total'] for source in spaceinfo if source['source'] == 'srm']
-    srmused = [source['used'] for source in spaceinfo if source['source'] == 'srm']
+    capacity = [source['total'] for source in spaceinfo if source['source'] == 'storage']
+    storageused = [source['used'] for source in spaceinfo if source['source'] == 'storage']
     rucioused = [source['used'] for source in spaceinfo if source['source'] == 'rucio']
-    if not capacity or not srmused or not rucioused:
+    if not capacity or not storageused or not rucioused:
         print 'Missing space info for %s' % rse
         continue
     capacity = capacity[0]
-    srmused = srmused[0]
+    storageused = storageused[0]
     rucioused = rucioused[0]
 
-    print "RSE %s: total capacity %sTB, SRM used %sTB, Rucio used %sTB" % (rse, TB(capacity), TB(srmused), TB(rucioused))
+    print "RSE %s: total capacity %sTB, Storage used %sTB, Rucio used %sTB" % (rse, TB(capacity), TB(storageused), TB(rucioused))
 
     # If this RSE shares space with others remove rucio used from total space
     # to calculate the limit
     used_others = 0
     for endpoint in data:
         if endpoint['name'] != rse and (rse_host[endpoint['name']] == rse_host[rse] and spacetoken == endpoint['token']):
             try:
                 if server:
-                    used = c.get_rse_usage(endpoint['name'], None, source='rucio')
+                    used = client.get_rse_usage(endpoint['name'], None, source='rucio')
                 else:
-                    used = c.get_rse_usage(endpoint['name'], filters={'source': 'rucio'})
-            except Exception, e:
-                print "Could not get used Rucio space for %s: %s" % (endpoint['name'], str(e))
+                    used = client.get_rse_usage(endpoint['name'], filters={'source': 'rucio'})
+            except Exception as error:
+                print "Could not get used Rucio space for %s: %s" % (endpoint['name'], str(error))
                 continue
 
             used = [source['used'] for source in used if source['source'] == 'rucio']
             if not used:
                 print "No Rucio used space information for %s" % rse
                 continue
             used = used[0]
@@ -165,19 +166,19 @@
     print "Remaining capacity for %s: %sTB" % (rse, TB(capacity))
 
     minfree = min(capacity * policy[token][0] / 100.0, policy[token][1] * (1000**4))
     print "RSE %s: calculated minimum free space %sTB" % (rse, TB(minfree))
 
     try:
         if server:
-            c.set_rse_limits(rse, 'MinFreeSpace', minfree, 'root')
-            c.set_rse_limits(rse, 'MaxBeingDeletedFiles', max_files_to_delete, 'root')
+            client.set_rse_limits(rse, 'MinFreeSpace', minfree, 'root')
+            client.set_rse_limits(rse, 'MaxBeingDeletedFiles', max_files_to_delete, 'root')
         else:
-            c.set_rse_limits(rse, 'MinFreeSpace', minfree)
-            c.set_rse_limits(rse, 'MaxBeingDeletedFiles', max_files_to_delete)
-    except Exception, e:
-        print "Failed to set RSE limits for %s: %s" % (rse, str(e))
+            client.set_rse_limits(rse, 'MinFreeSpace', minfree)
+            client.set_rse_limits(rse, 'MaxBeingDeletedFiles', max_files_to_delete)
+    except Exception as error:
+        print "Failed to set RSE limits for %s: %s" % (rse, str(error))
         continue
 
     print "Set MinFreeSpace for %s to %fTB" % (rse, TB(minfree))
 
 sys.exit(OK)
```

### Comparing `rucio-1.9.5/tools/probes/common/check_site_status` & `rucio-1.9.6/tools/probes/common/check_site_status`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_srm_space` & `rucio-1.9.6/tools/probes/common/check_srm_space`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_stalled_fts_connections` & `rucio-1.9.6/tools/probes/common/check_stalled_fts_connections`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_stresstest_dids_requests_replicas_daily` & `rucio-1.9.6/tools/probes/common/check_stresstest_dids_requests_replicas_daily`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_stresstest_dids_requests_replicas_hourly` & `rucio-1.9.6/tools/probes/common/check_stresstest_dids_requests_replicas_hourly`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_stresstest_replicas_replicating_time_hourly` & `rucio-1.9.6/tools/probes/common/check_stresstest_replicas_replicating_time_hourly`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_stresstest_replicas_replicating_time_statistics_2hours` & `rucio-1.9.6/tools/probes/common/check_stresstest_replicas_replicating_time_statistics_2hours`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_stresstest_replicas_replicating_time_statistics_daily` & `rucio-1.9.6/tools/probes/common/check_stresstest_replicas_replicating_time_statistics_daily`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_stuck_rules` & `rucio-1.9.6/tools/probes/common/check_stuck_rules`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_sync_rses_with_agis` & `rucio-1.9.6/tools/probes/common/check_sync_rses_with_agis`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_transfer_queues_status` & `rucio-1.9.6/tools/probes/common/check_transfer_queues_status`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_unevaluated_dids` & `rucio-1.9.6/tools/probes/common/check_unevaluated_dids`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_unlocked_replicas` & `rucio-1.9.6/tools/probes/common/check_unlocked_replicas`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_updated_account_counters` & `rucio-1.9.6/tools/probes/common/check_updated_account_counters`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_updated_dids` & `rucio-1.9.6/tools/probes/common/check_updated_dids`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_updated_rse_counters` & `rucio-1.9.6/tools/probes/common/check_updated_rse_counters`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_used_space` & `rucio-1.9.6/tools/probes/common/check_used_space`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_voms` & `rucio-1.9.6/tools/probes/common/check_voms`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_voms_admin` & `rucio-1.9.6/tools/probes/common/check_voms_admin`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_webDAV_service` & `rucio-1.9.6/tools/probes/common/check_webDAV_service`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/check_webdav_space` & `rucio-1.9.6/tools/probes/common/check_webdav_space`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/daemon_activity_reports` & `rucio-1.9.6/tools/probes/common/daemon_activity_reports`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/graphite2nagios` & `rucio-1.9.6/tools/probes/common/graphite2nagios`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/monitor_apache` & `rucio-1.9.6/tools/probes/common/monitor_apache`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/monitor_client` & `rucio-1.9.6/tools/probes/common/monitor_client`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/monitor_flume` & `rucio-1.9.6/tools/probes/common/monitor_flume`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/monitor_haproxy_local` & `rucio-1.9.6/tools/probes/common/monitor_haproxy_local`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/service_monitoring.cfg` & `rucio-1.9.6/tools/probes/common/service_monitoring.cfg`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/probes/common/service_monitoring.py` & `rucio-1.9.6/tools/probes/common/service_monitoring.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/bootstrap.py` & `rucio-1.9.6/tools/bootstrap.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/pip-requires` & `rucio-1.9.6/tools/pip-requires`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/pip-requires-client` & `rucio-1.9.6/tools/pip-requires-client`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/pip-requires-test` & `rucio-1.9.6/tools/pip-requires-test`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/tools/reset_database.py` & `rucio-1.9.6/tools/reset_database.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/AUTHORS` & `rucio-1.9.6/AUTHORS`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/MANIFEST.in` & `rucio-1.9.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/pylintrc` & `rucio-1.9.6/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/setup.cfg` & `rucio-1.9.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/setup.py` & `rucio-1.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `rucio-1.9.5/PKG-INFO` & `rucio-1.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rucio
-Version: 1.9.5
+Version: 1.9.6
 Summary: Rucio Package
 Home-page: http://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

