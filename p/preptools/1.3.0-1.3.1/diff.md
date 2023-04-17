# Comparing `tmp/preptools-1.3.0.tar.gz` & `tmp/preptools-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/preptools-1.3.0.tar", last modified: Wed Apr  6 10:08:45 2022, max compression
+gzip compressed data, was "dist/preptools-1.3.1.tar", last modified: Mon Apr 17 07:25:48 2023, max compression
```

## Comparing `preptools-1.3.0.tar` & `preptools-1.3.1.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 10:08:45.000000 preptools-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)    88599 2022-04-06 10:08:45.000000 preptools-1.3.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)    72084 2022-04-06 10:08:38.000000 preptools-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 10:08:45.000000 preptools-1.3.0/preptools/
--rwxr-xr-x   0 runner    (1001) docker     (121)      680 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      793 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 10:08:45.000000 preptools-1.3.0/preptools/command/
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3468 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/bond_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     3265 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/common_command.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 10:08:45.000000 preptools-1.3.0/preptools/command/make_proposal/
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/make_proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1824 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/make_proposal/accumulated_validation_failure_slashing_rate_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1686 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/make_proposal/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/make_proposal/malicious_score_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/make_proposal/missed_network_proposal_vote_slashing_rate_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     2372 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/make_proposal/network_score_designation_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     2261 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/make_proposal/network_score_update_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/make_proposal/prep_disqualification_command.py
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/make_proposal/revision_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/make_proposal/reward_fund_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/make_proposal/reward_funds_allocation_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/make_proposal/step_costs_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/make_proposal/step_price_command.py
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/make_proposal/text_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/make_proposal_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     3364 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/prep_info_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     9862 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/prep_setting_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     3367 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/proposal_info_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     7498 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/proposal_setting_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     3706 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/register_proposal2_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/tx_info_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/command/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 10:08:45.000000 preptools-1.3.0/preptools/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11075 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/core/prep.py
--rw-r--r--   0 runner    (1001) docker     (121)     3789 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     3477 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/preptools_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 10:08:45.000000 preptools-1.3.0/preptools/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2975 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/utils/argparse_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3221 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/utils/preptools_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3175 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11360 2022-04-06 10:08:38.000000 preptools-1.3.0/preptools/utils/validation_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 10:08:45.000000 preptools-1.3.0/preptools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    88599 2022-04-06 10:08:45.000000 preptools-1.3.0/preptools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2022-04-06 10:08:45.000000 preptools-1.3.0/preptools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-06 10:08:45.000000 preptools-1.3.0/preptools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-04-06 10:08:45.000000 preptools-1.3.0/preptools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-04-06 10:08:45.000000 preptools-1.3.0/preptools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-04-06 10:08:45.000000 preptools-1.3.0/preptools.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)       67 2022-04-06 10:08:45.000000 preptools-1.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1468 2022-04-06 10:08:38.000000 preptools-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:25:48.000000 preptools-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    89449 2023-04-17 07:25:48.000000 preptools-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    72589 2023-04-17 07:25:38.000000 preptools-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:25:48.000000 preptools-1.3.1/preptools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      680 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      793 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:25:48.000000 preptools-1.3.1/preptools/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/bond_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/common_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:25:48.000000 preptools-1.3.1/preptools/command/make_proposal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/make_proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/make_proposal/accumulated_validation_failure_slashing_rate_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/make_proposal/call_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/make_proposal/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/make_proposal/malicious_score_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/make_proposal/missed_network_proposal_vote_slashing_rate_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/make_proposal/network_score_designation_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/make_proposal/network_score_update_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/make_proposal/prep_disqualification_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/make_proposal/revision_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/make_proposal/reward_fund_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/make_proposal/reward_funds_allocation_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/make_proposal/step_costs_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/make_proposal/step_price_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/make_proposal/text_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/make_proposal_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/prep_info_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/prep_setting_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/proposal_info_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/proposal_setting_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/register_proposal2_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/tx_info_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/command/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:25:48.000000 preptools-1.3.1/preptools/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/core/prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/preptools_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:25:48.000000 preptools-1.3.1/preptools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/utils/argparse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/utils/preptools_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/utils/validation_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 07:25:38.000000 preptools-1.3.1/preptools/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 07:25:48.000000 preptools-1.3.1/preptools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    89449 2023-04-17 07:25:48.000000 preptools-1.3.1/preptools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-17 07:25:48.000000 preptools-1.3.1/preptools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 07:25:48.000000 preptools-1.3.1/preptools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-17 07:25:48.000000 preptools-1.3.1/preptools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-17 07:25:48.000000 preptools-1.3.1/preptools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 07:25:48.000000 preptools-1.3.1/preptools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-17 07:25:48.000000 preptools-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-17 07:25:38.000000 preptools-1.3.1/setup.py
```

### Comparing `preptools-1.3.0/PKG-INFO` & `preptools-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: preptools
-Version: 1.3.0
+Version: 1.3.1
 Summary: P-Rep management command line interface
 Home-page: https://github.com/icon-project/preptools
 Author: ICON Foundation
 Author-email: foo@icon.foundation
 License: Apache License 2.0
-Description: [![unittest](https://img.shields.io/github/workflow/status/icon-project/preptools/unittest%20and%20publish%20to%20pypi/master?label=unittest&logo=github)](https://github.com/icon-project/preptools/actions/workflows/preptools-workflow.yml)
+Description: [![unittest](https://img.shields.io/github/actions/workflow/status/icon-project/preptools/preptools-workflow.yml?branch=master&label=unittest&logo=github)](https://github.com/icon-project/preptools/actions/workflows/preptools-workflow.yml)
         [![PyPI - latest](https://img.shields.io/pypi/v/preptools?label=latest&logo=pypi)](https://pypi.org/project/preptools)
         [![PyPI - Python](https://img.shields.io/pypi/pyversions/preptools?logo=pypi)](https://pypi.org/project/preptools)
         
         # P-Rep tools (preptools) Tutorial
         
         * This document is intended to explain how to use preptools.
         * This guide will walk through the basics of setting up the development environment and the usage of preptools CLI commands.
@@ -71,15 +71,15 @@
         
         ```bash
         (venv) $ preptools                                                                                                                                                                                                                            [12:10:25]
         usage: preptools [-h]
                          {registerPRep,unregisterPRep,setPRep,setGovernanceVariables,setBonderList,getPRep,getBonderList,getPReps,registerProposal,cancelProposal,voteProposal,applyProposal,makeProposal,registerProposal2,getProposal,getProposals,setStake,getStake,setBond,getBond,txresult,txbyhash,keystore,genconf}
                          ...
         
-        P-Rep management command line interface v1.3.0
+        P-Rep management command line interface v1.3.1
         
         optional arguments:
           -h, --help            show this help message and exit
         
         subcommands:
           {registerPRep,unregisterPRep,setPRep,setGovernanceVariables,setBonderList,getPRep,getBonderList,getPReps,registerProposal,cancelProposal,voteProposal,applyProposal,makeProposal,registerProposal2,getProposal,getProposals,setStake,getStake,setBond,getBond,txresult,txbyhash,keystore,genconf}
             registerPRep        Register P-Rep
@@ -921,15 +921,15 @@
             "id": 1234
         }
         ```
         
         #### registerProposal2
         
         * The command is used to register network protocols in a new format supported by governance-2.x.x score.
-        * CAUTION: Each time a proposer run this command, he/or she will be charged a fee of `100 ICX`.
+        * CAUTION: a proposer must pay a fee of `100 ICX` to submit a proposal to blockchain.
         * For more detail on the new protocol specification, refer to [governance2 score registerProposal format](https://github.com/icon-project/governance2#registerproposal).
         * The new proposal format will make main P-Reps possible handle multiple proposals with a transaction. 
         
         *Usage*
         
         ```bash
         (venv) $ preptools registerProposal2 -h                                                                                                                       [14:37:44]
@@ -976,78 +976,79 @@
         
         (venv) $ cat step_costs.json
         {"name":"stepCosts","value":{"get":"0x19","getBase":"0xc8","input":"0xc8"}}
         ```
         
         #### makeProposal
         
-        This command is used to make a variety of network proposal contents easily.
-        Note that there is no network cit does not communicate with blockchain but just creates the content of a specific network proposal.
-        The proposal content created here is used as a parameters of [registerProposal2](#registerproposal2) command.
+        * This command is used to make a variety of network proposal contents easily.
+        * Note that it does not have any connection to blockchain while making the content of a specific network proposal.
+        * The created proposal content is used as a parameter of [registerProposal2](#registerproposal2) command.
         
-        **> Usage**
+        *Usage*
         
         ```bash
         (venv) $ preptools makeProposal -h
         usage: preptools makeProposal [-h]
-                                      {text,revision,maliciousScore,prepDisqualification,stepPrice,stepCosts,rewardFund,rewardFundsAllocation,networkScoreDesignation,networkScoreUpdate,accumulatedValidationFailureSlashingRate,missedNetworkProposalVoteSlashingRate}
+                                      {text,revision,maliciousScore,prepDisqualification,stepPrice,stepCosts,rewardFund,rewardFundsAllocation,networkScoreDesignation,networkScoreUpdate,accumulatedValidationFailureSlashingRate,missedNetworkProposalVoteSlashingRate,call}
                                       ...
         
         positional arguments:
-          {text,revision,maliciousScore,prepDisqualification,stepPrice,stepCosts,rewardFund,rewardFundsAllocation,networkScoreDesignation,networkScoreUpdate,accumulatedValidationFailureSlashingRate,missedNetworkProposalVoteSlashingRate}
+          {text,revision,maliciousScore,prepDisqualification,stepPrice,stepCosts,rewardFund,rewardFundsAllocation,networkScoreDesignation,networkScoreUpdate,accumulatedValidationFailureSlashingRate,missedNetworkProposalVoteSlashingRate,call}
             text                text network proposal
             revision            revision network proposal
             maliciousScore      maliciousScore network proposal
             prepDisqualification
                                 prepDisqualification network proposal
             stepPrice           stepPrice network proposal
             stepCosts           stepCosts network proposal
-            rewardFund          rewardFund network proposal for Monthly Reward Fund
-                                Setting
+            rewardFund          rewardFund network proposal for Monthly Reward Fund Setting
             rewardFundsAllocation
-                                rewardFundsAllocation network proposal to determine
-                                the allocation of the monthly reward fund
+                                rewardFundsAllocation network proposal to determine the allocation of the monthly reward fund
             networkScoreDesignation
                                 networkScoreDesignation network proposal
             networkScoreUpdate  networkScoreUpdate network proposal
             accumulatedValidationFailureSlashingRate
-                                accumulatedValidationFailureSlashingRate network
-                                proposal
+                                accumulatedValidationFailureSlashingRate network proposal
             missedNetworkProposalVoteSlashingRate
                                 missedNetworkProposalVoteSlashingRate network proposal
+            call                call network proposal
         
         optional arguments:
           -h, --help            show this help message and exit
         ```  
           
-        **> Example**
+        *Example*
         
         ```bash
-        (venv) $ preptools makeProposal rewardFund -h                                                                                                                  [15:08:12]
-        usage: preptools makeProposal rewardFund [-h] [-o OUTPUT] iglobal
+        (venv) $ preptools makeProposal call -h
+        usage: preptools makeProposal call [-h] [-o OUTPUT] [--params PARAMS [PARAMS ...]] to method
         
         positional arguments:
-          iglobal               The total amount of monthly reward fund in loop
+          to                    SCORE address
+          method                method name to call
         
         optional arguments:
           -h, --help            show this help message and exit
           -o OUTPUT, --output OUTPUT
                                 filepath to save proposal contents
-                                
-        (venv) $ preptools makeProposal rewardFund 3000000000000000000000000 -o reward_fund.json
-        (venv) $ cat reward_fund.json
-        {"name":"rewardFund","value":{"iglobal":"0x27b46536c66c8e3000000"}}
+          --params PARAMS [PARAMS ...]
+                                Arguments information to be passed to method (TYPE@VALUE[@FIELDS], FIELDS required if parameter is struct or []struct)
+        
+        (venv) $ preptools makeProposal call cx0000000000000000000000000000000000000000 openBTPNetwork \
+            --params str@eth str@sepolia Address@cxf1b0808f09138fffdb890772315aeabb37072a8a
+        {"name":"call","value":{"to":"cx0000000000000000000000000000000000000000","method":"openBTPNetwork","params":[{"type":"str","value":"eth"},{"type":"str","value":"sepolia"},{"type":"Address","value":"cxf1b0808f09138fffdb890772315aeabb37072a8a"}]}}
         ```
         
         #### voteProposal
         
         *Description*
         
-        Vote Network-proposal  
-        Refer to [voteProposal request format](https://github.com/icon-project/governance2#voteproposal) for details.
+        * Votes for Network-proposal.
+        * Refer to [voteProposal request format](https://github.com/icon-project/governance2#voteproposal) for details.
         
         *Usage*
         
         ```bash
         usage: preptools voteProposal [-h] [--url URL] [--nid NID] [--config CONFIG]
                                       [--yes] [--verbose] [--password PASSWORD]
                                       [--keystore KEYSTORE]
@@ -1176,19 +1177,23 @@
         * Applies an approved network proposal to the network.
         * It should be executed within the voting period, otherwise the proposal will be expired and cannot be applied anymore.
         * Refer to [applyProposal request format](https://github.com/icon-project/governance2#applyproposal) for details.
         
         *Usage*
         
         ```bash
-        (venv) $ preptools applyProposal -h
+        (venv) $ preptools applyProposal -h                                                                                                                                                                                                                                           [12:07:48]
         usage: preptools applyProposal [-h] [--url URL] [--nid NID] [--config CONFIG]
                                        [--yes] [--verbose] [--password PASSWORD]
                                        [--keystore KEYSTORE] [--step-limit STEP_LIMIT]
-                                       [--step-margin STEP_MARGIN] --id ID
+                                       [--step-margin STEP_MARGIN]
+                                       id
+        
+        positional arguments:
+          id                    hash of registerProposal TX
         
         optional arguments:
           -h, --help            show this help message and exit
           --url URL, -u URL     node url default(http://127.0.0.1:9000/api/v3)
           --nid NID, -n NID     networkId default(3) ex) mainnet(1), testnet(2)
           --config CONFIG, -c CONFIG
                                 preptools config file path
@@ -1200,23 +1205,20 @@
                                 keystore file path
           --step-limit STEP_LIMIT, -s STEP_LIMIT
                                 step limit to set
           --step-margin STEP_MARGIN, -m STEP_MARGIN
                                 Can be used when step-limit option is not given. Set
                                 step-limit value to estimated Step + this value(step-
                                 margin)
-          --id ID               hash of registerProposal TX
-          
-        (venv) $ preptools applyProposal  
         ```
         
         *Example*
         
         ```bash
-        (venv) $ preptools applyProposal -k prep_keys0 --id 0x02221f9346f9c9b3322ea33e67a1ca0fbe9491e0ea3aefb5154a43e2ea829fa4
+        (venv) $ preptools applyProposal -k prep_keys0 0x02221f9346f9c9b3322ea33e67a1ca0fbe9491e0ea3aefb5154a43e2ea829fa4
         > Password:
         [Request] ======================================================================
         {
             "from_": "hxb74e29fba1809a105fdec433040a4e713bbe91fe",
             "to": "cx0000000000000000000000000000000000000001",
             "value": 0,
             "step_limit": 268435456,
@@ -1993,10 +1995,17 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `preptools-1.3.0/README.md` & `preptools-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![unittest](https://img.shields.io/github/workflow/status/icon-project/preptools/unittest%20and%20publish%20to%20pypi/master?label=unittest&logo=github)](https://github.com/icon-project/preptools/actions/workflows/preptools-workflow.yml)
+[![unittest](https://img.shields.io/github/actions/workflow/status/icon-project/preptools/preptools-workflow.yml?branch=master&label=unittest&logo=github)](https://github.com/icon-project/preptools/actions/workflows/preptools-workflow.yml)
 [![PyPI - latest](https://img.shields.io/pypi/v/preptools?label=latest&logo=pypi)](https://pypi.org/project/preptools)
 [![PyPI - Python](https://img.shields.io/pypi/pyversions/preptools?logo=pypi)](https://pypi.org/project/preptools)
 
 # P-Rep tools (preptools) Tutorial
 
 * This document is intended to explain how to use preptools.
 * This guide will walk through the basics of setting up the development environment and the usage of preptools CLI commands.
@@ -63,15 +63,15 @@
 
 ```bash
 (venv) $ preptools                                                                                                                                                                                                                            [12:10:25]
 usage: preptools [-h]
                  {registerPRep,unregisterPRep,setPRep,setGovernanceVariables,setBonderList,getPRep,getBonderList,getPReps,registerProposal,cancelProposal,voteProposal,applyProposal,makeProposal,registerProposal2,getProposal,getProposals,setStake,getStake,setBond,getBond,txresult,txbyhash,keystore,genconf}
                  ...
 
-P-Rep management command line interface v1.3.0
+P-Rep management command line interface v1.3.1
 
 optional arguments:
   -h, --help            show this help message and exit
 
 subcommands:
   {registerPRep,unregisterPRep,setPRep,setGovernanceVariables,setBonderList,getPRep,getBonderList,getPReps,registerProposal,cancelProposal,voteProposal,applyProposal,makeProposal,registerProposal2,getProposal,getProposals,setStake,getStake,setBond,getBond,txresult,txbyhash,keystore,genconf}
     registerPRep        Register P-Rep
@@ -913,15 +913,15 @@
     "id": 1234
 }
 ```
 
 #### registerProposal2
 
 * The command is used to register network protocols in a new format supported by governance-2.x.x score.
-* CAUTION: Each time a proposer run this command, he/or she will be charged a fee of `100 ICX`.
+* CAUTION: a proposer must pay a fee of `100 ICX` to submit a proposal to blockchain.
 * For more detail on the new protocol specification, refer to [governance2 score registerProposal format](https://github.com/icon-project/governance2#registerproposal).
 * The new proposal format will make main P-Reps possible handle multiple proposals with a transaction. 
 
 *Usage*
 
 ```bash
 (venv) $ preptools registerProposal2 -h                                                                                                                       [14:37:44]
@@ -968,78 +968,79 @@
 
 (venv) $ cat step_costs.json
 {"name":"stepCosts","value":{"get":"0x19","getBase":"0xc8","input":"0xc8"}}
 ```
 
 #### makeProposal
 
-This command is used to make a variety of network proposal contents easily.
-Note that there is no network cit does not communicate with blockchain but just creates the content of a specific network proposal.
-The proposal content created here is used as a parameters of [registerProposal2](#registerproposal2) command.
+* This command is used to make a variety of network proposal contents easily.
+* Note that it does not have any connection to blockchain while making the content of a specific network proposal.
+* The created proposal content is used as a parameter of [registerProposal2](#registerproposal2) command.
 
-**> Usage**
+*Usage*
 
 ```bash
 (venv) $ preptools makeProposal -h
 usage: preptools makeProposal [-h]
-                              {text,revision,maliciousScore,prepDisqualification,stepPrice,stepCosts,rewardFund,rewardFundsAllocation,networkScoreDesignation,networkScoreUpdate,accumulatedValidationFailureSlashingRate,missedNetworkProposalVoteSlashingRate}
+                              {text,revision,maliciousScore,prepDisqualification,stepPrice,stepCosts,rewardFund,rewardFundsAllocation,networkScoreDesignation,networkScoreUpdate,accumulatedValidationFailureSlashingRate,missedNetworkProposalVoteSlashingRate,call}
                               ...
 
 positional arguments:
-  {text,revision,maliciousScore,prepDisqualification,stepPrice,stepCosts,rewardFund,rewardFundsAllocation,networkScoreDesignation,networkScoreUpdate,accumulatedValidationFailureSlashingRate,missedNetworkProposalVoteSlashingRate}
+  {text,revision,maliciousScore,prepDisqualification,stepPrice,stepCosts,rewardFund,rewardFundsAllocation,networkScoreDesignation,networkScoreUpdate,accumulatedValidationFailureSlashingRate,missedNetworkProposalVoteSlashingRate,call}
     text                text network proposal
     revision            revision network proposal
     maliciousScore      maliciousScore network proposal
     prepDisqualification
                         prepDisqualification network proposal
     stepPrice           stepPrice network proposal
     stepCosts           stepCosts network proposal
-    rewardFund          rewardFund network proposal for Monthly Reward Fund
-                        Setting
+    rewardFund          rewardFund network proposal for Monthly Reward Fund Setting
     rewardFundsAllocation
-                        rewardFundsAllocation network proposal to determine
-                        the allocation of the monthly reward fund
+                        rewardFundsAllocation network proposal to determine the allocation of the monthly reward fund
     networkScoreDesignation
                         networkScoreDesignation network proposal
     networkScoreUpdate  networkScoreUpdate network proposal
     accumulatedValidationFailureSlashingRate
-                        accumulatedValidationFailureSlashingRate network
-                        proposal
+                        accumulatedValidationFailureSlashingRate network proposal
     missedNetworkProposalVoteSlashingRate
                         missedNetworkProposalVoteSlashingRate network proposal
+    call                call network proposal
 
 optional arguments:
   -h, --help            show this help message and exit
 ```  
   
-**> Example**
+*Example*
 
 ```bash
-(venv) $ preptools makeProposal rewardFund -h                                                                                                                  [15:08:12]
-usage: preptools makeProposal rewardFund [-h] [-o OUTPUT] iglobal
+(venv) $ preptools makeProposal call -h
+usage: preptools makeProposal call [-h] [-o OUTPUT] [--params PARAMS [PARAMS ...]] to method
 
 positional arguments:
-  iglobal               The total amount of monthly reward fund in loop
+  to                    SCORE address
+  method                method name to call
 
 optional arguments:
   -h, --help            show this help message and exit
   -o OUTPUT, --output OUTPUT
                         filepath to save proposal contents
-                        
-(venv) $ preptools makeProposal rewardFund 3000000000000000000000000 -o reward_fund.json
-(venv) $ cat reward_fund.json
-{"name":"rewardFund","value":{"iglobal":"0x27b46536c66c8e3000000"}}
+  --params PARAMS [PARAMS ...]
+                        Arguments information to be passed to method (TYPE@VALUE[@FIELDS], FIELDS required if parameter is struct or []struct)
+
+(venv) $ preptools makeProposal call cx0000000000000000000000000000000000000000 openBTPNetwork \
+    --params str@eth str@sepolia Address@cxf1b0808f09138fffdb890772315aeabb37072a8a
+{"name":"call","value":{"to":"cx0000000000000000000000000000000000000000","method":"openBTPNetwork","params":[{"type":"str","value":"eth"},{"type":"str","value":"sepolia"},{"type":"Address","value":"cxf1b0808f09138fffdb890772315aeabb37072a8a"}]}}
 ```
 
 #### voteProposal
 
 *Description*
 
-Vote Network-proposal  
-Refer to [voteProposal request format](https://github.com/icon-project/governance2#voteproposal) for details.
+* Votes for Network-proposal.
+* Refer to [voteProposal request format](https://github.com/icon-project/governance2#voteproposal) for details.
 
 *Usage*
 
 ```bash
 usage: preptools voteProposal [-h] [--url URL] [--nid NID] [--config CONFIG]
                               [--yes] [--verbose] [--password PASSWORD]
                               [--keystore KEYSTORE]
@@ -1168,19 +1169,23 @@
 * Applies an approved network proposal to the network.
 * It should be executed within the voting period, otherwise the proposal will be expired and cannot be applied anymore.
 * Refer to [applyProposal request format](https://github.com/icon-project/governance2#applyproposal) for details.
 
 *Usage*
 
 ```bash
-(venv) $ preptools applyProposal -h
+(venv) $ preptools applyProposal -h                                                                                                                                                                                                                                           [12:07:48]
 usage: preptools applyProposal [-h] [--url URL] [--nid NID] [--config CONFIG]
                                [--yes] [--verbose] [--password PASSWORD]
                                [--keystore KEYSTORE] [--step-limit STEP_LIMIT]
-                               [--step-margin STEP_MARGIN] --id ID
+                               [--step-margin STEP_MARGIN]
+                               id
+
+positional arguments:
+  id                    hash of registerProposal TX
 
 optional arguments:
   -h, --help            show this help message and exit
   --url URL, -u URL     node url default(http://127.0.0.1:9000/api/v3)
   --nid NID, -n NID     networkId default(3) ex) mainnet(1), testnet(2)
   --config CONFIG, -c CONFIG
                         preptools config file path
@@ -1192,23 +1197,20 @@
                         keystore file path
   --step-limit STEP_LIMIT, -s STEP_LIMIT
                         step limit to set
   --step-margin STEP_MARGIN, -m STEP_MARGIN
                         Can be used when step-limit option is not given. Set
                         step-limit value to estimated Step + this value(step-
                         margin)
-  --id ID               hash of registerProposal TX
-  
-(venv) $ preptools applyProposal  
 ```
 
 *Example*
 
 ```bash
-(venv) $ preptools applyProposal -k prep_keys0 --id 0x02221f9346f9c9b3322ea33e67a1ca0fbe9491e0ea3aefb5154a43e2ea829fa4
+(venv) $ preptools applyProposal -k prep_keys0 0x02221f9346f9c9b3322ea33e67a1ca0fbe9491e0ea3aefb5154a43e2ea829fa4
 > Password:
 [Request] ======================================================================
 {
     "from_": "hxb74e29fba1809a105fdec433040a4e713bbe91fe",
     "to": "cx0000000000000000000000000000000000000001",
     "value": 0,
     "step_limit": 268435456,
```

### Comparing `preptools-1.3.0/preptools/__init__.py` & `preptools-1.3.1/preptools/__init__.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/__main__.py` & `preptools-1.3.1/preptools/__main__.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/__init__.py` & `preptools-1.3.1/preptools/command/__init__.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/bond_command.py` & `preptools-1.3.1/preptools/command/bond_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/common_command.py` & `preptools-1.3.1/preptools/command/common_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/make_proposal/__init__.py` & `preptools-1.3.1/preptools/command/make_proposal/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,8 +21,9 @@
     step_costs_command,
     reward_fund_command,
     reward_funds_allocation_command,
     network_score_designation_command,
     network_score_update_command,
     accumulated_validation_failure_slashing_rate_command,
     missed_network_proposal_vote_slashing_rate_command,
+    call_method,
 )
```

### Comparing `preptools-1.3.0/preptools/command/make_proposal/accumulated_validation_failure_slashing_rate_command.py` & `preptools-1.3.1/preptools/command/make_proposal/accumulated_validation_failure_slashing_rate_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/make_proposal/command.py` & `preptools-1.3.1/preptools/command/make_proposal/command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/make_proposal/malicious_score_command.py` & `preptools-1.3.1/preptools/command/make_proposal/malicious_score_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/make_proposal/missed_network_proposal_vote_slashing_rate_command.py` & `preptools-1.3.1/preptools/command/make_proposal/missed_network_proposal_vote_slashing_rate_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/make_proposal/network_score_designation_command.py` & `preptools-1.3.1/preptools/command/make_proposal/network_score_designation_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/make_proposal/network_score_update_command.py` & `preptools-1.3.1/preptools/command/make_proposal/network_score_update_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/make_proposal/prep_disqualification_command.py` & `preptools-1.3.1/preptools/command/make_proposal/prep_disqualification_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/make_proposal/revision_command.py` & `preptools-1.3.1/preptools/command/make_proposal/revision_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/make_proposal/reward_fund_command.py` & `preptools-1.3.1/preptools/command/make_proposal/reward_fund_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/make_proposal/reward_funds_allocation_command.py` & `preptools-1.3.1/preptools/command/make_proposal/reward_funds_allocation_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/make_proposal/step_costs_command.py` & `preptools-1.3.1/preptools/command/make_proposal/step_costs_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/make_proposal/step_price_command.py` & `preptools-1.3.1/preptools/command/make_proposal/step_price_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/make_proposal/text_command.py` & `preptools-1.3.1/preptools/command/make_proposal/text_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/make_proposal_command.py` & `preptools-1.3.1/preptools/command/make_proposal_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/prep_info_command.py` & `preptools-1.3.1/preptools/command/prep_info_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/prep_setting_command.py` & `preptools-1.3.1/preptools/command/prep_setting_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/proposal_info_command.py` & `preptools-1.3.1/preptools/command/proposal_info_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/proposal_setting_command.py` & `preptools-1.3.1/preptools/command/proposal_setting_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/register_proposal2_command.py` & `preptools-1.3.1/preptools/command/register_proposal2_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/tx_info_command.py` & `preptools-1.3.1/preptools/command/tx_info_command.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/command/utils.py` & `preptools-1.3.1/preptools/command/utils.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/core/prep.py` & `preptools-1.3.1/preptools/core/prep.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/exception.py` & `preptools-1.3.1/preptools/exception.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/preptools_cli.py` & `preptools-1.3.1/preptools/preptools_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import argparse
 import sys
 from typing import Dict, Any, Optional
 
-from iconsdk.exception import IconServiceBaseException
 from .command import *
 from .exception import PRepToolsExceptionCode, PRepToolsBaseException
 from .utils.constants import DEFAULT_NID, DEFAULT_URL
 from .utils.utils import get_preptools_version
 from .utils.utils import print_response
 
 
@@ -58,15 +57,15 @@
     try:
         args = parser.parse_args()
         if not hasattr(args, "func"):
             parser.print_help(sys.stderr)
             sys.exit(exit_code)
 
         response: Optional[dict, int, str] = args.func(args)
-    except (PRepToolsBaseException, IconServiceBaseException) as e:
+    except PRepToolsBaseException as e:
         response: Dict[str, Any] = e.message
         exit_code = e.code.value
     except Exception as e:
         response = str(e)
         exit_code = PRepToolsExceptionCode.COMMAND_ERROR.value
     except KeyboardInterrupt:
         response = "\nexit"
```

### Comparing `preptools-1.3.0/preptools/utils/argparse_utils.py` & `preptools-1.3.1/preptools/utils/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/utils/constants.py` & `preptools-1.3.1/preptools/utils/constants.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/utils/utils.py` & `preptools-1.3.1/preptools/utils/utils.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools/utils/validation_checker.py` & `preptools-1.3.1/preptools/utils/validation_checker.py`

 * *Files identical despite different names*

### Comparing `preptools-1.3.0/preptools.egg-info/PKG-INFO` & `preptools-1.3.1/preptools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: preptools
-Version: 1.3.0
+Version: 1.3.1
 Summary: P-Rep management command line interface
 Home-page: https://github.com/icon-project/preptools
 Author: ICON Foundation
 Author-email: foo@icon.foundation
 License: Apache License 2.0
-Description: [![unittest](https://img.shields.io/github/workflow/status/icon-project/preptools/unittest%20and%20publish%20to%20pypi/master?label=unittest&logo=github)](https://github.com/icon-project/preptools/actions/workflows/preptools-workflow.yml)
+Description: [![unittest](https://img.shields.io/github/actions/workflow/status/icon-project/preptools/preptools-workflow.yml?branch=master&label=unittest&logo=github)](https://github.com/icon-project/preptools/actions/workflows/preptools-workflow.yml)
         [![PyPI - latest](https://img.shields.io/pypi/v/preptools?label=latest&logo=pypi)](https://pypi.org/project/preptools)
         [![PyPI - Python](https://img.shields.io/pypi/pyversions/preptools?logo=pypi)](https://pypi.org/project/preptools)
         
         # P-Rep tools (preptools) Tutorial
         
         * This document is intended to explain how to use preptools.
         * This guide will walk through the basics of setting up the development environment and the usage of preptools CLI commands.
@@ -71,15 +71,15 @@
         
         ```bash
         (venv) $ preptools                                                                                                                                                                                                                            [12:10:25]
         usage: preptools [-h]
                          {registerPRep,unregisterPRep,setPRep,setGovernanceVariables,setBonderList,getPRep,getBonderList,getPReps,registerProposal,cancelProposal,voteProposal,applyProposal,makeProposal,registerProposal2,getProposal,getProposals,setStake,getStake,setBond,getBond,txresult,txbyhash,keystore,genconf}
                          ...
         
-        P-Rep management command line interface v1.3.0
+        P-Rep management command line interface v1.3.1
         
         optional arguments:
           -h, --help            show this help message and exit
         
         subcommands:
           {registerPRep,unregisterPRep,setPRep,setGovernanceVariables,setBonderList,getPRep,getBonderList,getPReps,registerProposal,cancelProposal,voteProposal,applyProposal,makeProposal,registerProposal2,getProposal,getProposals,setStake,getStake,setBond,getBond,txresult,txbyhash,keystore,genconf}
             registerPRep        Register P-Rep
@@ -921,15 +921,15 @@
             "id": 1234
         }
         ```
         
         #### registerProposal2
         
         * The command is used to register network protocols in a new format supported by governance-2.x.x score.
-        * CAUTION: Each time a proposer run this command, he/or she will be charged a fee of `100 ICX`.
+        * CAUTION: a proposer must pay a fee of `100 ICX` to submit a proposal to blockchain.
         * For more detail on the new protocol specification, refer to [governance2 score registerProposal format](https://github.com/icon-project/governance2#registerproposal).
         * The new proposal format will make main P-Reps possible handle multiple proposals with a transaction. 
         
         *Usage*
         
         ```bash
         (venv) $ preptools registerProposal2 -h                                                                                                                       [14:37:44]
@@ -976,78 +976,79 @@
         
         (venv) $ cat step_costs.json
         {"name":"stepCosts","value":{"get":"0x19","getBase":"0xc8","input":"0xc8"}}
         ```
         
         #### makeProposal
         
-        This command is used to make a variety of network proposal contents easily.
-        Note that there is no network cit does not communicate with blockchain but just creates the content of a specific network proposal.
-        The proposal content created here is used as a parameters of [registerProposal2](#registerproposal2) command.
+        * This command is used to make a variety of network proposal contents easily.
+        * Note that it does not have any connection to blockchain while making the content of a specific network proposal.
+        * The created proposal content is used as a parameter of [registerProposal2](#registerproposal2) command.
         
-        **> Usage**
+        *Usage*
         
         ```bash
         (venv) $ preptools makeProposal -h
         usage: preptools makeProposal [-h]
-                                      {text,revision,maliciousScore,prepDisqualification,stepPrice,stepCosts,rewardFund,rewardFundsAllocation,networkScoreDesignation,networkScoreUpdate,accumulatedValidationFailureSlashingRate,missedNetworkProposalVoteSlashingRate}
+                                      {text,revision,maliciousScore,prepDisqualification,stepPrice,stepCosts,rewardFund,rewardFundsAllocation,networkScoreDesignation,networkScoreUpdate,accumulatedValidationFailureSlashingRate,missedNetworkProposalVoteSlashingRate,call}
                                       ...
         
         positional arguments:
-          {text,revision,maliciousScore,prepDisqualification,stepPrice,stepCosts,rewardFund,rewardFundsAllocation,networkScoreDesignation,networkScoreUpdate,accumulatedValidationFailureSlashingRate,missedNetworkProposalVoteSlashingRate}
+          {text,revision,maliciousScore,prepDisqualification,stepPrice,stepCosts,rewardFund,rewardFundsAllocation,networkScoreDesignation,networkScoreUpdate,accumulatedValidationFailureSlashingRate,missedNetworkProposalVoteSlashingRate,call}
             text                text network proposal
             revision            revision network proposal
             maliciousScore      maliciousScore network proposal
             prepDisqualification
                                 prepDisqualification network proposal
             stepPrice           stepPrice network proposal
             stepCosts           stepCosts network proposal
-            rewardFund          rewardFund network proposal for Monthly Reward Fund
-                                Setting
+            rewardFund          rewardFund network proposal for Monthly Reward Fund Setting
             rewardFundsAllocation
-                                rewardFundsAllocation network proposal to determine
-                                the allocation of the monthly reward fund
+                                rewardFundsAllocation network proposal to determine the allocation of the monthly reward fund
             networkScoreDesignation
                                 networkScoreDesignation network proposal
             networkScoreUpdate  networkScoreUpdate network proposal
             accumulatedValidationFailureSlashingRate
-                                accumulatedValidationFailureSlashingRate network
-                                proposal
+                                accumulatedValidationFailureSlashingRate network proposal
             missedNetworkProposalVoteSlashingRate
                                 missedNetworkProposalVoteSlashingRate network proposal
+            call                call network proposal
         
         optional arguments:
           -h, --help            show this help message and exit
         ```  
           
-        **> Example**
+        *Example*
         
         ```bash
-        (venv) $ preptools makeProposal rewardFund -h                                                                                                                  [15:08:12]
-        usage: preptools makeProposal rewardFund [-h] [-o OUTPUT] iglobal
+        (venv) $ preptools makeProposal call -h
+        usage: preptools makeProposal call [-h] [-o OUTPUT] [--params PARAMS [PARAMS ...]] to method
         
         positional arguments:
-          iglobal               The total amount of monthly reward fund in loop
+          to                    SCORE address
+          method                method name to call
         
         optional arguments:
           -h, --help            show this help message and exit
           -o OUTPUT, --output OUTPUT
                                 filepath to save proposal contents
-                                
-        (venv) $ preptools makeProposal rewardFund 3000000000000000000000000 -o reward_fund.json
-        (venv) $ cat reward_fund.json
-        {"name":"rewardFund","value":{"iglobal":"0x27b46536c66c8e3000000"}}
+          --params PARAMS [PARAMS ...]
+                                Arguments information to be passed to method (TYPE@VALUE[@FIELDS], FIELDS required if parameter is struct or []struct)
+        
+        (venv) $ preptools makeProposal call cx0000000000000000000000000000000000000000 openBTPNetwork \
+            --params str@eth str@sepolia Address@cxf1b0808f09138fffdb890772315aeabb37072a8a
+        {"name":"call","value":{"to":"cx0000000000000000000000000000000000000000","method":"openBTPNetwork","params":[{"type":"str","value":"eth"},{"type":"str","value":"sepolia"},{"type":"Address","value":"cxf1b0808f09138fffdb890772315aeabb37072a8a"}]}}
         ```
         
         #### voteProposal
         
         *Description*
         
-        Vote Network-proposal  
-        Refer to [voteProposal request format](https://github.com/icon-project/governance2#voteproposal) for details.
+        * Votes for Network-proposal.
+        * Refer to [voteProposal request format](https://github.com/icon-project/governance2#voteproposal) for details.
         
         *Usage*
         
         ```bash
         usage: preptools voteProposal [-h] [--url URL] [--nid NID] [--config CONFIG]
                                       [--yes] [--verbose] [--password PASSWORD]
                                       [--keystore KEYSTORE]
@@ -1176,19 +1177,23 @@
         * Applies an approved network proposal to the network.
         * It should be executed within the voting period, otherwise the proposal will be expired and cannot be applied anymore.
         * Refer to [applyProposal request format](https://github.com/icon-project/governance2#applyproposal) for details.
         
         *Usage*
         
         ```bash
-        (venv) $ preptools applyProposal -h
+        (venv) $ preptools applyProposal -h                                                                                                                                                                                                                                           [12:07:48]
         usage: preptools applyProposal [-h] [--url URL] [--nid NID] [--config CONFIG]
                                        [--yes] [--verbose] [--password PASSWORD]
                                        [--keystore KEYSTORE] [--step-limit STEP_LIMIT]
-                                       [--step-margin STEP_MARGIN] --id ID
+                                       [--step-margin STEP_MARGIN]
+                                       id
+        
+        positional arguments:
+          id                    hash of registerProposal TX
         
         optional arguments:
           -h, --help            show this help message and exit
           --url URL, -u URL     node url default(http://127.0.0.1:9000/api/v3)
           --nid NID, -n NID     networkId default(3) ex) mainnet(1), testnet(2)
           --config CONFIG, -c CONFIG
                                 preptools config file path
@@ -1200,23 +1205,20 @@
                                 keystore file path
           --step-limit STEP_LIMIT, -s STEP_LIMIT
                                 step limit to set
           --step-margin STEP_MARGIN, -m STEP_MARGIN
                                 Can be used when step-limit option is not given. Set
                                 step-limit value to estimated Step + this value(step-
                                 margin)
-          --id ID               hash of registerProposal TX
-          
-        (venv) $ preptools applyProposal  
         ```
         
         *Example*
         
         ```bash
-        (venv) $ preptools applyProposal -k prep_keys0 --id 0x02221f9346f9c9b3322ea33e67a1ca0fbe9491e0ea3aefb5154a43e2ea829fa4
+        (venv) $ preptools applyProposal -k prep_keys0 0x02221f9346f9c9b3322ea33e67a1ca0fbe9491e0ea3aefb5154a43e2ea829fa4
         > Password:
         [Request] ======================================================================
         {
             "from_": "hxb74e29fba1809a105fdec433040a4e713bbe91fe",
             "to": "cx0000000000000000000000000000000000000001",
             "value": 0,
             "step_limit": 268435456,
@@ -1993,10 +1995,17 @@
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `preptools-1.3.0/preptools.egg-info/SOURCES.txt` & `preptools-1.3.1/preptools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.md
 setup.cfg
 setup.py
 preptools/__init__.py
 preptools/__main__.py
 preptools/exception.py
 preptools/preptools_cli.py
+preptools/version.py
 preptools.egg-info/PKG-INFO
 preptools.egg-info/SOURCES.txt
 preptools.egg-info/dependency_links.txt
 preptools.egg-info/entry_points.txt
 preptools.egg-info/requires.txt
 preptools.egg-info/top_level.txt
 preptools/command/__init__.py
@@ -20,14 +21,15 @@
 preptools/command/proposal_info_command.py
 preptools/command/proposal_setting_command.py
 preptools/command/register_proposal2_command.py
 preptools/command/tx_info_command.py
 preptools/command/utils.py
 preptools/command/make_proposal/__init__.py
 preptools/command/make_proposal/accumulated_validation_failure_slashing_rate_command.py
+preptools/command/make_proposal/call_method.py
 preptools/command/make_proposal/command.py
 preptools/command/make_proposal/malicious_score_command.py
 preptools/command/make_proposal/missed_network_proposal_vote_slashing_rate_command.py
 preptools/command/make_proposal/network_score_designation_command.py
 preptools/command/make_proposal/network_score_update_command.py
 preptools/command/make_proposal/prep_disqualification_command.py
 preptools/command/make_proposal/revision_command.py
```

