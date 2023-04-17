# Comparing `tmp/aiida-core-2.2.2.tar.gz` & `tmp/aiida-core-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-core-2.2.2.tar", last modified: Fri Feb 10 13:09:43 2023, max compression
+gzip compressed data, was "aiida-core-2.3.0.tar", last modified: Mon Apr 17 09:37:56 2023, max compression
```

## Comparing `aiida-core-2.2.2.tar` & `aiida-core-2.3.0.tar`

### file list

```diff
@@ -1,676 +1,680 @@
--rw-r--r--   0        0        0      759 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.docker/docker-rabbitmq.yml
--rwxr-xr-x   0        0        0       66 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.docker/my_init.d/configure-aiida.sh
--rwxr-xr-x   0        0        0     3720 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.docker/opt/configure-aiida.sh
--rw-r--r--   0        0        0      155 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.dockerignore
--rw-r--r--   0        0        0      649 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/CODEOWNERS
--rw-r--r--   0        0        0      972 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      275 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      434 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/ISSUE_TEMPLATE/doc-improvements.md
--rw-r--r--   0        0        0      754 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      181 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/config/README.md
--rw-r--r--   0        0        0      307 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/config/add-singularity.yaml
--rw-r--r--   0        0        0      163 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/config/add.yaml
--rwxr-xr-x   0        0        0      347 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/config/doubler.sh
--rw-r--r--   0        0        0      199 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/config/doubler.yaml
--rw-r--r--   0        0        0       43 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/config/localhost-config.yaml
--rw-r--r--   0        0        0      274 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/config/localhost.yaml
--rw-r--r--   0        0        0      453 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/config/profile.yaml
--rw-r--r--   0        0        0      130 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/config/slurm-ssh-config.yaml
--rw-r--r--   0        0        0      275 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/config/slurm-ssh.yaml
--rw-r--r--   0        0        0     1679 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/config/slurm_rsa
--rw-r--r--   0        0        0      202 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/system_tests/README.md
--rw-r--r--   0        0        0     3176 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/system_tests/pytest/test_memory_leaks.py
--rw-r--r--   0        0        0     1387 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/system_tests/test_containerized_code.py
--rw-r--r--   0        0        0    24024 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/system_tests/test_daemon.py
--rw-r--r--   0        0        0     1126 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/system_tests/test_ipython_magics.py
--rwxr-xr-x   0        0        0      911 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/system_tests/test_polish_workchains.sh
--rw-r--r--   0        0        0     3912 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/system_tests/test_profile_manager.py
--rw-r--r--   0        0        0     1972 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/system_tests/test_test_manager.py
--rwxr-xr-x   0        0        0     1611 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/system_tests/test_verdi_load_time.sh
--rw-r--r--   0        0        0     8572 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/system_tests/workchains.py
--rw-r--r--   0        0        0     1681 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/benchmark-config.json
--rw-r--r--   0        0        0     2211 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/benchmark.yml
--rw-r--r--   0        0        0     1719 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/build_and_test_docker_on_pr.yml
--rw-r--r--   0        0        0     1327 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/check_release_tag.py
--rw-r--r--   0        0        0     3561 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/ci-code.yml
--rw-r--r--   0        0        0      888 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/ci-style.yml
--rw-r--r--   0        0        0     1086 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/docs-build.yml
--rw-r--r--   0        0        0     3477 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/nightly.yml
--rw-r--r--   0        0        0     1620 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/post-release.yml
--rw-r--r--   0        0        0     1377 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/push_image_to_dockerhub.yml
--rw-r--r--   0        0        0     1696 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/rabbitmq.yml
--rw-r--r--   0        0        0     3095 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/release.yml
--rwxr-xr-x   0        0        0     1814 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/setup.sh
--rw-r--r--   0        0        0    11204 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/test-install.yml
--rwxr-xr-x   0        0        0      898 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/tests.sh
--rwxr-xr-x   0        0        0      589 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/tests_nightly.sh
--rwxr-xr-x   0        0        0     2135 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.github/workflows/verdi.sh
--rw-r--r--   0        0        0      419 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.gitignore
--rw-r--r--   0        0        0     2005 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/README.md
--rw-r--r--   0        0        0      413 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/default/Dockerfile
--rw-r--r--   0        0        0     1790 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/default/config_local.yml
--rw-r--r--   0        0        0     6342 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/default/create_docker.yml
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/default/files/polish/__init__.py
--rwxr-xr-x   0        0        0     7706 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/default/files/polish/cli.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/default/files/polish/lib/__init__.py
--rw-r--r--   0        0        0     5384 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/default/files/polish/lib/expression.py
--rw-r--r--   0        0        0     1032 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/default/files/polish/lib/template/base.tpl
--rw-r--r--   0        0        0     5300 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/default/files/polish/lib/template/workchain.tpl
--rw-r--r--   0        0        0     8117 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/default/files/polish/lib/workchain.py
--rw-r--r--   0        0        0       46 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/default/run_tests.yml
--rw-r--r--   0        0        0     2717 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/default/setup_aiida.yml
--rw-r--r--   0        0        0      716 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/default/setup_python.yml
--rw-r--r--   0        0        0     1650 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/default/tasks/log_query_stats.yml
--rw-r--r--   0        0        0      239 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/default/tasks/reset_query_stats.yml
--rw-r--r--   0        0        0     2814 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.molecule/default/test_polish_workchains.yml
--rw-r--r--   0        0        0     9475 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      802 2023-02-10 13:09:40.018780 aiida-core-2.2.2/.readthedocs.yml
--rw-r--r--   0        0        0     1746 2023-02-10 13:09:40.018780 aiida-core-2.2.2/AUTHORS.txt
--rw-r--r--   0        0        0   182437 2023-02-10 13:09:40.022780 aiida-core-2.2.2/CHANGELOG.md
--rw-r--r--   0        0        0     3352 2023-02-10 13:09:40.022780 aiida-core-2.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      585 2023-02-10 13:09:40.022780 aiida-core-2.2.2/Dockerfile
--rw-r--r--   0        0        0     1312 2023-02-10 13:09:40.022780 aiida-core-2.2.2/LICENSE.txt
--rw-r--r--   0        0        0     5905 2023-02-10 13:09:40.022780 aiida-core-2.2.2/README.md
--rw-r--r--   0        0        0     3610 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/__init__.py
--rw-r--r--   0        0        0      807 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/__main__.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/calculations/__init__.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/calculations/arithmetic/__init__.py
--rw-r--r--   0        0        0     3907 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/calculations/arithmetic/add.py
--rw-r--r--   0        0        0     2547 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/calculations/diff_tutorial/calculations.py
--rw-r--r--   0        0        0        0 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/calculations/importers/__init__.py
--rw-r--r--   0        0        0        0 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/calculations/importers/arithmetic/__init__.py
--rw-r--r--   0        0        0     1644 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/calculations/importers/arithmetic/add.py
--rw-r--r--   0        0        0        0 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/calculations/monitors/__init__.py
--rw-r--r--   0        0        0     1161 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/calculations/monitors/base.py
--rw-r--r--   0        0        0     9273 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/calculations/templatereplacer.py
--rw-r--r--   0        0        0    10738 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/calculations/transfer.py
--rw-r--r--   0        0        0     1734 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/__init__.py
--rw-r--r--   0        0        0     1194 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/__init__.py
--rw-r--r--   0        0        0    19446 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_archive.py
--rw-r--r--   0        0        0    11381 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_calcjob.py
--rw-r--r--   0        0        0    13993 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_code.py
--rw-r--r--   0        0        0    23855 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_computer.py
--rw-r--r--   0        0        0     7900 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_config.py
--rw-r--r--   0        0        0     9512 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_daemon.py
--rw-r--r--   0        0        0      931 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/__init__.py
--rw-r--r--   0        0        0     1332 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_array.py
--rw-r--r--   0        0        0     4803 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_bands.py
--rw-r--r--   0        0        0     4387 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_cif.py
--rw-r--r--   0        0        0     1214 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_dict.py
--rw-r--r--   0        0        0     4692 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_export.py
--rw-r--r--   0        0        0     2889 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_list.py
--rw-r--r--   0        0        0     3594 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_remote.py
--rw-r--r--   0        0        0     8026 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_show.py
--rw-r--r--   0        0        0     1336 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_singlefile.py
--rw-r--r--   0        0        0     8885 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_structure.py
--rw-r--r--   0        0        0     3570 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_trajectory.py
--rw-r--r--   0        0        0     5204 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_upf.py
--rw-r--r--   0        0        0     4761 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_database.py
--rw-r--r--   0        0        0     7557 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_devel.py
--rw-r--r--   0        0        0    18115 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_group.py
--rw-r--r--   0        0        0     1392 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_help.py
--rw-r--r--   0        0        0    19788 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_node.py
--rw-r--r--   0        0        0     2950 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_plugin.py
--rw-r--r--   0        0        0    11205 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_process.py
--rw-r--r--   0        0        0     5739 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_profile.py
--rw-r--r--   0        0        0    14051 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_rabbitmq.py
--rw-r--r--   0        0        0     2530 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_restapi.py
--rw-r--r--   0        0        0     4837 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_run.py
--rw-r--r--   0        0        0     9359 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_setup.py
--rw-r--r--   0        0        0     3439 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_shell.py
--rw-r--r--   0        0        0     6946 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_status.py
--rw-r--r--   0        0        0     6418 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_storage.py
--rw-r--r--   0        0        0     4582 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_user.py
--rw-r--r--   0        0        0     1265 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/commands/cmd_verdi.py
--rw-r--r--   0        0        0      297 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/groups/__init__.py
--rw-r--r--   0        0        0     4949 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/groups/dynamic.py
--rw-r--r--   0        0        0     6501 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/groups/verdi.py
--rw-r--r--   0        0        0     1373 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/params/__init__.py
--rw-r--r--   0        0        0     1277 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/params/arguments/__init__.py
--rw-r--r--   0        0        0     2924 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/params/arguments/main.py
--rw-r--r--   0        0        0     2374 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/params/arguments/overridable.py
--rw-r--r--   0        0        0     2652 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/params/options/__init__.py
--rw-r--r--   0        0        0      697 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/params/options/commands/__init__.py
--rw-r--r--   0        0        0     6869 2023-02-10 13:09:40.022780 aiida-core-2.2.2/aiida/cmdline/params/options/commands/code.py
--rw-r--r--   0        0        0     6882 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/options/commands/computer.py
--rw-r--r--   0        0        0    13950 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/options/commands/setup.py
--rw-r--r--   0        0        0     2383 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/options/conditional.py
--rw-r--r--   0        0        0     2593 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/options/config.py
--rw-r--r--   0        0        0     9190 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/options/interactive.py
--rw-r--r--   0        0        0    20691 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/options/main.py
--rw-r--r--   0        0        0     3764 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/options/multivalue.py
--rw-r--r--   0        0        0     3918 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/options/overridable.py
--rw-r--r--   0        0        0     1739 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/__init__.py
--rw-r--r--   0        0        0     1348 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/calculation.py
--rw-r--r--   0        0        0     2364 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/choice.py
--rw-r--r--   0        0        0     2742 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/code.py
--rw-r--r--   0        0        0     4052 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/computer.py
--rw-r--r--   0        0        0     1714 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/config.py
--rw-r--r--   0        0        0     1311 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/data.py
--rw-r--r--   0        0        0     3901 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/group.py
--rw-r--r--   0        0        0     6199 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/identifier.py
--rw-r--r--   0        0        0     1568 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/multiple.py
--rw-r--r--   0        0        0     1317 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/node.py
--rw-r--r--   0        0        0     4488 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/path.py
--rw-r--r--   0        0        0    10750 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/plugin.py
--rw-r--r--   0        0        0     1329 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/process.py
--rw-r--r--   0        0        0     3766 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/profile.py
--rw-r--r--   0        0        0     3800 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/strings.py
--rw-r--r--   0        0        0     2058 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/user.py
--rw-r--r--   0        0        0     1335 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/params/types/workflow.py
--rw-r--r--   0        0        0      177 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/templates/deprecated.tpl
--rw-r--r--   0        0        0      218 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/templates/multiline.tpl
--rw-r--r--   0        0        0      213 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/templates/new_cmt.txt.tpl
--rw-r--r--   0        0        0      165 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/templates/warning.tpl
--rw-r--r--   0        0        0     1122 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/__init__.py
--rw-r--r--   0        0        0     4001 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/ascii_vis.py
--rw-r--r--   0        0        0    20250 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/common.py
--rw-r--r--   0        0        0     5675 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/daemon.py
--rw-r--r--   0        0        0     8517 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/decorators.py
--rw-r--r--   0        0        0     1764 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/defaults.py
--rw-r--r--   0        0        0    10912 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/echo.py
--rw-r--r--   0        0        0     1768 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/log.py
--rw-r--r--   0        0        0     2336 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/multi_line_input.py
--rw-r--r--   0        0        0     2709 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/pluginable.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/query/__init__.py
--rw-r--r--   0        0        0      981 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/query/calculation.py
--rw-r--r--   0        0        0     1026 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/query/formatting.py
--rw-r--r--   0        0        0     1007 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/query/mapping.py
--rw-r--r--   0        0        0     1393 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/repository.py
--rw-r--r--   0        0        0     5008 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/shell.py
--rw-r--r--   0        0        0      831 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/cmdline/utils/templates.py
--rw-r--r--   0        0        0     2634 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/__init__.py
--rw-r--r--   0        0        0    12464 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/constants.py
--rw-r--r--   0        0        0     8031 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/datastructures.py
--rw-r--r--   0        0        0     6332 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/escaping.py
--rw-r--r--   0        0        0     8794 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/exceptions.py
--rw-r--r--   0        0        0     8975 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/extendeddicts.py
--rw-r--r--   0        0        0     3067 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/files.py
--rw-r--r--   0        0        0    18668 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/folders.py
--rw-r--r--   0        0        0    10933 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/hashing.py
--rw-r--r--   0        0        0     2803 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/json.py
--rw-r--r--   0        0        0     3717 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/lang.py
--rw-r--r--   0        0        0     6586 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/links.py
--rw-r--r--   0        0        0     8836 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/log.py
--rw-r--r--   0        0        0     6909 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/progress_reporter.py
--rw-r--r--   0        0        0     2800 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/timezone.py
--rw-r--r--   0        0        0    19341 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/utils.py
--rw-r--r--   0        0        0     1888 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/common/warnings.py
--rw-r--r--   0        0        0     1996 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/engine/__init__.py
--rw-r--r--   0        0        0      819 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/engine/daemon/__init__.py
--rw-r--r--   0        0        0    24588 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/engine/daemon/client.py
--rw-r--r--   0        0        0    31125 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/engine/daemon/execmanager.py
--rw-r--r--   0        0        0     2295 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/engine/daemon/worker.py
--rw-r--r--   0        0        0      919 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/engine/exceptions.py
--rw-r--r--   0        0        0     5713 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/engine/launch.py
--rw-r--r--   0        0        0     6617 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/engine/persistence.py
--rw-r--r--   0        0        0     1756 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/engine/processes/__init__.py
--rw-r--r--   0        0        0    11817 2023-02-10 13:09:40.026781 aiida-core-2.2.2/aiida/engine/processes/builder.py
--rw-r--r--   0        0        0      937 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/calcjobs/__init__.py
--rw-r--r--   0        0        0    46733 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/calcjobs/calcjob.py
--rw-r--r--   0        0        0     1125 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/calcjobs/importer.py
--rw-r--r--   0        0        0    12526 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/calcjobs/manager.py
--rw-r--r--   0        0        0     8671 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/calcjobs/monitors.py
--rw-r--r--   0        0        0    31883 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/calcjobs/tasks.py
--rw-r--r--   0        0        0    12339 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/control.py
--rw-r--r--   0        0        0     3690 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/exit_code.py
--rw-r--r--   0        0        0    18038 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/functions.py
--rw-r--r--   0        0        0     3852 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/futures.py
--rw-r--r--   0        0        0    10076 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/ports.py
--rw-r--r--   0        0        0    40899 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/process.py
--rw-r--r--   0        0        0     4547 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/process_spec.py
--rw-r--r--   0        0        0     1187 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/workchains/__init__.py
--rw-r--r--   0        0        0     2470 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/workchains/awaitable.py
--rw-r--r--   0        0        0     1968 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/workchains/context.py
--rw-r--r--   0        0        0    21825 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/workchains/restart.py
--rw-r--r--   0        0        0     7604 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/workchains/utils.py
--rw-r--r--   0        0        0    17279 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/processes/workchains/workchain.py
--rw-r--r--   0        0        0    14996 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/runners.py
--rw-r--r--   0        0        0     6129 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/transports.py
--rw-r--r--   0        0        0    12231 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/engine/utils.py
--rw-r--r--   0        0        0     1845 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/__init__.py
--rw-r--r--   0        0        0    11086 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/caching.py
--rw-r--r--   0        0        0    11486 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/configuration/__init__.py
--rw-r--r--   0        0        0    20965 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/configuration/config.py
--rw-r--r--   0        0        0     1075 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/configuration/migrations/__init__.py
--rw-r--r--   0        0        0    20944 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/configuration/migrations/migrations.py
--rw-r--r--   0        0        0     4732 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/configuration/options.py
--rw-r--r--   0        0        0    10267 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/configuration/profile.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/configuration/schema/__init__.py
--rw-r--r--   0        0        0    15472 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/configuration/schema/config-v5.schema.json
--rw-r--r--   0        0        0    12291 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/configuration/schema/config-v6.schema.json
--rw-r--r--   0        0        0    12289 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/configuration/schema/config-v7.schema.json
--rw-r--r--   0        0        0    12749 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/configuration/schema/config-v8.schema.json
--rw-r--r--   0        0        0    12997 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/configuration/schema/config-v9.schema.json
--rw-r--r--   0        0        0     5305 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/configuration/settings.py
--rw-r--r--   0        0        0     1148 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/external/__init__.py
--rw-r--r--   0        0        0     8809 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/external/postgres.py
--rw-r--r--   0        0        0     1104 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/external/rmq/__init__.py
--rw-r--r--   0        0        0     3868 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/external/rmq/client.py
--rw-r--r--   0        0        0      432 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/external/rmq/defaults.py
--rw-r--r--   0        0        0     7433 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/external/rmq/launcher.py
--rw-r--r--   0        0        0     2743 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/external/rmq/utils.py
--rw-r--r--   0        0        0    20986 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/manager.py
--rw-r--r--   0        0        0    10232 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/profile_access.py
--rw-r--r--   0        0        0      993 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/tests/__init__.py
--rw-r--r--   0        0        0    19379 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/tests/main.py
--rw-r--r--   0        0        0    34029 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/manage/tests/pytest_fixtures.py
--rw-r--r--   0        0        0     2738 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/orm/__init__.py
--rw-r--r--   0        0        0     5386 2023-02-10 13:09:40.030781 aiida-core-2.2.2/aiida/orm/authinfos.py
--rw-r--r--   0        0        0    12110 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/autogroup.py
--rw-r--r--   0        0        0     4441 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/comments.py
--rw-r--r--   0        0        0    26480 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/computers.py
--rw-r--r--   0        0        0     4658 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/convert.py
--rw-r--r--   0        0        0    10299 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/entities.py
--rw-r--r--   0        0        0     7190 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/extras.py
--rw-r--r--   0        0        0    13710 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/groups.py
--rw-r--r--   0        0        0     1628 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/implementation/__init__.py
--rw-r--r--   0        0        0     3059 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/implementation/authinfos.py
--rw-r--r--   0        0        0     3806 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/implementation/comments.py
--rw-r--r--   0        0        0     3550 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/implementation/computers.py
--rw-r--r--   0        0        0     7922 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/implementation/entities.py
--rw-r--r--   0        0        0     5840 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/implementation/groups.py
--rw-r--r--   0        0        0     3025 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/implementation/logs.py
--rw-r--r--   0        0        0    11547 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/implementation/nodes.py
--rw-r--r--   0        0        0     6576 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/implementation/querybuilder.py
--rw-r--r--   0        0        0    14652 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/implementation/storage_backend.py
--rw-r--r--   0        0        0     2459 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/implementation/users.py
--rw-r--r--   0        0        0     5746 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/implementation/utils.py
--rw-r--r--   0        0        0     7505 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/logs.py
--rw-r--r--   0        0        0     1786 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/__init__.py
--rw-r--r--   0        0        0     8303 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/attributes.py
--rw-r--r--   0        0        0     7099 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/caching.py
--rw-r--r--   0        0        0     2497 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/comments.py
--rw-r--r--   0        0        0     1885 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/__init__.py
--rw-r--r--   0        0        0     1069 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/array/__init__.py
--rw-r--r--   0        0        0     9322 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/array/array.py
--rw-r--r--   0        0        0    73820 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/array/bands.py
--rw-r--r--   0        0        0    20634 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/array/kpoints.py
--rw-r--r--   0        0        0    13142 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/array/projection.py
--rw-r--r--   0        0        0    38839 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/array/trajectory.py
--rw-r--r--   0        0        0     6269 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/array/xy.py
--rw-r--r--   0        0        0     2038 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/base.py
--rw-r--r--   0        0        0     1828 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/bool.py
--rw-r--r--   0        0        0    30429 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/cif.py
--rw-r--r--   0        0        0      401 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/code/__init__.py
--rw-r--r--   0        0        0    14550 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/code/abstract.py
--rw-r--r--   0        0        0     4953 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/code/containerized.py
--rw-r--r--   0        0        0     8194 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/code/installed.py
--rw-r--r--   0        0        0    23043 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/code/legacy.py
--rw-r--r--   0        0        0     8095 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/code/portable.py
--rw-r--r--   0        0        0    14609 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/data.py
--rw-r--r--   0        0        0     5667 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/dict.py
--rw-r--r--   0        0        0     4588 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/enum.py
--rw-r--r--   0        0        0      967 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/float.py
--rw-r--r--   0        0        0     1690 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/folder.py
--rw-r--r--   0        0        0      969 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/int.py
--rw-r--r--   0        0        0     7427 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/jsonable.py
--rw-r--r--   0        0        0     4948 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/list.py
--rw-r--r--   0        0        0     3207 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/numeric.py
--rw-r--r--   0        0        0     4784 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/orbital.py
--rw-r--r--   0        0        0      338 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/remote/__init__.py
--rw-r--r--   0        0        0     8173 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/remote/base.py
--rw-r--r--   0        0        0      326 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/remote/stash/__init__.py
--rw-r--r--   0        0        0     2371 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/remote/stash/base.py
--rw-r--r--   0        0        0     2250 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/remote/stash/folder.py
--rw-r--r--   0        0        0     4935 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/singlefile.py
--rw-r--r--   0        0        0      910 2023-02-10 13:09:40.034781 aiida-core-2.2.2/aiida/orm/nodes/data/str.py
--rw-r--r--   0        0        0    92833 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/nodes/data/structure.py
--rw-r--r--   0        0        0    19092 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/nodes/data/upf.py
--rw-r--r--   0        0        0    11454 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/nodes/links.py
--rw-r--r--   0        0        0    27896 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/nodes/node.py
--rw-r--r--   0        0        0     1009 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/nodes/process/__init__.py
--rw-r--r--   0        0        0      941 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/nodes/process/calculation/__init__.py
--rw-r--r--   0        0        0     2605 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/nodes/process/calculation/calcfunction.py
--rw-r--r--   0        0        0    22161 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/nodes/process/calculation/calcjob.py
--rw-r--r--   0        0        0     2115 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/nodes/process/calculation/calculation.py
--rw-r--r--   0        0        0    19708 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/nodes/process/process.py
--rw-r--r--   0        0        0      936 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/nodes/process/workflow/__init__.py
--rw-r--r--   0        0        0     1775 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/nodes/process/workflow/workchain.py
--rw-r--r--   0        0        0     3631 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/nodes/process/workflow/workflow.py
--rw-r--r--   0        0        0     2442 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/nodes/process/workflow/workfunction.py
--rw-r--r--   0        0        0    15675 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/nodes/repository.py
--rw-r--r--   0        0        0    61503 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/querybuilder.py
--rw-r--r--   0        0        0     4785 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/users.py
--rw-r--r--   0        0        0     1415 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/utils/__init__.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/utils/builders/__init__.py
--rw-r--r--   0        0        0     8496 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/utils/builders/code.py
--rw-r--r--   0        0        0     8108 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/utils/builders/computer.py
--rw-r--r--   0        0        0     4952 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/utils/calcjob.py
--rw-r--r--   0        0        0    17089 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/utils/links.py
--rw-r--r--   0        0        0    36736 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/utils/loaders.py
--rw-r--r--   0        0        0     2808 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/utils/log.py
--rw-r--r--   0        0        0    10970 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/utils/managers.py
--rw-r--r--   0        0        0     9786 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/utils/mixins.py
--rw-r--r--   0        0        0     7008 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/utils/node.py
--rw-r--r--   0        0        0     4573 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/utils/remote.py
--rw-r--r--   0        0        0     9165 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/orm/utils/serialize.py
--rw-r--r--   0        0        0      847 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/parsers/__init__.py
--rw-r--r--   0        0        0     8094 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/parsers/parser.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/parsers/plugins/__init__.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/parsers/plugins/arithmetic/__init__.py
--rw-r--r--   0        0        0     2226 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/parsers/plugins/arithmetic/add.py
--rw-r--r--   0        0        0     1984 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/parsers/plugins/diff_tutorial/parsers.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/parsers/plugins/templatereplacer/__init__.py
--rw-r--r--   0        0        0     3244 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/parsers/plugins/templatereplacer/parser.py
--rw-r--r--   0        0        0     1329 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/plugins/__init__.py
--rw-r--r--   0        0        0    17402 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/plugins/entry_point.py
--rw-r--r--   0        0        0    16492 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/plugins/factories.py
--rw-r--r--   0        0        0     4405 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/plugins/utils.py
--rw-r--r--   0        0        0       26 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/py.typed
--rw-r--r--   0        0        0     1017 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/repository/__init__.py
--rw-r--r--   0        0        0      368 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/repository/backend/__init__.py
--rw-r--r--   0        0        0     9748 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/repository/backend/abstract.py
--rw-r--r--   0        0        0     9651 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/repository/backend/disk_object_store.py
--rw-r--r--   0        0        0     4392 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/repository/backend/sandbox.py
--rw-r--r--   0        0        0     5382 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/repository/common.py
--rw-r--r--   0        0        0    24331 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/repository/repository.py
--rw-r--r--   0        0        0      823 2023-02-10 13:09:40.038781 aiida-core-2.2.2/aiida/restapi/__init__.py
--rw-r--r--   0        0        0     7379 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/api.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/common/__init__.py
--rw-r--r--   0        0        0     1701 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/common/config.py
--rw-r--r--   0        0        0     1589 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/common/exceptions.py
--rw-r--r--   0        0        0    19386 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/common/identifiers.py
--rw-r--r--   0        0        0    34328 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/common/utils.py
--rw-r--r--   0        0        0    28984 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/resources.py
--rwxr-xr-x   0        0        0     4911 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/run_api.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/__init__.py
--rw-r--r--   0        0        0    18895 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/base.py
--rw-r--r--   0        0        0     4211 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/computer.py
--rw-r--r--   0        0        0     3321 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/group.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/__init__.py
--rw-r--r--   0        0        0     2835 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/data/__init__.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/data/array/__init__.py
--rw-r--r--   0        0        0     2051 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/data/array/bands.py
--rw-r--r--   0        0        0     1478 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/data/cif.py
--rw-r--r--   0        0        0     1464 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/data/code.py
--rw-r--r--   0        0        0     5420 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/data/kpoints.py
--rw-r--r--   0        0        0     1579 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/data/structure.py
--rw-r--r--   0        0        0     1388 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/data/upf.py
--rw-r--r--   0        0        0    31726 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/node.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/process/__init__.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/process/calculation/__init__.py
--rw-r--r--   0        0        0     1579 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/process/calculation/calcfunction.py
--rw-r--r--   0        0        0     2619 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/process/calculation/calcjob.py
--rw-r--r--   0        0        0     4530 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/process/process.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/process/workflow/__init__.py
--rw-r--r--   0        0        0     1545 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/process/workflow/workchain.py
--rw-r--r--   0        0        0     1576 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/nodes/process/workflow/workfunction.py
--rw-r--r--   0        0        0     2765 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/restapi/translator/user.py
--rw-r--r--   0        0        0     1074 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/schedulers/__init__.py
--rw-r--r--   0        0        0    25077 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/schedulers/datastructures.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/schedulers/plugins/__init__.py
--rw-r--r--   0        0        0    15626 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/schedulers/plugins/direct.py
--rw-r--r--   0        0        0    33430 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/schedulers/plugins/lsf.py
--rw-r--r--   0        0        0    31222 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/schedulers/plugins/pbsbaseclasses.py
--rw-r--r--   0        0        0     3699 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/schedulers/plugins/pbspro.py
--rw-r--r--   0        0        0    20539 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/schedulers/plugins/sge.py
--rw-r--r--   0        0        0    35020 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/schedulers/plugins/slurm.py
--rw-r--r--   0        0        0     3799 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/schedulers/plugins/torque.py
--rw-r--r--   0        0        0    17852 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/schedulers/scheduler.py
--rw-r--r--   0        0        0     1108 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/sphinxext/__init__.py
--rw-r--r--   0        0        0     1450 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/sphinxext/calcjob.py
--rw-r--r--   0        0        0     8844 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/sphinxext/process.py
--rw-r--r--   0        0        0     1475 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/sphinxext/workchain.py
--rw-r--r--   0        0        0      810 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/__init__.py
--rw-r--r--   0        0        0      815 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/log.py
--rw-r--r--   0        0        0      877 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/__init__.py
--rwxr-xr-x   0        0        0     3996 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/alembic_cli.py
--rw-r--r--   0        0        0    18190 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/backend.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/__init__.py
--rw-r--r--   0        0        0     2198 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/env.py
--rw-r--r--   0        0        0      494 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/script.py.mako
--rw-r--r--   0        0        0      748 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/__init__.py
--rw-r--r--   0        0        0     2260 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/calc_state.py
--rw-r--r--   0        0        0     3916 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/create_dbattribute.py
--rw-r--r--   0        0        0     8837 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/dblog_update.py
--rw-r--r--   0        0        0     1563 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/duplicate_uuids.py
--rw-r--r--   0        0        0    12177 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/integrity.py
--rw-r--r--   0        0        0     3477 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/legacy_workflows.py
--rw-r--r--   0        0        0     5991 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/migrate_repository.py
--rw-r--r--   0        0        0     9306 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/parity.py
--rw-r--r--   0        0        0     7520 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/provenance_redesign.py
--rw-r--r--   0        0        0     5534 2023-02-10 13:09:40.042781 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/reflect.py
--rw-r--r--   0        0        0    18164 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/utils.py
--rw-r--r--   0        0        0     2902 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/041a79fc615f_dblog_cleaning.py
--rw-r--r--   0        0        0     1486 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/07fac78e6209_drop_computer_transport_params.py
--rw-r--r--   0        0        0     2482 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/0aebbeab274d_base_data_plugin_type_string.py
--rw-r--r--   0        0        0     1819 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/0edcdd5a30f0_dbgroup_extras.py
--rw-r--r--   0        0        0     1829 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/118349c10896_default_link_label.py
--rw-r--r--   0        0        0     2727 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/12536798d4d3_trajectory_symbols_to_attribute.py
--rw-r--r--   0        0        0     2856 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/140c971ae0a3_migrate_builtin_calculations.py
--rw-r--r--   0        0        0     1168 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/162b99bca4a2_drop_dbcalcstate.py
--rw-r--r--   0        0        0     1361 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/1830c8430131_drop_node_columns_nodeversion_public.py
--rw-r--r--   0        0        0     1872 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/1b8ed3425af9_remove_legacy_workflows.py
--rw-r--r--   0        0        0     9697 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/1de112340b16_django_parity_1.py
--rw-r--r--   0        0        0    10079 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/1de112340b17_django_parity_2.py
--rw-r--r--   0        0        0     1252 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/1de112340b18_django_parity_3.py
--rw-r--r--   0        0        0     1382 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/1feaea71bd5a_migrate_repository.py
--rw-r--r--   0        0        0     5530 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/239cea6d2452_provenance_redesign.py
--rw-r--r--   0        0        0     8062 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/26d561acd560_data_migration_legacy_job_calculations.py
--rw-r--r--   0        0        0     5861 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/34a831f4286d_entry_point_core_prefix.py
--rw-r--r--   0        0        0     2044 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/35d4ee9a1b0e_code_hidden_attr_to_extra.py
--rw-r--r--   0        0        0     1309 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/375c2db70663_dblog_uuid_uniqueness_constraint.py
--rw-r--r--   0        0        0     1615 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/37f3d4882837_make_all_uuid_columns_unique.py
--rw-r--r--   0        0        0     1335 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/3d6190594e19_remove_dbcomputer_enabled.py
--rw-r--r--   0        0        0      802 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/535039300e4a_computer_name_to_label.py
--rw-r--r--   0        0        0     1892 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/59edaf8a8b79_adding_indexes_and_constraints_to_the_.py
--rw-r--r--   0        0        0     1689 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/5a49629f0d45_dblink_indices.py
--rw-r--r--   0        0        0     1742 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/5d4d844852b6_invalidating_node_hash.py
--rw-r--r--   0        0        0     1762 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/5ddd24e52864_dbnode_type_to_dbnode_node_type.py
--rw-r--r--   0        0        0     1866 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/61fc0913fae9_remove_node_prefix.py
--rw-r--r--   0        0        0     1391 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/62fe0d36de90_add_node_uuid_unique_constraint.py
--rw-r--r--   0        0        0     1621 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/6a5c2ea1439d_move_data_within_node_module.py
--rw-r--r--   0        0        0     1376 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/6c629c886f84_process_type.py
--rw-r--r--   0        0        0     1351 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/70c7d732f1b2_delete_dbpath.py
--rw-r--r--   0        0        0     1466 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/7536a82b2cc4_add_node_repository_metadata.py
--rw-r--r--   0        0        0     1360 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/7a6587e16f4c_unique_constraints_for_the_db_dbgroup_.py
--rw-r--r--   0        0        0     2610 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/7b38a9e783e7_seal_unsealed_processes.py
--rw-r--r--   0        0        0     3849 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/7ca08c391c49_calc_job_option_attribute_keys.py
--rw-r--r--   0        0        0     1311 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/89176227b25_add_indexes_to_dbworkflowdata_table.py
--rw-r--r--   0        0        0     2309 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/91b573400be5_prepare_schema_reset.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/__init__.py
--rw-r--r--   0        0        0     1158 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/a514d673c163_drop_dblock.py
--rw-r--r--   0        0        0     1656 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/a603da2cc809_code_sub_class_of_data.py
--rw-r--r--   0        0        0     6613 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/a6048f0ffca8_update_linktypes.py
--rw-r--r--   0        0        0     1840 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/b8b23ddefad4_dbgroup_name_to_label_type_to_type_string.py
--rw-r--r--   0        0        0     1778 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/bf591f31dd12_dbgroup_type_string.py
--rw-r--r--   0        0        0     2269 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/ce56d84bcc35_delete_trajectory_symbols_array.py
--rw-r--r--   0        0        0     1599 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/d254fdfed416_rename_parameter_data_to_dict.py
--rw-r--r--   0        0        0     1564 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/de2eaf6978b4_simplify_user_model.py
--rw-r--r--   0        0        0    30892 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0001_initial.py
--rw-r--r--   0        0        0     1505 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0002_db_state_change.py
--rw-r--r--   0        0        0     1809 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0003_add_link_type.py
--rw-r--r--   0        0        0     1547 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0004_add_daemon_and_uuid_indices.py
--rw-r--r--   0        0        0     1246 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0005_add_cmtime_indices.py
--rw-r--r--   0        0        0     1295 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0006_delete_dbpath.py
--rw-r--r--   0        0        0     6316 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0007_update_linktypes.py
--rw-r--r--   0        0        0     2359 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0008_code_hidden_to_extra.py
--rw-r--r--   0        0        0     2275 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0009_base_data_plugin_type_string.py
--rw-r--r--   0        0        0     1474 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0010_process_type.py
--rw-r--r--   0        0        0     1712 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0011_delete_kombu_tables.py
--rw-r--r--   0        0        0     1073 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0012_drop_dblock.py
--rw-r--r--   0        0        0     1747 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0013_django_1_8.py
--rw-r--r--   0        0        0     1374 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0014_add_node_uuid_unique_constraint.py
--rw-r--r--   0        0        0     1192 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0015_invalidating_node_hash.py
--rw-r--r--   0        0        0     1171 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0016_code_sub_class_of_data.py
--rw-r--r--   0        0        0     1083 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0017_drop_dbcalcstate.py
--rw-r--r--   0        0        0     2391 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0018_django_1_11.py
--rw-r--r--   0        0        0     2558 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0019_migrate_builtin_calculations.py
--rw-r--r--   0        0        0     6233 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0020_provenance_redesign.py
--rw-r--r--   0        0        0     2439 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0021_dbgroup_name_to_label_type_to_type_string.py
--rw-r--r--   0        0        0     1539 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0022_dbgroup_type_string_change_content.py
--rw-r--r--   0        0        0     3316 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0023_calc_job_option_attribute_keys.py
--rw-r--r--   0        0        0     3663 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0024a_dblog_update.py
--rw-r--r--   0        0        0     1248 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0024b_dblog_update.py
--rw-r--r--   0        0        0     1480 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0025_move_data_within_node_module.py
--rw-r--r--   0        0        0     2250 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0026_trajectory_symbols_to_attribute.py
--rw-r--r--   0        0        0     2415 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0027_delete_trajectory_symbols_array.py
--rw-r--r--   0        0        0     1598 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0028_remove_node_prefix.py
--rw-r--r--   0        0        0     1383 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0029_rename_parameter_data_to_dict.py
--rw-r--r--   0        0        0     1267 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0030_dbnode_type_to_dbnode_node_type.py
--rw-r--r--   0        0        0     1140 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0031_remove_dbcomputer_enabled.py
--rw-r--r--   0        0        0     1552 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0032_remove_legacy_workflows.py
--rw-r--r--   0        0        0     1516 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0033_replace_text_field_with_json_field.py
--rw-r--r--   0        0        0     1203 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0034_drop_node_columns_nodeversion_public.py
--rw-r--r--   0        0        0     1550 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0035_simplify_user_model.py
--rw-r--r--   0        0        0     1156 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0036_drop_computer_transport_params.py
--rw-r--r--   0        0        0     7292 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0037_attributes_extras_settings_json.py
--rw-r--r--   0        0        0     7899 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0038_data_migration_legacy_job_calculations.py
--rw-r--r--   0        0        0     1220 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0039_reset_hash.py
--rw-r--r--   0        0        0     3186 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0040_data_migration_legacy_process_attributes.py
--rw-r--r--   0        0        0     2403 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0041_seal_unsealed_processes.py
--rw-r--r--   0        0        0     2115 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0042_prepare_schema_reset.py
--rw-r--r--   0        0        0     1612 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0043_default_link_label.py
--rw-r--r--   0        0        0     1615 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0044_dbgroup_type_string.py
--rw-r--r--   0        0        0     1673 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0045_dbgroup_extras.py
--rw-r--r--   0        0        0     1378 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0046_add_node_repository_metadata.py
--rw-r--r--   0        0        0     1297 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0047_migrate_repository.py
--rw-r--r--   0        0        0     1728 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0048_computer_name_to_label.py
--rw-r--r--   0        0        0     5770 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0049_entry_point_core_prefix.py
--rw-r--r--   0        0        0     1974 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0050_sqlalchemy_parity.py
--rw-r--r--   0        0        0    21476 2023-02-10 13:09:40.046782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/e15ef2630a1b_initial_schema.py
--rw-r--r--   0        0        0     2135 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/e72ad251bcdb_dbgroup_class_change_type_string_values.py
--rw-r--r--   0        0        0     3393 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/e734dd5e50d7_data_migration_legacy_process_attributes.py
--rw-r--r--   0        0        0     1303 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/e797afa09270_reset_hash.py
--rw-r--r--   0        0        0     1760 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/ea2f50e7f615_dblog_create_uuid_column.py
--rw-r--r--   0        0        0     2221 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/f9a69de76a9a_delete_kombu_tables.py
--rw-r--r--   0        0        0    11820 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/main_0001_initial.py
--rw-r--r--   0        0        0    21817 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/migrator.py
--rw-r--r--   0        0        0      703 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/models/__init__.py
--rw-r--r--   0        0        0     2660 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/models/authinfo.py
--rw-r--r--   0        0        0     4494 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/models/base.py
--rw-r--r--   0        0        0     2322 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/models/comment.py
--rw-r--r--   0        0        0     2904 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/models/computer.py
--rw-r--r--   0        0        0     3635 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/models/group.py
--rw-r--r--   0        0        0     2677 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/models/log.py
--rw-r--r--   0        0        0     8274 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/models/node.py
--rw-r--r--   0        0        0     1749 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/models/settings.py
--rw-r--r--   0        0        0     1739 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/models/user.py
--rw-r--r--   0        0        0      678 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/orm/__init__.py
--rw-r--r--   0        0        0     4752 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/orm/authinfos.py
--rw-r--r--   0        0        0     6320 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/orm/comments.py
--rw-r--r--   0        0        0     4282 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/orm/computers.py
--rw-r--r--   0        0        0     3537 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/orm/convert.py
--rw-r--r--   0        0        0     3451 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/orm/entities.py
--rw-r--r--   0        0        0     3251 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/orm/extras_mixin.py
--rw-r--r--   0        0        0    10474 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/orm/groups.py
--rw-r--r--   0        0        0     5113 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/orm/logs.py
--rw-r--r--   0        0        0    10981 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/orm/nodes.py
--rw-r--r--   0        0        0      746 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/orm/querybuilder/__init__.py
--rw-r--r--   0        0        0    23343 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/orm/querybuilder/joiner.py
--rw-r--r--   0        0        0    45822 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/orm/querybuilder/main.py
--rw-r--r--   0        0        0     2324 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/orm/users.py
--rw-r--r--   0        0        0     7345 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/orm/utils.py
--rw-r--r--   0        0        0     8962 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/psql_dos/utils.py
--rw-r--r--   0        0        0     1022 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_temp/__init__.py
--rw-r--r--   0        0        0     7561 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_temp/backend.py
--rw-r--r--   0        0        0     1664 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/__init__.py
--rw-r--r--   0        0        0    15085 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/backend.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/__init__.py
--rw-r--r--   0        0        0     1999 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/env.py
--rw-r--r--   0        0        0     1754 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/__init__.py
--rw-r--r--   0        0        0     3332 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v04_to_v05.py
--rw-r--r--   0        0        0     7335 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v05_to_v06.py
--rw-r--r--   0        0        0     5971 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v06_to_v07.py
--rw-r--r--   0        0        0     2107 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v07_to_v08.py
--rw-r--r--   0        0        0     2361 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v08_to_v09.py
--rw-r--r--   0        0        0     1355 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v09_to_v10.py
--rw-r--r--   0        0        0     1480 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v10_to_v11.py
--rw-r--r--   0        0        0     5486 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v11_to_v12.py
--rw-r--r--   0        0        0     1698 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v12_to_v13.py
--rw-r--r--   0        0        0    12668 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy_to_main.py
--rw-r--r--   0        0        0      572 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/script.py.mako
--rw-r--r--   0        0        0     8212 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/utils.py
--rw-r--r--   0        0        0     8703 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/v1_db_schema.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/versions/__init__.py
--rw-r--r--   0        0        0     8710 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/versions/main_0000_initial.py
--rw-r--r--   0        0        0     6790 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/versions/main_0000a_replace_nulls.py
--rw-r--r--   0        0        0     4413 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/versions/main_0000b_non_nullable.py
--rw-r--r--   0        0        0     1044 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/versions/main_0001.py
--rw-r--r--   0        0        0    17760 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/migrator.py
--rw-r--r--   0        0        0     7070 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/models.py
--rw-r--r--   0        0        0    15167 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/orm.py
--rw-r--r--   0        0        0     4882 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/storage/sqlite_zip/utils.py
--rw-r--r--   0        0        0     1845 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/tools/__init__.py
--rw-r--r--   0        0        0     1366 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/tools/archive/__init__.py
--rw-r--r--   0        0        0     9493 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/tools/archive/abstract.py
--rw-r--r--   0        0        0     3349 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/tools/archive/common.py
--rw-r--r--   0        0        0    29933 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/tools/archive/create.py
--rw-r--r--   0        0        0     2018 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/tools/archive/exceptions.py
--rw-r--r--   0        0        0      844 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/tools/archive/implementations/__init__.py
--rw-r--r--   0        0        0      836 2023-02-10 13:09:40.050782 aiida-core-2.2.2/aiida/tools/archive/implementations/sqlite_zip/__init__.py
--rw-r--r--   0        0        0     3280 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/archive/implementations/sqlite_zip/main.py
--rw-r--r--   0        0        0     2268 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/archive/implementations/sqlite_zip/reader.py
--rw-r--r--   0        0        0    12744 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/archive/implementations/sqlite_zip/writer.py
--rw-r--r--   0        0        0    50475 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/archive/imports.py
--rw-r--r--   0        0        0      833 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/calculations/__init__.py
--rw-r--r--   0        0        0     1053 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/calculations/base.py
--rw-r--r--   0        0        0      997 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/data/__init__.py
--rw-r--r--   0        0        0      862 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/data/array/__init__.py
--rw-r--r--   0        0        0      952 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/data/array/kpoints/__init__.py
--rw-r--r--   0        0        0    77224 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/data/array/kpoints/legacy.py
--rw-r--r--   0        0        0    10772 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/data/array/kpoints/main.py
--rw-r--r--   0        0        0     7034 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/data/array/kpoints/seekpath.py
--rw-r--r--   0        0        0     1377 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/data/array/trajectory.py
--rw-r--r--   0        0        0     8683 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/data/cif.py
--rw-r--r--   0        0        0      899 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/data/orbital/__init__.py
--rw-r--r--   0        0        0     6521 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/data/orbital/orbital.py
--rw-r--r--   0        0        0    13938 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/data/orbital/realhydrogen.py
--rw-r--r--   0        0        0    11892 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/data/structure.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/dbexporters/__init__.py
--rw-r--r--   0        0        0      783 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/dbimporters/__init__.py
--rw-r--r--   0        0        0    12063 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/dbimporters/baseclasses.py
--rw-r--r--   0        0        0      720 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/dbimporters/plugins/__init__.py
--rw-r--r--   0        0        0    12105 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/dbimporters/plugins/cod.py
--rw-r--r--   0        0        0    27176 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/dbimporters/plugins/icsd.py
--rw-r--r--   0        0        0     6920 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/dbimporters/plugins/materialsproject.py
--rw-r--r--   0        0        0    11604 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/dbimporters/plugins/mpds.py
--rw-r--r--   0        0        0     5697 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/dbimporters/plugins/mpod.py
--rw-r--r--   0        0        0     5399 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/dbimporters/plugins/nninc.py
--rw-r--r--   0        0        0     4692 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/dbimporters/plugins/oqmd.py
--rw-r--r--   0        0        0     4463 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/dbimporters/plugins/pcod.py
--rw-r--r--   0        0        0     2691 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/dbimporters/plugins/tcod.py
--rw-r--r--   0        0        0      883 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/graph/__init__.py
--rw-r--r--   0        0        0    17095 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/graph/age_entities.py
--rw-r--r--   0        0        0    18095 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/graph/age_rules.py
--rw-r--r--   0        0        0     7116 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/graph/deletions.py
--rw-r--r--   0        0        0    12733 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/graph/graph_traversers.py
--rw-r--r--   0        0        0     1382 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/groups/__init__.py
--rw-r--r--   0        0        0    12617 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/groups/paths.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/ipython/__init__.py
--rw-r--r--   0        0        0     1212 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/ipython/aiida_magic_register.py
--rw-r--r--   0        0        0     5344 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/ipython/ipython_magics.py
--rw-r--r--   0        0        0        0 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/query/__init__.py
--rw-r--r--   0        0        0     6810 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/query/calculation.py
--rw-r--r--   0        0        0     2963 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/query/formatting.py
--rw-r--r--   0        0        0     6958 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/query/mapping.py
--rw-r--r--   0        0        0      941 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/visualization/__init__.py
--rw-r--r--   0        0        0    37650 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/tools/visualization/graph.py
--rw-r--r--   0        0        0      943 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/transports/__init__.py
--rw-r--r--   0        0        0     6400 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/transports/cli.py
--rw-r--r--   0        0        0      851 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/transports/plugins/__init__.py
--rw-r--r--   0        0        0    37052 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/transports/plugins/local.py
--rw-r--r--   0        0        0    62936 2023-02-10 13:09:40.054782 aiida-core-2.2.2/aiida/transports/plugins/ssh.py
--rw-r--r--   0        0        0    30993 2023-02-10 13:09:40.058782 aiida-core-2.2.2/aiida/transports/transport.py
--rw-r--r--   0        0        0     3273 2023-02-10 13:09:40.058782 aiida-core-2.2.2/aiida/transports/util.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.058782 aiida-core-2.2.2/aiida/workflows/__init__.py
--rw-r--r--   0        0        0      632 2023-02-10 13:09:40.058782 aiida-core-2.2.2/aiida/workflows/arithmetic/__init__.py
--rw-r--r--   0        0        0     1057 2023-02-10 13:09:40.058782 aiida-core-2.2.2/aiida/workflows/arithmetic/add_multiply.py
--rw-r--r--   0        0        0     2538 2023-02-10 13:09:40.058782 aiida-core-2.2.2/aiida/workflows/arithmetic/multiply_add.py
--rw-r--r--   0        0        0      327 2023-02-10 13:09:40.058782 aiida-core-2.2.2/codecov.yml
--rw-r--r--   0        0        0      695 2023-02-10 13:09:40.106785 aiida-core-2.2.2/environment.yml
--rw-r--r--   0        0        0    13919 2023-02-10 13:09:40.106785 aiida-core-2.2.2/open_source_licenses.txt
--rw-r--r--   0        0        0    15686 2023-02-10 13:09:40.106785 aiida-core-2.2.2/pyproject.toml
--rw-r--r--   0        0        0      510 2023-02-10 13:09:40.106785 aiida-core-2.2.2/requirements/README.md
--rw-r--r--   0        0        0     3159 2023-02-10 13:09:40.106785 aiida-core-2.2.2/requirements/requirements-py-3.10.txt
--rw-r--r--   0        0        0     3609 2023-02-10 13:09:40.106785 aiida-core-2.2.2/requirements/requirements-py-3.11.txt
--rw-r--r--   0        0        0     3210 2023-02-10 13:09:40.106785 aiida-core-2.2.2/requirements/requirements-py-3.8.txt
--rw-r--r--   0        0        0     3183 2023-02-10 13:09:40.106785 aiida-core-2.2.2/requirements/requirements-py-3.9.txt
--rw-r--r--   0        0        0      473 2023-02-10 13:09:40.158788 aiida-core-2.2.2/utils/.gource.conf
--rw-r--r--   0        0        0      697 2023-02-10 13:09:40.158788 aiida-core-2.2.2/utils/__init__.py
--rwxr-xr-x   0        0        0    16784 2023-02-10 13:09:40.158788 aiida-core-2.2.2/utils/dependency_management.py
--rw-r--r--   0        0        0     6562 2023-02-10 13:09:40.158788 aiida-core-2.2.2/utils/make_all.py
--rw-r--r--   0        0        0       73 2023-02-10 13:09:40.158788 aiida-core-2.2.2/utils/requirements.txt
--rw-r--r--   0        0        0     5871 2023-02-10 13:09:40.158788 aiida-core-2.2.2/utils/validate_consistency.py
--rw-r--r--   0        0        0    10955 1970-01-01 00:00:00.000000 aiida-core-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0      539 2023-04-17 09:37:52.841524 aiida-core-2.3.0/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0      347 2023-04-17 09:37:52.841524 aiida-core-2.3.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1056 2023-04-17 09:37:52.841524 aiida-core-2.3.0/.devcontainer/docker-compose.yml
+-rw-r--r--   0        0        0       56 2023-04-17 09:37:52.841524 aiida-core-2.3.0/.devcontainer/post_create.sh
+-rw-r--r--   0        0        0      759 2023-04-17 09:37:52.841524 aiida-core-2.3.0/.docker/docker-rabbitmq.yml
+-rwxr-xr-x   0        0        0       66 2023-04-17 09:37:52.841524 aiida-core-2.3.0/.docker/my_init.d/configure-aiida.sh
+-rwxr-xr-x   0        0        0     3773 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.docker/opt/configure-aiida.sh
+-rw-r--r--   0        0        0      155 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.dockerignore
+-rw-r--r--   0        0        0      649 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      972 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      275 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      434 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/ISSUE_TEMPLATE/doc-improvements.md
+-rw-r--r--   0        0        0      754 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      181 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/config/README.md
+-rw-r--r--   0        0        0      307 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/config/add-singularity.yaml
+-rw-r--r--   0        0        0      163 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/config/add.yaml
+-rwxr-xr-x   0        0        0      347 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/config/doubler.sh
+-rw-r--r--   0        0        0      199 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/config/doubler.yaml
+-rw-r--r--   0        0        0       43 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/config/localhost-config.yaml
+-rw-r--r--   0        0        0      274 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/config/localhost.yaml
+-rw-r--r--   0        0        0      453 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/config/profile.yaml
+-rw-r--r--   0        0        0      130 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/config/slurm-ssh-config.yaml
+-rw-r--r--   0        0        0      275 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/config/slurm-ssh.yaml
+-rw-r--r--   0        0        0     1679 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/config/slurm_rsa
+-rw-r--r--   0        0        0      202 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/system_tests/README.md
+-rw-r--r--   0        0        0     3176 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/system_tests/pytest/test_memory_leaks.py
+-rw-r--r--   0        0        0     1387 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/system_tests/test_containerized_code.py
+-rw-r--r--   0        0        0    24024 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/system_tests/test_daemon.py
+-rw-r--r--   0        0        0     1126 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/system_tests/test_ipython_magics.py
+-rwxr-xr-x   0        0        0      911 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/system_tests/test_polish_workchains.sh
+-rw-r--r--   0        0        0     3912 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/system_tests/test_profile_manager.py
+-rw-r--r--   0        0        0     1972 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/system_tests/test_test_manager.py
+-rwxr-xr-x   0        0        0     1611 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/system_tests/test_verdi_load_time.sh
+-rw-r--r--   0        0        0     8572 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/system_tests/workchains.py
+-rw-r--r--   0        0        0     1901 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/benchmark-config.json
+-rw-r--r--   0        0        0     2226 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/benchmark.yml
+-rw-r--r--   0        0        0     1719 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/build_and_test_docker_on_pr.yml
+-rw-r--r--   0        0        0     1327 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/check_release_tag.py
+-rw-r--r--   0        0        0     3561 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/ci-code.yml
+-rw-r--r--   0        0        0      888 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/ci-style.yml
+-rw-r--r--   0        0        0     1086 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/docs-build.yml
+-rw-r--r--   0        0        0     3477 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/nightly.yml
+-rw-r--r--   0        0        0     1803 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/post-release.yml
+-rw-r--r--   0        0        0     1377 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/push_image_to_dockerhub.yml
+-rw-r--r--   0        0        0     1696 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/rabbitmq.yml
+-rw-r--r--   0        0        0     3095 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/release.yml
+-rwxr-xr-x   0        0        0     1814 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/setup.sh
+-rw-r--r--   0        0        0    11253 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/test-install.yml
+-rwxr-xr-x   0        0        0      898 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/tests.sh
+-rwxr-xr-x   0        0        0      589 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/tests_nightly.sh
+-rwxr-xr-x   0        0        0     2135 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.github/workflows/verdi.sh
+-rw-r--r--   0        0        0      427 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.gitignore
+-rw-r--r--   0        0        0     2005 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/README.md
+-rw-r--r--   0        0        0      413 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/default/Dockerfile
+-rw-r--r--   0        0        0     1790 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/default/config_local.yml
+-rw-r--r--   0        0        0     6342 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/default/create_docker.yml
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/default/files/polish/__init__.py
+-rwxr-xr-x   0        0        0     7706 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/default/files/polish/cli.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/default/files/polish/lib/__init__.py
+-rw-r--r--   0        0        0     5384 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/default/files/polish/lib/expression.py
+-rw-r--r--   0        0        0     1032 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/default/files/polish/lib/template/base.tpl
+-rw-r--r--   0        0        0     5300 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/default/files/polish/lib/template/workchain.tpl
+-rw-r--r--   0        0        0     8117 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/default/files/polish/lib/workchain.py
+-rw-r--r--   0        0        0       46 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/default/run_tests.yml
+-rw-r--r--   0        0        0     2717 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/default/setup_aiida.yml
+-rw-r--r--   0        0        0      716 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/default/setup_python.yml
+-rw-r--r--   0        0        0     1650 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/default/tasks/log_query_stats.yml
+-rw-r--r--   0        0        0      239 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/default/tasks/reset_query_stats.yml
+-rw-r--r--   0        0        0     2814 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.molecule/default/test_polish_workchains.yml
+-rw-r--r--   0        0        0     9312 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      802 2023-04-17 09:37:52.845521 aiida-core-2.3.0/.readthedocs.yml
+-rw-r--r--   0        0        0     1746 2023-04-17 09:37:52.845521 aiida-core-2.3.0/AUTHORS.txt
+-rw-r--r--   0        0        0   201774 2023-04-17 09:37:52.845521 aiida-core-2.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3352 2023-04-17 09:37:52.845521 aiida-core-2.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      585 2023-04-17 09:37:52.845521 aiida-core-2.3.0/Dockerfile
+-rw-r--r--   0        0        0     1312 2023-04-17 09:37:52.845521 aiida-core-2.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     6031 2023-04-17 09:37:52.845521 aiida-core-2.3.0/README.md
+-rw-r--r--   0        0        0     3610 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/__init__.py
+-rw-r--r--   0        0        0      807 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/__main__.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/calculations/__init__.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/calculations/arithmetic/__init__.py
+-rw-r--r--   0        0        0     3907 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/calculations/arithmetic/add.py
+-rw-r--r--   0        0        0     2547 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/calculations/diff_tutorial/calculations.py
+-rw-r--r--   0        0        0        0 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/calculations/importers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/calculations/importers/arithmetic/__init__.py
+-rw-r--r--   0        0        0     1644 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/calculations/importers/arithmetic/add.py
+-rw-r--r--   0        0        0        0 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/calculations/monitors/__init__.py
+-rw-r--r--   0        0        0     1161 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/calculations/monitors/base.py
+-rw-r--r--   0        0        0     9273 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/calculations/templatereplacer.py
+-rw-r--r--   0        0        0    10738 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/calculations/transfer.py
+-rw-r--r--   0        0        0     1734 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/__init__.py
+-rw-r--r--   0        0        0     1194 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/__init__.py
+-rw-r--r--   0        0        0    19446 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_archive.py
+-rw-r--r--   0        0        0    14555 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_calcjob.py
+-rw-r--r--   0        0        0    14735 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_code.py
+-rw-r--r--   0        0        0    26949 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_computer.py
+-rw-r--r--   0        0        0     7913 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_config.py
+-rw-r--r--   0        0        0    10683 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_daemon.py
+-rw-r--r--   0        0        0      931 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/__init__.py
+-rw-r--r--   0        0        0     1337 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_array.py
+-rw-r--r--   0        0        0     4808 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_bands.py
+-rw-r--r--   0        0        0     4392 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_cif.py
+-rw-r--r--   0        0        0     1219 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_dict.py
+-rw-r--r--   0        0        0     4692 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_export.py
+-rw-r--r--   0        0        0     2889 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_list.py
+-rw-r--r--   0        0        0     3599 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_remote.py
+-rw-r--r--   0        0        0     8026 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_show.py
+-rw-r--r--   0        0        0     1341 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_singlefile.py
+-rw-r--r--   0        0        0     8890 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_structure.py
+-rw-r--r--   0        0        0     3575 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_trajectory.py
+-rw-r--r--   0        0        0     5209 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_upf.py
+-rw-r--r--   0        0        0     4761 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_database.py
+-rw-r--r--   0        0        0     7557 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_devel.py
+-rw-r--r--   0        0        0    18115 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_group.py
+-rw-r--r--   0        0        0     1392 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_help.py
+-rw-r--r--   0        0        0    20026 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_node.py
+-rw-r--r--   0        0        0     2950 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_plugin.py
+-rw-r--r--   0        0        0    12108 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_process.py
+-rw-r--r--   0        0        0     5739 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_profile.py
+-rw-r--r--   0        0        0    14051 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_rabbitmq.py
+-rw-r--r--   0        0        0     2530 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_restapi.py
+-rw-r--r--   0        0        0     4837 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_run.py
+-rw-r--r--   0        0        0     9391 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_setup.py
+-rw-r--r--   0        0        0     3439 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_shell.py
+-rw-r--r--   0        0        0     6934 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_status.py
+-rw-r--r--   0        0        0     6707 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_storage.py
+-rw-r--r--   0        0        0     4582 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_user.py
+-rw-r--r--   0        0        0     1265 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/commands/cmd_verdi.py
+-rw-r--r--   0        0        0      297 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/groups/__init__.py
+-rw-r--r--   0        0        0     5345 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/groups/dynamic.py
+-rw-r--r--   0        0        0     6501 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/groups/verdi.py
+-rw-r--r--   0        0        0     1373 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/params/__init__.py
+-rw-r--r--   0        0        0     1277 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/params/arguments/__init__.py
+-rw-r--r--   0        0        0     2924 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/params/arguments/main.py
+-rw-r--r--   0        0        0     2374 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/params/arguments/overridable.py
+-rw-r--r--   0        0        0     2652 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/params/options/__init__.py
+-rw-r--r--   0        0        0      697 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/params/options/commands/__init__.py
+-rw-r--r--   0        0        0     6869 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/params/options/commands/code.py
+-rw-r--r--   0        0        0     6882 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/params/options/commands/computer.py
+-rw-r--r--   0        0        0    13950 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/params/options/commands/setup.py
+-rw-r--r--   0        0        0     2383 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/params/options/conditional.py
+-rw-r--r--   0        0        0     8083 2023-04-17 09:37:52.849518 aiida-core-2.3.0/aiida/cmdline/params/options/config.py
+-rw-r--r--   0        0        0     9190 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/options/interactive.py
+-rw-r--r--   0        0        0    21132 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/options/main.py
+-rw-r--r--   0        0        0     3764 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/options/multivalue.py
+-rw-r--r--   0        0        0     3918 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/options/overridable.py
+-rw-r--r--   0        0        0     1739 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/__init__.py
+-rw-r--r--   0        0        0     1348 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/calculation.py
+-rw-r--r--   0        0        0     2364 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/choice.py
+-rw-r--r--   0        0        0     2742 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/code.py
+-rw-r--r--   0        0        0     4052 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/computer.py
+-rw-r--r--   0        0        0     1714 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/config.py
+-rw-r--r--   0        0        0     1311 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/data.py
+-rw-r--r--   0        0        0     3901 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/group.py
+-rw-r--r--   0        0        0     6199 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/identifier.py
+-rw-r--r--   0        0        0     1568 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/multiple.py
+-rw-r--r--   0        0        0     1317 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/node.py
+-rw-r--r--   0        0        0     4488 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/path.py
+-rw-r--r--   0        0        0    10750 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/plugin.py
+-rw-r--r--   0        0        0     1329 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/process.py
+-rw-r--r--   0        0        0     3766 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/profile.py
+-rw-r--r--   0        0        0     3800 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/strings.py
+-rw-r--r--   0        0        0     2058 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/user.py
+-rw-r--r--   0        0        0     1335 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/params/types/workflow.py
+-rw-r--r--   0        0        0      177 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/templates/deprecated.tpl
+-rw-r--r--   0        0        0      218 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/templates/multiline.tpl
+-rw-r--r--   0        0        0      213 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/templates/new_cmt.txt.tpl
+-rw-r--r--   0        0        0      165 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/templates/warning.tpl
+-rw-r--r--   0        0        0     1122 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/utils/__init__.py
+-rw-r--r--   0        0        0     4001 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/utils/ascii_vis.py
+-rw-r--r--   0        0        0    17700 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/utils/common.py
+-rw-r--r--   0        0        0     9347 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/utils/decorators.py
+-rw-r--r--   0        0        0     1764 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/utils/defaults.py
+-rw-r--r--   0        0        0    10878 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/utils/echo.py
+-rw-r--r--   0        0        0     1710 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/utils/log.py
+-rw-r--r--   0        0        0     2336 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/utils/multi_line_input.py
+-rw-r--r--   0        0        0     2709 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/utils/pluginable.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/utils/query/__init__.py
+-rw-r--r--   0        0        0      981 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/utils/query/calculation.py
+-rw-r--r--   0        0        0     1026 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/utils/query/formatting.py
+-rw-r--r--   0        0        0     1007 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/utils/query/mapping.py
+-rw-r--r--   0        0        0     1393 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/utils/repository.py
+-rw-r--r--   0        0        0     5008 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/utils/shell.py
+-rw-r--r--   0        0        0      831 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/cmdline/utils/templates.py
+-rw-r--r--   0        0        0     2634 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/__init__.py
+-rw-r--r--   0        0        0    12464 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/constants.py
+-rw-r--r--   0        0        0     8031 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/datastructures.py
+-rw-r--r--   0        0        0     6332 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/escaping.py
+-rw-r--r--   0        0        0     8794 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/exceptions.py
+-rw-r--r--   0        0        0     8975 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/extendeddicts.py
+-rw-r--r--   0        0        0     3067 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/files.py
+-rw-r--r--   0        0        0    18668 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/folders.py
+-rw-r--r--   0        0        0    10933 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/hashing.py
+-rw-r--r--   0        0        0     2803 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/json.py
+-rw-r--r--   0        0        0     3717 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/lang.py
+-rw-r--r--   0        0        0     6586 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/links.py
+-rw-r--r--   0        0        0     9703 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/log.py
+-rw-r--r--   0        0        0     6909 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/progress_reporter.py
+-rw-r--r--   0        0        0     2800 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/timezone.py
+-rw-r--r--   0        0        0    19341 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/utils.py
+-rw-r--r--   0        0        0     1888 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/common/warnings.py
+-rw-r--r--   0        0        0     1996 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/engine/__init__.py
+-rw-r--r--   0        0        0      819 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/engine/daemon/__init__.py
+-rw-r--r--   0        0        0    31549 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/engine/daemon/client.py
+-rw-r--r--   0        0        0    31263 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/engine/daemon/execmanager.py
+-rw-r--r--   0        0        0     2295 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/engine/daemon/worker.py
+-rw-r--r--   0        0        0      919 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/engine/exceptions.py
+-rw-r--r--   0        0        0     5713 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/engine/launch.py
+-rw-r--r--   0        0        0     6617 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/engine/persistence.py
+-rw-r--r--   0        0        0     1756 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/engine/processes/__init__.py
+-rw-r--r--   0        0        0    10915 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/engine/processes/builder.py
+-rw-r--r--   0        0        0      937 2023-04-17 09:37:52.853514 aiida-core-2.3.0/aiida/engine/processes/calcjobs/__init__.py
+-rw-r--r--   0        0        0    48403 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/calcjobs/calcjob.py
+-rw-r--r--   0        0        0     1125 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/calcjobs/importer.py
+-rw-r--r--   0        0        0    12526 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/calcjobs/manager.py
+-rw-r--r--   0        0        0     8671 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/calcjobs/monitors.py
+-rw-r--r--   0        0        0    32269 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/calcjobs/tasks.py
+-rw-r--r--   0        0        0    12331 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/control.py
+-rw-r--r--   0        0        0     3690 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/exit_code.py
+-rw-r--r--   0        0        0    23589 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/functions.py
+-rw-r--r--   0        0        0     3852 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/futures.py
+-rw-r--r--   0        0        0    11954 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/ports.py
+-rw-r--r--   0        0        0    43594 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/process.py
+-rw-r--r--   0        0        0     4547 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/process_spec.py
+-rw-r--r--   0        0        0     1018 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/utils.py
+-rw-r--r--   0        0        0     1187 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/workchains/__init__.py
+-rw-r--r--   0        0        0     2470 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/workchains/awaitable.py
+-rw-r--r--   0        0        0     1968 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/workchains/context.py
+-rw-r--r--   0        0        0    21825 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/workchains/restart.py
+-rw-r--r--   0        0        0     7604 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/workchains/utils.py
+-rw-r--r--   0        0        0    17279 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/processes/workchains/workchain.py
+-rw-r--r--   0        0        0    14996 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/runners.py
+-rw-r--r--   0        0        0     6129 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/transports.py
+-rw-r--r--   0        0        0    12275 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/engine/utils.py
+-rw-r--r--   0        0        0     1845 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/__init__.py
+-rw-r--r--   0        0        0    11086 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/caching.py
+-rw-r--r--   0        0        0    11486 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/configuration/__init__.py
+-rw-r--r--   0        0        0    20965 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/configuration/config.py
+-rw-r--r--   0        0        0     1075 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/configuration/migrations/__init__.py
+-rw-r--r--   0        0        0    20944 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/configuration/migrations/migrations.py
+-rw-r--r--   0        0        0     4732 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/configuration/options.py
+-rw-r--r--   0        0        0    10267 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/configuration/profile.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/configuration/schema/__init__.py
+-rw-r--r--   0        0        0    15472 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/configuration/schema/config-v5.schema.json
+-rw-r--r--   0        0        0    12291 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/configuration/schema/config-v6.schema.json
+-rw-r--r--   0        0        0    12289 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/configuration/schema/config-v7.schema.json
+-rw-r--r--   0        0        0    12749 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/configuration/schema/config-v8.schema.json
+-rw-r--r--   0        0        0    13329 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/configuration/schema/config-v9.schema.json
+-rw-r--r--   0        0        0     5305 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/configuration/settings.py
+-rw-r--r--   0        0        0     1148 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/external/__init__.py
+-rw-r--r--   0        0        0     9955 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/external/postgres.py
+-rw-r--r--   0        0        0     1104 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/external/rmq/__init__.py
+-rw-r--r--   0        0        0     3868 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/external/rmq/client.py
+-rw-r--r--   0        0        0      432 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/external/rmq/defaults.py
+-rw-r--r--   0        0        0     7433 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/external/rmq/launcher.py
+-rw-r--r--   0        0        0     2743 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/external/rmq/utils.py
+-rw-r--r--   0        0        0    20986 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/manager.py
+-rw-r--r--   0        0        0    10232 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/profile_access.py
+-rw-r--r--   0        0        0      993 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/tests/__init__.py
+-rw-r--r--   0        0        0    19379 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/tests/main.py
+-rw-r--r--   0        0        0    34536 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/manage/tests/pytest_fixtures.py
+-rw-r--r--   0        0        0     2738 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/orm/__init__.py
+-rw-r--r--   0        0        0     5406 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/orm/authinfos.py
+-rw-r--r--   0        0        0    12110 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/orm/autogroup.py
+-rw-r--r--   0        0        0     4451 2023-04-17 09:37:52.857511 aiida-core-2.3.0/aiida/orm/comments.py
+-rw-r--r--   0        0        0    26490 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/computers.py
+-rw-r--r--   0        0        0     4716 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/convert.py
+-rw-r--r--   0        0        0    10275 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/entities.py
+-rw-r--r--   0        0        0     7190 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/extras.py
+-rw-r--r--   0        0        0    13709 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/groups.py
+-rw-r--r--   0        0        0     1628 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/implementation/__init__.py
+-rw-r--r--   0        0        0     3059 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/implementation/authinfos.py
+-rw-r--r--   0        0        0     3806 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/implementation/comments.py
+-rw-r--r--   0        0        0     3550 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/implementation/computers.py
+-rw-r--r--   0        0        0     7922 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/implementation/entities.py
+-rw-r--r--   0        0        0     5840 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/implementation/groups.py
+-rw-r--r--   0        0        0     3025 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/implementation/logs.py
+-rw-r--r--   0        0        0    11547 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/implementation/nodes.py
+-rw-r--r--   0        0        0     6576 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/implementation/querybuilder.py
+-rw-r--r--   0        0        0    14652 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/implementation/storage_backend.py
+-rw-r--r--   0        0        0     2459 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/implementation/users.py
+-rw-r--r--   0        0        0     5746 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/implementation/utils.py
+-rw-r--r--   0        0        0     7505 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/logs.py
+-rw-r--r--   0        0        0     1786 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/__init__.py
+-rw-r--r--   0        0        0     8303 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/attributes.py
+-rw-r--r--   0        0        0     7099 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/caching.py
+-rw-r--r--   0        0        0     2497 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/comments.py
+-rw-r--r--   0        0        0     1885 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/__init__.py
+-rw-r--r--   0        0        0     1069 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/array/__init__.py
+-rw-r--r--   0        0        0     9322 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/array/array.py
+-rw-r--r--   0        0        0    73820 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/array/bands.py
+-rw-r--r--   0        0        0    20634 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/array/kpoints.py
+-rw-r--r--   0        0        0    13142 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/array/projection.py
+-rw-r--r--   0        0        0    38839 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/array/trajectory.py
+-rw-r--r--   0        0        0     6269 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/array/xy.py
+-rw-r--r--   0        0        0     2038 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/base.py
+-rw-r--r--   0        0        0     1828 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/bool.py
+-rw-r--r--   0        0        0    30429 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/cif.py
+-rw-r--r--   0        0        0      401 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/code/__init__.py
+-rw-r--r--   0        0        0    17202 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/code/abstract.py
+-rw-r--r--   0        0        0     5354 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/code/containerized.py
+-rw-r--r--   0        0        0     8279 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/code/installed.py
+-rw-r--r--   0        0        0    23043 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/code/legacy.py
+-rw-r--r--   0        0        0     8095 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/code/portable.py
+-rw-r--r--   0        0        0    14661 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/data.py
+-rw-r--r--   0        0        0     5667 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/dict.py
+-rw-r--r--   0        0        0     4588 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/enum.py
+-rw-r--r--   0        0        0      967 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/float.py
+-rw-r--r--   0        0        0     1690 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/folder.py
+-rw-r--r--   0        0        0      969 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/int.py
+-rw-r--r--   0        0        0     7427 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/jsonable.py
+-rw-r--r--   0        0        0     4948 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/list.py
+-rw-r--r--   0        0        0     3373 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/numeric.py
+-rw-r--r--   0        0        0     4784 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/orbital.py
+-rw-r--r--   0        0        0      338 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/remote/__init__.py
+-rw-r--r--   0        0        0     8173 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/remote/base.py
+-rw-r--r--   0        0        0      326 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/remote/stash/__init__.py
+-rw-r--r--   0        0        0     2371 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/remote/stash/base.py
+-rw-r--r--   0        0        0     2250 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/remote/stash/folder.py
+-rw-r--r--   0        0        0     4935 2023-04-17 09:37:52.861508 aiida-core-2.3.0/aiida/orm/nodes/data/singlefile.py
+-rw-r--r--   0        0        0      910 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/nodes/data/str.py
+-rw-r--r--   0        0        0    93793 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/nodes/data/structure.py
+-rw-r--r--   0        0        0    19092 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/nodes/data/upf.py
+-rw-r--r--   0        0        0    11454 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/nodes/links.py
+-rw-r--r--   0        0        0    27920 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/nodes/node.py
+-rw-r--r--   0        0        0     1009 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/nodes/process/__init__.py
+-rw-r--r--   0        0        0      941 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/nodes/process/calculation/__init__.py
+-rw-r--r--   0        0        0     2605 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/nodes/process/calculation/calcfunction.py
+-rw-r--r--   0        0        0    21120 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/nodes/process/calculation/calcjob.py
+-rw-r--r--   0        0        0     2115 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/nodes/process/calculation/calculation.py
+-rw-r--r--   0        0        0    20753 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/nodes/process/process.py
+-rw-r--r--   0        0        0      936 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/nodes/process/workflow/__init__.py
+-rw-r--r--   0        0        0     1775 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/nodes/process/workflow/workchain.py
+-rw-r--r--   0        0        0     3631 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/nodes/process/workflow/workflow.py
+-rw-r--r--   0        0        0     2442 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/nodes/process/workflow/workfunction.py
+-rw-r--r--   0        0        0    15675 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/nodes/repository.py
+-rw-r--r--   0        0        0    61503 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/querybuilder.py
+-rw-r--r--   0        0        0     4785 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/users.py
+-rw-r--r--   0        0        0     1415 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/utils/__init__.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/utils/builders/__init__.py
+-rw-r--r--   0        0        0     8496 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/utils/builders/code.py
+-rw-r--r--   0        0        0     8108 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/utils/builders/computer.py
+-rw-r--r--   0        0        0     4952 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/utils/calcjob.py
+-rw-r--r--   0        0        0    17089 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/utils/links.py
+-rw-r--r--   0        0        0    36736 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/utils/loaders.py
+-rw-r--r--   0        0        0     2808 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/utils/log.py
+-rw-r--r--   0        0        0    10970 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/utils/managers.py
+-rw-r--r--   0        0        0     9786 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/utils/mixins.py
+-rw-r--r--   0        0        0     7008 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/utils/node.py
+-rw-r--r--   0        0        0     4573 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/utils/remote.py
+-rw-r--r--   0        0        0     9126 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/orm/utils/serialize.py
+-rw-r--r--   0        0        0      847 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/parsers/__init__.py
+-rw-r--r--   0        0        0     8094 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/parsers/parser.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/parsers/plugins/__init__.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/parsers/plugins/arithmetic/__init__.py
+-rw-r--r--   0        0        0     2226 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/parsers/plugins/arithmetic/add.py
+-rw-r--r--   0        0        0     1984 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/parsers/plugins/diff_tutorial/parsers.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/parsers/plugins/templatereplacer/__init__.py
+-rw-r--r--   0        0        0     3244 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/parsers/plugins/templatereplacer/parser.py
+-rw-r--r--   0        0        0     1329 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/plugins/__init__.py
+-rw-r--r--   0        0        0    17411 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/plugins/entry_point.py
+-rw-r--r--   0        0        0    16492 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/plugins/factories.py
+-rw-r--r--   0        0        0     4405 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/plugins/utils.py
+-rw-r--r--   0        0        0       26 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/py.typed
+-rw-r--r--   0        0        0     1017 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/repository/__init__.py
+-rw-r--r--   0        0        0      368 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/repository/backend/__init__.py
+-rw-r--r--   0        0        0     9748 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/repository/backend/abstract.py
+-rw-r--r--   0        0        0     9659 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/repository/backend/disk_object_store.py
+-rw-r--r--   0        0        0     4392 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/repository/backend/sandbox.py
+-rw-r--r--   0        0        0     5382 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/repository/common.py
+-rw-r--r--   0        0        0    24331 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/repository/repository.py
+-rw-r--r--   0        0        0      823 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/restapi/__init__.py
+-rw-r--r--   0        0        0     7379 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/restapi/api.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.865504 aiida-core-2.3.0/aiida/restapi/common/__init__.py
+-rw-r--r--   0        0        0     1701 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/common/config.py
+-rw-r--r--   0        0        0     1589 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/common/exceptions.py
+-rw-r--r--   0        0        0    19441 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/common/identifiers.py
+-rw-r--r--   0        0        0    34328 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/common/utils.py
+-rw-r--r--   0        0        0    28984 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/resources.py
+-rwxr-xr-x   0        0        0     4911 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/run_api.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/__init__.py
+-rw-r--r--   0        0        0    18895 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/base.py
+-rw-r--r--   0        0        0     4211 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/computer.py
+-rw-r--r--   0        0        0     3321 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/group.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/__init__.py
+-rw-r--r--   0        0        0     2835 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/data/__init__.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/data/array/__init__.py
+-rw-r--r--   0        0        0     2051 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/data/array/bands.py
+-rw-r--r--   0        0        0     1478 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/data/cif.py
+-rw-r--r--   0        0        0     1464 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/data/code.py
+-rw-r--r--   0        0        0     5420 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/data/kpoints.py
+-rw-r--r--   0        0        0     1579 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/data/structure.py
+-rw-r--r--   0        0        0     1388 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/data/upf.py
+-rw-r--r--   0        0        0    31726 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/node.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/process/__init__.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/process/calculation/__init__.py
+-rw-r--r--   0        0        0     1579 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/process/calculation/calcfunction.py
+-rw-r--r--   0        0        0     2619 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/process/calculation/calcjob.py
+-rw-r--r--   0        0        0     4530 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/process/process.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/process/workflow/__init__.py
+-rw-r--r--   0        0        0     1545 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/process/workflow/workchain.py
+-rw-r--r--   0        0        0     1576 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/nodes/process/workflow/workfunction.py
+-rw-r--r--   0        0        0     2765 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/restapi/translator/user.py
+-rw-r--r--   0        0        0     1074 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/schedulers/__init__.py
+-rw-r--r--   0        0        0    25535 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/schedulers/datastructures.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/schedulers/plugins/__init__.py
+-rw-r--r--   0        0        0    15506 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/schedulers/plugins/direct.py
+-rw-r--r--   0        0        0    33310 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/schedulers/plugins/lsf.py
+-rw-r--r--   0        0        0    31102 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/schedulers/plugins/pbsbaseclasses.py
+-rw-r--r--   0        0        0     3701 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/schedulers/plugins/pbspro.py
+-rw-r--r--   0        0        0    20419 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/schedulers/plugins/sge.py
+-rw-r--r--   0        0        0    35179 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/schedulers/plugins/slurm.py
+-rw-r--r--   0        0        0     3799 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/schedulers/plugins/torque.py
+-rw-r--r--   0        0        0    20077 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/schedulers/scheduler.py
+-rw-r--r--   0        0        0     1108 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/sphinxext/__init__.py
+-rw-r--r--   0        0        0     1450 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/sphinxext/calcjob.py
+-rw-r--r--   0        0        0     9048 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/sphinxext/process.py
+-rw-r--r--   0        0        0     1475 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/sphinxext/workchain.py
+-rw-r--r--   0        0        0      810 2023-04-17 09:37:52.869501 aiida-core-2.3.0/aiida/storage/__init__.py
+-rw-r--r--   0        0        0      815 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/log.py
+-rw-r--r--   0        0        0      877 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/__init__.py
+-rwxr-xr-x   0        0        0     3996 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/alembic_cli.py
+-rw-r--r--   0        0        0    18190 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/backend.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/__init__.py
+-rw-r--r--   0        0        0     2198 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/env.py
+-rw-r--r--   0        0        0      494 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/script.py.mako
+-rw-r--r--   0        0        0      748 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/__init__.py
+-rw-r--r--   0        0        0     2260 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/calc_state.py
+-rw-r--r--   0        0        0     3916 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/create_dbattribute.py
+-rw-r--r--   0        0        0     8837 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/dblog_update.py
+-rw-r--r--   0        0        0     1563 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/duplicate_uuids.py
+-rw-r--r--   0        0        0    12177 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/integrity.py
+-rw-r--r--   0        0        0     3477 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/legacy_workflows.py
+-rw-r--r--   0        0        0     5991 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/migrate_repository.py
+-rw-r--r--   0        0        0     9306 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/parity.py
+-rw-r--r--   0        0        0     7520 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/provenance_redesign.py
+-rw-r--r--   0        0        0     5534 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/reflect.py
+-rw-r--r--   0        0        0    18164 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/utils.py
+-rw-r--r--   0        0        0     2902 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/041a79fc615f_dblog_cleaning.py
+-rw-r--r--   0        0        0     1486 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/07fac78e6209_drop_computer_transport_params.py
+-rw-r--r--   0        0        0     2482 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/0aebbeab274d_base_data_plugin_type_string.py
+-rw-r--r--   0        0        0     1819 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/0edcdd5a30f0_dbgroup_extras.py
+-rw-r--r--   0        0        0     1829 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/118349c10896_default_link_label.py
+-rw-r--r--   0        0        0     2727 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/12536798d4d3_trajectory_symbols_to_attribute.py
+-rw-r--r--   0        0        0     2856 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/140c971ae0a3_migrate_builtin_calculations.py
+-rw-r--r--   0        0        0     1168 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/162b99bca4a2_drop_dbcalcstate.py
+-rw-r--r--   0        0        0     1361 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/1830c8430131_drop_node_columns_nodeversion_public.py
+-rw-r--r--   0        0        0     1872 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/1b8ed3425af9_remove_legacy_workflows.py
+-rw-r--r--   0        0        0     9697 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/1de112340b16_django_parity_1.py
+-rw-r--r--   0        0        0    10079 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/1de112340b17_django_parity_2.py
+-rw-r--r--   0        0        0     1252 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/1de112340b18_django_parity_3.py
+-rw-r--r--   0        0        0     1382 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/1feaea71bd5a_migrate_repository.py
+-rw-r--r--   0        0        0     5530 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/239cea6d2452_provenance_redesign.py
+-rw-r--r--   0        0        0     8062 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/26d561acd560_data_migration_legacy_job_calculations.py
+-rw-r--r--   0        0        0     5861 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/34a831f4286d_entry_point_core_prefix.py
+-rw-r--r--   0        0        0     2044 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/35d4ee9a1b0e_code_hidden_attr_to_extra.py
+-rw-r--r--   0        0        0     1309 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/375c2db70663_dblog_uuid_uniqueness_constraint.py
+-rw-r--r--   0        0        0     1615 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/37f3d4882837_make_all_uuid_columns_unique.py
+-rw-r--r--   0        0        0     1335 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/3d6190594e19_remove_dbcomputer_enabled.py
+-rw-r--r--   0        0        0      802 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/535039300e4a_computer_name_to_label.py
+-rw-r--r--   0        0        0     1892 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/59edaf8a8b79_adding_indexes_and_constraints_to_the_.py
+-rw-r--r--   0        0        0     1689 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/5a49629f0d45_dblink_indices.py
+-rw-r--r--   0        0        0     1742 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/5d4d844852b6_invalidating_node_hash.py
+-rw-r--r--   0        0        0     1762 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/5ddd24e52864_dbnode_type_to_dbnode_node_type.py
+-rw-r--r--   0        0        0     1866 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/61fc0913fae9_remove_node_prefix.py
+-rw-r--r--   0        0        0     1391 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/62fe0d36de90_add_node_uuid_unique_constraint.py
+-rw-r--r--   0        0        0     1621 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/6a5c2ea1439d_move_data_within_node_module.py
+-rw-r--r--   0        0        0     1376 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/6c629c886f84_process_type.py
+-rw-r--r--   0        0        0     1351 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/70c7d732f1b2_delete_dbpath.py
+-rw-r--r--   0        0        0     1466 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/7536a82b2cc4_add_node_repository_metadata.py
+-rw-r--r--   0        0        0     1360 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/7a6587e16f4c_unique_constraints_for_the_db_dbgroup_.py
+-rw-r--r--   0        0        0     2610 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/7b38a9e783e7_seal_unsealed_processes.py
+-rw-r--r--   0        0        0     3849 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/7ca08c391c49_calc_job_option_attribute_keys.py
+-rw-r--r--   0        0        0     1311 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/89176227b25_add_indexes_to_dbworkflowdata_table.py
+-rw-r--r--   0        0        0     2309 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/91b573400be5_prepare_schema_reset.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/__init__.py
+-rw-r--r--   0        0        0     1158 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/a514d673c163_drop_dblock.py
+-rw-r--r--   0        0        0     1656 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/a603da2cc809_code_sub_class_of_data.py
+-rw-r--r--   0        0        0     6613 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/a6048f0ffca8_update_linktypes.py
+-rw-r--r--   0        0        0     1840 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/b8b23ddefad4_dbgroup_name_to_label_type_to_type_string.py
+-rw-r--r--   0        0        0     1778 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/bf591f31dd12_dbgroup_type_string.py
+-rw-r--r--   0        0        0     2269 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/ce56d84bcc35_delete_trajectory_symbols_array.py
+-rw-r--r--   0        0        0     1599 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/d254fdfed416_rename_parameter_data_to_dict.py
+-rw-r--r--   0        0        0     1564 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/de2eaf6978b4_simplify_user_model.py
+-rw-r--r--   0        0        0    30892 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0001_initial.py
+-rw-r--r--   0        0        0     1505 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0002_db_state_change.py
+-rw-r--r--   0        0        0     1809 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0003_add_link_type.py
+-rw-r--r--   0        0        0     1547 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0004_add_daemon_and_uuid_indices.py
+-rw-r--r--   0        0        0     1246 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0005_add_cmtime_indices.py
+-rw-r--r--   0        0        0     1295 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0006_delete_dbpath.py
+-rw-r--r--   0        0        0     6316 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0007_update_linktypes.py
+-rw-r--r--   0        0        0     2359 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0008_code_hidden_to_extra.py
+-rw-r--r--   0        0        0     2275 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0009_base_data_plugin_type_string.py
+-rw-r--r--   0        0        0     1474 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0010_process_type.py
+-rw-r--r--   0        0        0     1712 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0011_delete_kombu_tables.py
+-rw-r--r--   0        0        0     1073 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0012_drop_dblock.py
+-rw-r--r--   0        0        0     1747 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0013_django_1_8.py
+-rw-r--r--   0        0        0     1374 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0014_add_node_uuid_unique_constraint.py
+-rw-r--r--   0        0        0     1192 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0015_invalidating_node_hash.py
+-rw-r--r--   0        0        0     1171 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0016_code_sub_class_of_data.py
+-rw-r--r--   0        0        0     1083 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0017_drop_dbcalcstate.py
+-rw-r--r--   0        0        0     2391 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0018_django_1_11.py
+-rw-r--r--   0        0        0     2558 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0019_migrate_builtin_calculations.py
+-rw-r--r--   0        0        0     6233 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0020_provenance_redesign.py
+-rw-r--r--   0        0        0     2439 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0021_dbgroup_name_to_label_type_to_type_string.py
+-rw-r--r--   0        0        0     1539 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0022_dbgroup_type_string_change_content.py
+-rw-r--r--   0        0        0     3316 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0023_calc_job_option_attribute_keys.py
+-rw-r--r--   0        0        0     3663 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0024a_dblog_update.py
+-rw-r--r--   0        0        0     1248 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0024b_dblog_update.py
+-rw-r--r--   0        0        0     1480 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0025_move_data_within_node_module.py
+-rw-r--r--   0        0        0     2250 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0026_trajectory_symbols_to_attribute.py
+-rw-r--r--   0        0        0     2415 2023-04-17 09:37:52.873498 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0027_delete_trajectory_symbols_array.py
+-rw-r--r--   0        0        0     1598 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0028_remove_node_prefix.py
+-rw-r--r--   0        0        0     1383 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0029_rename_parameter_data_to_dict.py
+-rw-r--r--   0        0        0     1267 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0030_dbnode_type_to_dbnode_node_type.py
+-rw-r--r--   0        0        0     1140 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0031_remove_dbcomputer_enabled.py
+-rw-r--r--   0        0        0     1552 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0032_remove_legacy_workflows.py
+-rw-r--r--   0        0        0     1516 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0033_replace_text_field_with_json_field.py
+-rw-r--r--   0        0        0     1203 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0034_drop_node_columns_nodeversion_public.py
+-rw-r--r--   0        0        0     1550 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0035_simplify_user_model.py
+-rw-r--r--   0        0        0     1156 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0036_drop_computer_transport_params.py
+-rw-r--r--   0        0        0     7292 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0037_attributes_extras_settings_json.py
+-rw-r--r--   0        0        0     7899 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0038_data_migration_legacy_job_calculations.py
+-rw-r--r--   0        0        0     1220 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0039_reset_hash.py
+-rw-r--r--   0        0        0     3186 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0040_data_migration_legacy_process_attributes.py
+-rw-r--r--   0        0        0     2403 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0041_seal_unsealed_processes.py
+-rw-r--r--   0        0        0     2115 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0042_prepare_schema_reset.py
+-rw-r--r--   0        0        0     1612 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0043_default_link_label.py
+-rw-r--r--   0        0        0     1615 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0044_dbgroup_type_string.py
+-rw-r--r--   0        0        0     1673 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0045_dbgroup_extras.py
+-rw-r--r--   0        0        0     1378 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0046_add_node_repository_metadata.py
+-rw-r--r--   0        0        0     1297 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0047_migrate_repository.py
+-rw-r--r--   0        0        0     1728 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0048_computer_name_to_label.py
+-rw-r--r--   0        0        0     5770 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0049_entry_point_core_prefix.py
+-rw-r--r--   0        0        0     1974 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0050_sqlalchemy_parity.py
+-rw-r--r--   0        0        0    21476 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/e15ef2630a1b_initial_schema.py
+-rw-r--r--   0        0        0     2135 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/e72ad251bcdb_dbgroup_class_change_type_string_values.py
+-rw-r--r--   0        0        0     3393 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/e734dd5e50d7_data_migration_legacy_process_attributes.py
+-rw-r--r--   0        0        0     1303 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/e797afa09270_reset_hash.py
+-rw-r--r--   0        0        0     1760 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/ea2f50e7f615_dblog_create_uuid_column.py
+-rw-r--r--   0        0        0     2221 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/f9a69de76a9a_delete_kombu_tables.py
+-rw-r--r--   0        0        0    11820 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/main_0001_initial.py
+-rw-r--r--   0        0        0    21817 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/migrator.py
+-rw-r--r--   0        0        0      703 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/models/__init__.py
+-rw-r--r--   0        0        0     2660 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/models/authinfo.py
+-rw-r--r--   0        0        0     4494 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/models/base.py
+-rw-r--r--   0        0        0     2322 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/models/comment.py
+-rw-r--r--   0        0        0     2904 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/models/computer.py
+-rw-r--r--   0        0        0     3635 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/models/group.py
+-rw-r--r--   0        0        0     2677 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/models/log.py
+-rw-r--r--   0        0        0     8274 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/models/node.py
+-rw-r--r--   0        0        0     1749 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/models/settings.py
+-rw-r--r--   0        0        0     1739 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/models/user.py
+-rw-r--r--   0        0        0      678 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/orm/__init__.py
+-rw-r--r--   0        0        0     4752 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/orm/authinfos.py
+-rw-r--r--   0        0        0     6320 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/orm/comments.py
+-rw-r--r--   0        0        0     4282 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/orm/computers.py
+-rw-r--r--   0        0        0     3537 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/orm/convert.py
+-rw-r--r--   0        0        0     3451 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/orm/entities.py
+-rw-r--r--   0        0        0     3251 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/orm/extras_mixin.py
+-rw-r--r--   0        0        0    10474 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/orm/groups.py
+-rw-r--r--   0        0        0     5113 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/orm/logs.py
+-rw-r--r--   0        0        0    10981 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/orm/nodes.py
+-rw-r--r--   0        0        0      746 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/orm/querybuilder/__init__.py
+-rw-r--r--   0        0        0    23343 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/orm/querybuilder/joiner.py
+-rw-r--r--   0        0        0    45951 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/orm/querybuilder/main.py
+-rw-r--r--   0        0        0     2324 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/orm/users.py
+-rw-r--r--   0        0        0     7345 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/orm/utils.py
+-rw-r--r--   0        0        0     8962 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/psql_dos/utils.py
+-rw-r--r--   0        0        0     1022 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_temp/__init__.py
+-rw-r--r--   0        0        0     7561 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_temp/backend.py
+-rw-r--r--   0        0        0     1664 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/__init__.py
+-rw-r--r--   0        0        0    15085 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/backend.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/__init__.py
+-rw-r--r--   0        0        0     1999 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/env.py
+-rw-r--r--   0        0        0     1754 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/__init__.py
+-rw-r--r--   0        0        0     3332 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v04_to_v05.py
+-rw-r--r--   0        0        0     7335 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v05_to_v06.py
+-rw-r--r--   0        0        0     5971 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v06_to_v07.py
+-rw-r--r--   0        0        0     2107 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v07_to_v08.py
+-rw-r--r--   0        0        0     2361 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v08_to_v09.py
+-rw-r--r--   0        0        0     1355 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v09_to_v10.py
+-rw-r--r--   0        0        0     1480 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v10_to_v11.py
+-rw-r--r--   0        0        0     5486 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v11_to_v12.py
+-rw-r--r--   0        0        0     1698 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v12_to_v13.py
+-rw-r--r--   0        0        0    12668 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy_to_main.py
+-rw-r--r--   0        0        0      572 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/script.py.mako
+-rw-r--r--   0        0        0     8212 2023-04-17 09:37:52.877494 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/utils.py
+-rw-r--r--   0        0        0     8703 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/v1_db_schema.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/versions/__init__.py
+-rw-r--r--   0        0        0     8710 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/versions/main_0000_initial.py
+-rw-r--r--   0        0        0     6790 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/versions/main_0000a_replace_nulls.py
+-rw-r--r--   0        0        0     4413 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/versions/main_0000b_non_nullable.py
+-rw-r--r--   0        0        0     1044 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/versions/main_0001.py
+-rw-r--r--   0        0        0    17760 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/storage/sqlite_zip/migrator.py
+-rw-r--r--   0        0        0     7070 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/storage/sqlite_zip/models.py
+-rw-r--r--   0        0        0    15167 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/storage/sqlite_zip/orm.py
+-rw-r--r--   0        0        0     4882 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/storage/sqlite_zip/utils.py
+-rw-r--r--   0        0        0     1845 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/__init__.py
+-rw-r--r--   0        0        0     1366 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/archive/__init__.py
+-rw-r--r--   0        0        0     9493 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/archive/abstract.py
+-rw-r--r--   0        0        0     3349 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/archive/common.py
+-rw-r--r--   0        0        0    29933 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/archive/create.py
+-rw-r--r--   0        0        0     2018 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/archive/exceptions.py
+-rw-r--r--   0        0        0      844 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/archive/implementations/__init__.py
+-rw-r--r--   0        0        0      836 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/archive/implementations/sqlite_zip/__init__.py
+-rw-r--r--   0        0        0     3280 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/archive/implementations/sqlite_zip/main.py
+-rw-r--r--   0        0        0     2268 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/archive/implementations/sqlite_zip/reader.py
+-rw-r--r--   0        0        0    12744 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/archive/implementations/sqlite_zip/writer.py
+-rw-r--r--   0        0        0    50475 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/archive/imports.py
+-rw-r--r--   0        0        0      833 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/calculations/__init__.py
+-rw-r--r--   0        0        0     1053 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/calculations/base.py
+-rw-r--r--   0        0        0      997 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/data/__init__.py
+-rw-r--r--   0        0        0      862 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/data/array/__init__.py
+-rw-r--r--   0        0        0      952 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/data/array/kpoints/__init__.py
+-rw-r--r--   0        0        0    77224 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/data/array/kpoints/legacy.py
+-rw-r--r--   0        0        0    10772 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/data/array/kpoints/main.py
+-rw-r--r--   0        0        0     7034 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/data/array/kpoints/seekpath.py
+-rw-r--r--   0        0        0     1377 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/data/array/trajectory.py
+-rw-r--r--   0        0        0     8683 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/data/cif.py
+-rw-r--r--   0        0        0      899 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/data/orbital/__init__.py
+-rw-r--r--   0        0        0     6521 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/data/orbital/orbital.py
+-rw-r--r--   0        0        0    13938 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/data/orbital/realhydrogen.py
+-rw-r--r--   0        0        0    11892 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/data/structure.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/dbexporters/__init__.py
+-rw-r--r--   0        0        0      783 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/dbimporters/__init__.py
+-rw-r--r--   0        0        0    12063 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/dbimporters/baseclasses.py
+-rw-r--r--   0        0        0      720 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/dbimporters/plugins/__init__.py
+-rw-r--r--   0        0        0    12105 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/dbimporters/plugins/cod.py
+-rw-r--r--   0        0        0    28472 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/dbimporters/plugins/icsd.py
+-rw-r--r--   0        0        0     6920 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/dbimporters/plugins/materialsproject.py
+-rw-r--r--   0        0        0    11604 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/dbimporters/plugins/mpds.py
+-rw-r--r--   0        0        0     5697 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/dbimporters/plugins/mpod.py
+-rw-r--r--   0        0        0     5399 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/dbimporters/plugins/nninc.py
+-rw-r--r--   0        0        0     4692 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/dbimporters/plugins/oqmd.py
+-rw-r--r--   0        0        0     4463 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/dbimporters/plugins/pcod.py
+-rw-r--r--   0        0        0     2691 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/dbimporters/plugins/tcod.py
+-rw-r--r--   0        0        0      883 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/graph/__init__.py
+-rw-r--r--   0        0        0    17095 2023-04-17 09:37:52.881491 aiida-core-2.3.0/aiida/tools/graph/age_entities.py
+-rw-r--r--   0        0        0    18095 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/tools/graph/age_rules.py
+-rw-r--r--   0        0        0     7116 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/tools/graph/deletions.py
+-rw-r--r--   0        0        0    12733 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/tools/graph/graph_traversers.py
+-rw-r--r--   0        0        0     1382 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/tools/groups/__init__.py
+-rw-r--r--   0        0        0    12617 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/tools/groups/paths.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/tools/ipython/__init__.py
+-rw-r--r--   0        0        0     1212 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/tools/ipython/aiida_magic_register.py
+-rw-r--r--   0        0        0     7832 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/tools/ipython/ipython_magics.py
+-rw-r--r--   0        0        0        0 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/tools/query/__init__.py
+-rw-r--r--   0        0        0     6826 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/tools/query/calculation.py
+-rw-r--r--   0        0        0     2963 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/tools/query/formatting.py
+-rw-r--r--   0        0        0     7054 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/tools/query/mapping.py
+-rw-r--r--   0        0        0      941 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/tools/visualization/__init__.py
+-rw-r--r--   0        0        0    35782 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/tools/visualization/graph.py
+-rw-r--r--   0        0        0      943 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/transports/__init__.py
+-rw-r--r--   0        0        0     6400 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/transports/cli.py
+-rw-r--r--   0        0        0      851 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/transports/plugins/__init__.py
+-rw-r--r--   0        0        0    37052 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/transports/plugins/local.py
+-rw-r--r--   0        0        0    62840 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/transports/plugins/ssh.py
+-rw-r--r--   0        0        0    30913 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/transports/transport.py
+-rw-r--r--   0        0        0     3273 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/transports/util.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/workflows/__init__.py
+-rw-r--r--   0        0        0      632 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/workflows/arithmetic/__init__.py
+-rw-r--r--   0        0        0     1057 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/workflows/arithmetic/add_multiply.py
+-rw-r--r--   0        0        0     2538 2023-04-17 09:37:52.885487 aiida-core-2.3.0/aiida/workflows/arithmetic/multiply_add.py
+-rw-r--r--   0        0        0      327 2023-04-17 09:37:52.885487 aiida-core-2.3.0/codecov.yml
+-rw-r--r--   0        0        0      696 2023-04-17 09:37:52.937444 aiida-core-2.3.0/environment.yml
+-rw-r--r--   0        0        0    13919 2023-04-17 09:37:52.937444 aiida-core-2.3.0/open_source_licenses.txt
+-rw-r--r--   0        0        0    15761 2023-04-17 09:37:52.937444 aiida-core-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      510 2023-04-17 09:37:52.937444 aiida-core-2.3.0/requirements/README.md
+-rw-r--r--   0        0        0     3160 2023-04-17 09:37:52.937444 aiida-core-2.3.0/requirements/requirements-py-3.10.txt
+-rw-r--r--   0        0        0     3609 2023-04-17 09:37:52.937444 aiida-core-2.3.0/requirements/requirements-py-3.11.txt
+-rw-r--r--   0        0        0     3234 2023-04-17 09:37:52.937444 aiida-core-2.3.0/requirements/requirements-py-3.8.txt
+-rw-r--r--   0        0        0     3207 2023-04-17 09:37:52.937444 aiida-core-2.3.0/requirements/requirements-py-3.9.txt
+-rw-r--r--   0        0        0      473 2023-04-17 09:37:52.993397 aiida-core-2.3.0/utils/.gource.conf
+-rw-r--r--   0        0        0      697 2023-04-17 09:37:52.993397 aiida-core-2.3.0/utils/__init__.py
+-rwxr-xr-x   0        0        0    16828 2023-04-17 09:37:52.993397 aiida-core-2.3.0/utils/dependency_management.py
+-rw-r--r--   0        0        0     6562 2023-04-17 09:37:52.993397 aiida-core-2.3.0/utils/make_all.py
+-rw-r--r--   0        0        0       73 2023-04-17 09:37:52.993397 aiida-core-2.3.0/utils/requirements.txt
+-rw-r--r--   0        0        0     5871 2023-04-17 09:37:52.993397 aiida-core-2.3.0/utils/validate_consistency.py
+-rw-r--r--   0        0        0    11093 1970-01-01 00:00:00.000000 aiida-core-2.3.0/PKG-INFO
```

### Comparing `aiida-core-2.2.2/.docker/docker-rabbitmq.yml` & `aiida-core-2.3.0/.docker/docker-rabbitmq.yml`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.docker/opt/configure-aiida.sh` & `aiida-core-2.3.0/.docker/opt/configure-aiida.sh`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     verdi quicksetup                           \
         --non-interactive                      \
         --profile "${PROFILE_NAME}"            \
         --email "${USER_EMAIL}"                \
         --first-name "${USER_FIRST_NAME}"      \
         --last-name "${USER_LAST_NAME}"        \
         --institution "${USER_INSTITUTION}"    \
-        --db-backend "${AIIDADB_BACKEND}"
+        --db-host "${DB_HOST:localhost}"    \
+        --broker-host "${BROKER_HOST:localhost}"
 
     # Setup and configure local computer.
     computer_name=localhost
 
     # Determine the number of physical cores as a default for the number of
     # available MPI ranks on the localhost. We do not count "logical" cores,
     # since MPI parallelization over hyper-threaded cores is typically
```

### Comparing `aiida-core-2.2.2/.github/CODEOWNERS` & `aiida-core-2.3.0/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/ISSUE_TEMPLATE/bug_report.md` & `aiida-core-2.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/ISSUE_TEMPLATE/feature_request.md` & `aiida-core-2.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/config/slurm_rsa` & `aiida-core-2.3.0/.github/config/slurm_rsa`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/system_tests/pytest/test_memory_leaks.py` & `aiida-core-2.3.0/.github/system_tests/pytest/test_memory_leaks.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/system_tests/test_containerized_code.py` & `aiida-core-2.3.0/.github/system_tests/test_containerized_code.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/system_tests/test_daemon.py` & `aiida-core-2.3.0/.github/system_tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/system_tests/test_ipython_magics.py` & `aiida-core-2.3.0/.github/system_tests/test_ipython_magics.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/system_tests/test_polish_workchains.sh` & `aiida-core-2.3.0/.github/system_tests/test_polish_workchains.sh`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/system_tests/test_profile_manager.py` & `aiida-core-2.3.0/.github/system_tests/test_profile_manager.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/system_tests/test_test_manager.py` & `aiida-core-2.3.0/.github/system_tests/test_test_manager.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/system_tests/test_verdi_load_time.sh` & `aiida-core-2.3.0/.github/system_tests/test_verdi_load_time.sh`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/system_tests/workchains.py` & `aiida-core-2.3.0/.github/system_tests/workchains.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/workflows/benchmark-config.json` & `aiida-core-2.3.0/.github/workflows/benchmark-config.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'suites'": "{'pytest-benchmarks:ubuntu-22.04,psql_dos': OrderedDict([('header', 'Performance "*

 * *             "Benchmarks (Ubuntu-22.04)'), ('description', 'Performance benchmark tests, generated "*

 * *             "using pytest-benchmark.')])}"}*

```diff
@@ -34,10 +34,14 @@
         "pytest-benchmarks:ubuntu-18.04,psql_dos": {
             "description": "Performance benchmark tests, generated using pytest-benchmark.",
             "header": "Performance Benchmarks (Ubuntu-18.04)"
         },
         "pytest-benchmarks:ubuntu-18.04,sqlalchemy": {
             "description": "Performance benchmark tests, generated using pytest-benchmark.",
             "header": "Performance Benchmarks (Ubuntu-18.04, SQLAlchemy)"
+        },
+        "pytest-benchmarks:ubuntu-22.04,psql_dos": {
+            "description": "Performance benchmark tests, generated using pytest-benchmark.",
+            "header": "Performance Benchmarks (Ubuntu-22.04)"
         }
     }
 }
```

### Comparing `aiida-core-2.2.2/.github/workflows/benchmark.yml` & `aiida-core-2.3.0/.github/workflows/benchmark.yml`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
     # Only run on pushes and when the job is on the main repository and not on forks
     if: github.repository == 'aiidateam/aiida-core'
 
     strategy:
       fail-fast: false
       matrix:
-        os: [ubuntu-18.04]
-        postgres: ['12.3']
-        rabbitmq: ['3.8.3']
+        os: [ubuntu-22.04]
+        postgres: ['12.14']
+        rabbitmq: ['3.8.14-management']
 
     runs-on: ${{ matrix.os }}
     timeout-minutes: 60
 
     services:
       postgres:
         image: "postgres:${{ matrix.postgres }}"
@@ -38,28 +38,28 @@
           - 5432:5432
       rabbitmq:
         image: "rabbitmq:${{ matrix.rabbitmq }}"
         ports:
           - 5672:5672
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
-        python-version: '3.8'
+        python-version: '3.10'
 
     - name: Upgrade pip
       run: |
         pip install --upgrade pip
         pip --version
 
     - name: Install python dependencies
       run: |
-        pip install -r requirements/requirements-py-3.8.txt
+        pip install -r requirements/requirements-py-3.10.txt
         pip install --no-deps -e .
         pip freeze
 
     - name: Run benchmarks
       run: pytest --benchmark-only --benchmark-json benchmark.json
 
     - name: Store benchmark result
```

### Comparing `aiida-core-2.2.2/.github/workflows/build_and_test_docker_on_pr.yml` & `aiida-core-2.3.0/.github/workflows/build_and_test_docker_on_pr.yml`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/workflows/check_release_tag.py` & `aiida-core-2.3.0/.github/workflows/check_release_tag.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/workflows/ci-code.yml` & `aiida-core-2.3.0/.github/workflows/ci-code.yml`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
           Click [here](https://github.com/aiidateam/aiida-core/wiki/AiiDA-Dependency-Management) for more information on dependency management.
 
   tests:
 
     needs: [check-requirements]
 
     runs-on: ubuntu-latest
-    timeout-minutes: 35
+    timeout-minutes: 45
 
     strategy:
       fail-fast: false
       matrix:
         python-version: ['3.8', '3.11']
 
     services:
```

### Comparing `aiida-core-2.2.2/.github/workflows/ci-style.yml` & `aiida-core-2.3.0/.github/workflows/ci-style.yml`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/workflows/docs-build.yml` & `aiida-core-2.3.0/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/workflows/nightly.yml` & `aiida-core-2.3.0/.github/workflows/nightly.yml`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/workflows/post-release.yml` & `aiida-core-2.3.0/.github/workflows/post-release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,19 @@
     - name: Build pot files
       env:
         READTHEDOCS: 'True'
         RUN_APIDOC: 'True'
       run:
         make -C docs gettext
 
+    - name: Install Transifex CLI
+      run: |
+        curl -o- https://raw.githubusercontent.com/transifex/cli/master/install.sh | bash -s -- v1.6.5
+        mv tx /usr/local/bin/tx
+
     - name: Setting transifex configuration and upload pot files
       env:
         PROJECT_NAME: aiida-core
         USER: ${{ secrets.TRANSIFEX_USER }}
         PASSWD: ${{ secrets.TRANSIFEX_PASSWORD }}
       run: |
         sphinx-intl create-txconfig
```

### Comparing `aiida-core-2.2.2/.github/workflows/push_image_to_dockerhub.yml` & `aiida-core-2.3.0/.github/workflows/push_image_to_dockerhub.yml`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/workflows/rabbitmq.yml` & `aiida-core-2.3.0/.github/workflows/rabbitmq.yml`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/workflows/release.yml` & `aiida-core-2.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/workflows/setup.sh` & `aiida-core-2.3.0/.github/workflows/setup.sh`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/workflows/test-install.yml` & `aiida-core-2.3.0/.github/workflows/test-install.yml`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,17 @@
     runs-on: ubuntu-latest
     timeout-minutes: 5
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Setup Conda
-      uses: s-weigand/setup-conda@v1
+      uses: conda-incubator/setup-miniconda@v2
       with:
-        conda-channels: conda-forge
+        channels: conda-forge
 
     - run: conda --version
 
     - name: Test conda environment
       run: |
         conda env create --dry-run -f environment.yml -n test-environment
 
@@ -152,33 +152,32 @@
           - python-version: ''
             optional: false
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Setup Conda
-      uses: s-weigand/setup-conda@v1
+      uses: conda-incubator/setup-miniconda@v2
       with:
-        conda-channels: conda-forge
-
-    - run: conda update conda
-    - run: conda --version
+        channels: conda-forge
 
     # Use mamba because conda is running out of memory
-    - run: conda install mamba -n base -c conda-forge
-    - run: mamba --version
+    # see https://github.com/conda-incubator/setup-miniconda/issues/274
+    - run: |
+        conda install -n base conda-libmamba-solver
+        conda config --set solver libmamba
 
     # Temporary workaround: https://github.com/mamba-org/mamba/issues/488
     - run: rm /usr/share/miniconda/pkgs/cache/*.json
 
     - name: Test installation
       id: test_installation
       continue-on-error: ${{ matrix.optional }}
       run: >
-        mamba create --dry-run -n test-install aiida-core
+        conda create --dry-run -n test-install aiida-core
         ${{ matrix.python-version && format('python={0}', matrix.python-version) }}
 
     - name: Warn about failure
       if: steps.test_installation.outcome == 'Failure'
       run: >
         echo "::warning ::Failed conda installation for
         Python ${{ matrix.python-version }}."
```

### Comparing `aiida-core-2.2.2/.github/workflows/tests.sh` & `aiida-core-2.3.0/.github/workflows/tests.sh`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/workflows/tests_nightly.sh` & `aiida-core-2.3.0/.github/workflows/tests_nightly.sh`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.github/workflows/verdi.sh` & `aiida-core-2.3.0/.github/workflows/verdi.sh`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.molecule/README.md` & `aiida-core-2.3.0/.molecule/README.md`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.molecule/default/config_local.yml` & `aiida-core-2.3.0/.molecule/default/config_local.yml`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.molecule/default/create_docker.yml` & `aiida-core-2.3.0/.molecule/default/create_docker.yml`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.molecule/default/files/polish/__init__.py` & `aiida-core-2.3.0/.molecule/default/files/polish/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.molecule/default/files/polish/cli.py` & `aiida-core-2.3.0/.molecule/default/files/polish/cli.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.molecule/default/files/polish/lib/__init__.py` & `aiida-core-2.3.0/.molecule/default/files/polish/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.molecule/default/files/polish/lib/expression.py` & `aiida-core-2.3.0/.molecule/default/files/polish/lib/expression.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.molecule/default/files/polish/lib/template/base.tpl` & `aiida-core-2.3.0/.molecule/default/files/polish/lib/template/base.tpl`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.molecule/default/files/polish/lib/template/workchain.tpl` & `aiida-core-2.3.0/.molecule/default/files/polish/lib/template/workchain.tpl`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.molecule/default/files/polish/lib/workchain.py` & `aiida-core-2.3.0/.molecule/default/files/polish/lib/workchain.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.molecule/default/setup_aiida.yml` & `aiida-core-2.3.0/.molecule/default/setup_aiida.yml`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.molecule/default/setup_python.yml` & `aiida-core-2.3.0/.molecule/default/setup_python.yml`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.molecule/default/tasks/log_query_stats.yml` & `aiida-core-2.3.0/.molecule/default/tasks/log_query_stats.yml`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.molecule/default/test_polish_workchains.yml` & `aiida-core-2.3.0/.molecule/default/test_polish_workchains.yml`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/.pre-commit-config.yaml` & `aiida-core-2.3.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     hooks:
     -   id: flynt
         args: [
             '--line-length=120',
             '--fail-on-change',
         ]
 
--   repo: https://github.com/pre-commit/mirrors-yapf
+-   repo: https://github.com/google/yapf
     rev: v0.32.0
     hooks:
     -   id: yapf
         name: yapf
         types: [python]
         exclude: &exclude_files >
             (?x)^(
@@ -106,15 +106,14 @@
                 aiida/common/hashing.py|
                 aiida/common/utils.py|
                 aiida/engine/daemon/execmanager.py|
                 aiida/engine/processes/calcjobs/manager.py|
                 aiida/engine/processes/calcjobs/monitors.py|
                 aiida/engine/processes/calcjobs/tasks.py|
                 aiida/engine/processes/control.py|
-                aiida/engine/processes/functions.py|
                 aiida/engine/processes/ports.py|
                 aiida/manage/configuration/__init__.py|
                 aiida/manage/configuration/config.py|
                 aiida/manage/configuration/profile.py|
                 aiida/manage/configuration/settings.py|
                 aiida/manage/external/rmq/launcher.py|
                 aiida/manage/tests/main.py|
@@ -134,15 +133,14 @@
                 aiida/orm/nodes/process/calculation/calcjob.py|
                 aiida/orm/nodes/process/process.py|
                 aiida/orm/utils/builders/code.py|
                 aiida/orm/utils/builders/computer.py|
                 aiida/orm/utils/calcjob.py|
                 aiida/orm/utils/node.py|
                 aiida/orm/utils/remote.py|
-                aiida/orm/utils/serialize.py|
                 aiida/repository/backend/disk_object_store.py|
                 aiida/repository/backend/sandbox.py|
                 aiida/restapi/common/utils.py|
                 aiida/restapi/resources.py|
                 aiida/restapi/run_api.py|
                 aiida/restapi/translator/base.py|
                 aiida/restapi/translator/computer.py|
@@ -178,15 +176,14 @@
                 aiida/tools/graph/age_entities.py|
                 aiida/tools/graph/age_rules.py|
                 aiida/tools/graph/deletions.py|
                 aiida/tools/graph/graph_traversers.py|
                 aiida/tools/groups/paths.py|
                 aiida/tools/query/calculation.py|
                 aiida/tools/query/mapping.py|
-                aiida/tools/visualization/graph.py|
                 aiida/transports/cli.py|
                 aiida/transports/plugins/local.py|
                 aiida/transports/plugins/ssh.py|
                 aiida/workflows/arithmetic/multiply_add.py|
 
                 tests/conftest.py|
                 tests/repository/conftest.py|
```

### Comparing `aiida-core-2.2.2/.readthedocs.yml` & `aiida-core-2.3.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/AUTHORS.txt` & `aiida-core-2.3.0/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/CHANGELOG.md` & `aiida-core-2.3.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,306 @@
 # Changelog
 
+## v2.3.0 - 2023-04-17
+
+This release comes with a number of improvements, some of the more useful and important of which are quickly highlighted.
+A full list of changes can be found below.
+
+- [Process function improvements](#process-function-improvements)
+- [Scheduler plugins: including `environment_variables`](#scheduler-plugins-including-environment_variables)
+- [`WorkChain`: conditional predicates should return boolean-like](#workchain-conditional-predicates-should-return-boolean-like)
+- [Controlling usage of MPI](#controlling-usage-of-mpi)
+- [Add support for Docker containers](#add-support-for-docker-containers)
+- [Exporting code configurations](#exporting-code-configurations)
+- [Full list of changes](#full-list-of-changes)
+    - [Features](#features)
+    - [Fixes](#fixes)
+    - [Deprecations](#deprecations)
+    - [Changes](#changes)
+    - [Documentation](#documentation)
+    - [DevOps](#devops)
+    - [Dependencies](#dependencies)
+- [New contributors](#new-contributors)
+
+
+### Process function improvements
+A number of improvements in the usage of process functions, i.e., `calcfunction` and `workfunction`, have been added.
+Each subsection title is a link to the documentation for more details.
+
+#### [Variable arguments](https://aiida.readthedocs.io/projects/aiida-core/en/latest/topics/processes/functions.html#variable-and-keyword-arguments)
+Variable arguments can be used in case the function should accept a list of inputs of unknown length.
+Consider the example of a calculation function that computes the average of a number of `Int` nodes:
+```python
+@calcfunction
+def average(*args):
+    return sum(args) / len(args)
+
+result = average(*(1, 2, 3))
+```
+
+#### [Automatic type validation](https://aiida.readthedocs.io/projects/aiida-core/en/latest/topics/processes/functions.html#type-validation)
+Type hint annotations can now be used to add automatic type validation to process functions.
+```python
+@calcfunction
+def add(x: Int, y: Int):
+    return x + y
+
+add(1, 1.0)  # Passes
+add(1, '1.0')  # Raises an exception
+```
+Since the Python base types (`int`, `str`, `bool`, etc.) are automatically serialized, these can also be used in type hints.
+The following example is therefore identical to the previous:
+```python
+@calcfunction
+def add(x: int, y: int):
+    return x + y
+```
+
+#### [Docstring parsing](https://aiida.readthedocs.io/projects/aiida-core/en/latest/topics/processes/functions.html#docstring-parsing)
+The `calcfunction` and `workfunction` generate a `Process` of the decorated function on-the-fly.
+In doing so, it automatically defines the `ProcessSpec` that is normally done manually, such as for a `CalcJob` or a `WorkChain`.
+Before, this would just define the ports that the function process accepts, but the `help` attribute of the port would be left empty.
+This is now parsed from the docstring, if it can be correctly parsed:
+```python
+@calcfunction
+def add(x: int, y: int):
+    """Add two integers.
+
+    :param x: Left hand operand.
+    :param y: Right hand operand.
+    """
+    return x + y
+
+assert add.spec().inputs['a'].help == 'Left hand operand.'
+assert add.spec().inputs['b'].help == 'Right hand operand.'
+```
+This functionality is particularly useful when exposing process functions in work chains.
+Since the process specification of the exposed function will be automatically inherited, the user can inspect the `help` string through the builder.
+The automatic documentation produced by the Sphinx plugin will now also display the help string parsed from the docstring.
+
+#### [Nested labels for output nodes](https://aiida.readthedocs.io/projects/aiida-core/en/latest/topics/processes/functions.html#return-values)
+The keys in the output dictionary can now contain nested namespaces:
+```python
+@calcfunction
+def add(alpha, beta):
+    return {'nested.sum': alpha + beta}
+
+result = add(Int(1), Int(2))
+assert result['nested']['sum'] == 3
+```
+
+#### [As class member methods](https://aiida.readthedocs.io/projects/aiida-core/en/latest/topics/processes/functions.html#as-class-member-methods)
+Process functions can now be defined as class member methods of work chains:
+```python
+class CalcFunctionWorkChain(WorkChain):
+
+    @classmethod
+    def define(cls, spec):
+        super().define(spec)
+        spec.input('x')
+        spec.input('y')
+        spec.output('sum')
+        spec.outline(
+            cls.run_compute_sum,
+        )
+
+    @staticmethod
+    @calcfunction
+    def compute_sum(x, y):
+        return x + y
+
+    def run_compute_sum(self):
+        self.out('sum', self.compute_sum(self.inputs.x, self.inputs.y))
+```
+The function should be declared as a `staticmethod` and it should not include the `self` argument in its function signature.
+It can then be called from within the work chain as `self.function_name(*args, **kwargs)`.
+
+
+### Scheduler plugins: including `environment_variables`
+The `Scheduler` base class implements the concrete method `_get_submit_script_environment_variables` which formats the lines for the submission script that set the environment variables that were defined in the `metadata.options.environment_variables` input.
+Before it was left up to the plugins to actually call this method in the `_get_submit_script_header`, but this is now done by the base class in the `get_submit_script`.
+You can now remove the call to `_get_submit_script_environment_variables` from your scheduler plugins, as the base class will take care of it.
+A deprecation warning is emitted if the base class detects that the plugin is still calling it manually.
+See the [pull request](https://github.com/aiidateam/aiida-core/pull/5948) for more details.
+
+### `WorkChain`: conditional predicates should return boolean-like
+Up till now, work chain methods that are used as the predicate in a conditional, e.g., `if_` or `while_` could return any type.
+For example:
+
+```python
+class SomeWorkChain(WorkChain):
+
+    @classmethod
+    def define(cls, spec):
+        super().define(spec)
+        spec.outline(if_(cls.some_conditional)())
+
+    def some_conditional(self):
+        if self.ctx.something == 'something':
+            return True
+```
+The `some_conditional` method is used as the "predicate" of the `if_` conditional.
+It returns `True` or `None`.
+Since the `None` value in Python is "falsey", it would be considered as returning `False`.
+However, this duck-typing could accidentally lead to unexpected situations, so we decided to be more strict on the return type.
+As of now, a deprecation warning is emitted if the method returns anything that is not "boolean-like", i.e., does not implement the `__bool__` method.
+If you see this warning, please make sure to return a boolean, like the built-ins `True` or `False`, or a `numpy.bool` or `aiida.orm.Bool`.
+See the [pull request](https://github.com/aiidateam/aiida-core/pull/5924) for more details.
+
+### Controlling usage of MPI
+It is now possible to define on a code object whether it should be run with or without MPI through the `with_mpi` attribute.
+It can be set from the Python API as `AbstractCode(with_mpi=with_mpi)` or through the `--with-mpi / --no-with-mpi` option of the `verdi code create` CLI command.
+This option adds a manner to control the use of MPI in calculation jobs, in addition to the existing ones defined by the `CalcJob` plugin and the `metadata.options.withmpi` input.
+For more details on how these are controlled and how conflicts are handled, please refer to [the documentation](https://aiida.readthedocs.io/projects/aiida-core/en/latest/topics/calculations/usage.html#controlling-mpi).
+
+### Add support for Docker containers
+Support is added for running calculation within Docker containers.
+For example, to run Quantum ESPRESSO pw.x in a Docker container, write the following file to `config.yml`:
+```yaml
+label: qe-pw-on-docker
+computer: localhost
+engine_command: docker run -i -v $PWD:/workdir:rw -w /workdir {image_name} sh -c
+image_name: haya4kun/quantum_espresso
+filepath_executable: pw.x
+default_calc_job_plugin: quantumespresso.pw
+use_double_quotes: false
+wrap_cmdline_params: true
+```
+and run the CLI command:
+```
+verdi code create core.code.containerized --config config.yml --non-interactive
+```
+This should create a `ContainerizedCode` that you can now use to launch a `PwCalculation`.
+For more details, please refer to [the documentation](https://aiida.readthedocs.io/projects/aiida-core/en/latest/topics/data_types.html#supported-container-technologies).
+
+### Exporting code configurations
+It is now possible to export the configuration of an existing code through the `verdi code export` command.
+The produced YAML file can be used to recreate the code through the `verdi code create` command.
+Note that you should use the correct subcommand based on the type of the original code.
+For example, if it was an `InstalledCode` you should use `verdi code create core.code.installed`.
+For the legacy `Code` instances, you should use `verdi code setup`.
+See the [pull request](https://github.com/aiidateam/aiida-core/pull/5860) for more details.
+
+### Full list of changes
+
+#### Features
+- `AbstractCode`: Add the `with_mpi` attribute [[#5922]](https://github.com/aiidateam/aiida-core/pull/5922)
+- `ContainerizedCode`: Add support for Docker images to use as `Code` for `CalcJob`s [[#5841]](https://github.com/aiidateam/aiida-core/pull/5841)
+- `InstalledCode`: Allow relative path for `filepath_executable` [[#5879]](https://github.com/aiidateam/aiida-core/pull/5879)
+- CLI: Allow specifying output filename in `verdi node graph generate` [[#5897]](https://github.com/aiidateam/aiida-core/pull/5897)
+- CLI: Add `--timeout` option to all `verdi daemon` commands [[#5966]](https://github.com/aiidateam/aiida-core/pull/5966)
+- CLI: Add the `verdi calcjob remotecat` command [[#4861]](https://github.com/aiidateam/aiida-core/pull/4861)
+- CLI: Add the `verdi code export` command [[#5860]](https://github.com/aiidateam/aiida-core/pull/5860)
+- CLI: Improved customizability and scriptability of `verdi storage maintain` [[#5936]](https://github.com/aiidateam/aiida-core/pull/5936)
+- CLI: `verdi quicksetup`: Further reduce required user interaction [[#5768]](https://github.com/aiidateam/aiida-core/pull/5768)
+- CLI: `verdi computer test`: Add test for login shell being slow [[#5845]](https://github.com/aiidateam/aiida-core/pull/5845)
+- CLI: `verdi process list`: Add `exit_message` as projectable attribute [[#5853]](https://github.com/aiidateam/aiida-core/pull/5853)
+- CLI: `verdi node delete`: Add verbose list of pks to be deleted [[#5878]](https://github.com/aiidateam/aiida-core/pull/5878)
+- CLI: Fail command if `--config` file contains unknown key [[#5939]](https://github.com/aiidateam/aiida-core/pull/5939)
+- CLI: `verdi daemon status`: Do not except when no profiles are defined [[#5874]](https://github.com/aiidateam/aiida-core/pull/5874)
+- ORM: Add unary operations `+`, `-` and `abs` to `NumericType` [[#5946]](https://github.com/aiidateam/aiida-core/pull/5946)
+- Process functions: Support class member functions as process functions [[#4963]](https://github.com/aiidateam/aiida-core/pull/4963)
+- Process functions: Infer argument `valid_type` from type hints [[#5900]](https://github.com/aiidateam/aiida-core/pull/5900)
+- Process functions: Parse docstring to set input port help attribute [[#5919]](https://github.com/aiidateam/aiida-core/pull/5919)
+- Process functions: Add support for variadic arguments [[#5691]](https://github.com/aiidateam/aiida-core/pull/5691)
+- Process functions: Allow nested output namespaces [[#5954]](https://github.com/aiidateam/aiida-core/pull/5954)
+- `Process`: Store JSON-serializable metadata inputs on the node [[#5801]](https://github.com/aiidateam/aiida-core/pull/5801)
+- `Port`: Add the `is_metadata` keyword [[#5801]](https://github.com/aiidateam/aiida-core/pull/5801)
+- `ProcessBuilder`: Include metadata inputs in `get_builder_restart` [[#5801]](https://github.com/aiidateam/aiida-core/pull/5801)
+- `StructureData`: Add `mode` argument to `get_composition` [[#5926]](https://github.com/aiidateam/aiida-core/pull/5926)
+- `Scheduler`: Allow terminating job if submission script is invalid [[#5849]](https://github.com/aiidateam/aiida-core/pull/5849)
+- `SlurmScheduler`: Detect broken submission scripts for invalid account [[#5850]](https://github.com/aiidateam/aiida-core/pull/5850)
+- `SlurmScheduler`: Parse the `NODE_FAIL` state [[#5866]](https://github.com/aiidateam/aiida-core/pull/5866)
+- `WorkChain`: Add dataclass serialisation to context [[#5833]](https://github.com/aiidateam/aiida-core/pull/5833)
+- `IcsdDbImporter`: Add `is_theoretical` tag to queried entries [[#5868]](https://github.com/aiidateam/aiida-core/pull/5868)
+
+#### Fixes
+- CLI: Prefix the `verdi data` subcommands with `core.` [[#5846]](https://github.com/aiidateam/aiida-core/pull/5846)
+- CLI: Respect config log levels if `--verbosity` not explicitly passed [[#5925]](https://github.com/aiidateam/aiida-core/pull/5925)
+- CLI: `verdi config list`: Do not except if no profiles are defined [[#5921]](https://github.com/aiidateam/aiida-core/pull/5921)
+- CLI: `verdi code show`: Add missing code attributes [[#5916]](https://github.com/aiidateam/aiida-core/pull/5916)
+- CLI: `verdi quicksetup`: Fix error incorrect role when creating database [[#5828]](https://github.com/aiidateam/aiida-core/pull/5828)
+- CLI: Fix error in `aiida.cmdline.utils.log.CliFormatter` [[#5957]](https://github.com/aiidateam/aiida-core/pull/5957)
+- Daemon: Fix false-positive of stopped daemon in `verdi daemon status` [[#5862]](https://github.com/aiidateam/aiida-core/pull/5862)
+- `DaemonClient`: Fix and homogenize use of `timeout` in client calls [[#5960]](https://github.com/aiidateam/aiida-core/pull/5960)
+- `ProcessBuilder`: Fix bug in `_recursive_merge` [[#5801]](https://github.com/aiidateam/aiida-core/pull/5801)
+- `QueryBuilder`: Catch new exception raised by `sqlalchemy>=1.4.45` [[#5875]](https://github.com/aiidateam/aiida-core/pull/5875)
+- Fix the `%verdi` IPython magics utility [[#5961]](https://github.com/aiidateam/aiida-core/pull/5961)
+- Fix bug in `aiida.engine.utils.instantiate_process` [[#5952]](https://github.com/aiidateam/aiida-core/pull/5952)
+- Fix incorrect import of exception from `kiwipy.communications` [[#5947]](https://github.com/aiidateam/aiida-core/pull/5947)
+
+#### Deprecations
+- `Scheduler`: Move setting of environment variables into base class [[#5948]](https://github.com/aiidateam/aiida-core/pull/5948)
+- `WorkChains`: Emit deprecation warning if predicate `if_/while_` does not return boolean-like [[#5924]](https://github.com/aiidateam/aiida-core/pull/5924)
+
+#### Changes
+- `DaemonClient`: Refactor to include parsing of client response [[#5850]](https://github.com/aiidateam/aiida-core/pull/5850)
+- ORM: Remove `Entity.from_backend_entity` from the public API [[#5447]](https://github.com/aiidateam/aiida-core/pull/5447)
+- `PbsproScheduler`: Replace deprecated `ppn` tag with `ncpus` [[#5910]](https://github.com/aiidateam/aiida-core/pull/5910)
+- `ProcessBuilder`: Move `_prune` method to standalone utility [[#5801]](https://github.com/aiidateam/aiida-core/pull/5801)
+- `verdi process list`: Simplify the daemon load implementation [[#5850]](https://github.com/aiidateam/aiida-core/pull/5850)
+
+#### Documentation
+- Add FAQ on MFA-enabled computers [[#5887]](https://github.com/aiidateam/aiida-core/pull/5887)
+- Add link to all `metadata.options` inputs in `CalcJob` submission example [[#5912]](https://github.com/aiidateam/aiida-core/pull/5912)
+- Add warning that `Data` constructor is not called on loading [[#5898]](https://github.com/aiidateam/aiida-core/pull/5898)
+- Add note on how to create a code that uses Conda environment [[#5905]](https://github.com/aiidateam/aiida-core/pull/5905)
+- Add `--without-daemon` flag to benchmark script [[#5839]](https://github.com/aiidateam/aiida-core/pull/5839)
+- Add alternative for conda env activation in submission script [[#5950]](https://github.com/aiidateam/aiida-core/pull/5950)
+- Clarify that process functions can be exposed in work chains [[#5919]](https://github.com/aiidateam/aiida-core/pull/5919)
+- Fix the `intro/tutorial.md` notebook [[#5961]](https://github.com/aiidateam/aiida-core/pull/5961)
+- Fix the overindentation of lists [[#5915]](https://github.com/aiidateam/aiida-core/pull/5915)
+- Hide the "Edit this page" button on the API reference pages [[#5956]](https://github.com/aiidateam/aiida-core/pull/5956)
+- Note that an entry point is required for using a data plugin [[#5907]](https://github.com/aiidateam/aiida-core/pull/5907)
+- Set `use_login_shell=False` for `localhost` in performance benchmark [[#5847]](https://github.com/aiidateam/aiida-core/pull/5847)
+- Small improvements to the benchmark script [[#5854]](https://github.com/aiidateam/aiida-core/pull/5854)
+- Use mamba instead of conda [[#5891]](https://github.com/aiidateam/aiida-core/pull/5891)
+
+#### DevOps
+- Add devcontainer for easy integration with VSCode [[#5913]](https://github.com/aiidateam/aiida-core/pull/5913)
+- CI: Update `sphinx-intl` and install transifex CLI [[#5908]](https://github.com/aiidateam/aiida-core/pull/5908)
+- Fix the `test-install` workflow [[#5873]](https://github.com/aiidateam/aiida-core/pull/5873)
+- Pre-commit: Improve typing of `aiida.schedulers.scheduler` [[#5849]](https://github.com/aiidateam/aiida-core/pull/5849)
+- Pre-commit: Set `yapf` option `allow_split_before_dict_value = false`[[#5931]](https://github.com/aiidateam/aiida-core/pull/5931)
+- Process functions: Replace `getfullargspec` with `signature` [[#5900]](https://github.com/aiidateam/aiida-core/pull/5900)
+- Fixtures: Add argument `use_subprocess` to `run_cli_command` [[#5846]](https://github.com/aiidateam/aiida-core/pull/5846)
+- Fixtures: Change default `use_subprocess=False` for `run_cli_command` [[#5846]](https://github.com/aiidateam/aiida-core/pull/5846)
+- Tests: Use `use_subprocess=False` and `suppress_warnings=True` [[#5846]](https://github.com/aiidateam/aiida-core/pull/5846)
+- Tests: Fix bugs revealed by running with `use_subprocess=True` [[#5846]](https://github.com/aiidateam/aiida-core/pull/5846)
+- Typing: Annotate `aiida/orm/utils/serialize.py` [[#5832]](https://github.com/aiidateam/aiida-core/pull/5832)
+- Typing: Annotate `aiida/tools/visualization/graph.py` [[#5821]](https://github.com/aiidateam/aiida-core/pull/5821)
+- Typing: Use modern syntax for `aiida.engine.processes.functions` [[#5900]](https://github.com/aiidateam/aiida-core/pull/5900)
+
+#### Dependencies
+- Add compatibility for `ipython~=8.0` [[#5888]](https://github.com/aiidateam/aiida-core/pull/5888)
+- Bump cryptography from 36.0.0 to 39.0.1 [[#5885]](https://github.com/aiidateam/aiida-core/pull/5885)
+- Remove upper limit on `werkzeug` [[#5904]](https://github.com/aiidateam/aiida-core/pull/5904)
+- Update pre-commit requirement `isort==5.12.0` [[#5877]](https://github.com/aiidateam/aiida-core/pull/5877)
+- Update requirement `importlib-metadata~=4.13` [[#5963]](https://github.com/aiidateam/aiida-core/pull/5963)
+- Bump `graphviz` version to `0.19` [[#5965]](https://github.com/aiidateam/aiida-core/pull/5965)
+
+### New contributors
+Thanks a lot to the following new contributors:
+
+- [Ahmed Basem](https://github.com/AhmedBasem20)
+- [Mahhheshh](https://github.com/Mahhheshh)
+- [Kyle Wang](https://github.com/TurboKyle)
+- [Kartikey Saran](https://github.com/kartikeysaran)
+- [zahid47](https://github.com/zahid47)
+
 ## v2.2.2 - 2023-02-10
 
 ### Fixes
-- Critical bug fix: Fix bug causing `CalcJob`s to except after restarting daemon [#5886]](https://github.com/aiidateam/aiida-core/pull/5886)
+- Critical bug fix: Fix bug causing `CalcJob`s to except after restarting daemon [[#5886]](https://github.com/aiidateam/aiida-core/pull/5886)
 
 
 ## v2.2.1 - 2022-12-22
 
 ### Fixes
-- Critical bug fix: Revert the changes of PR [#5804](https://github.com/aiidateam/aiida-core/pull/5804) released with v2.2.0, which addressed a bug when mutating nodes during `QueryBuilder.iterall`. Unfortunately, the change caused changes performed by `verdi` commands (as well as changes made in `verdi shell`) to not be persisted to the database. [[#5851]](https://github.com/aiidateam/aiida-core/pull/5851)
+- Critical bug fix: Revert the changes of PR [[#5804]](https://github.com/aiidateam/aiida-core/pull/5804) released with v2.2.0, which addressed a bug when mutating nodes during `QueryBuilder.iterall`. Unfortunately, the change caused changes performed by `verdi` commands (as well as changes made in `verdi shell`) to not be persisted to the database. [[#5851]](https://github.com/aiidateam/aiida-core/pull/5851)
 
 
 ## v2.2.0 - 2022-12-13
 
 This feature release comes with a significant feature and a number of improvements and fixes.
 
 ### Live calculation job monitoring
```

### Comparing `aiida-core-2.2.2/CODE_OF_CONDUCT.md` & `aiida-core-2.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/Dockerfile` & `aiida-core-2.3.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/LICENSE.txt` & `aiida-core-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/README.md` & `aiida-core-2.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# <img src="http://www.aiida.net/wp-content/uploads/2020/06/logo_aiida.png" alt="AiiDA" width="200"/>
+# <img src="https://raw.githubusercontent.com/aiidateam/aiida-core/main/docs/source/images/aiida-logo.svg" alt="AiiDA" width="200"/>
 
 AiiDA (www.aiida.net) is a workflow manager for computational science with a strong focus on provenance, performance and extensibility.
 
 |    | |
 |-----|----------------------------------------------------------------------------|
 |Latest release| [![PyPI version](https://badge.fury.io/py/aiida-core.svg)](https://badge.fury.io/py/aiida-core) [![conda-forge](https://img.shields.io/conda/vn/conda-forge/aiida-core.svg?style=flat)](https://anaconda.org/conda-forge/aiida-core) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-core.svg)](https://pypi.python.org/pypi/aiida-core/) |
 |Getting help| [![Docs status](https://readthedocs.org/projects/aiida-core/badge)](http://aiida-core.readthedocs.io/) [![Google Group](https://img.shields.io/badge/-Google%20Group-lightgrey.svg)](https://groups.google.com/forum/#!forum/aiidausers)
-|Build status| [![Build Status](https://github.com/aiidateam/aiida-core/workflows/aiida-core/badge.svg)](https://github.com/aiidateam/aiida-core/actions) [![Coverage Status](https://codecov.io/gh/aiidateam/aiida-core/branch/main/graph/badge.svg)](https://codecov.io/gh/aiidateam/aiida-core) |
+|Build status| [![Build Status](https://github.com/aiidateam/aiida-core/actions/workflows/ci-code.yml/badge.svg)](https://github.com/aiidateam/aiida-core/actions) [![Coverage Status](https://codecov.io/gh/aiidateam/aiida-core/branch/main/graph/badge.svg)](https://codecov.io/gh/aiidateam/aiida-core) [Benchmarks](https://aiidateam.github.io/aiida-core/dev/bench/ubuntu-22.04/psql_dos/) |
 |Activity| [![PyPI-downloads](https://img.shields.io/pypi/dm/aiida-core.svg?style=flat)](https://pypistats.org/packages/aiida-core) [![Commit Activity](https://img.shields.io/github/commit-activity/m/aiidateam/aiida-core.svg)](https://github.com/aiidateam/aiida-core/pulse)
 |Community| [![Affiliated with NumFOCUS](https://img.shields.io/badge/NumFOCUS-affiliated%20project-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org/sponsored-projects/affiliated-projects) [![Twitter](https://img.shields.io/twitter/follow/aiidateam.svg?style=social&label=Follow)](https://twitter.com/aiidateam)
 
 
 ## Features
 
  -   **Workflows:** Write complex, auto-documenting workflows in
```

### Comparing `aiida-core-2.2.2/aiida/__init__.py` & `aiida-core-2.3.0/aiida/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from aiida.manage.configuration import get_config_option, get_profile, load_profile, profile_context
 
 __copyright__ = (
     'Copyright (c), This file is part of the AiiDA platform. '
     'For further information please visit http://www.aiida.net/. All rights reserved.'
 )
 __license__ = 'MIT license, see LICENSE.txt file.'
-__version__ = '2.2.2'
+__version__ = '2.3.0'
 __authors__ = 'The AiiDA team.'
 __paper__ = (
     'S. P. Huber et al., "AiiDA 1.0, a scalable computational infrastructure for automated reproducible workflows and '
     'data provenance", Scientific Data 7, 300 (2020); https://doi.org/10.1038/s41597-020-00638-4'
 )
 __paper_short__ = 'S. P. Huber et al., Scientific Data 7, 300 (2020).'
```

### Comparing `aiida-core-2.2.2/aiida/__main__.py` & `aiida-core-2.3.0/aiida/__main__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/calculations/__init__.py` & `aiida-core-2.3.0/aiida/calculations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/calculations/arithmetic/__init__.py` & `aiida-core-2.3.0/aiida/calculations/arithmetic/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/calculations/arithmetic/add.py` & `aiida-core-2.3.0/aiida/calculations/arithmetic/add.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/calculations/diff_tutorial/calculations.py` & `aiida-core-2.3.0/aiida/calculations/diff_tutorial/calculations.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/calculations/importers/arithmetic/add.py` & `aiida-core-2.3.0/aiida/calculations/importers/arithmetic/add.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/calculations/monitors/base.py` & `aiida-core-2.3.0/aiida/calculations/monitors/base.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/calculations/templatereplacer.py` & `aiida-core-2.3.0/aiida/calculations/templatereplacer.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/calculations/transfer.py` & `aiida-core-2.3.0/aiida/calculations/transfer.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/__init__.py` & `aiida-core-2.3.0/aiida/cmdline/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/__init__.py` & `aiida-core-2.3.0/aiida/cmdline/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_archive.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_archive.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_calcjob.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_calcjob.py`

 * *Files 12% similar despite different names*

```diff
@@ -117,14 +117,39 @@
         # The sepcial case is breakon pipe error, which is usually OK.
         # It can happen if the output is redirected, for example, to `head`.
         if exception.errno != errno.EPIPE:
             # Incorrect path or file not readable
             echo.echo_critical(f'Could not open output path "{path}". Exception: {exception}')
 
 
+@verdi_calcjob.command('remotecat')
+@arguments.CALCULATION('calcjob', type=CalculationParamType(sub_classes=('aiida.node:process.calculation.calcjob',)))
+@click.argument('path', type=str, required=False)
+@decorators.with_dbenv()
+def calcjob_remotecat(calcjob, path):
+    """Show the contents of a file in the remote working directory.
+
+    The file to show can be specified using the PATH argument. If PATH is not specified, the default output file path
+    as defined by the `CalcJob` plugin class will be used instead.
+    """
+    import shutil
+    import sys
+    import tempfile
+
+    remote_folder, path = get_remote_and_path(calcjob, path)
+
+    with tempfile.NamedTemporaryFile() as tmp_path:
+        try:
+            remote_folder.getfile(path, tmp_path.name)
+            with open(tmp_path.name, 'rb') as handle:
+                shutil.copyfileobj(handle, sys.stdout.buffer)
+        except IOError as exception:
+            echo.echo_critical(str(exception))
+
+
 @verdi_calcjob.command('outputcat')
 @arguments.CALCULATION('calcjob', type=CalculationParamType(sub_classes=('aiida.node:process.calculation.calcjob',)))
 @click.argument('path', type=click.STRING, required=False)
 @decorators.with_dbenv()
 def calcjob_outputcat(calcjob, path):
     """
     Show the contents of one of the calcjob retrieved outputs.
@@ -275,7 +300,60 @@
 
         with transport:
             for remote_folder in paths:
                 remote_folder._clean(transport=transport)  # pylint:disable=protected-access
                 counter += 1
 
         echo.echo_success(f'{counter} remote folders cleaned on {computer.label}')
+
+
+def get_remote_and_path(calcjob, path=None):
+    """Return the remote folder output node and process the path argument.
+
+    :param calcjob: The ``CalcJobNode`` whose remote_folder to be returned.
+    :param path: The relative path of file. If not defined, it is attempted to determine the default output file from
+        the node options or otherwise from the associated process class. If neither are defined, a ``ValueError`` is
+        raised.
+    :returns: A tuple of the ``RemoteData`` and the path of the output file to be used.
+    :raises ValueError: If path is not defined and no default output file is defined on the node nor its associated
+        process class.
+    """
+    remote_folder_linkname = 'remote_folder'  # The `remote_folder` is the standard output of a calculation.
+
+    try:
+        remote_folder = getattr(calcjob.outputs, remote_folder_linkname)
+    except AttributeError:
+        echo.echo_critical(
+            f'`CalcJobNode<{calcjob.pk}>` has no `{remote_folder_linkname}` output. '
+            'It probably has not started running yet.'
+        )
+
+    if path is not None:
+        return remote_folder, path
+
+    # Try to get the default output filename from the node
+    path = calcjob.get_option('output_filename')
+
+    if path is not None:
+        return remote_folder, path
+
+    try:
+        process_class = calcjob.process_class
+    except ValueError as exception:
+        raise ValueError(
+            f'The process class of `CalcJobNode<{calcjob.pk}>` cannot be loaded and so the default output filename '
+            'cannot be determined.\nPlease specify a path explicitly.'
+        ) from exception
+
+    # Try to get the default output filename from the node's associated process class spec
+    port = process_class.spec_options.get('output_filename')
+    if port and port.has_default():
+        path = port.default
+
+    if path is not None:
+        return remote_folder, path
+
+    raise ValueError(
+        f'`CalcJobNode<{calcjob.pk}>` does not define a default output file (option "output_filename" not found) '
+        f'nor does its associated process class `{calcjob.process_class.__class__.__name__}`\n'
+        'Please specify a path explicitly.'
+    )
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_code.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_code.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ###########################################################################
 """`verdi code` command."""
 from collections import defaultdict
 from functools import partial
 
 import click
 import tabulate
+import yaml
 
 from aiida.cmdline.commands.cmd_verdi import verdi
 from aiida.cmdline.groups.dynamic import DynamicEntryPointCommandGroup
 from aiida.cmdline.params import arguments, options, types
 from aiida.cmdline.params.options.commands import code as options_code
 from aiida.cmdline.utils import echo
 from aiida.cmdline.utils.decorators import deprecated_command, with_dbenv
@@ -219,27 +220,50 @@
 def show(code):
     """Display detailed information for a code."""
     from aiida.cmdline import is_verbose
 
     table = []
     table.append(['PK', code.pk])
     table.append(['UUID', code.uuid])
-    table.append(['Label', code.label])
-    table.append(['Description', code.description])
-    table.append(['Default plugin', code.default_calc_job_plugin])
-    table.append(['Prepend text', code.prepend_text])
-    table.append(['Append text', code.append_text])
-
+    table.append(['Type', code.entry_point.name])
+    for key in code.get_cli_options().keys():
+        try:
+            table.append([key.capitalize().replace('_', ' '), getattr(code, key)])
+        except AttributeError:
+            continue
     if is_verbose():
         table.append(['Calculations', len(code.base.links.get_outgoing().all())])
 
     echo.echo(tabulate.tabulate(table))
 
 
 @verdi_code.command()
+@arguments.CODE()
+@arguments.OUTPUT_FILE(type=click.Path(exists=False))
+@with_dbenv()
+def export(code, output_file):
+    """Export code to a yaml file."""
+    code_data = {}
+
+    for key in code.get_cli_options().keys():
+        if key == 'computer':
+            value = getattr(code, key).label
+        else:
+            value = getattr(code, key)
+
+        # If the attribute is not set, for example ``with_mpi`` do not export it, because the YAML won't be valid for
+        # use in ``verdi code create`` since ``None`` is not a valid value on the CLI.
+        if value is not None:
+            code_data[key] = str(value)
+
+    with open(output_file, 'w', encoding='utf-8') as yfhandle:
+        yaml.dump(code_data, yfhandle)
+
+
+@verdi_code.command()
 @arguments.CODES()
 @options.DRY_RUN()
 @options.FORCE()
 @with_dbenv()
 def delete(codes, dry_run, force):
     """Delete a code.
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_computer.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_computer.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 # pylint: disable=invalid-name,too-many-statements,too-many-branches
 """`verdi computer` command."""
+from copy import deepcopy
 from functools import partial
 
 import click
 import tabulate
 
 from aiida.cmdline.commands.cmd_verdi import VerdiCommandGroup, verdi
 from aiida.cmdline.params import arguments, options
@@ -157,14 +158,79 @@
         os.remove(destfile)
 
     transport.remove(remote_file_path)
 
     return True, None
 
 
+def time_use_login_shell(authinfo, auth_params, use_login_shell: bool, iterations: int = 3) -> float:
+    """Execute the ``whoami`` over the transport for the given ``use_login_shell`` and report the time taken.
+
+    :param authinfo: The ``AuthInfo`` instance to use.
+    :param auth_params: The base authentication parameters.
+    :param use_login_shell: Whether to use a login shell or not.
+    :param iterations: The number of iterations of the command to call. Command will return the average call time.
+    :return: The average call time of the ``Transport.whoami`` command.
+    """
+    import time
+
+    auth_params['use_login_shell'] = use_login_shell
+    authinfo.set_auth_params(auth_params)
+
+    timings = []
+
+    for _ in range(iterations):
+        time_start = time.time()
+        with authinfo.get_transport() as transport:
+            transport.whoami()
+        timings.append(time.time() - time_start)
+
+    return sum(timings) / iterations
+
+
+def _computer_use_login_shell_performance(transport, scheduler, authinfo):  # pylint: disable=unused-argument
+    """Execute a command over the transport with and without the ``use_login_shell`` option enabled.
+
+    By default, AiiDA uses a login shell when connecting to a computer in order to operate in the same environment as a
+    user connecting to the computer. However, loading the login scripts of the shell can take time, which can
+    significantly slow down all commands executed by AiiDA and impact the throughput of calculation jobs. This test
+    executes a simple command both with and without using a login shell and emits a warning if the login shell is slower
+    by at least 100 ms. If the computer is already configured to avoid using a login shell, the test is skipped and the
+    function returns a successful test result.
+    """
+    tolerance = 0.1  # 100 ms
+    iterations = 3
+
+    auth_params = authinfo.get_auth_params()
+
+    # If ``use_login_shell=False`` we don't need to test for it being slower.
+    if not auth_params.get('use_login_shell', True):
+        return True, None
+
+    auth_params_clone = deepcopy(auth_params)
+
+    try:
+        timing_false = time_use_login_shell(authinfo, auth_params_clone, False, iterations)
+        timing_true = time_use_login_shell(authinfo, auth_params_clone, True, iterations)
+    finally:
+        authinfo.set_auth_params(auth_params)
+
+    echo.echo_debug(f'Execution time: {timing_true} vs {timing_false} for login shell and normal, respectively')
+
+    if timing_true - timing_false > tolerance:
+        message = (
+            'computer is configured to use a login shell, which is slower compared to a normal shell (Command execution'
+            f' time of {timing_true} s versus {timing_false}, respectively).\nUnless this setting is really necessary, '
+            'consider disabling it with: verdi computer configure core.local COMPUTER_NAME -n --no-use-login-shell'
+        )
+        return False, message
+
+    return True, None
+
+
 def get_parameter_default(parameter, ctx):
     """
     Get the value for a specific parameter from the computer_builder or the default value of that option
 
     :param parameter: parameter name
     :param ctx: click context of the command
     :return: parameter default value, or None
@@ -462,15 +528,16 @@
     num_failures = 0
     num_tests = 0
 
     tests = {
         _computer_test_no_unexpected_output: 'Checking for spurious output',
         _computer_test_get_jobs: 'Getting number of jobs from scheduler',
         _computer_get_remote_username: 'Determining remote user name',
-        _computer_create_temp_file: 'Creating and deleting temporary file'
+        _computer_create_temp_file: 'Creating and deleting temporary file',
+        _computer_use_login_shell_performance: 'Checking for possible delay from using login shell',
     }
 
     try:
         echo.echo('* Opening connection... ', nl=False)
 
         with transport:
             num_tests += 1
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_config.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     Optionally filtered by a prefix.
     """
     from tabulate import tabulate
 
     from aiida.manage.configuration import Config, Profile
 
     config: Config = ctx.obj.config
-    profile: Profile = ctx.obj.profile
+    profile: Profile = ctx.obj.get('profile', None)
 
     if not profile:
         echo.echo_warning('no profiles configured: run `verdi setup` to create one')
 
     option_values = config.get_options(profile.name if profile else None)
 
     def _join(val):
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_daemon.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_daemon.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 """`verdi daemon` commands."""
+from __future__ import annotations
+
 import subprocess
 import sys
-import time
+import typing as t
 
 import click
-from click_spinner import spinner
 
 from aiida.cmdline.commands.cmd_verdi import verdi
+from aiida.cmdline.params import options
 from aiida.cmdline.utils import decorators, echo
-from aiida.cmdline.utils.daemon import delete_stale_pid_file, get_daemon_status, print_client_response_status
-from aiida.manage import get_manager
 
 
 def validate_daemon_workers(ctx, param, value):  # pylint: disable=unused-argument,invalid-name
     """Validate the value for the number of daemon workers to start with default set by config."""
     if value is None:
         value = ctx.obj.config.get_option('daemon.default_workers', ctx.obj.profile.name)
 
@@ -36,110 +36,147 @@
 
 
 @verdi.group('daemon')
 def verdi_daemon():
     """Inspect and manage the daemon."""
 
 
+def execute_client_command(command: str, daemon_not_running_ok: bool = False, **kwargs) -> dict[str, t.Any] | None:
+    """Execute a command of the :class:`aiida.engine.daemon.client.DaemonClient` and echo whether it failed or not.
+
+    :param command: The name of hte method.
+    :param daemon_not_running_ok: If ``True``, the command raising an exception because the daemon was not running is
+        not treated as a failure.
+    :param kwargs: Keyword arguments that are passed to the client method.
+    """
+    from aiida.engine.daemon.client import DaemonException, DaemonNotRunningException, get_daemon_client
+
+    client = get_daemon_client()
+
+    try:
+        response = getattr(client, command)(**kwargs)
+    except DaemonNotRunningException as exception:
+        if daemon_not_running_ok:
+            echo.echo('OK', fg=echo.COLORS['success'], bold=True)
+        else:
+            echo.echo('FAILED', fg=echo.COLORS['error'], bold=True)
+            echo.echo_critical(str(exception))
+    except DaemonException as exception:
+        echo.echo('FAILED', fg=echo.COLORS['error'], bold=True)
+        echo.echo_critical(str(exception))
+    else:
+        echo.echo('OK', fg=echo.COLORS['success'], bold=True)
+        return response
+
+    return None
+
+
 @verdi_daemon.command()
 @click.option('--foreground', is_flag=True, help='Run in foreground.')
 @click.argument('number', required=False, type=int, callback=validate_daemon_workers)
+@options.TIMEOUT(default=None, required=False, type=int)
 @decorators.with_dbenv()
 @decorators.check_circus_zmq_version
-def start(foreground, number):
+def start(foreground, number, timeout):
     """Start the daemon with NUMBER workers.
 
     If the NUMBER of desired workers is not specified, the default is used, which is determined by the configuration
     option `daemon.default_workers`, which if not explicitly changed defaults to 1.
 
     Returns exit code 0 if the daemon is OK, non-zero if there was an error.
     """
-    from aiida.engine.daemon.client import DaemonException, get_daemon_client
-
-    client = get_daemon_client()
-
-    try:
-        echo.echo(f'Starting the daemon with {number} workers... ', nl=False)
-        client.start_daemon(number_workers=number, foreground=foreground)
-    except DaemonException as exception:
-        echo.echo('FAILED', fg=echo.COLORS['error'], bold=True)
-        echo.echo_critical(str(exception))
-
-    with spinner():
-        time.sleep(1)
-        response = client.get_status()
-
-    retcode = print_client_response_status(response)
-    if retcode:
-        sys.exit(retcode)
+    echo.echo(f'Starting the daemon with {number} workers... ', nl=False)
+    execute_client_command('start_daemon', number_workers=number, foreground=foreground, timeout=timeout)
 
 
 @verdi_daemon.command()
 @click.option('--all', 'all_profiles', is_flag=True, help='Show status of all daemons.')
-def status(all_profiles):
+@options.TIMEOUT(default=None, required=False, type=int)
+@click.pass_context
+@decorators.requires_loaded_profile()
+def status(ctx, all_profiles, timeout):
     """Print the status of the current daemon or all daemons.
 
     Returns exit code 0 if all requested daemons are running, else exit code 3.
     """
-    from aiida.engine.daemon.client import get_daemon_client
+    from tabulate import tabulate
 
-    manager = get_manager()
-    config = manager.get_config()
+    from aiida.cmdline.utils.common import format_local_time
+    from aiida.engine.daemon.client import DaemonException, get_daemon_client
 
     if all_profiles is True:
-        profiles = [profile for profile in config.profiles if not profile.is_test_profile]
+        profiles = [profile for profile in ctx.obj.config.profiles if not profile.is_test_profile]
     else:
-        profiles = [manager.get_profile()]
+        profiles = [ctx.obj.profile]
 
     daemons_running = []
+
     for profile in profiles:
         client = get_daemon_client(profile.name)
-        delete_stale_pid_file(client)
         echo.echo('Profile: ', fg=echo.COLORS['report'], bold=True, nl=False)
         echo.echo(f'{profile.name}', bold=True)
-        result = get_daemon_status(client)
-        echo.echo(result)
-        daemons_running.append(client.is_daemon_running)
+
+        try:
+            client.get_status(timeout=timeout)
+        except DaemonException as exception:
+            echo.echo_error(str(exception))
+            daemons_running.append(False)
+            continue
+
+        worker_response = client.get_worker_info()
+        daemon_response = client.get_daemon_info()
+
+        workers = []
+        for pid, info in worker_response['info'].items():
+            if isinstance(info, dict):
+                row = [pid, info['mem'], info['cpu'], format_local_time(info['create_time'])]
+            else:
+                row = [pid, '-', '-', '-']
+            workers.append(row)
+
+        if workers:
+            workers_info = tabulate(workers, headers=['PID', 'MEM %', 'CPU %', 'started'], tablefmt='simple')
+        else:
+            workers_info = '--> No workers are running. Use `verdi daemon incr` to start some!\n'
+
+        start_time = format_local_time(daemon_response['info']['create_time'])
+        echo.echo(
+            f'Daemon is running as PID {daemon_response["info"]["pid"]} since {start_time}\n'
+            f'Active workers [{len(workers)}]:\n{workers_info}\n'
+            'Use `verdi daemon [incr | decr] [num]` to increase / decrease the number of workers'
+        )
 
     if not all(daemons_running):
         sys.exit(3)
 
 
 @verdi_daemon.command()
 @click.argument('number', default=1, type=int)
+@options.TIMEOUT(default=None, required=False, type=int)
 @decorators.only_if_daemon_running()
-def incr(number):
+def incr(number, timeout):
     """Add NUMBER [default=1] workers to the running daemon.
 
     Returns exit code 0 if the daemon is OK, non-zero if there was an error.
     """
-    from aiida.engine.daemon.client import get_daemon_client
-
-    client = get_daemon_client()
-    response = client.increase_workers(number)
-    retcode = print_client_response_status(response)
-    if retcode:
-        sys.exit(retcode)
+    echo.echo(f'Starting {number} daemon workers... ', nl=False)
+    execute_client_command('increase_workers', number=number, timeout=timeout)
 
 
 @verdi_daemon.command()
 @click.argument('number', default=1, type=int)
+@options.TIMEOUT(default=None, required=False, type=int)
 @decorators.only_if_daemon_running()
-def decr(number):
+def decr(number, timeout):
     """Remove NUMBER [default=1] workers from the running daemon.
 
     Returns exit code 0 if the daemon is OK, non-zero if there was an error.
     """
-    from aiida.engine.daemon.client import get_daemon_client
-
-    client = get_daemon_client()
-    response = client.decrease_workers(number)
-    retcode = print_client_response_status(response)
-    if retcode:
-        sys.exit(retcode)
+    echo.echo(f'Stopping {number} daemon workers... ', nl=False)
+    execute_client_command('decrease_workers', number=number, timeout=timeout)
 
 
 @verdi_daemon.command()
 def logshow():
     """Show the log of the daemon, press CTRL+C to quit."""
     from aiida.engine.daemon.client import get_daemon_client
 
@@ -148,101 +185,61 @@
     with subprocess.Popen(['tail', '-f', client.daemon_log_file], env=client.get_env()) as process:
         process.wait()
 
 
 @verdi_daemon.command()
 @click.option('--no-wait', is_flag=True, help='Do not wait for confirmation.')
 @click.option('--all', 'all_profiles', is_flag=True, help='Stop all daemons.')
-def stop(no_wait, all_profiles):
+@options.TIMEOUT(default=None, required=False, type=int)
+@click.pass_context
+def stop(ctx, no_wait, all_profiles, timeout):
     """Stop the daemon.
 
     Returns exit code 0 if the daemon was shut down successfully (or was not running), non-zero if there was an error.
     """
-    from aiida.engine.daemon.client import get_daemon_client
-
-    manager = get_manager()
-    config = manager.get_config()
-
     if all_profiles is True:
-        profiles = [profile for profile in config.profiles if not profile.is_test_profile]
+        profiles = [profile for profile in ctx.obj.config.profiles if not profile.is_test_profile]
     else:
-        profiles = [manager.get_profile()]
+        profiles = [ctx.obj.profile]
 
     for profile in profiles:
-
-        client = get_daemon_client(profile.name)
-
         echo.echo('Profile: ', fg=echo.COLORS['report'], bold=True, nl=False)
         echo.echo(f'{profile.name}', bold=True)
-
-        if not client.is_daemon_running:
-            echo.echo('Daemon was not running')
-            continue
-
-        delete_stale_pid_file(client)
-
-        wait = not no_wait
-
-        if wait:
-            echo.echo('Waiting for the daemon to shut down... ', nl=False)
-        else:
-            echo.echo('Shutting the daemon down')
-
-        response = client.stop_daemon(wait)
-
-        if wait:
-            if response['status'] == client.DAEMON_ERROR_NOT_RUNNING:
-                echo.echo('The daemon was not running.')
-            else:
-                retcode = print_client_response_status(response)
-                if retcode:
-                    sys.exit(retcode)
+        echo.echo('Stopping the daemon... ', nl=False)
+        execute_client_command('stop_daemon', daemon_not_running_ok=True, wait=not no_wait, timeout=timeout)
 
 
 @verdi_daemon.command()
 @click.option('--reset', is_flag=True, help='Completely reset the daemon.')
 @click.option('--no-wait', is_flag=True, help='Do not wait for confirmation.')
+@options.TIMEOUT(default=None, required=False, type=int)
 @click.pass_context
 @decorators.with_dbenv()
 @decorators.only_if_daemon_running()
-def restart(ctx, reset, no_wait):
+def restart(ctx, reset, no_wait, timeout):
     """Restart the daemon.
 
     By default will only reset the workers of the running daemon. After the restart the same amount of workers will be
     running. If the `--reset` flag is passed, however, the full daemon will be stopped and restarted with the default
     number of workers that is started when calling `verdi daemon start` manually.
 
     Returns exit code 0 if the result is OK, non-zero if there was an error.
     """
-    from aiida.engine.daemon.client import get_daemon_client
-
-    client = get_daemon_client()
-    wait = not no_wait
-
     if reset:
-        ctx.invoke(stop)
         # These two lines can be simplified to `ctx.invoke(start)` once issue #950 in `click` is resolved.
         # Due to that bug, the `callback` of the `number` argument the `start` command is not being called, which is
         # responsible for settting the default value, which causes `None` to be passed and that triggers an exception.
         # As a temporary workaround, we fetch the default here manually and pass that in explicitly.
         number = ctx.obj.config.get_option('daemon.default_workers', ctx.obj.profile.name)
+        ctx.invoke(stop)
         ctx.invoke(start, number=number)
-    else:
-
-        if wait:
-            echo.echo('Restarting the daemon... ', nl=False)
-        else:
-            echo.echo('Restarting the daemon')
-
-        response = client.restart_daemon(wait)
+        return
 
-        if wait:
-            retcode = print_client_response_status(response)
-            if retcode:
-                sys.exit(retcode)
+    echo.echo('Restarting the daemon... ', nl=False)
+    execute_client_command('restart_daemon', wait=not no_wait, timeout=timeout)
 
 
 @verdi_daemon.command(hidden=True)
 @click.option('--foreground', is_flag=True, help='Run in foreground.')
 @click.argument('number', required=False, type=int, callback=validate_daemon_workers)
 @decorators.with_dbenv()
 @decorators.check_circus_zmq_version
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/__init__.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_array.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ###########################################################################
 """`verdi data array` command."""
 
 from aiida.cmdline.commands.cmd_data import verdi_data
 from aiida.cmdline.params import arguments, options, types
 
 
-@verdi_data.group('array')
+@verdi_data.group('core.array')
 def array():
     """Manipulate ArrayData objects (numpy arrays)."""
 
 
 @array.command('show')
 @arguments.DATA(type=types.DataParamType(sub_classes=('aiida.data:core.array',)))
 @options.DICT_FORMAT()
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_bands.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_bands.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 EXPORT_FORMATS = [
     'agr', 'agr_batch', 'dat_blocks', 'dat_multicolumn', 'gnuplot', 'json', 'mpl_pdf', 'mpl_png', 'mpl_singlefile',
     'mpl_withjson'
 ]
 VISUALIZATION_FORMATS = ['xmgrace']
 
 
-@verdi_data.group('bands')
+@verdi_data.group('core.bands')
 def bands():
     """Manipulate BandsData objects (band structures)."""
 
 
 # pylint: disable=too-many-arguments
 @bands.command('list')
 @decorators.with_dbenv()
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_cif.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_cif.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from aiida.cmdline.utils import decorators, echo
 
 LIST_PROJECT_HEADERS = ['Id', 'Formulae', 'Source.URI']
 EXPORT_FORMATS = ['cif']
 VISUALIZATION_FORMATS = ['jmol', 'vesta']
 
 
-@verdi_data.group('cif')
+@verdi_data.group('core.cif')
 def cif():
     """Manipulate CifData objects (crystal structures in .cif format)."""
 
 
 @cif.command('list')
 @options.FORMULA_MODE()
 @list_options
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_dict.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ###########################################################################
 """`verdi data dict` command."""
 
 from aiida.cmdline.commands.cmd_data import verdi_data
 from aiida.cmdline.params import arguments, options, types
 
 
-@verdi_data.group('dict')
+@verdi_data.group('core.dict')
 def dictionary():
     """Manipulate Dict objects (python dictionaries)."""
 
 
 @dictionary.command('show')
 @arguments.DATA(type=types.DataParamType(sub_classes=('aiida.data:core.dict',)))
 @options.DICT_FORMAT()
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_export.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_export.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_list.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_list.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_remote.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import click
 
 from aiida.cmdline.commands.cmd_data import verdi_data
 from aiida.cmdline.params import arguments, types
 from aiida.cmdline.utils import echo
 
 
-@verdi_data.group('remote')
+@verdi_data.group('core.remote')
 def remote():
     """Manipulate RemoteData objects (reference to remote folders).
 
     A RemoteData can be thought as a "symbolic link" to a folder on one of the
     Computers set up in AiiDA (e.g. where a CalcJob will run).
     This folder is called "remote" in the sense that it is on a Computer and
     not in the AiiDA repository. Note, however, that the "remote" computer
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_show.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_show.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_singlefile.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_singlefile.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """`verdi data singlefile` command."""
 
 from aiida.cmdline.commands.cmd_data import verdi_data
 from aiida.cmdline.params import arguments, types
 from aiida.cmdline.utils import decorators, echo
 
 
-@verdi_data.group('singlefile')
+@verdi_data.group('core.singlefile')
 def singlefile():
     """Work with SinglefileData nodes."""
 
 
 @singlefile.command('content')
 @arguments.DATUM(type=types.DataParamType(sub_classes=('aiida.data:core.singlefile',)))
 @decorators.with_dbenv()
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_structure.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             f'  Successfully imported structure {new_structure.get_formula()} (not storing it, dry-run requested)'
         )
     else:
         new_structure.store()
         echo.echo(f'  Successfully imported structure {new_structure.get_formula()} (PK = {new_structure.pk})')
 
 
-@verdi_data.group('structure')
+@verdi_data.group('core.structure')
 def structure():
     """Manipulate StructureData objects (crystal structures)."""
 
 
 # pylint: disable=too-many-locals,too-many-branches
 @structure.command('list')
 @options.FORMULA_MODE()
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_trajectory.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_trajectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from aiida.cmdline.utils import decorators, echo
 
 LIST_PROJECT_HEADERS = ['Id', 'Label']
 EXPORT_FORMATS = ['cif', 'xsf']
 VISUALIZATION_FORMATS = ['jmol', 'xcrysden', 'mpl_heatmap', 'mpl_pos']
 
 
-@verdi_data.group('trajectory')
+@verdi_data.group('core.trajectory')
 def trajectory():
     """Manipulate TrajectoryData objects (molecular trajectories)."""
 
 
 @trajectory.command('list')
 @list_options
 @decorators.with_dbenv()
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_data/cmd_upf.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_data/cmd_upf.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from aiida.cmdline.commands.cmd_data import verdi_data
 from aiida.cmdline.commands.cmd_data.cmd_export import data_export, export_options
 from aiida.cmdline.params import arguments, options, types
 from aiida.cmdline.utils import decorators, echo
 
 
-@verdi_data.group('upf')
+@verdi_data.group('core.upf')
 def upf():
     """Manipulate UpfData objects (UPF-format pseudopotentials)."""
 
 
 @upf.command('uploadfamily')
 @click.argument('folder', type=click.Path(exists=True, file_okay=False, resolve_path=True))
 @click.argument('group_label', type=click.STRING)
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_database.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_database.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_devel.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_devel.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_group.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_group.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_help.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_help.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_node.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,14 +311,15 @@
         except ValueError:
             pks.append(NodeEntityLoader.load_entity(obj).pk)
 
     def _dry_run_callback(pks):
         if not pks or force:
             return False
         echo.echo_warning(f'YOU ARE ABOUT TO DELETE {len(pks)} NODES! THIS CANNOT BE UNDONE!')
+        echo.echo_info('The nodes with the following pks would be deleted: ' + ' '.join(map(str, pks)))
         return not click.confirm('Shall I continue?', abort=True)
 
     _, was_deleted = delete_nodes(pks, dry_run=dry_run or _dry_run_callback, **traversal_rules)
 
     if was_deleted:
         echo.echo_success('Finished deletion.')
 
@@ -430,18 +431,19 @@
     help=
     "Only color nodes of specific class label (as displayed in the graph, e.g. 'StructureData', 'FolderData', etc.).",
     type=click.STRING,
     default=None,
     multiple=True
 )
 @click.option('-s', '--show', is_flag=True, help='Open the rendered result with the default application.')
+@arguments.OUTPUT_FILE(required=False)
 @decorators.with_dbenv()
 def graph_generate(
     root_node, link_types, identifier, ancestor_depth, descendant_depth, process_out, process_in, engine, output_format,
-    highlight_classes, show
+    highlight_classes, show, output_file
 ):
     """
     Generate a graph from a ROOT_NODE (specified by pk or uuid).
     """
     # pylint: disable=too-many-arguments
     from aiida.tools.visualization import Graph
     link_types = {'all': (), 'logic': ('input_work', 'return'), 'data': ('input_calc', 'create')}[link_types]
@@ -463,19 +465,21 @@
         root_node,
         depth=descendant_depth,
         link_types=link_types,
         annotate_links='both',
         include_process_inputs=process_in,
         highlight_classes=highlight_classes,
     )
-    output_file_name = graph.graphviz.render(
-        filename=f'{root_node.pk}.{engine}', format=output_format, view=show, cleanup=True
-    )
 
-    echo.echo_success(f'Output file: {output_file_name}')
+    if not output_file:
+        output_file = pathlib.Path(f'{root_node.pk}.{engine}.{output_format}')
+
+    output_file_name = graph.graphviz.render(outfile=output_file, format=output_format, view=show, cleanup=True)
+
+    echo.echo_success(f'Output written to `{output_file_name}`')
 
 
 @verdi_node.group('comment')
 def verdi_comment():
     """Inspect, create and manage node comments."""
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_plugin.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_plugin.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_process.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_process.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,65 +51,89 @@
 @options.PROCESS_LABEL()
 @options.PAUSED()
 @options.EXIT_STATUS()
 @options.FAILED()
 @options.PAST_DAYS()
 @options.LIMIT()
 @options.RAW()
+@click.pass_context
 @decorators.with_dbenv()
 def process_list(
-    all_entries, group, process_state, process_label, paused, exit_status, failed, past_days, limit, project, raw,
+    ctx, all_entries, group, process_state, process_label, paused, exit_status, failed, past_days, limit, project, raw,
     order_by, order_dir
 ):
     """Show a list of running or terminated processes.
 
     By default, only those that are still running are shown, but there are options to show also the finished ones.
     """
     # pylint: disable=too-many-locals
     from tabulate import tabulate
 
-    from aiida.cmdline.utils.common import check_worker_load, print_last_process_state_change
+    from aiida.cmdline.commands.cmd_daemon import execute_client_command
+    from aiida.cmdline.utils.common import print_last_process_state_change
     from aiida.engine.daemon.client import get_daemon_client
+    from aiida.orm import ProcessNode, QueryBuilder
     from aiida.tools.query.calculation import CalculationQueryBuilder
 
     relationships = {}
 
     if group:
         relationships['with_node'] = group
 
     builder = CalculationQueryBuilder()
     filters = builder.get_filters(all_entries, process_state, process_label, paused, exit_status, failed)
     query_set = builder.get_query_set(
         relationships=relationships, filters=filters, order_by={order_by: order_dir}, past_days=past_days, limit=limit
     )
     projected = builder.get_projected(query_set, projections=project)
-
     headers = projected.pop(0)
 
     if raw:
         tabulated = tabulate(projected, tablefmt='plain')
         echo.echo(tabulated)
-    else:
-        tabulated = tabulate(projected, headers=headers)
-        echo.echo(tabulated)
-        echo.echo(f'\nTotal results: {len(projected)}\n')
-        print_last_process_state_change()
+        return
 
-        if not get_daemon_client().is_daemon_running:
-            echo.echo_warning('the daemon is not running', bold=True)
+    tabulated = tabulate(projected, headers=headers)
+    echo.echo(tabulated)
+    echo.echo(f'\nTotal results: {len(projected)}\n')
+    print_last_process_state_change()
+
+    if not get_daemon_client().is_daemon_running:
+        echo.echo_warning('The daemon is not running', bold=True)
+        return
+
+    echo.echo_report('Checking daemon load... ', nl=False)
+    response = execute_client_command('get_numprocesses')
+
+    if not response:
+        # Daemon could not be reached
+        return
+
+    try:
+        active_workers = response['numprocesses']
+    except KeyError:
+        echo.echo_report('No active daemon workers.')
+    else:
+        # Second query to get active process count. Currently this is slow but will be fixed with issue #2770. It is
+        # placed at the end of the command so that the user can Ctrl+C after getting the process table.
+        slots_per_worker = ctx.obj.config.get_option('daemon.worker_process_slots', scope=ctx.obj.profile.name)
+        active_processes = QueryBuilder().append(
+            ProcessNode, filters={
+                'attributes.process_state': {
+                    'in': ('created', 'waiting', 'running')
+                }
+            }
+        ).count()
+        available_slots = active_workers * slots_per_worker
+        percent_load = active_processes / available_slots
+        if percent_load > 0.9:  # 90%
+            echo.echo_warning(f'{percent_load * 100:.0f}%% of the available daemon worker slots have been used!')
+            echo.echo_warning('Increase the number of workers with `verdi daemon incr`.')
         else:
-            # Second query to get active process count
-            # Currently this is slow but will be fixed with issue #2770
-            # We place it at the end so that the user can Ctrl+C after getting the process table.
-            builder = CalculationQueryBuilder()
-            filters = builder.get_filters(process_state=('created', 'waiting', 'running'))
-            query_set = builder.get_query_set(filters=filters)
-            projected = builder.get_projected(query_set, projections=['pk'])
-            worker_slot_use = len(projected) - 1
-            check_worker_load(worker_slot_use)
+            echo.echo_report(f'Using {percent_load * 100:.0f}%% of the available daemon worker slots.')
 
 
 @verdi_process.command('show')
 @arguments.PROCESSES()
 @decorators.with_dbenv()
 def process_show(processes):
     """Show details for one or multiple processes."""
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_profile.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_profile.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_rabbitmq.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_restapi.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_restapi.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_run.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_run.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_setup.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,30 +159,31 @@
     _store_default_user_settings(ctx.obj.config, email, first_name, last_name, institution)
 
     dbinfo_su = {
         'host': db_host,
         'port': db_port,
         'user': su_db_username,
         'password': su_db_password,
+        'database': su_db_name,
     }
     postgres = Postgres(interactive=not non_interactive, quiet=False, dbinfo=dbinfo_su)
 
     if not postgres.is_connected:
         echo.echo_critical('failed to determine the PostgreSQL setup')
 
     try:
         db_username, db_name = postgres.create_dbuser_db_safe(dbname=db_name, dbuser=db_username, dbpass=db_password)
     except Exception as exception:
         echo.echo_error(
             '\n'.join([
                 'Oops! quicksetup was unable to create the AiiDA database for you.',
                 'See `verdi quicksetup -h` for how to specify non-standard parameters for the postgresql connection.\n'
                 'Alternatively, create the AiiDA database yourself: ',
-                manual_setup_instructions(dbuser=su_db_username,
-                                          dbname=su_db_name), '', 'and then use `verdi setup` instead', ''
+                manual_setup_instructions(db_username=db_username,
+                                          db_name=db_name), '', 'and then use `verdi setup` instead', ''
             ])
         )
         raise exception
 
     # The contextual defaults or `verdi setup` are not being called when `invoking`, so we have to explicitly define
     # them here, even though the `verdi setup` command would populate those when called from the command line.
     setup_parameters = {
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_shell.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_shell.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_status.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_status.py`

 * *Files 19% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 @verdi.command('status')
 @options.PRINT_TRACEBACK()
 @click.option('--no-rmq', is_flag=True, help='Do not check RabbitMQ status')
 def verdi_status(print_traceback, no_rmq):
     """Print status of AiiDA services."""
     # pylint: disable=broad-except,too-many-statements,too-many-branches,too-many-locals,
     from aiida import __version__
-    from aiida.cmdline.utils.daemon import delete_stale_pid_file, get_daemon_status
     from aiida.common.utils import Capturing
+    from aiida.engine.daemon.client import DaemonException, DaemonNotRunningException
     from aiida.manage.configuration.settings import AIIDA_CONFIG_FOLDER
     from aiida.manage.manager import get_manager
 
     exit_code = ExitCode.SUCCESS
 
     print_status(ServiceStatus.UP, 'version', f'AiiDA v{__version__}')
     print_status(ServiceStatus.UP, 'config', AIIDA_CONFIG_FOLDER)
@@ -132,28 +132,25 @@
             if supported:
                 print_status(ServiceStatus.UP, 'rabbitmq', connection)
             else:
                 print_status(ServiceStatus.WARNING, 'rabbitmq', 'Incompatible RabbitMQ version detected! ' + connection)
 
     # Getting the daemon status
     try:
-        client = manager.get_daemon_client()
-        delete_stale_pid_file(client)
-        daemon_status = get_daemon_status(client)
-
-        daemon_status = daemon_status.split('\n', maxsplit=1)[0]  # take only the first line
-        if client.is_daemon_running:
-            print_status(ServiceStatus.UP, 'daemon', daemon_status)
-        else:
-            print_status(ServiceStatus.WARNING, 'daemon', daemon_status)
-
-    except Exception as exc:
+        status = manager.get_daemon_client().get_status()
+    except DaemonNotRunningException as exception:
+        print_status(ServiceStatus.WARNING, 'daemon', str(exception))
+    except DaemonException as exception:
+        print_status(ServiceStatus.ERROR, 'daemon', str(exception))
+    except Exception as exception:
         message = 'Error getting daemon status'
-        print_status(ServiceStatus.ERROR, 'daemon', message, exception=exc, print_traceback=print_traceback)
+        print_status(ServiceStatus.ERROR, 'daemon', message, exception=exception, print_traceback=print_traceback)
         exit_code = ExitCode.CRITICAL
+    else:
+        print_status(ServiceStatus.UP, 'daemon', f'Daemon is running with PID {status["pid"]}')
 
     # Note: click does not forward return values to the exit code, see https://github.com/pallets/click/issues/747
     if exit_code != ExitCode.SUCCESS:
         sys.exit(exit_code)
 
 
 def print_status(status, service, msg='', exception=None, print_traceback=False):
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_storage.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_storage.py`

 * *Files 9% similar despite different names*

```diff
@@ -106,22 +106,26 @@
 @verdi_storage.command('maintain')
 @click.option(
     '--full',
     is_flag=True,
     help='Perform all maintenance tasks, including the ones that should not be executed while the profile is in use.'
 )
 @click.option(
+    '--no-repack', is_flag=True, help='Disable the repacking of the storage when running a `full maintenance`.'
+)
+@options.FORCE()
+@click.option(
     '--dry-run',
     is_flag=True,
     help=
     'Run the maintenance in dry-run mode which will print actions that would be taken without actually executing them.'
 )
 @decorators.with_dbenv()
 @click.pass_context
-def storage_maintain(ctx, full, dry_run):
+def storage_maintain(ctx, full, no_repack, force, dry_run):
     """Performs maintenance tasks on the repository."""
     from aiida.common.exceptions import LockingProfileError
     from aiida.manage.manager import get_manager
 
     manager = get_manager()
     profile = ctx.obj.profile
     storage = manager.get_profile_storage()
@@ -144,16 +148,18 @@
             'executed while still running AiiDA. '
             'However, not all operations that are required to fully optimize disk usage and future performance '
             'can be done in this way.\n'
             'Whenever you find the time or opportunity, please consider running `verdi storage maintain --full` '
             'for a more complete optimization.\n'
         )
 
-    if not dry_run:
-        if not click.confirm('Are you sure you want continue in this mode?'):
-            return
+    if not dry_run and not force and not click.confirm('Are you sure you want continue in this mode?'):
+        return
 
     try:
-        storage.maintain(full=full, dry_run=dry_run)
+        if full and no_repack:
+            storage.maintain(full=full, dry_run=dry_run, do_repack=False)
+        else:
+            storage.maintain(full=full, dry_run=dry_run)
     except LockingProfileError as exception:
         echo.echo_critical(str(exception))
     echo.echo_success('Requested maintenance procedures finished.')
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_user.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_user.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/commands/cmd_verdi.py` & `aiida-core-2.3.0/aiida/cmdline/commands/cmd_verdi.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/groups/dynamic.py` & `aiida-core-2.3.0/aiida/cmdline/groups/dynamic.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,20 +110,25 @@
 
     @staticmethod
     def create_option(name, spec):
         """Create a click option from a name and a specification."""
         spec = copy.deepcopy(spec)
 
         is_flag = spec.pop('is_flag', False)
+        default = spec.get('default')
         name_dashed = name.replace('_', '-')
         option_name = f'--{name_dashed}/--no-{name_dashed}' if is_flag else f'--{name_dashed}'
-
         option_short_name = spec.pop('short_name', None)
 
         kwargs = {'cls': spec.pop('cls', InteractiveOption), 'show_default': True, 'is_flag': is_flag, **spec}
 
+        # If the option is a flag with no default, make sure it is not prompted for, as that will force the user to
+        # specify it to be on or off, but cannot let it unspecified.
+        if kwargs['cls'] is InteractiveOption and is_flag and default is None:
+            kwargs['cls'] = functools.partial(InteractiveOption, prompt_fn=lambda ctx: False)
+
         if option_short_name:
             option = click.option(option_short_name, option_name, **kwargs)
         else:
             option = click.option(option_name, **kwargs)
 
         return option
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/groups/verdi.py` & `aiida-core-2.3.0/aiida/cmdline/groups/verdi.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/__init__.py` & `aiida-core-2.3.0/aiida/cmdline/params/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/arguments/__init__.py` & `aiida-core-2.3.0/aiida/cmdline/params/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/arguments/main.py` & `aiida-core-2.3.0/aiida/cmdline/params/arguments/main.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/arguments/overridable.py` & `aiida-core-2.3.0/aiida/cmdline/params/arguments/overridable.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/options/__init__.py` & `aiida-core-2.3.0/aiida/cmdline/params/options/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/options/commands/__init__.py` & `aiida-core-2.3.0/aiida/cmdline/params/options/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/options/commands/code.py` & `aiida-core-2.3.0/aiida/cmdline/params/options/commands/code.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/options/commands/computer.py` & `aiida-core-2.3.0/aiida/cmdline/params/options/commands/computer.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/options/commands/setup.py` & `aiida-core-2.3.0/aiida/cmdline/params/options/commands/setup.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/options/conditional.py` & `aiida-core-2.3.0/aiida/cmdline/params/options/conditional.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/options/interactive.py` & `aiida-core-2.3.0/aiida/cmdline/params/options/interactive.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/options/main.py` & `aiida-core-2.3.0/aiida/cmdline/params/options/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,27 +87,37 @@
 
         return command
 
     return decorator
 
 
 def set_log_level(_ctx, _param, value):
-    """Fix the log level for all loggers from the cli.
+    """Configure the logging for the CLI command being executed.
 
-    Note that we cannot use the most obvious approach of directly setting the level on the ``AIIDA_LOGGER``. The reason
+    Note that we cannot use the most obvious approach of directly setting the level on the various loggers. The reason
     is that after this callback is finished, the :meth:`aiida.common.log.configure_logging` method can be called again,
-    for example when the database backend is loaded, and this will undo this change. So instead, we change the value of
-    the `aiida.common.log.CLI_LOG_LEVEL` constant. When the logging is reconfigured, that value is no longer ``None``
-    which will ensure that the ``cli`` handler is configured for all handlers with the level of ``CLI_LOG_LEVEL``. This
-    approach tighly couples the generic :mod:`aiida.common.log` module to the :mod:`aiida.cmdline` module, which is not
-    the cleanest, but given that other module code can undo the logging configuration by calling that method, there
-    seems no easy way around this approach.
+    for example when the database backend is loaded, and this will undo this change. So instead, we set to globals in
+    the :mod:`aiida.common.log` module: ``CLI_ACTIVE`` and ``CLI_LOG_LEVEL``. The ``CLI_ACTIVE`` global is always set to
+    ``True``. The ``configure_logging`` function will interpret this as the code being executed through a ``verdi``
+    call. The ``CLI_LOG_LEVEL`` global is only set if an explicit value is set for the ``--verbosity`` option. In this
+    case, it is set to the specified log level and ``configure_logging`` will then set this log level for all loggers.
+
+    This approach tightly couples the generic :mod:`aiida.common.log` module to the :mod:`aiida.cmdline` module, which
+    is not the cleanest, but given that other module code can undo the logging configuration by calling that method,
+    there seems no easy way around this approach.
     """
     from aiida.common import log
 
+    log.CLI_ACTIVE = True
+
+    # If the value is ``None``, it means the option was not specified, but we still configure logging for the CLI
+    if value is None:
+        configure_logging()
+        return None
+
     try:
         log_level = value.upper()
     except AttributeError:
         raise click.BadParameter(f'`{value}` is not a string.')
 
     if log_level not in LOG_LEVELS:
         raise click.BadParameter(f'`{log_level}` is not a valid log level.')
@@ -120,15 +130,14 @@
     return log_level
 
 
 VERBOSITY = OverridableOption(
     '-v',
     '--verbosity',
     type=click.Choice(tuple(map(str.lower, LOG_LEVELS.keys())), case_sensitive=False),
-    default='REPORT',
     callback=set_log_level,
     expose_value=False,  # Ensures that the option is not actually passed to the command, because it doesn't need it
     help='Set the verbosity of the output.'
 )
 
 PROFILE = OverridableOption(
     '-p',
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/options/multivalue.py` & `aiida-core-2.3.0/aiida/cmdline/params/options/multivalue.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/options/overridable.py` & `aiida-core-2.3.0/aiida/cmdline/params/options/overridable.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/__init__.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/calculation.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/calculation.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/choice.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/choice.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/code.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/code.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/computer.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/computer.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/config.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/config.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/data.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/data.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/group.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/group.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/identifier.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/identifier.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/multiple.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/multiple.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/node.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/node.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/path.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/path.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/plugin.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/plugin.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/process.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/process.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/profile.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/profile.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/strings.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/strings.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/user.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/user.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/params/types/workflow.py` & `aiida-core-2.3.0/aiida/cmdline/params/types/workflow.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/utils/__init__.py` & `aiida-core-2.3.0/aiida/cmdline/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/utils/ascii_vis.py` & `aiida-core-2.3.0/aiida/cmdline/utils/ascii_vis.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/utils/common.py` & `aiida-core-2.3.0/aiida/cmdline/utils/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -480,68 +480,7 @@
                 status = style(exit_code.status, bold=True, fg='red')
             else:
                 status = exit_code.status
             table.append((status, '\n'.join(textwrap.wrap(exit_code.message, width=75))))
 
         echo.echo(tabulate(table, tablefmt='plain'))
         echo.echo(style('\nExit codes that invalidate the cache are marked in bold red.\n', italic=True))
-
-
-def get_num_workers():
-    """
-    Get the number of active daemon workers from the circus client
-    """
-    from aiida.common.exceptions import CircusCallError
-    from aiida.manage import get_manager
-
-    manager = get_manager()
-    client = manager.get_daemon_client()
-
-    if client.is_daemon_running:
-        response = client.get_numprocesses()
-        if response['status'] != 'ok':
-            if response['status'] == client.DAEMON_ERROR_TIMEOUT:
-                raise CircusCallError('verdi thought the daemon was alive, but the call to the daemon timed-out')
-            elif response['status'] == client.DAEMON_ERROR_NOT_RUNNING:
-                raise CircusCallError('verdi thought the daemon was running, but really it is not')
-            else:
-                raise CircusCallError
-        try:
-            return response['numprocesses']
-        except KeyError as exc:
-            raise CircusCallError('Circus did not return the number of daemon processes') from exc
-
-
-def check_worker_load(active_slots):
-    """Log a message with information on the current daemon worker load.
-
-    If there are daemon workers active, it logs the current load. If that exceeds 90%, a warning is included with the
-    suggestion to run ``verdi daemon incr``.
-
-    The purpose of this check is to warn the user if they are close to running out of worker slots which could lead to
-    their processes becoming stuck indefinitely.
-
-    :param active_slots: the number of currently active worker slots
-    """
-    from aiida.common.exceptions import CircusCallError
-    from aiida.manage import get_config_option
-
-    warning_threshold = 0.9  # 90%
-
-    slots_per_worker = get_config_option('daemon.worker_process_slots')
-
-    try:
-        active_workers = get_num_workers()
-    except CircusCallError:
-        echo.echo_critical('Could not contact Circus to get the number of active workers.')
-
-    if active_workers is not None:
-        available_slots = active_workers * slots_per_worker
-        percent_load = 1.0 if not available_slots else (active_slots / available_slots)
-        if percent_load > warning_threshold:
-            echo.echo('')  # New line
-            echo.echo_warning(f'{percent_load * 100:.0f}%% of the available daemon worker slots have been used!')
-            echo.echo_warning('Increase the number of workers with `verdi daemon incr`.')
-        else:
-            echo.echo_report(f'Using {percent_load * 100:.0f}%% of the available daemon worker slots.')
-    else:
-        echo.echo_report('No active daemon workers.')
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/utils/decorators.py` & `aiida-core-2.3.0/aiida/cmdline/utils/decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -232,7 +232,33 @@
         template = templates.env.get_template('deprecated.tpl')
         width = 80
         echo.echo(template.render(msg=wrap(message, width - 4), width=width))
 
         return wrapped(*args, **kwargs)
 
     return wrapper
+
+
+def requires_loaded_profile():
+    """Function decorator for CLI command that requires a profile to be loaded.
+
+    Example::
+
+        @requires_loaded_profile()
+        def create_node():
+            pass
+
+    If no profile has been loaded, the command will exit with a critical error. Most ``verdi`` commands will
+    automatically load the default profile. So if this error is hit, it is most likely that either no profile have been
+    defined at all or the default is unspecified.
+    """
+
+    @decorator
+    def wrapper(wrapped, _, args, kwargs):
+        from aiida.manage.configuration import get_profile
+
+        if get_profile() is None:
+            echo.echo_critical('No profile loaded: make sure at least one profile is configured and a default is set.')
+
+        return wrapped(*args, **kwargs)
+
+    return wrapper
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/utils/defaults.py` & `aiida-core-2.3.0/aiida/cmdline/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/utils/echo.py` & `aiida-core-2.3.0/aiida/cmdline/utils/echo.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,22 @@
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 """Convenience functions for logging output from ``verdi`` commands."""
 import collections
 import enum
 import json
+import logging
 import sys
 from typing import Any, Optional
 
 import click
 import yaml
 
-from aiida.common.log import AIIDA_LOGGER
-
-CMDLINE_LOGGER = AIIDA_LOGGER.getChild('cmdline')
+CMDLINE_LOGGER = logging.getLogger('verdi')
 
 __all__ = ('echo_report', 'echo_info', 'echo_success', 'echo_warning', 'echo_error', 'echo_critical', 'echo_dictionary')
 
 
 class ExitCode(enum.IntEnum):
     """Exit codes for the verdi command line."""
     CRITICAL = 1
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/utils/log.py` & `aiida-core-2.3.0/aiida/cmdline/utils/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,27 +39,25 @@
         except Exception:  # pylint: disable=broad-except
             self.handleError(record)
 
 
 class CliFormatter(logging.Formatter):
     """Formatter that automatically prefixes log messages with a colored version of the log level."""
 
-    @staticmethod
-    def format(record):
+    def format(self, record):
         """Format the record using the style required for the command line interface."""
         try:
             fg = COLORS[record.levelname.lower()]
         except KeyError:
             fg = 'white'
 
         try:
             prefix = record.prefix
         except AttributeError:
             prefix = None
 
-        if prefix:
-            return f'{click.style(record.levelname.capitalize(), fg=fg, bold=True)}: {record.msg % record.args}'
+        formatted = super().format(record)
 
-        if record.args:
-            return f'{record.msg % record.args}'
+        if prefix:
+            return f'{click.style(record.levelname.capitalize(), fg=fg, bold=True)}: {formatted}'
 
-        return record.msg
+        return formatted
```

### Comparing `aiida-core-2.2.2/aiida/cmdline/utils/multi_line_input.py` & `aiida-core-2.3.0/aiida/cmdline/utils/multi_line_input.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/utils/pluginable.py` & `aiida-core-2.3.0/aiida/cmdline/utils/pluginable.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/utils/query/__init__.py` & `aiida-core-2.3.0/aiida/cmdline/utils/query/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/utils/query/calculation.py` & `aiida-core-2.3.0/aiida/cmdline/utils/query/calculation.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/utils/query/formatting.py` & `aiida-core-2.3.0/aiida/cmdline/utils/query/formatting.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/utils/query/mapping.py` & `aiida-core-2.3.0/aiida/cmdline/utils/query/mapping.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/utils/repository.py` & `aiida-core-2.3.0/aiida/cmdline/utils/repository.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/utils/shell.py` & `aiida-core-2.3.0/aiida/cmdline/utils/shell.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/cmdline/utils/templates.py` & `aiida-core-2.3.0/aiida/cmdline/utils/templates.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/common/__init__.py` & `aiida-core-2.3.0/aiida/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/common/constants.py` & `aiida-core-2.3.0/aiida/common/constants.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/common/datastructures.py` & `aiida-core-2.3.0/aiida/common/datastructures.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/common/escaping.py` & `aiida-core-2.3.0/aiida/common/escaping.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/common/exceptions.py` & `aiida-core-2.3.0/aiida/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/common/extendeddicts.py` & `aiida-core-2.3.0/aiida/common/extendeddicts.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/common/files.py` & `aiida-core-2.3.0/aiida/common/files.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/common/folders.py` & `aiida-core-2.3.0/aiida/common/folders.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/common/hashing.py` & `aiida-core-2.3.0/aiida/common/hashing.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/common/json.py` & `aiida-core-2.3.0/aiida/common/json.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/common/lang.py` & `aiida-core-2.3.0/aiida/common/lang.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/common/links.py` & `aiida-core-2.3.0/aiida/common/links.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/common/log.py` & `aiida-core-2.3.0/aiida/common/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 """Module for all logging methods/classes that don't need the ORM."""
+from __future__ import annotations
+
 import collections
 import contextlib
 import logging
 import types
 from typing import cast
 
 __all__ = ('AIIDA_LOGGER', 'override_log_level')
@@ -47,15 +49,20 @@
     logging.getLevelName(LOG_LEVEL_REPORT): LOG_LEVEL_REPORT,
     logging.getLevelName(logging.WARNING): logging.WARNING,
     logging.getLevelName(logging.ERROR): logging.ERROR,
     logging.getLevelName(logging.CRITICAL): logging.CRITICAL,
 }
 
 AIIDA_LOGGER = cast(AiidaLoggerType, logging.getLogger('aiida'))
-CLI_LOG_LEVEL = None
+
+CLI_ACTIVE: bool | None = None
+"""Flag that is set to ``True`` if the module is imported by ``verdi`` being called."""
+
+CLI_LOG_LEVEL: str | None = None
+"""Set if ``verdi`` is called with ``--verbosity`` flag specified, and is set to corresponding log level."""
 
 
 # The default logging dictionary for AiiDA that can be used in conjunction
 # with the config.dictConfig method of python's logging module
 def get_logging_config():
     from aiida.manage.configuration import get_config_option
 
@@ -78,25 +85,26 @@
         'handlers': {
             'console': {
                 'class': 'logging.StreamHandler',
                 'formatter': 'halfverbose',
             },
             'cli': {
                 'class': 'aiida.cmdline.utils.log.CliHandler',
-                'formatter': 'cli',
-            }
+                'formatter': 'cli'
+            },
         },
         'loggers': {
             'aiida': {
                 'handlers': ['console'],
                 'level': lambda: get_config_option('logging.aiida_loglevel'),
                 'propagate': True,
             },
-            'aiida.cmdline': {
+            'verdi': {
                 'handlers': ['cli'],
+                'level': lambda: get_config_option('logging.verdi_loglevel'),
                 'propagate': False,
             },
             'plumpy': {
                 'handlers': ['console'],
                 'level': lambda: get_config_option('logging.plumpy_loglevel'),
                 'propagate': False,
             },
@@ -165,16 +173,14 @@
         We don't configure this by default, since it would load the modules that slow the CLI
     :param daemon: configure the logging for a daemon task by adding a file handler instead
         of the default 'console' StreamHandler
     :param daemon_log_file: absolute filepath of the log file for the RotatingFileHandler
     """
     from logging.config import dictConfig
 
-    from aiida.manage.configuration import get_config_option
-
     # Evaluate the `LOGGING` configuration to resolve the lambdas that will retrieve the correct values based on the
     # currently configured profile.
     config = evaluate_logging_configuration(get_logging_config())
     daemon_handler_name = 'daemon_log_file'
 
     # Add the daemon file handler to all loggers if daemon=True
     if daemon is True:
@@ -200,28 +206,37 @@
             logger.setdefault('handlers', []).append(daemon_handler_name)
             try:
                 # Remove the `console` stdout stream handler to prevent messages being duplicated in the daemon log file
                 logger['handlers'].remove('console')
             except ValueError:
                 pass
 
+    # If the ``CLI_ACTIVE`` is set, a ``verdi`` command is being executed, so we replace the ``console`` handler with
+    # the ``cli`` one for all loggers.
+    if CLI_ACTIVE is True:
+        for logger in config['loggers'].values():
+            handlers = logger['handlers']
+            if 'console' in handlers:
+                handlers.remove('console')
+            handlers.append('cli')
+
+    # If ``CLI_LOG_LEVEL`` is set, a ``verdi`` command is being executed with the ``--verbosity`` option. In this case
+    # we override the log levels of all loggers with the specified log level.
     if CLI_LOG_LEVEL is not None:
-        config['loggers']['aiida']['handlers'] = ['cli']
-        config['loggers']['aiida']['level'] = CLI_LOG_LEVEL
+        for logger in config['loggers'].values():
+            logger['level'] = CLI_LOG_LEVEL
 
     # Add the `DbLogHandler` if `with_orm` is `True`
     if with_orm:
-
-        handler_dblogger = 'dblogger'
-
-        config['handlers'][handler_dblogger] = {
+        from aiida.manage.configuration import get_config_option
+        config['handlers']['db_logger'] = {
             'level': get_config_option('logging.db_loglevel'),
-            'class': 'aiida.orm.utils.log.DBLogHandler',
+            'class': 'aiida.orm.utils.log.DBLogHandler'
         }
-        config['loggers']['aiida']['handlers'].append(handler_dblogger)
+        config['loggers']['aiida']['handlers'].append('db_logger')
 
     dictConfig(config)
 
 
 @contextlib.contextmanager
 def override_log_level(level=logging.CRITICAL):
     """Temporarily adjust the log-level of logger."""
```

### Comparing `aiida-core-2.2.2/aiida/common/progress_reporter.py` & `aiida-core-2.3.0/aiida/common/progress_reporter.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/common/timezone.py` & `aiida-core-2.3.0/aiida/common/timezone.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/common/utils.py` & `aiida-core-2.3.0/aiida/common/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/common/warnings.py` & `aiida-core-2.3.0/aiida/common/warnings.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/__init__.py` & `aiida-core-2.3.0/aiida/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/daemon/__init__.py` & `aiida-core-2.3.0/aiida/engine/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/daemon/client.py` & `aiida-core-2.3.0/aiida/engine/daemon/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,51 +9,66 @@
 ###########################################################################
 """Client to interact with the daemon."""
 from __future__ import annotations
 
 import contextlib
 import enum
 import os
+import pathlib
 import shutil
 import socket
 import subprocess
 import sys
 import tempfile
 import time
 import typing as t
 from typing import TYPE_CHECKING
 
+import psutil
+
 from aiida.common.exceptions import AiidaException, ConfigurationError
 from aiida.common.lang import type_check
+from aiida.common.log import AIIDA_LOGGER
 from aiida.manage.configuration import get_config, get_config_option
 from aiida.manage.configuration.profile import Profile
 from aiida.manage.manager import get_manager
 
 if TYPE_CHECKING:
     from circus.client import CircusClient
 
+LOGGER = AIIDA_LOGGER.getChild('engine.daemon.client')
+
 VERDI_BIN = shutil.which('verdi')
 # Recent versions of virtualenv create the environment variable VIRTUAL_ENV
 VIRTUALENV = os.environ.get('VIRTUAL_ENV', None)
 
-# see https://github.com/python/typing/issues/182
-JsonDictType = t.Dict[str, t.Any]
-
 __all__ = ('DaemonClient',)
 
 
 class ControllerProtocol(enum.Enum):
     """The protocol to use for the controller of the Circus daemon."""
 
     IPC = 0
     TCP = 1
 
 
 class DaemonException(AiidaException):
-    """Raised when the starting of the daemon failed."""
+    """Base class for exceptions related to the daemon."""
+
+
+class DaemonNotRunningException(DaemonException):
+    """Raised when a connection to the daemon is attempted but it is not running."""
+
+
+class DaemonTimeoutException(DaemonException):
+    """Raised when a connection to the daemon is attempted but it times out."""
+
+
+class DaemonStalePidException(DaemonException):
+    """Raised when a connection to the daemon is attempted but it fails and the PID file appears to be stale."""
 
 
 def get_daemon_client(profile_name: str | None = None) -> 'DaemonClient':
     """Return the daemon client for the given profile or the current profile if not specified.
 
     :param profile_name: Optional profile name to load.
     :return: The daemon client.
@@ -64,30 +79,27 @@
     profile = get_manager().load_profile(profile_name)
     return DaemonClient(profile)
 
 
 class DaemonClient:  # pylint: disable=too-many-public-methods
     """Client to interact with the daemon."""
 
-    DAEMON_ERROR_NOT_RUNNING = 'daemon-error-not-running'
-    DAEMON_ERROR_TIMEOUT = 'daemon-error-timeout'
-
     _DAEMON_NAME = 'aiida-{name}'
     _ENDPOINT_PROTOCOL = ControllerProtocol.IPC
 
     def __init__(self, profile: Profile):
         """Construct an instance for a given profile.
 
         :param profile: The profile instance.
         """
         type_check(profile, Profile)
         config = get_config()
         self._profile = profile
-        self._SOCKET_DIRECTORY: str | None = None  # pylint: disable=invalid-name
-        self._DAEMON_TIMEOUT: int = config.get_option('daemon.timeout')  # pylint: disable=invalid-name
+        self._socket_directory: str | None = None
+        self._daemon_timeout: int = config.get_option('daemon.timeout', scope=profile.name)
 
     @property
     def profile(self) -> Profile:
         return self._profile
 
     @property
     def daemon_name(self) -> str:
@@ -225,22 +237,22 @@
                     content = fhandle.read().strip()
                 return content
             except (ValueError, IOError):
                 raise RuntimeError('daemon is running so sockets file should have been there but could not read it')
         else:
 
             # The SOCKET_DIRECTORY is already set, a temporary directory was already created and the same should be used
-            if self._SOCKET_DIRECTORY is not None:
-                return self._SOCKET_DIRECTORY
+            if self._socket_directory is not None:
+                return self._socket_directory
 
             socket_dir_path = tempfile.mkdtemp()
             with open(self.circus_socket_file, 'w', encoding='utf8') as fhandle:
                 fhandle.write(str(socket_dir_path))
 
-            self._SOCKET_DIRECTORY = socket_dir_path
+            self._socket_directory = socket_dir_path
             return socket_dir_path
 
     def get_daemon_pid(self) -> int | None:
         """Get the daemon pid which should be written in the daemon pid file specific to the profile.
 
         :return: The pid of the circus daemon process or None if not found.
         """
@@ -364,163 +376,265 @@
 
         template = 'tcp://127.0.0.1:{port}'
         endpoint = template.format(port=port)
 
         return endpoint
 
     @contextlib.contextmanager
-    def get_client(self) -> 'CircusClient':
+    def get_client(self, timeout: int | None = None) -> 'CircusClient':
         """Return an instance of the CircusClient.
 
         The endpoint is defined by the controller endpoint, which used the port that was written to the port file upon
         starting of the daemon.
 
+        :param timeout: Optional timeout to set for trying to reach the circus daemon. Default is set on the client upon
+            instantiation taken from the ``daemon.timeout`` config option.
         :return: CircusClient instance
         """
         from circus.client import CircusClient
 
         try:
-            client = CircusClient(endpoint=self.get_controller_endpoint(), timeout=self._DAEMON_TIMEOUT)
+            client = CircusClient(endpoint=self.get_controller_endpoint(), timeout=timeout or self._daemon_timeout)
             yield client
         finally:
             client.stop()
 
-    def call_client(self, command: JsonDictType) -> JsonDictType:
+    def call_client(self, command: dict[str, t.Any], timeout: int | None = None) -> dict[str, t.Any]:
         """Call the client with a specific command.
 
         Will check whether the daemon is running first by checking for the pid file. When the pid is found yet the call
         still fails with a timeout, this means the daemon was actually not running and it was terminated unexpectedly
         causing the pid file to not be cleaned up properly.
 
         :param command: Command to call the circus client with.
+        :param timeout: Optional timeout to set for trying to reach the circus daemon. Default is set on the client upon
+            instantiation taken from the ``daemon.timeout`` config option.
         :return: The result of the circus client call.
+        :raises DaemonException: If the daemon is not running or cannot be reached.
+        :raises DaemonTimeoutException: If the connection to the daemon timed out.
+        :raises DaemonException: If the connection to the daemon failed for any other reason.
         """
         from circus.exc import CallError
 
-        if not self.get_daemon_pid():
-            return {'status': self.DAEMON_ERROR_NOT_RUNNING}
-
         try:
-            with self.get_client() as client:
+            with self.get_client(timeout=timeout) as client:
                 result = client.call(command)
         except CallError as exception:
+            if self.get_daemon_pid() is None:
+                raise DaemonNotRunningException('The daemon is not running.') from exception
+
+            if self._is_pid_file_stale:
+                raise DaemonStalePidException(
+                    'The daemon could not be reached, seemingly because of a stale PID file. Try starting the daemon '
+                    'to remove it and restore the daemon.'
+                ) from exception
+
             if str(exception) == 'Timed out.':
-                return {'status': self.DAEMON_ERROR_TIMEOUT}
-            raise exception
+                raise DaemonTimeoutException('Connection to the daemon timed out.') from exception
+
+            raise DaemonException('Connection to the daemon failed.') from exception
 
         return result
 
-    def get_status(self) -> JsonDictType:
-        """Get the daemon running status.
+    def get_status(self, timeout: int | None = None) -> dict[str, t.Any]:
+        """Return the status of the daemon.
 
-        :return: The client call response. If successful, will will contain 'status' key.
+        :param timeout: Optional timeout to set for trying to reach the circus daemon. Default is set on the client upon
+            instantiation taken from the ``daemon.timeout`` config option.
+        :returns: The client call response. If successful, will contain 'pid' key.
         """
         command = {'command': 'status', 'properties': {'name': self.daemon_name}}
-        return self.call_client(command)
+        response = self.call_client(command, timeout=timeout)
+        response['pid'] = self.get_daemon_pid()
+        return response
 
-    def get_numprocesses(self) -> JsonDictType:
+    def get_numprocesses(self, timeout: int | None = None) -> dict[str, t.Any]:
         """Get the number of running daemon processes.
 
+        :param timeout: Optional timeout to set for trying to reach the circus daemon. Default is set on the client upon
+            instantiation taken from the ``daemon.timeout`` config option.
         :return: The client call response. If successful, will contain 'numprocesses' key.
         """
         command = {'command': 'numprocesses', 'properties': {'name': self.daemon_name}}
-        return self.call_client(command)
+        return self.call_client(command, timeout=timeout)
 
-    def get_worker_info(self) -> JsonDictType:
+    def get_worker_info(self, timeout: int | None = None) -> dict[str, t.Any]:
         """Get workers statistics for this daemon.
 
+        :param timeout: Optional timeout to set for trying to reach the circus daemon. Default is set on the client upon
+            instantiation taken from the ``daemon.timeout`` config option.
         :return: The client call response. If successful, will contain 'info' key.
         """
         command = {'command': 'stats', 'properties': {'name': self.daemon_name}}
-        return self.call_client(command)
+        return self.call_client(command, timeout=timeout)
 
-    def get_daemon_info(self) -> JsonDictType:
+    def get_daemon_info(self, timeout: int | None = None) -> dict[str, t.Any]:
         """Get statistics about this daemon itself.
 
+        :param timeout: Optional timeout to set for trying to reach the circus daemon. Default is set on the client upon
+            instantiation taken from the ``daemon.timeout`` config option.
         :return: The client call response. If successful, will contain 'info' key.
         """
         command = {'command': 'dstats', 'properties': {}}
-        return self.call_client(command)
+        return self.call_client(command, timeout=timeout)
 
-    def increase_workers(self, number: int) -> JsonDictType:
+    def increase_workers(self, number: int, timeout: int | None = None) -> dict[str, t.Any]:
         """Increase the number of workers.
 
         :param number: The number of workers to add.
+        :param timeout: Optional timeout to set for trying to reach the circus daemon. Default is set on the client upon
+            instantiation taken from the ``daemon.timeout`` config option.
         :return: The client call response.
         """
         command = {'command': 'incr', 'properties': {'name': self.daemon_name, 'nb': number}}
-        return self.call_client(command)
+        return self.call_client(command, timeout=timeout)
 
-    def decrease_workers(self, number: int) -> JsonDictType:
+    def decrease_workers(self, number: int, timeout: int | None = None) -> dict[str, t.Any]:
         """Decrease the number of workers.
 
         :param number: The number of workers to remove.
+        :param timeout: Optional timeout to set for trying to reach the circus daemon. Default is set on the client upon
+            instantiation taken from the ``daemon.timeout`` config option.
         :return: The client call response.
         """
         command = {'command': 'decr', 'properties': {'name': self.daemon_name, 'nb': number}}
-        return self.call_client(command)
+        return self.call_client(command, timeout=timeout)
 
-    def stop_daemon(self, wait: bool = True, timeout: int = 5) -> JsonDictType:
-        """Stop the daemon.
+    def start_daemon(
+        self, number_workers: int = 1, foreground: bool = False, wait: bool = True, timeout: int | None = None
+    ) -> None:
+        """Start the daemon in a sub process running in the background.
 
+        :param number_workers: Number of daemon workers to start.
+        :param foreground: Whether to launch the subprocess in the background or not.
         :param wait: Boolean to indicate whether to wait for the result of the command.
-        :param timeout: Wait this number of seconds for the ``is_daemon_running`` to return ``False`` before raising.
-        :return: The client call response.
-        :raises DaemonException: If ``is_daemon_running`` returns ``True`` after the ``timeout`` has passed.
+        :param timeout: Optional timeout to set for trying to reach the circus daemon after the subprocess has started.
+            Default is set on the client upon instantiation taken from the ``daemon.timeout`` config option.
+        :raises DaemonException: If the command to start the daemon subprocess excepts.
+        :raises DaemonTimeoutException: If the daemon starts but then is unresponsive or in an unexpected state.
         """
-        command = {'command': 'quit', 'properties': {'waiting': wait}}
+        self._clean_potentially_stale_pid_file()
 
-        result = self.call_client(command)
+        env = self.get_env()
+        command = self.cmd_start_daemon(number_workers, foreground)
+        timeout = timeout or self._daemon_timeout
 
-        if self._ENDPOINT_PROTOCOL == ControllerProtocol.IPC:
-            self.delete_circus_socket_directory()
+        try:
+            subprocess.check_output(command, env=env, stderr=subprocess.STDOUT)  # pylint: disable=unexpected-keyword-arg
+        except subprocess.CalledProcessError as exception:
+            raise DaemonException('The daemon failed to start.') from exception
 
         if not wait:
-            return result
+            return
 
         self._await_condition(
-            lambda: not self.is_daemon_running,
-            DaemonException(f'The daemon failed to stop within {timeout} seconds.'),
+            lambda: self.is_daemon_running,
+            DaemonTimeoutException(f'The daemon failed to start or is unresponsive after {timeout} seconds.'),
             timeout=timeout,
         )
 
-        return result
-
-    def restart_daemon(self, wait: bool) -> JsonDictType:
+    def restart_daemon(self, wait: bool = True, timeout: int | None = None) -> dict[str, t.Any]:
         """Restart the daemon.
 
         :param wait: Boolean to indicate whether to wait for the result of the command.
-        :return: The client call response.
+        :param timeout: Optional timeout to set for trying to reach the circus daemon. Default is set on the client upon
+            instantiation taken from the ``daemon.timeout`` config option.
+        :returns: The client call response.
+        :raises DaemonException: If the daemon is not running or cannot be reached.
+        :raises DaemonTimeoutException: If the connection to the daemon timed out.
+        :raises DaemonException: If the connection to the daemon failed for any other reason.
         """
         command = {'command': 'restart', 'properties': {'name': self.daemon_name, 'waiting': wait}}
-        return self.call_client(command)
+        return self.call_client(command, timeout=timeout)
 
-    def start_daemon(self, number_workers: int = 1, foreground: bool = False, timeout: int = 5) -> None:
-        """Start the daemon in a sub process running in the background.
+    def stop_daemon(self, wait: bool = True, timeout: int | None = None) -> dict[str, t.Any]:
+        """Stop the daemon.
 
-        :param number_workers: Number of daemon workers to start.
-        :param foreground: Whether to launch the subprocess in the background or not.
-        :param timeout: Wait this number of seconds for the ``is_daemon_running`` to return ``True`` before raising.
-        :raises DaemonException: If the daemon fails to start.
-        :raises DaemonException: If the daemon starts but then is unresponsive or in an unexpected state.
-        :raises DaemonException: If ``is_daemon_running`` returns ``False`` after the ``timeout`` has passed.
+        :param wait: Boolean to indicate whether to wait for the result of the command.
+        :param timeout: Optional timeout to set for trying to reach the circus daemon. Default is set on the client upon
+            instantiation taken from the ``daemon.timeout`` config option.
+        :returns: The client call response.
+        :raises DaemonException: If the daemon is not running or cannot be reached.
+        :raises DaemonTimeoutException: If the connection to the daemon timed out.
+        :raises DaemonException: If the connection to the daemon failed for any other reason.
         """
-        env = self.get_env()
-        command = self.cmd_start_daemon(number_workers, foreground)
+        command = {'command': 'quit', 'properties': {'waiting': wait}}
+        response = self.call_client(command, timeout=timeout)
+
+        if self._ENDPOINT_PROTOCOL == ControllerProtocol.IPC:
+            self.delete_circus_socket_directory()
 
+        return response
+
+    def _clean_potentially_stale_pid_file(self) -> None:
+        """Check the daemon PID file and delete it if it is likely to be stale."""
         try:
-            subprocess.check_output(command, env=env, stderr=subprocess.STDOUT)  # pylint: disable=unexpected-keyword-arg
-        except subprocess.CalledProcessError as exception:
-            raise DaemonException('The daemon failed to start.') from exception
+            self._check_pid_file()
+        except DaemonException as exception:
+            pathlib.Path(self.circus_pid_file).unlink(missing_ok=True)
+            LOGGER.warning(f'Deleted apparently stale daemon PID file: {exception}')
 
-        self._await_condition(
-            lambda: self.is_daemon_running,
-            DaemonException(f'The daemon failed to start within {timeout} seconds.'),
-            timeout=timeout,
-        )
+    @property
+    def _is_pid_file_stale(self) -> bool:
+        """Return whether the daemon PID file is likely to be stale.
+
+        :returns: ``True`` if the PID file is likely to be stale, ``False`` otherwise.
+        """
+        try:
+            self._check_pid_file()
+        except DaemonException:
+            return True
+
+        return False
+
+    def _check_pid_file(self) -> None:
+        """Check that the daemon's PID file is not stale.
+
+        Checks if the PID contained in the circus PID file matches a valid running ``verdi`` process. The PID file is
+        considered stale if any of the following conditions are true:
+
+        * The process with the given PID no longer exists
+        * The process name does not match the command of the circus daemon
+        * The process username does not match the username of this Python interpreter
+
+        In the latter two cases, the process with the PID of the PID file exists, but it is very likely that it is not
+        the original process that created the PID file, since the command or user is different, indicating the original
+        process died and the PID was recycled for a new process.
+
+        The PID file can got stale if a system is shut down suddenly and so the process is killed but the PID file is
+        not deleted in time. When the `get_daemon_pid()` method is called, an incorrect PID is returned. Alternatively,
+        another process or the user may have meddled with the PID file in some way, corrupting it.
+
+        :raises DaemonException: If the PID file is likely to be stale.
+        """
+        pid = self.get_daemon_pid()
+
+        if pid is None:
+            return
+
+        try:
+            process = psutil.Process(pid)
+
+            # The circus daemon process can appear as ``start-circus`` or ``circusd``. See this issue comment for
+            # details: https://github.com/aiidateam/aiida-core/issues/5336#issuecomment-1376093322
+            if not any(cmd in process.cmdline() for cmd in ['start-circus', 'circusd']):
+                raise DaemonException(
+                    f'process command `{process.cmdline()}` of PID `{pid}` does not match expected AiiDA daemon command'
+                )
+
+            process_user = process.username()
+            current_user = psutil.Process().username()
+
+            if process_user != current_user:
+                raise DaemonException(
+                    f'process user `{process_user}` of PID `{pid}` does not match current user `{current_user}`'
+                )
+
+        except (psutil.AccessDenied, psutil.NoSuchProcess, DaemonException) as exception:
+            raise DaemonException(exception) from exception
 
     @staticmethod
     def _await_condition(condition: t.Callable, exception: Exception, timeout: int = 5, interval: float = 0.1):
         """Await a condition to evaluate to ``True`` or raise the exception if the timeout is reached.
 
         :param condition: A callable that is waited for to return ``True``.
         :param exception: Raise this exception if ``condition`` does not return ``True`` after ``timeout`` seconds.
```

### Comparing `aiida-core-2.2.2/aiida/engine/daemon/execmanager.py` & `aiida-core-2.3.0/aiida/engine/daemon/execmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,31 @@
 ###########################################################################
 """
 This file contains the main routines to submit, check and retrieve calculation
 results. These are general and contain only the main logic; where appropriate,
 the routines make reference to the suitable plugins for all
 plugin-specific operations.
 """
+from __future__ import annotations
+
 from collections.abc import Mapping
 from logging import LoggerAdapter
 import os
 import pathlib
 import shutil
 from tempfile import NamedTemporaryFile
 from typing import Any, List
 from typing import Mapping as MappingType
 from typing import Optional, Tuple, Union
 
 from aiida.common import AIIDA_LOGGER, exceptions
 from aiida.common.datastructures import CalcInfo
 from aiida.common.folders import SandboxFolder
 from aiida.common.links import LinkType
+from aiida.engine.processes.exit_code import ExitCode
 from aiida.manage.configuration import get_config_option
 from aiida.orm import CalcJobNode, Code, FolderData, Node, PortableCode, RemoteData, load_node
 from aiida.orm.utils.log import get_dblogger_extra
 from aiida.repository.common import FileType
 from aiida.schedulers.datastructures import JobState
 from aiida.transports import Transport
 
@@ -347,15 +350,15 @@
         # task. Because in that case, the check for the existence of this link at the top of this function will exit
         # early from this command.
         remotedata = RemoteData(computer=computer, remote_path=workdir)
         remotedata.base.links.add_incoming(node, link_type=LinkType.CREATE, link_label='remote_folder')
         remotedata.store()
 
 
-def submit_calculation(calculation: CalcJobNode, transport: Transport) -> str:
+def submit_calculation(calculation: CalcJobNode, transport: Transport) -> str | ExitCode:
     """Submit a previously uploaded `CalcJob` to the scheduler.
 
     :param calculation: the instance of CalcJobNode to submit.
     :param transport: an already opened transport to use to submit the calculation.
     :return: the job id as returned by the scheduler `submit_from_script` call
     """
     job_id = calculation.get_job_id()
@@ -369,18 +372,20 @@
         return job_id
 
     scheduler = calculation.computer.get_scheduler()
     scheduler.set_transport(transport)
 
     submit_script_filename = calculation.get_option('submit_script_filename')
     workdir = calculation.get_remote_workdir()
-    job_id = scheduler.submit_from_script(workdir, submit_script_filename)
-    calculation.set_job_id(job_id)
+    result = scheduler.submit_from_script(workdir, submit_script_filename)
+
+    if isinstance(result, str):
+        calculation.set_job_id(result)
 
-    return job_id
+    return result
 
 
 def stash_calculation(calculation: CalcJobNode, transport: Transport) -> None:
     """Stash files from the working directory of a completed calculation to a permanent remote folder.
 
     After a calculation has been completed, optionally stash files from the work directory to a storage location on the
     same remote machine. This is useful if one wants to keep certain files from a completed calculation to be removed
```

### Comparing `aiida-core-2.2.2/aiida/engine/daemon/worker.py` & `aiida-core-2.3.0/aiida/engine/daemon/worker.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/exceptions.py` & `aiida-core-2.3.0/aiida/engine/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/launch.py` & `aiida-core-2.3.0/aiida/engine/launch.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/persistence.py` & `aiida-core-2.3.0/aiida/engine/persistence.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/processes/__init__.py` & `aiida-core-2.3.0/aiida/engine/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/processes/builder.py` & `aiida-core-2.3.0/aiida/engine/processes/builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 import yaml
 
 from aiida.engine.processes.ports import PortNamespace
 from aiida.orm import Dict, Node
 from aiida.orm.nodes.data.base import BaseType
 
+from .utils import prune_mapping
+
 if TYPE_CHECKING:
     from aiida.engine.processes.process import Process
 
 __all__ = ('ProcessBuilder', 'ProcessBuilderNamespace')
 
 
 class PrettyEncoder(json.JSONEncoder):
@@ -158,15 +160,15 @@
         self._data.__delitem__(item)
 
     def __delattr__(self, item):
         self._data.__delitem__(item)
 
     def _recursive_merge(self, dictionary, key, value):
         """Recursively merge the contents of ``dictionary`` setting its ``key`` to ``value``."""
-        if isinstance(value, Mapping):
+        if isinstance(value, Mapping) and key in dictionary:
             for inner_key, inner_value in value.items():
                 self._recursive_merge(dictionary[key], inner_key, inner_value)
         else:
             dictionary[key] = value
 
     def _merge(self, *args, **kwds):
         """Merge the content of a dictionary or keyword arguments in .
@@ -215,38 +217,18 @@
     def _inputs(self, prune: bool = False) -> dict:
         """Return the entire mapping of inputs specified for this builder.
 
         :param prune: boolean, when True, will prune nested namespaces that contain no actual values whatsoever
         :return: mapping of inputs ports and their input values.
         """
         if prune:
-            return self._prune(dict(self))
+            return prune_mapping(dict(self))
 
         return dict(self)
 
-    def _prune(self, value):
-        """Prune a nested mapping from all mappings that are completely empty.
-
-        .. note:: a nested mapping that is completely empty means it contains at most other empty mappings. Other null
-            values, such as `None` or empty lists, should not be pruned.
-
-        :param value: a nested mapping of port values
-        :return: the same mapping but without any nested namespace that is completely empty.
-        """
-        if isinstance(value, Mapping) and not isinstance(value, Node):
-            result = {}
-            for key, sub_value in value.items():
-                pruned = self._prune(sub_value)
-                # If `pruned` is an "empty'ish" mapping and not an instance of `Node`, skip it, otherwise keep it.
-                if not (isinstance(pruned, Mapping) and not pruned and not isinstance(pruned, Node)):
-                    result[key] = pruned
-            return result
-
-        return value
-
 
 class ProcessBuilder(ProcessBuilderNamespace):  # pylint: disable=too-many-ancestors
     """A process builder that helps setting up the inputs for creating a new process."""
 
     def __init__(self, process_class: Type['Process']):
         """Construct a `ProcessBuilder` instance for the given `Process` class.
```

### Comparing `aiida-core-2.2.2/aiida/engine/processes/calcjobs/__init__.py` & `aiida-core-2.3.0/aiida/engine/processes/calcjobs/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/processes/calcjobs/calcjob.py` & `aiida-core-2.3.0/aiida/engine/processes/calcjobs/calcjob.py`

 * *Files 4% similar despite different names*

```diff
@@ -448,14 +448,20 @@
         )
         spec.exit_code(
             110, 'ERROR_SCHEDULER_OUT_OF_MEMORY', invalidates_cache=True, message='The job ran out of memory.'
         )
         spec.exit_code(
             120, 'ERROR_SCHEDULER_OUT_OF_WALLTIME', invalidates_cache=True, message='The job ran out of walltime.'
         )
+        spec.exit_code(
+            131, 'ERROR_SCHEDULER_INVALID_ACCOUNT', invalidates_cache=True, message='The specified account is invalid.'
+        )
+        spec.exit_code(
+            140, 'ERROR_SCHEDULER_NODE_FAILURE', invalidates_cache=True, message='The node running the job failed.'
+        )
         spec.exit_code(150, 'STOPPED_BY_MONITOR', invalidates_cache=True, message='{message}')
 
     @classproperty
     def spec_options(cls):  # pylint: disable=no-self-argument
         """Return the metadata options port namespace of the process specification of this process.
 
         :return: options dictionary
@@ -476,15 +482,15 @@
         """
         from aiida.plugins import CalcJobImporterFactory
         from aiida.plugins.entry_point import get_entry_point_from_class
 
         if entry_point_name is None:
             _, entry_point = get_entry_point_from_class(cls.__module__, cls.__name__)
             if entry_point is not None:
-                entry_point_name = entry_point.name  # type: ignore
+                entry_point_name = entry_point.name
 
         assert entry_point_name is not None
 
         return CalcJobImporterFactory(entry_point_name)()
 
     @property
     def options(self) -> AttributeDict:
@@ -727,30 +733,34 @@
             self.logger.info('could not parse scheduler output: return value of `detailed_job_info` is non-zero')
             detailed_job_info = None
 
         if filename_stderr is None:
             self.logger.warning('could not determine `stderr` filename because `scheduler_stderr` option was not set.')
         else:
             try:
-                scheduler_stderr = retrieved.base.repository.get_object_content(filename_stderr)
+                scheduler_stderr = retrieved.base.repository.get_object_content(filename_stderr, mode='r')
             except FileNotFoundError:
                 scheduler_stderr = None
                 self.logger.warning(f'could not parse scheduler output: the `{filename_stderr}` file is missing')
 
         if filename_stdout is None:
             self.logger.warning('could not determine `stdout` filename because `scheduler_stdout` option was not set.')
         else:
             try:
-                scheduler_stdout = retrieved.base.repository.get_object_content(filename_stdout)
+                scheduler_stdout = retrieved.base.repository.get_object_content(filename_stdout, mode='r')
             except FileNotFoundError:
                 scheduler_stdout = None
                 self.logger.warning(f'could not parse scheduler output: the `{filename_stdout}` file is missing')
 
         try:
-            exit_code = scheduler.parse_output(detailed_job_info, scheduler_stdout, scheduler_stderr)
+            exit_code = scheduler.parse_output(
+                detailed_job_info,
+                scheduler_stdout or '',  # type: ignore[arg-type]
+                scheduler_stderr or '',  # type: ignore[arg-type]
+            )
         except exceptions.FeatureNotAvailable:
             self.logger.info(f'`{scheduler.__class__.__name__}` does not implement scheduler output parsing')
             return None
         except Exception as exception:  # pylint: disable=broad-except
             self.logger.error(f'the `parse_output` method of the scheduler excepted: {exception}')
             return None
 
@@ -826,15 +836,14 @@
         calc_info = self.prepare_for_submission(folder)
         calc_info.uuid = str(self.node.uuid)
 
         # I create the job template to pass to the scheduler
         job_tmpl = JobTemplate()
         job_tmpl.submit_as_hold = False
         job_tmpl.rerunnable = self.options.get('rerunnable', False)
-        job_tmpl.job_environment = {}
         # 'email', 'email_on_started', 'email_on_terminated',
         job_tmpl.job_name = f'aiida-{self.node.pk}'
         job_tmpl.sched_output_path = self.options.scheduler_stdout
         if computer is not None:
             job_tmpl.shebang = computer.get_shebang()
         if self.options.scheduler_stderr == self.options.scheduler_stdout:
             job_tmpl.sched_join_files = True
@@ -877,15 +886,15 @@
         append_texts = [self.node.get_option('append_text'), calc_info.append_text] + \
             [code.append_text for code in codes] + \
             [computer.get_append_text()]
         job_tmpl.append_text = '\n\n'.join(append_text for append_text in append_texts if append_text)
 
         # Set resources, also with get_default_mpiprocs_per_machine
         resources = self.node.get_option('resources')
-        scheduler.preprocess_resources(resources, computer.get_default_mpiprocs_per_machine())
+        scheduler.preprocess_resources(resources or {}, computer.get_default_mpiprocs_per_machine())
         job_tmpl.job_resource = scheduler.create_job_resource(**resources)  # type: ignore
 
         subst_dict = {'tot_num_mpiprocs': job_tmpl.job_resource.get_tot_num_mpiprocs()}
 
         for key, value in job_tmpl.job_resource.items():
             subst_dict[key] = value
         mpi_args = [arg.format(**subst_dict) for arg in computer.get_mpirun_command()]
@@ -899,39 +908,60 @@
         for code_info in calc_info.codes_info:
 
             if not isinstance(code_info, CodeInfo):
                 raise PluginInternalError('Invalid codes_info, must be a list of CodeInfo objects')
 
             if code_info.code_uuid is None:
                 raise PluginInternalError('CalcInfo should have the information of the code to be launched')
-            this_code = load_code(code_info.code_uuid)
 
-            # To determine whether this code should be run with MPI enabled, we get the value that was set in the inputs
-            # of the entire process, which can then be overwritten by the value from the `CodeInfo`. This allows plugins
-            # to force certain codes to run without MPI, even if the user wants to run all codes with MPI whenever
-            # possible. This use case is typically useful for `CalcJob`s that consist of multiple codes where one or
-            # multiple codes always have to be executed without MPI.
-
-            this_withmpi = self.node.get_option('withmpi')
-
-            # Override the value of `withmpi` with that of the `CodeInfo` if and only if it is set
-            if code_info.withmpi is not None:
-                this_withmpi = code_info.withmpi
+            code = load_code(code_info.code_uuid)
+
+            # Here are the three values that will determine whether the code is to be run with MPI _if_ they are not
+            # ``None``. If any of them are explicitly defined but are not equivalent, an exception is raised. We use the
+            # ``self._raw_inputs`` to determine the actual value passed for ``metadata.options.withmpi`` and
+            # distinghuish it from the default.
+            raw_inputs = self._raw_inputs or {}  # type: ignore[var-annotated]
+            with_mpi_option = raw_inputs.get('metadata', {}).get('options', {}).get('withmpi', None)
+            with_mpi_plugin = code_info.withmpi
+            with_mpi_code = code.with_mpi
+
+            with_mpi_values = [with_mpi_option, with_mpi_plugin, with_mpi_code]
+            with_mpi_values_defined = [value for value in with_mpi_values if value is not None]
+            with_mpi_values_set = set(with_mpi_values_defined)
+
+            # If more than one value is defined, they have to be identical, or we raise that a conflict is encountered
+            if len(with_mpi_values_set) > 1:
+                error = f'Inconsistent requirements as to whether code `{code}` should be run with or without MPI.'
+                if with_mpi_option is not None:
+                    error += f'\nThe `metadata.options.withmpi` input was set to `{with_mpi_option}`.'
+                if with_mpi_plugin is not None:
+                    error += f'\nThe plugin require `{with_mpi_plugin}`.'
+                if with_mpi_code is not None:
+                    error += f'\nThe code `{code}` required `{with_mpi_code}`.'
+                raise RuntimeError(error)
+
+            # At this point we know that the three explicit values agree if they are defined, so we simply set the value
+            if with_mpi_values_set:
+                with_mpi = with_mpi_values_set.pop()
+            else:
+                # Fall back to the default of the ``metadata.options.withmpi`` of the ``Calcjob`` class
+                with_mpi = self.node.get_option('withmpi')
 
-            if this_withmpi:
-                prepend_cmdline_params = this_code.get_prepend_cmdline_params(mpi_args, extra_mpirun_params)
+            if with_mpi:
+                prepend_cmdline_params = code.get_prepend_cmdline_params(mpi_args, extra_mpirun_params)
             else:
-                prepend_cmdline_params = this_code.get_prepend_cmdline_params()
+                prepend_cmdline_params = code.get_prepend_cmdline_params()
 
-            cmdline_params = this_code.get_executable_cmdline_params(code_info.cmdline_params)
+            cmdline_params = code.get_executable_cmdline_params(code_info.cmdline_params)
 
             tmpl_code_info = JobTemplateCodeInfo()
             tmpl_code_info.prepend_cmdline_params = prepend_cmdline_params
             tmpl_code_info.cmdline_params = cmdline_params
-            tmpl_code_info.use_double_quotes = [computer.get_use_double_quotes(), this_code.use_double_quotes]
+            tmpl_code_info.use_double_quotes = [computer.get_use_double_quotes(), code.use_double_quotes]
+            tmpl_code_info.wrap_cmdline_params = code.wrap_cmdline_params
             tmpl_code_info.stdin_name = code_info.stdin_name
             tmpl_code_info.stdout_name = code_info.stdout_name
             tmpl_code_info.stderr_name = code_info.stderr_name
             tmpl_code_info.join_files = code_info.join_files
 
             tmpl_codes_info.append(tmpl_code_info)
         job_tmpl.codes_info = tmpl_codes_info
```

### Comparing `aiida-core-2.2.2/aiida/engine/processes/calcjobs/importer.py` & `aiida-core-2.3.0/aiida/engine/processes/calcjobs/importer.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/processes/calcjobs/manager.py` & `aiida-core-2.3.0/aiida/engine/processes/calcjobs/manager.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/processes/calcjobs/monitors.py` & `aiida-core-2.3.0/aiida/engine/processes/calcjobs/monitors.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/processes/calcjobs/tasks.py` & `aiida-core-2.3.0/aiida/engine/processes/calcjobs/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,15 +499,21 @@
                 skip_submit = await self._launch_task(task_upload_job, self.process, transport_queue)
                 if skip_submit:
                     result = self.retrieve(monitor_result=self._monitor_result)
                 else:
                     result = self.submit()
 
             elif self._command == SUBMIT_COMMAND:
-                await self._launch_task(task_submit_job, node, transport_queue)
+                result = await self._launch_task(task_submit_job, node, transport_queue)
+
+                if isinstance(result, ExitCode):
+                    # The scheduler plugin returned an exit code from ``Scheduler.submit_from_script`` indicating the
+                    # job submission failed due to a non-transient problem and the job should be terminated.
+                    return self.create_state(ProcessState.RUNNING, self.process.terminate, result)
+
                 result = self.update()
 
             elif self._command == UPDATE_COMMAND:
                 job_done = False
 
                 while not job_done:
                     scheduler_state = node.get_scheduler_state()
```

### Comparing `aiida-core-2.2.2/aiida/engine/processes/control.py` & `aiida-core-2.3.0/aiida/engine/processes/control.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,15 @@
 
             process = futures[future]
 
             try:
                 # unwrap is need here since LoopCommunicator will also wrap a future
                 future = unwrap_kiwi_future(future)
                 result = future.result()
-            except communications.CommunicationTimeout:
+            except communications.TimeoutError:
                 LOGGER.error(f'call to {infinitive} Process<{process.pk}> timed out')
             except Exception as exception:  # pylint: disable=broad-except
                 LOGGER.error(f'failed to {infinitive} Process<{process.pk}>: {exception}')
             else:
                 if isinstance(result, kiwipy.Future):
                     LOGGER.report(f'scheduled {infinitive} Process<{process.pk}>')
                     scheduled[result] = process
```

### Comparing `aiida-core-2.2.2/aiida/engine/processes/exit_code.py` & `aiida-core-2.3.0/aiida/engine/processes/exit_code.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/processes/functions.py` & `aiida-core-2.3.0/aiida/engine/processes/functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,36 +4,66 @@
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 """Class and decorators to generate processes out of simple python functions."""
+from __future__ import annotations
+
 import collections
 import functools
 import inspect
 import logging
 import signal
-from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Sequence, Tuple, Type, TypeVar
+import types
+import typing as t
+from typing import TYPE_CHECKING
+
+import docstring_parser
 
 from aiida.common.lang import override
 from aiida.manage import get_manager
-from aiida.orm import CalcFunctionNode, Data, ProcessNode, WorkFunctionNode, to_aiida_type
+from aiida.orm import (
+    Bool,
+    CalcFunctionNode,
+    Data,
+    Dict,
+    Float,
+    Int,
+    List,
+    ProcessNode,
+    Str,
+    WorkFunctionNode,
+    to_aiida_type,
+)
 from aiida.orm.utils.mixins import FunctionCalculationMixin
 
 from .process import Process
 
+try:
+    UnionType = types.UnionType  # type: ignore[attr-defined]
+except AttributeError:
+    # This type is not available for Python 3.9 and older
+    UnionType = None  # pylint: disable=invalid-name
+
+try:
+    get_annotations = inspect.get_annotations  # type: ignore[attr-defined]
+except AttributeError:
+    # This is the backport for Python 3.9 and older
+    from get_annotations import get_annotations  # type: ignore[no-redef]
+
 if TYPE_CHECKING:
     from .exit_code import ExitCode
 
 __all__ = ('calcfunction', 'workfunction', 'FunctionProcess')
 
 LOGGER = logging.getLogger(__name__)
 
-FunctionType = TypeVar('FunctionType', bound=Callable[..., Any])
+FunctionType = t.TypeVar('FunctionType', bound=t.Callable[..., t.Any])
 
 
 def calcfunction(function: FunctionType) -> FunctionType:
     """
     A decorator to turn a standard python function into a calcfunction.
     Example usage:
 
@@ -82,31 +112,31 @@
 
     :param function: The function to decorate.
     :return: The decorated function.
     """
     return process_function(node_class=WorkFunctionNode)(function)
 
 
-def process_function(node_class: Type['ProcessNode']) -> Callable[[Callable[..., Any]], Callable[..., Any]]:
+def process_function(node_class: t.Type['ProcessNode']) -> t.Callable[[FunctionType], FunctionType]:
     """
     The base function decorator to create a FunctionProcess out of a normal python function.
 
     :param node_class: the ORM class to be used as the Node record for the FunctionProcess
     """
 
-    def decorator(function: Callable[..., Any]) -> Callable[..., Any]:
+    def decorator(function: FunctionType) -> FunctionType:
         """
         Turn the decorated function into a FunctionProcess.
 
         :param callable function: the actual decorated function that the FunctionProcess represents
         :return callable: The decorated function.
         """
         process_class = FunctionProcess.build(function, node_class=node_class)
 
-        def run_get_node(*args, **kwargs) -> Tuple[Optional[Dict[str, Any]], 'ProcessNode']:
+        def run_get_node(*args, **kwargs) -> tuple[dict[str, t.Any] | None, 'ProcessNode']:
             """
             Run the FunctionProcess with the supplied inputs in a local runner.
 
             :param args: input arguments to construct the FunctionProcess
             :param kwargs: input keyword arguments to construct the FunctionProcess
             :return: tuple of the outputs of the process and the process node
 
@@ -153,15 +183,15 @@
             store_provenance = inputs.get('metadata', {}).get('store_provenance', True)
             if not store_provenance:
                 process.node._storable = False  # pylint: disable=protected-access
                 process.node._unstorable_message = 'cannot store node because it was run with `store_provenance=False`'  # pylint: disable=protected-access
 
             return result, process.node
 
-        def run_get_pk(*args, **kwargs) -> Tuple[Optional[Dict[str, Any]], int]:
+        def run_get_pk(*args, **kwargs) -> tuple[dict[str, t.Any] | None, int]:
             """Recreate the `run_get_pk` utility launcher.
 
             :param args: input arguments to construct the FunctionProcess
             :param kwargs: input keyword arguments to construct the FunctionProcess
             :return: tuple of the outputs of the process and the process node pk
 
             """
@@ -179,188 +209,299 @@
         decorated_function.run_get_node = run_get_node  # type: ignore[attr-defined]
         decorated_function.is_process_function = True  # type: ignore[attr-defined]
         decorated_function.node_class = node_class  # type: ignore[attr-defined]
         decorated_function.process_class = process_class  # type: ignore[attr-defined]
         decorated_function.recreate_from = process_class.recreate_from  # type: ignore[attr-defined]
         decorated_function.spec = process_class.spec  # type: ignore[attr-defined]
 
-        return decorated_function
+        return decorated_function  # type: ignore[return-value]
 
     return decorator
 
 
+def infer_valid_type_from_type_annotation(annotation: t.Any) -> tuple[t.Any, ...]:
+    """Infer the value for the ``valid_type`` of an input port from the given function argument annotation.
+
+    :param annotation: The annotation of a function argument as returned by ``inspect.get_annotation``.
+    :returns: A tuple of valid types. If no valid types were defined or they could not be successfully parsed, an empty
+        tuple is returned.
+    """
+
+    def get_type_from_annotation(annotation):
+        valid_type_map = {
+            bool: Bool,
+            dict: Dict,
+            t.Dict: Dict,
+            float: Float,
+            int: Int,
+            list: List,
+            t.List: List,
+            str: Str,
+        }
+
+        if inspect.isclass(annotation) and issubclass(annotation, Data):
+            return annotation
+
+        return valid_type_map.get(annotation)
+
+    inferred_valid_type: tuple[t.Any, ...] = ()
+
+    if inspect.isclass(annotation):
+        inferred_valid_type = (get_type_from_annotation(annotation),)
+    elif t.get_origin(annotation) is t.Union or t.get_origin(annotation) is UnionType:
+        inferred_valid_type = tuple(get_type_from_annotation(valid_type) for valid_type in t.get_args(annotation))
+    elif t.get_origin(annotation) is t.Optional:
+        inferred_valid_type = (t.get_args(annotation),)
+
+    return tuple(valid_type for valid_type in inferred_valid_type if valid_type is not None)
+
+
 class FunctionProcess(Process):
     """Function process class used for turning functions into a Process"""
 
-    _func_args: Sequence[str] = ()
+    _func_args: t.Sequence[str] = ()
+    _varargs: str | None = None
 
     @staticmethod
     def _func(*_args, **_kwargs) -> dict:
         """
         This is used internally to store the actual function that is being
         wrapped and will be replaced by the build method.
         """
         return {}
 
     @staticmethod
-    def build(func: Callable[..., Any], node_class: Type['ProcessNode']) -> Type['FunctionProcess']:
+    def build(func: FunctionType, node_class: t.Type['ProcessNode']) -> t.Type['FunctionProcess']:
         """
         Build a Process from the given function.
 
         All function arguments will be assigned as process inputs. If keyword arguments are specified then
         these will also become inputs.
 
         :param func: The function to build a process from
         :param node_class: Provide a custom node class to be used, has to be constructable with no arguments. It has to
             be a sub class of `ProcessNode` and the mixin :class:`~aiida.orm.utils.mixins.FunctionCalculationMixin`.
 
         :return: A Process class that represents the function
 
         """
+        # pylint: disable=too-many-statements
         if not issubclass(node_class, ProcessNode) or not issubclass(node_class, FunctionCalculationMixin):
             raise TypeError('the node_class should be a sub class of `ProcessNode` and `FunctionCalculationMixin`')
 
-        args, varargs, keywords, defaults, _, _, _ = inspect.getfullargspec(func)
-        nargs = len(args)
-        ndefaults = len(defaults) if defaults else 0
-        first_default_pos = nargs - ndefaults
+        signature = inspect.signature(func)
+
+        args: list[str] = []
+        varargs: str | None = None
+        keywords: str | None = None
+
+        try:
+            annotations = get_annotations(func, eval_str=True)
+        except Exception as exception:  # pylint: disable=broad-except
+            # Since we are running with ``eval_str=True`` to unstringize the annotations, the call can except if the
+            # annotations are incorrect. In this case we simply want to log a warning and continue with type inference.
+            LOGGER.warning(f'function `{func.__name__}` has invalid type hints: {exception}')
+            annotations = {}
+
+        try:
+            parsed_docstring = docstring_parser.parse(func.__doc__)
+        except Exception as exception:  # pylint: disable=broad-except
+            LOGGER.warning(f'function `{func.__name__}` has a docstring that could not be parsed: {exception}')
+            param_help_string = {}
+            namespace_help_string = None
+        else:
+            param_help_string = {param.arg_name: param.description for param in parsed_docstring.params}
+            namespace_help_string = parsed_docstring.short_description if parsed_docstring.short_description else ''
+            if parsed_docstring.long_description is not None:
+                namespace_help_string += f'\n\n{parsed_docstring.long_description}'
+
+        for key, parameter in signature.parameters.items():
+
+            if parameter.kind in [parameter.POSITIONAL_ONLY, parameter.POSITIONAL_OR_KEYWORD, parameter.KEYWORD_ONLY]:
+                args.append(key)
 
-        if varargs is not None:
-            raise ValueError('variadic arguments are not supported')
+            if parameter.kind is parameter.VAR_POSITIONAL:
+                varargs = key
+
+            if parameter.kind is parameter.VAR_KEYWORD:
+                varargs = key
 
         def _define(cls, spec):  # pylint: disable=unused-argument
             """Define the spec dynamically"""
             from plumpy.ports import UNSPECIFIED
 
             super().define(spec)
 
-            for i, arg in enumerate(args):
+            for parameter in signature.parameters.values():
+
+                if parameter.kind in [parameter.VAR_POSITIONAL, parameter.VAR_KEYWORD]:
+                    continue
 
-                default = UNSPECIFIED
+                annotation = annotations.get(parameter.name)
+                valid_type = infer_valid_type_from_type_annotation(annotation) or (Data,)
+                help_string = param_help_string.get(parameter.name, None)
 
-                if defaults and i >= first_default_pos:
-                    default = defaults[i - first_default_pos]
+                default = parameter.default if parameter.default is not parameter.empty else UNSPECIFIED
 
                 # If the keyword was already specified, simply override the default
-                if spec.has_input(arg):
-                    spec.inputs[arg].default = default
+                if spec.has_input(parameter.name):
+                    spec.inputs[parameter.name].default = default
+                    continue
+
+                # If the default is ``None`` make sure that the port also accepts a ``NoneType``. Note that we cannot
+                # use ``None`` because the validation will call ``isinstance`` which does not work when passing ``None``
+                # but it does work with ``NoneType`` which is returned by calling ``type(None)``.
+                if default is None:
+                    valid_type += (type(None),)
+
+                # If a default is defined and it is not a ``Data`` instance it should be serialized, but this should be
+                # done lazily using a lambda, just as any port defaults should not define node instances directly as is
+                # also checked by the ``spec.input`` call.
+                if (
+                    default is not None and default != UNSPECIFIED and not isinstance(default, Data) and
+                    not callable(default)
+                ):
+                    indirect_default = lambda value=default: to_aiida_type(value)
                 else:
-                    # If the default is `None` make sure that the port also accepts a `NoneType`
-                    # Note that we cannot use `None` because the validation will call `isinstance` which does not work
-                    # when passing `None`, but it does work with `NoneType` which is returned by calling `type(None)`
-                    if default is None:
-                        valid_type = (Data, type(None))
-                    else:
-                        valid_type = (Data,)
-
-                    # If a default is defined and it is not a ``Data`` instance it should be serialized, but this should
-                    # be done lazily using a lambda, just as any port defaults should not define node instances directly
-                    # as is also checked by the ``spec.input`` call.
-                    if (
-                        default is not None and default != UNSPECIFIED and not isinstance(default, Data) and
-                        not callable(default)
-                    ):
-                        indirect_default = lambda value=default: to_aiida_type(value)
-                    else:
-                        indirect_default = default  # type: ignore[assignment]
+                    indirect_default = default
 
-                    spec.input(arg, valid_type=valid_type, default=indirect_default, serializer=to_aiida_type)
+                spec.input(
+                    parameter.name,
+                    valid_type=valid_type,
+                    default=indirect_default,
+                    serializer=to_aiida_type,
+                    help=help_string,
+                )
 
             # Set defaults for label and description based on function name and docstring, if not explicitly defined
             port_label = spec.inputs['metadata']['label']
 
             if not port_label.has_default():
                 port_label.default = func.__name__
 
-            # If the function support kwargs then allow dynamic inputs, otherwise disallow
-            spec.inputs.dynamic = keywords is not None
+            spec.inputs.help = namespace_help_string
+
+            # If the function supports varargs or kwargs then allow dynamic inputs, otherwise disallow
+            spec.inputs.dynamic = keywords is not None or varargs
 
             # Function processes must have a dynamic output namespace since we do not know beforehand what outputs
             # will be returned and the valid types for the value should be `Data` nodes as well as a dictionary because
             # the output namespace can be nested.
             spec.outputs.valid_type = (Data, dict)
 
         return type(
-            func.__name__, (FunctionProcess,), {
+            func.__qualname__, (FunctionProcess,), {
                 '__module__': func.__module__,
                 '__name__': func.__name__,
+                '__qualname__': func.__qualname__,
                 '_func': staticmethod(func),
                 Process.define.__name__: classmethod(_define),
                 '_func_args': args,
+                '_varargs': varargs or None,
                 '_node_class': node_class
             }
         )
 
     @classmethod
-    def validate_inputs(cls, *args: Any, **kwargs: Any) -> None:  # pylint: disable=unused-argument
+    def validate_inputs(cls, *args: t.Any, **kwargs: t.Any) -> None:  # pylint: disable=unused-argument
         """
         Validate the positional and keyword arguments passed in the function call.
 
         :raises TypeError: if more positional arguments are passed than the function defines
         """
         nargs = len(args)
         nparameters = len(cls._func_args)
+        has_varargs = cls._varargs is not None
 
         # If the spec is dynamic, i.e. the function signature includes `**kwargs` and the number of positional arguments
         # passed is larger than the number of explicitly defined parameters in the signature, the inputs are invalid and
         # we should raise. If we don't, some of the passed arguments, intended to be positional arguments, will be
         # misinterpreted as keyword arguments, but they won't have an explicit name to use for the link label, causing
-        # the input link to be completely lost.
-        if cls.spec().inputs.dynamic and nargs > nparameters:
+        # the input link to be completely lost. If the function supports variadic arguments, however, additional args
+        # should be accepted.
+        if cls.spec().inputs.dynamic and nargs > nparameters and not has_varargs:
             name = cls._func.__name__
             raise TypeError(f'{name}() takes {nparameters} positional arguments but {nargs} were given')
 
     @classmethod
-    def create_inputs(cls, *args: Any, **kwargs: Any) -> Dict[str, Any]:
+    def create_inputs(cls, *args: t.Any, **kwargs: t.Any) -> dict[str, t.Any]:
         """Create the input args for the FunctionProcess."""
         cls.validate_inputs(*args, **kwargs)
 
         ins = {}
         if kwargs:
             ins.update(kwargs)
         if args:
             ins.update(cls.args_to_dict(*args))
         return ins
 
     @classmethod
-    def args_to_dict(cls, *args: Any) -> Dict[str, Any]:
+    def args_to_dict(cls, *args: t.Any) -> dict[str, t.Any]:
         """
         Create an input dictionary (of form label -> value) from supplied args.
 
         :param args: The values to use for the dictionary
 
         :return: A label -> value dictionary
 
         """
-        return dict(list(zip(cls._func_args, args)))
+        dictionary = {}
+        values = list(args)
+
+        for arg in cls._func_args:
+            try:
+                dictionary[arg] = values.pop(0)
+            except IndexError:
+                pass
+
+        # If arguments remain and the function supports variadic arguments, add those as well.
+        if cls._varargs and args:
+
+            # By default the prefix for variadic labels is the key with which the varargs were declared
+            variadic_prefix = cls._varargs
+
+            for index, arg in enumerate(values):
+                label = f'{variadic_prefix}_{index}'
+
+                # If the generated vararg label overlaps with a keyword argument, function signature should be changed
+                if label in dictionary:
+                    raise RuntimeError(
+                        f'variadic argument with index `{index}` would get the label `{label}` but this is already in '
+                        'use by another function argument with the exact same name. To avoid this error, please change '
+                        f'the name of argument `{label}` to something else.'
+                    )
+
+                dictionary[label] = arg
+
+        return dictionary
 
     @classmethod
     def get_or_create_db_record(cls) -> 'ProcessNode':
         return cls._node_class()
 
     def __init__(self, *args, **kwargs) -> None:
         if kwargs.get('enable_persistence', False):
             raise RuntimeError('Cannot persist a function process')
         super().__init__(enable_persistence=False, *args, **kwargs)  # type: ignore
 
     @property
-    def process_class(self) -> Callable[..., Any]:
+    def process_class(self) -> t.Callable[..., t.Any]:
         """
         Return the class that represents this Process, for the FunctionProcess this is the function itself.
 
         For a standard Process or sub class of Process, this is the class itself. However, for legacy reasons,
         the Process class is a wrapper around another class. This function returns that original class, i.e. the
         class that really represents what was being executed.
 
         :return: A Process class that represents the function
 
         """
         return self._func
 
-    def execute(self) -> Optional[Dict[str, Any]]:
+    def execute(self) -> dict[str, t.Any] | None:
         """Execute the process."""
         result = super().execute()
 
         # FunctionProcesses can return a single value as output, and not a dictionary, so we should also return that
         if result and len(result) == 1 and self.SINGLE_OUTPUT_LINKNAME in result:
             return result[self.SINGLE_OUTPUT_LINKNAME]
 
@@ -369,42 +510,45 @@
     @override
     def _setup_db_record(self) -> None:
         """Set up the database record for the process."""
         super()._setup_db_record()
         self.node.store_source_info(self._func)
 
     @override
-    def run(self) -> Optional['ExitCode']:
+    def run(self) -> 'ExitCode' | None:
         """Run the process."""
         from .exit_code import ExitCode
 
         # The following conditional is required for the caching to properly work. Even if the source node has a process
         # state of `Finished` the cached process will still enter the running state. The process state will have then
         # been overridden by the engine to `Running` so we cannot check that, but if the `exit_status` is anything other
         # than `None`, it should mean this node was taken from the cache, so the process should not be rerun.
         if self.node.exit_status is not None:
-            return self.node.exit_status
+            return ExitCode(self.node.exit_status, self.node.exit_message)
 
         # Split the inputs into positional and keyword arguments
         args = [None] * len(self._func_args)
         kwargs = {}
 
         for name, value in (self.inputs or {}).items():
             try:
-                if self.spec().inputs[name].non_db:  # type: ignore[union-attr]
-                    # Don't consider non-database inputs
+                if self.spec().inputs[name].is_metadata:  # type: ignore[union-attr]
+                    # Don't consider ports that defined ``is_metadata=True``
                     continue
             except KeyError:
                 pass  # No port found
 
             # Check if it is a positional arg, if not then keyword
             try:
                 args[self._func_args.index(name)] = value
             except ValueError:
-                kwargs[name] = value
+                if name.startswith(f'{self._varargs}_'):
+                    args.append(value)
+                else:
+                    kwargs[name] = value
 
         result = self._func(*args, **kwargs)
 
         if result is None or isinstance(result, ExitCode):
             return result
 
         if isinstance(result, Data):
```

### Comparing `aiida-core-2.2.2/aiida/engine/processes/futures.py` & `aiida-core-2.3.0/aiida/engine/processes/futures.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/processes/ports.py` & `aiida-core-2.3.0/aiida/engine/processes/ports.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,52 +26,84 @@
 
 PORT_NAME_MAX_CONSECUTIVE_UNDERSCORES = 1  # pylint: disable=invalid-name
 PORT_NAMESPACE_SEPARATOR = '__'  # The character sequence to represent a nested port namespace in a flat link label
 OutputPort = ports.OutputPort  # pylint: disable=invalid-name
 
 
 class WithNonDb:
-    """
-    A mixin that adds support to a port to flag that it should not be stored
-    in the database using the non_db=True flag.
-
-    The mixins have to go before the main port class in the superclass order
-    to make sure the mixin has the chance to strip out the non_db keyword.
-    """
+    """A mixin that adds support to a port to flag it should not be stored in the database using the ``non_db`` flag."""
 
     def __init__(self, *args, **kwargs) -> None:
         self._non_db_explicitly_set: bool = bool('non_db' in kwargs)
         non_db = kwargs.pop('non_db', False)
         super().__init__(*args, **kwargs)
         self._non_db: bool = non_db
 
     @property
     def non_db_explicitly_set(self) -> bool:
-        """Return whether the a value for `non_db` was explicitly passed in the construction of the `Port`.
+        """Return whether the ``non_db`` keyword was explicitly passed in the construction of the ``InputPort``.
 
-        :return: boolean, True if `non_db` was explicitly defined during construction, False otherwise
+        :return: ``True`` if ``non_db`` was explicitly defined during construction, ``False`` otherwise
         """
         return self._non_db_explicitly_set
 
     @property
     def non_db(self) -> bool:
-        """Return whether the value of this `Port` should be stored as a `Node` in the database.
+        """Return whether the value of this ``InputPort`` should be stored in the database.
 
-        :return: boolean, True if it should be storable as a `Node`, False otherwise
+        :return: ``True`` if it should be stored, ``False`` otherwise
         """
         return self._non_db
 
     @non_db.setter
     def non_db(self, non_db: bool) -> None:
-        """Set whether the value of this `Port` should be stored as a `Node` in the database.
-        """
+        """Set whether the value of this ``InputPort`` should be stored as a ``Data`` in the database."""
         self._non_db_explicitly_set = True
         self._non_db = non_db
 
 
+class WithMetadata:
+    """A mixin that allows an input port to be marked as metadata through the keyword ``is_metadata``.
+
+    A metadata input differs from a normal input as in that it is not linked to the ``ProcessNode`` as a ``Data`` node
+    but rather is stored on the ``ProcessNode`` itself (as an attribute, for example).
+    """
+
+    def __init__(self, *args, **kwargs) -> None:
+        self._explicitly_set: bool = bool('is_metadata' in kwargs)
+        is_metadata = kwargs.pop('is_metadata', False)
+        super().__init__(*args, **kwargs)
+        self._is_metadata: bool = is_metadata
+
+    @property
+    def is_metadata_explicitly_set(self) -> bool:
+        """Return whether the ``is_metadata`` keyword was explicitly passed in the construction of the ``InputPort``.
+
+        :return: ``True`` if ``is_metadata`` was explicitly defined during construction, ``False`` otherwise
+        """
+        return self._explicitly_set
+
+    @property
+    def is_metadata(self) -> bool:
+        """Return whether the value of this ``InputPort`` should be stored as a ``Node`` in the database.
+
+        :return: ``True`` if it should be storable as a ``Node``, ``False`` otherwise
+        """
+        return self._is_metadata
+
+    @is_metadata.setter
+    def is_metadata(self, is_metadata: bool) -> None:
+        """Set whether the value of this ``InputPort`` should be stored as a ``Node`` in the database.
+
+        :param is_metadata: ``False`` if the port value should be linked as a ``Node``, ``True`` otherwise.
+        """
+        self._explicitly_set = True
+        self._is_metadata = is_metadata
+
+
 class WithSerialize:
     """
     A mixin that adds support for a serialization function which is automatically applied on inputs
     that are not AiiDA data types.
     """
 
     def __init__(self, *args, **kwargs) -> None:
@@ -87,18 +119,21 @@
         """
         if self._serializer is None or value is None or isinstance(value, Data):
             return value
 
         return self._serializer(value)
 
 
-class InputPort(WithSerialize, WithNonDb, ports.InputPort):
+class InputPort(WithMetadata, WithSerialize, WithNonDb, ports.InputPort):
     """
     Sub class of plumpy.InputPort which mixes in the WithSerialize and WithNonDb mixins to support automatic
     value serialization to database storable types and support non database storable input types as well.
+
+    The mixins have to go before the main port class in the superclass order to make sure they have the chance to
+    process their specific keywords.
     """
 
     def __init__(self, *args, **kwargs) -> None:
         """Override the constructor to check the type of the default if set and warn if not immutable."""
         # pylint: disable=redefined-builtin,too-many-arguments
         if 'default' in kwargs:
             default = kwargs['default']
@@ -117,20 +152,20 @@
 
         if not kwargs.get('required', True) and valid_type:
             kwargs['valid_type'] = tuple(valid_type) + (type(None),)
 
         super().__init__(*args, **kwargs)
 
     def get_description(self) -> Dict[str, str]:
-        """
-        Return a description of the InputPort, which will be a dictionary of its attributes
+        """Return a description of the InputPort, which will be a dictionary of its attributes
 
         :returns: a dictionary of the stringified InputPort attributes
         """
         description = super().get_description()
+        description['is_metadata'] = f'{self.is_metadata}'
         description['non_db'] = f'{self.non_db}'
 
         return description
 
 
 class CalcJobOutputPort(ports.OutputPort):
     """Sub class of plumpy.OutputPort which adds the `_pass_to_parser` attribute."""
@@ -141,15 +176,15 @@
         self._pass_to_parser: bool = pass_to_parser
 
     @property
     def pass_to_parser(self) -> bool:
         return self._pass_to_parser
 
 
-class PortNamespace(WithNonDb, ports.PortNamespace):
+class PortNamespace(WithMetadata, WithNonDb, ports.PortNamespace):
     """
     Sub class of plumpy.PortNamespace which implements the serialize method to support automatic recursive
     serialization of a given mapping onto the ports of the PortNamespace.
     """
 
     def __setitem__(self, key: str, port: ports.Port) -> None:
         """Ensure that a `Port` being added inherits the `non_db` attribute if not explicitly defined at construction.
@@ -161,14 +196,19 @@
         Note that the `non_db` attribute is not present for all `Port` sub classes so we have to check for it first.
         """
         if not isinstance(port, ports.Port):
             raise TypeError('port needs to be an instance of Port')
 
         self.validate_port_name(key)
 
+        if hasattr(
+            port, 'is_metadata_explicitly_set'
+        ) and not port.is_metadata_explicitly_set:  # type: ignore[attr-defined]
+            port.is_metadata = self.is_metadata  # type: ignore[attr-defined]
+
         if hasattr(port, 'non_db_explicitly_set') and not port.non_db_explicitly_set:  # type: ignore[attr-defined]
             port.non_db = self.non_db  # type: ignore[attr-defined]
 
         super().__setitem__(key, port)
 
     @staticmethod
     def validate_port_name(port_name: str) -> None:
```

### Comparing `aiida-core-2.2.2/aiida/engine/processes/process.py` & `aiida-core-2.3.0/aiida/engine/processes/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,20 +44,22 @@
 
 from aiida import orm
 from aiida.common import exceptions
 from aiida.common.extendeddicts import AttributeDict
 from aiida.common.lang import classproperty, override
 from aiida.common.links import LinkType
 from aiida.common.log import LOG_LEVEL_REPORT
+from aiida.orm.implementation.utils import clean_value
 from aiida.orm.utils import serialize
 
 from .builder import ProcessBuilder
 from .exit_code import ExitCode, ExitCodesNamespace
 from .ports import PORT_NAMESPACE_SEPARATOR, InputPort, OutputPort, PortNamespace
 from .process_spec import ProcessSpec
+from .utils import prune_mapping
 
 if TYPE_CHECKING:
     from aiida.engine.runners import Runner
 
 __all__ = ('Process', 'ProcessState')
 
 
@@ -88,15 +90,15 @@
     def define(cls, spec: ProcessSpec) -> None:  # type: ignore[override]
         """Define the specification of the process, including its inputs, outputs and known exit codes.
 
         A `metadata` input namespace is defined, with optional ports that are not stored in the database.
 
         """
         super().define(spec)
-        spec.input_namespace(spec.metadata_key, required=False, non_db=True)
+        spec.input_namespace(spec.metadata_key, required=False, is_metadata=True)
         spec.input(
             f'{spec.metadata_key}.store_provenance',
             valid_type=bool,
             default=True,
             help='If set to `False` provenance will not be stored in the database.'
         )
         spec.input(
@@ -741,14 +743,24 @@
             if name == 'label':
                 self.node.label = value
             elif name == 'description':
                 self.node.description = value
             else:
                 raise RuntimeError(f'unsupported metadata key: {name}')
 
+        # Store JSON-serializable values of ``metadata`` ports in the node's attributes. Note that instead of passing in
+        # the ``metadata`` inputs directly, the entire namespace of raw inputs is passed. The reason is that although
+        # currently in ``aiida-core`` all input ports with ``is_metadata=True`` in the port specification are located
+        # within the ``metadata`` port namespace, this may not always be the case. The ``_filter_serializable_metadata``
+        # method will filter out all ports that set ``is_metadata=True`` no matter where in the namespace they are
+        # defined so this approach is more robust for the future.
+        serializable_inputs = self._filter_serializable_metadata(self.spec().inputs, self.raw_inputs)
+        pruned = prune_mapping(serializable_inputs)
+        self.node.set_metadata_inputs(pruned)
+
     def _setup_inputs(self) -> None:
         """Create the links between the input nodes and the ProcessNode that represents this process."""
         for name, node in self._flat_inputs().items():
 
             # Certain processes allow to specify ports with `None` as acceptable values
             if node is None:
                 continue
@@ -756,14 +768,59 @@
             # Need this special case for tests that use ProcessNodes as classes
             if isinstance(self.node, orm.CalculationNode):
                 self.node.base.links.add_incoming(node, LinkType.INPUT_CALC, name)
 
             elif isinstance(self.node, orm.WorkflowNode):
                 self.node.base.links.add_incoming(node, LinkType.INPUT_WORK, name)
 
+    def _filter_serializable_metadata(
+        self,
+        port: Union[None, InputPort, PortNamespace],
+        port_value: Any,
+    ) -> Union[Any, None]:
+        """Return the inputs that correspond to ports with ``is_metadata=True`` and that are JSON serializable.
+
+        The function is called recursively for any port namespaces.
+
+        :param port: An ``InputPort`` or ``PortNamespace``. If an ``InputPort`` that specifies ``is_metadata=True`` the
+            ``port_value`` is returned. For a ``PortNamespace`` this method is called recursively for the keys within
+            the namespace and the resulting dictionary is returned, omitting ``None`` values. If either ``port`` or
+            ``port_value`` is ``None``, ``None`` is returned.
+        :return: The ``port_value`` where all inputs that do no correspond to a metadata port or are not JSON
+            serializable, have been filtered out.
+        """
+        if port is None or port_value is None:
+            return None
+
+        if isinstance(port, InputPort):
+            if not port.is_metadata:
+                return None
+
+            try:
+                clean_value(port_value)
+            except exceptions.ValidationError:
+                return None
+            else:
+                return port_value
+
+        result = {}
+
+        for key, value in port_value.items():
+            if key not in port:
+                continue
+
+            metadata_value = self._filter_serializable_metadata(port[key], value)  # type: ignore[arg-type]
+
+            if metadata_value is None:
+                continue
+
+            result[key] = metadata_value
+
+        return result or None
+
     def _flat_inputs(self) -> Dict[str, Any]:
         """
         Return a flattened version of the parsed inputs dictionary.
 
         The eventual keys will be a concatenation of the nested keys. Note that the `metadata` dictionary, if present,
         is not passed, as those are dealt with separately in `_setup_metadata`.
 
@@ -798,15 +855,17 @@
         :param port: port against which to map the port value, can be InputPort or PortNamespace
         :param port_value: value for the current port, can be a Mapping
         :param parent_name: the parent key with which to prefix the keys
         :param separator: character to use for the concatenation of keys
         :return: flat list of inputs
 
         """
-        if (port is None and isinstance(port_value, orm.Node)) or (isinstance(port, InputPort) and not port.non_db):
+        if (port is None and
+            isinstance(port_value,
+                       orm.Node)) or (isinstance(port, InputPort) and not (port.is_metadata or port.non_db)):
             return [(parent_name, port_value)]
 
         if port is None and isinstance(port_value, Mapping) or isinstance(port, PortNamespace):
             items = []
             for name, value in port_value.items():
 
                 prefixed_key = parent_name + separator + name if parent_name else name
@@ -818,15 +877,15 @@
 
                 sub_items = self._flatten_inputs(
                     port=nested_port, port_value=value, parent_name=prefixed_key, separator=separator
                 )
                 items.extend(sub_items)
             return items
 
-        assert (port is None) or (isinstance(port, InputPort) and port.non_db)
+        assert (port is None) or (isinstance(port, InputPort) and (port.is_metadata or port.non_db))
         return []
 
     def _flatten_outputs(
         self,
         port: Union[None, OutputPort, PortNamespace],
         port_value: Any,
         parent_name: str = '',
```

### Comparing `aiida-core-2.2.2/aiida/engine/processes/process_spec.py` & `aiida-core-2.3.0/aiida/engine/processes/process_spec.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/processes/workchains/__init__.py` & `aiida-core-2.3.0/aiida/engine/processes/workchains/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/processes/workchains/awaitable.py` & `aiida-core-2.3.0/aiida/engine/processes/workchains/awaitable.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/processes/workchains/context.py` & `aiida-core-2.3.0/aiida/engine/processes/workchains/context.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/processes/workchains/restart.py` & `aiida-core-2.3.0/aiida/engine/processes/workchains/restart.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/processes/workchains/utils.py` & `aiida-core-2.3.0/aiida/engine/processes/workchains/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/processes/workchains/workchain.py` & `aiida-core-2.3.0/aiida/engine/processes/workchains/workchain.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/runners.py` & `aiida-core-2.3.0/aiida/engine/runners.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/transports.py` & `aiida-core-2.3.0/aiida/engine/transports.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/engine/utils.py` & `aiida-core-2.3.0/aiida/engine/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 # pylint: disable=invalid-name
 """Utilities for the workflow engine."""
 import asyncio
 import contextlib
 from datetime import datetime
+import inspect
 import logging
 from typing import TYPE_CHECKING, Any, Awaitable, Callable, Iterator, List, Optional, Tuple, Type, Union
 
 if TYPE_CHECKING:
     from .processes import Process, ProcessBuilder
     from .runners import Runner
 
@@ -51,15 +52,15 @@
 
     if isinstance(process, ProcessBuilder):
         builder = process
         process_class = builder.process_class
         inputs.update(**builder._inputs(prune=True))  # pylint: disable=protected-access
     elif is_process_function(process):
         process_class = process.process_class  # type: ignore[attr-defined]
-    elif issubclass(process, Process):
+    elif inspect.isclass(process) and issubclass(process, Process):
         process_class = process
     else:
         raise ValueError(f'invalid process {type(process)}, needs to be Process or ProcessBuilder')
 
     process = process_class(runner=runner, inputs=inputs)
 
     return process
```

### Comparing `aiida-core-2.2.2/aiida/manage/__init__.py` & `aiida-core-2.3.0/aiida/manage/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/caching.py` & `aiida-core-2.3.0/aiida/manage/caching.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/configuration/__init__.py` & `aiida-core-2.3.0/aiida/manage/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/configuration/config.py` & `aiida-core-2.3.0/aiida/manage/configuration/config.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/configuration/migrations/__init__.py` & `aiida-core-2.3.0/aiida/manage/configuration/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/configuration/migrations/migrations.py` & `aiida-core-2.3.0/aiida/manage/configuration/migrations/migrations.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/configuration/options.py` & `aiida-core-2.3.0/aiida/manage/configuration/options.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/configuration/profile.py` & `aiida-core-2.3.0/aiida/manage/configuration/profile.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/configuration/schema/__init__.py` & `aiida-core-2.3.0/aiida/manage/configuration/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/configuration/schema/config-v5.schema.json` & `aiida-core-2.3.0/aiida/manage/configuration/schema/config-v5.schema.json`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/configuration/schema/config-v6.schema.json` & `aiida-core-2.3.0/aiida/manage/configuration/schema/config-v6.schema.json`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/configuration/schema/config-v7.schema.json` & `aiida-core-2.3.0/aiida/manage/configuration/schema/config-v7.schema.json`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/configuration/schema/config-v8.schema.json` & `aiida-core-2.3.0/aiida/manage/configuration/schema/config-v8.schema.json`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/configuration/schema/config-v9.schema.json` & `aiida-core-2.3.0/aiida/manage/configuration/schema/config-v9.schema.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998109879032259%*

 * *Differences: {"'definitions'": "{'options': {'properties': {'daemon.timeout': {'default': 2, 'description': "*

 * *                  "'Used to set default timeout in the "*

 * *                  ":class:`aiida.engine.daemon.client.DaemonClient` for calls to the daemon'}, "*

 * *                  "'logging.verdi_loglevel': OrderedDict([('type', 'string'), ('enum', "*

 * *                  "['CRITICAL', 'ERROR', 'WARNING', 'REPORT', 'INFO', 'DEBUG']), ('default', "*

 * *                  "'REPORT'), ('description', 'Minimum level to log to consol […]*

```diff
@@ -47,16 +47,16 @@
                 "daemon.default_workers": {
                     "default": 1,
                     "description": "Default number of workers to be launched by `verdi daemon start`",
                     "minimum": 1,
                     "type": "integer"
                 },
                 "daemon.timeout": {
-                    "default": 20,
-                    "description": "Timeout in seconds for calls to the circus client",
+                    "default": 2,
+                    "description": "Used to set default timeout in the :class:`aiida.engine.daemon.client.DaemonClient` for calls to the daemon",
                     "minimum": 0,
                     "type": "integer"
                 },
                 "daemon.worker_process_slots": {
                     "default": 200,
                     "description": "Maximum number of concurrent process tasks that each daemon worker can handle",
                     "minimum": 1,
@@ -179,14 +179,27 @@
                     "enum": [
                         "CRITICAL",
                         "ERROR",
                         "WARNING",
                         "REPORT",
                         "INFO",
                         "DEBUG"
+                    ],
+                    "type": "string"
+                },
+                "logging.verdi_loglevel": {
+                    "default": "REPORT",
+                    "description": "Minimum level to log to console when running a `verdi` command",
+                    "enum": [
+                        "CRITICAL",
+                        "ERROR",
+                        "WARNING",
+                        "REPORT",
+                        "INFO",
+                        "DEBUG"
                     ],
                     "type": "string"
                 },
                 "rest_api.profile_switching": {
                     "default": false,
                     "description": "Toggle whether the profile can be specified in requests submitted to the REST API",
                     "global_only": true,
```

### Comparing `aiida-core-2.2.2/aiida/manage/configuration/settings.py` & `aiida-core-2.3.0/aiida/manage/configuration/settings.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/external/__init__.py` & `aiida-core-2.3.0/aiida/manage/external/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/external/postgres.py` & `aiida-core-2.3.0/aiida/manage/external/postgres.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 ``verdi quicksetup`` commandline tool. It allows convenient access to this
 functionality from within python without knowing details about how postgres is
 installed by default on various systems. If the postgres setup is not the
 default installation, additional information needs to be provided.
 """
 from typing import TYPE_CHECKING
 
-import click
 from pgsu import DEFAULT_DSN as DEFAULT_DBINFO  # pylint: disable=no-name-in-module
 from pgsu import PGSU, PostgresConnectionMode
 
 from aiida.cmdline.utils import echo
 
 if TYPE_CHECKING:
     from aiida.manage.configuration import Profile
@@ -33,15 +32,15 @@
 _DROP_USER_COMMAND = 'DROP USER "{}"'
 _CREATE_DB_COMMAND = (
     'CREATE DATABASE "{}" OWNER "{}" ENCODING \'UTF8\' '
     'LC_COLLATE=\'en_US.UTF-8\' LC_CTYPE=\'en_US.UTF-8\' '
     'TEMPLATE=template0'
 )
 _DROP_DB_COMMAND = 'DROP DATABASE "{}"'
-_GRANT_PRIV_COMMAND = 'GRANT ALL PRIVILEGES ON DATABASE "{}" TO "{}"'
+_GRANT_ROLE_COMMAND = 'GRANT "{}" TO current_user'
 _USER_EXISTS_COMMAND = "SELECT usename FROM pg_user WHERE usename='{}'"
 _CHECK_DB_EXISTS_COMMAND = "SELECT datname FROM pg_database WHERE datname='{}'"
 _COPY_DB_COMMAND = 'CREATE DATABASE "{}" WITH TEMPLATE "{}" OWNER "{}"'
 
 
 class Postgres(PGSU):
     """
@@ -104,39 +103,64 @@
 
         :param str dbuser: Name of the user to be created.
         :param str dbpass: Password the user should be given.
         :raises: psycopg2.errors.DuplicateObject if user already exists and
             self.connection_mode == PostgresConnectionMode.PSYCOPG
         """
         self.execute(_CREATE_USER_COMMAND.format(dbuser, dbpass, privileges))
+        # Ensure the database superuser (current_user) has the right to make `dbuser` the owner of new databases.
+        # Required for some postgresql installations.
+        self.execute(_GRANT_ROLE_COMMAND.format(dbuser))
 
     def drop_dbuser(self, dbuser):
         """
         Drop a database user in postgres
 
         :param str dbuser: Name of the user to be dropped.
         """
         self.execute(_DROP_USER_COMMAND.format(dbuser))
 
-    def check_dbuser(self, dbuser):
-        """Looks up if a given user already exists, prompts for using or creating a differently named one.
+    def find_new_dbuser(self, start_from='aiida'):
+        """Find database user that does not yet exist.
 
-        :param str dbuser: Name of the user to be created or reused.
-        :returns: tuple (dbuser, created)
+        Generates names of the form "aiida_1", "aiida_2", etc. until it finds a name that does not yet exist.
+
+        :param str start_from: start from this name
+        :returns: dbuser
+        """
+        dbuser = start_from
+        i = 0
+        while self.dbuser_exists(dbuser):
+            i = i + 1
+            dbuser = f'{start_from}_{i}'
+
+        return dbuser
+
+    def can_user_authenticate(self, dbuser, dbpass):
+        """Check whether the database user credentials are valid.
+
+        Checks whether dbuser has access to the `template1` postgres database
+        via psycopg2.
+
+        :param dbuser: the database user
+        :param dbpass: the database password
+        :return: True if the credentials are valid, False otherwise
         """
-        if not self.interactive:
-            return dbuser, not self.dbuser_exists(dbuser)
-        create = True
-        while create and self.dbuser_exists(dbuser):
-            echo.echo_warning(f'Database user "{dbuser}" already exists!')
-            if not click.confirm('Use it? '):
-                dbuser = click.prompt('New database user name: ', type=str, default=dbuser)
-            else:
-                create = False
-        return dbuser, create
+        from pgsu import _execute_psyco
+        import psycopg2
+        dsn = self.dsn.copy()
+        dsn['user'] = dbuser
+        dsn['password'] = dbpass
+
+        try:
+            _execute_psyco('SELECT 1', dsn)
+        except psycopg2.OperationalError:
+            return False
+
+        return True
 
     ### DB functions ###
 
     def db_exists(self, dbname):
         """
         Check wether a postgres database with dbname exists
 
@@ -149,56 +173,68 @@
         """
         Create a database in postgres
 
         :param str dbuser: Name of the user which should own the db.
         :param str dbname: Name of the database.
         """
         self.execute(_CREATE_DB_COMMAND.format(dbname, dbuser))
-        self.execute(_GRANT_PRIV_COMMAND.format(dbname, dbuser))
 
     def drop_db(self, dbname):
         """
         Drop a database in postgres
 
         :param str dbname: Name of the database.
         """
         self.execute(_DROP_DB_COMMAND.format(dbname))
 
     def copy_db(self, src_db, dest_db, dbuser):
         self.execute(_COPY_DB_COMMAND.format(dest_db, src_db, dbuser))
 
-    def check_db(self, dbname):
-        """Looks up if a database with the name exists, prompts for using or creating a differently named one.
+    def find_new_db(self, start_from='aiida'):
+        """Find database name that does not yet exist.
 
-        :param str dbname: Name of the database to be created or reused.
-        :returns: tuple (dbname, created)
+        Generates names of the form "aiida_1", "aiida_2", etc. until it finds a name that does not yet exist.
+
+        :param str start_from: start from this name
+        :returns: dbname
         """
-        if not self.interactive:
-            return dbname, not self.db_exists(dbname)
-        create = True
-        while create and self.db_exists(dbname):
-            echo.echo_warning(f'database {dbname} already exists!')
-            if not click.confirm('Use it (make sure it is not used by another profile)?'):
-                dbname = click.prompt('new name', type=str, default=dbname)
-            else:
-                create = False
-        return dbname, create
+        dbname = start_from
+        i = 0
+        while self.db_exists(dbname):
+            i = i + 1
+            dbname = f'{start_from}_{i}'
+
+        return dbname
 
     def create_dbuser_db_safe(self, dbname, dbuser, dbpass):
         """Create DB and user + grant privileges.
 
-        Prompts when reusing existing users / databases.
+        An existing database user is reused, if it is able to authenticate.
+        If not, a new username is generated on the fly.
+
+        An existing database is not reused (unsafe), a new database name is generated on the fly.
+
+        :param str dbname: Name of the database.
+        :param str dbuser: Name of the user which should own the db.
+        :param str dbpass: Password the user should be given.
+        :returns: (dbuser, dbname)
         """
-        dbuser, create = self.check_dbuser(dbuser=dbuser)
-        if create:
+        if not self.dbuser_exists(dbuser):
+            self.create_dbuser(dbuser=dbuser, dbpass=dbpass)
+        elif not self.can_user_authenticate(dbuser, dbpass):
+            echo.echo_warning(f'Database user "{dbuser}" already exists but is unable to authenticate.')
+            dbuser = self.find_new_dbuser(dbuser)
             self.create_dbuser(dbuser=dbuser, dbpass=dbpass)
+        echo.echo_info(f'Using database user "{dbuser}".')
 
-        dbname, create = self.check_db(dbname=dbname)
-        if create:
-            self.create_db(dbuser, dbname)
+        if self.db_exists(dbname):
+            echo.echo_warning(f'Database "{dbname}" already exists.')
+            dbname = self.find_new_db(dbname)
+        self.create_db(dbuser=dbuser, dbname=dbname)
+        echo.echo_info(f'Using database "{dbname}".')
 
         return dbuser, dbname
 
     @property
     def host_for_psycopg2(self):
         """Return correct host for psycopg2 connection (as required by regular AiiDA operation)."""
         host = self.dsn.get('host')
@@ -216,19 +252,19 @@
 
     @property
     def dbinfo(self):
         """Alias for Postgres.dsn."""
         return self.dsn.copy()
 
 
-def manual_setup_instructions(dbuser, dbname):
+def manual_setup_instructions(db_username, db_name):
     """Create a message with instructions for manually creating a database"""
-    dbpass = '<password>'
+    db_pass = '<password>'
     instructions = '\n'.join([
         'Run the following commands as a UNIX user with access to PostgreSQL (Ubuntu: $ sudo su postgres):',
         '',
         '\t$ psql template1',
-        f'	==> {_CREATE_USER_COMMAND.format(dbuser, dbpass, "")}',
-        f'	==> {_CREATE_DB_COMMAND.format(dbname, dbuser)}',
-        f'	==> {_GRANT_PRIV_COMMAND.format(dbname, dbuser)}',
+        f'	==> {_CREATE_USER_COMMAND.format(db_username, db_pass, "")}',
+        f'	==> {_GRANT_ROLE_COMMAND.format(db_username)}',
+        f'	==> {_CREATE_DB_COMMAND.format(db_name, db_username)}',
     ])
     return instructions
```

### Comparing `aiida-core-2.2.2/aiida/manage/external/rmq/__init__.py` & `aiida-core-2.3.0/aiida/manage/external/rmq/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/external/rmq/client.py` & `aiida-core-2.3.0/aiida/manage/external/rmq/client.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/external/rmq/launcher.py` & `aiida-core-2.3.0/aiida/manage/external/rmq/launcher.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/external/rmq/utils.py` & `aiida-core-2.3.0/aiida/manage/external/rmq/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/manager.py` & `aiida-core-2.3.0/aiida/manage/manager.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/profile_access.py` & `aiida-core-2.3.0/aiida/manage/profile_access.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/tests/__init__.py` & `aiida-core-2.3.0/aiida/manage/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/tests/main.py` & `aiida-core-2.3.0/aiida/manage/tests/main.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/manage/tests/pytest_fixtures.py` & `aiida-core-2.3.0/aiida/manage/tests/pytest_fixtures.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 from aiida import plugins
 from aiida.common.exceptions import NotExistent
 from aiida.common.lang import type_check
 from aiida.common.log import AIIDA_LOGGER
 from aiida.common.warnings import warn_deprecation
 from aiida.engine import Process, ProcessBuilder, submit
-from aiida.engine.daemon.client import DaemonClient
+from aiida.engine.daemon.client import DaemonClient, DaemonNotRunningException, DaemonTimeoutException
 from aiida.manage import Config, Profile, get_manager, get_profile
 from aiida.manage.manager import Manager
 from aiida.orm import Computer, ProcessNode, User
 
 
 def recursive_merge(left: dict[t.Any, t.Any], right: dict[t.Any, t.Any]) -> None:
     """Recursively merge the ``right`` dictionary into the ``left`` dictionary.
@@ -424,24 +424,25 @@
           code = aiida_local_code_factory('quantumespresso.pw', '/usr/bin/pw.x')
           # use code for testing ...
 
     :return: A function get_code(entry_point, executable) that returns the `Code` node.
     :rtype: object
     """
 
-    def get_code(entry_point, executable, computer=aiida_localhost, label=None, prepend_text=None, append_text=None):
+    def get_code(entry_point, executable, computer=aiida_localhost, label=None, **kwargs):
         """Get local code.
 
         Sets up code for given entry point on given computer.
 
         :param entry_point: Entry point of calculation plugin
         :param executable: name of executable; will be searched for in local system PATH.
         :param computer: (local) AiiDA computer
-        :param prepend_text: a string of code that will be put in the scheduler script before the execution of the code.
-        :param append_text: a string of code that will be put in the scheduler script after the execution of the code.
+        :param label: Define the label of the code. By default the ``executable`` is taken. This can be useful if
+            multiple codes need to be created in a test which require unique labels.
+        :param kwargs: Additional keyword arguments that are passed to the code's constructor.
         :return: the `Code` either retrieved from the database or created if it did not yet exist.
         :rtype: :py:class:`~aiida.orm.Code`
         """
         from aiida.common import exceptions
         from aiida.orm import InstalledCode, QueryBuilder
 
         if label is None:
@@ -467,23 +468,18 @@
             raise ValueError(f'The executable "{executable}" was not found in the $PATH.')
 
         code = InstalledCode(
             label=label,
             description=label,
             default_calc_job_plugin=entry_point,
             computer=computer,
-            filepath_executable=executable_path
+            filepath_executable=executable_path,
+            **kwargs
         )
 
-        if prepend_text is not None:
-            code.prepend_text = prepend_text
-
-        if append_text is not None:
-            code.append_text = append_text
-
         return code.store()
 
     return get_code
 
 
 @pytest.fixture(scope='session')
 def ssh_key(tmp_path_factory) -> t.Generator[pathlib.Path, None, None]:
@@ -658,15 +654,18 @@
     The daemon will be automatically stopped at the end of the test session.
     """
     daemon_client = DaemonClient(aiida_profile)
 
     try:
         yield daemon_client
     finally:
-        daemon_client.stop_daemon(wait=True)
+        try:
+            daemon_client.stop_daemon(wait=True)
+        except DaemonNotRunningException:
+            pass
         assert not daemon_client.is_daemon_running
 
 
 @pytest.fixture()
 def started_daemon_client(daemon_client):
     """Ensure that the daemon is running for the test profile and return the associated client."""
     if not daemon_client.is_daemon_running:
@@ -677,15 +676,21 @@
 
 
 @pytest.fixture()
 def stopped_daemon_client(daemon_client):
     """Ensure that the daemon is not running for the test profile and return the associated client."""
     if daemon_client.is_daemon_running:
         daemon_client.stop_daemon(wait=True)
-        assert not daemon_client.is_daemon_running
+        # Give an additional grace period by manually waiting for the daemon to be stopped. In certain unit test
+        # scenarios, the built in wait time in ``daemon_client.stop_daemon`` is not sufficient and even though the
+        # daemon is stopped, ``daemon_client.is_daemon_running`` will return false for a little bit longer.
+        daemon_client._await_condition(  # pylint: disable=protected-access
+            lambda: not daemon_client.is_daemon_running,
+            DaemonTimeoutException('The daemon failed to stop.'),
+        )
 
     yield daemon_client
 
 
 @pytest.fixture
 def submit_and_await(started_daemon_client):
     """Submit a process and wait for it to achieve the given state."""
```

### Comparing `aiida-core-2.2.2/aiida/orm/__init__.py` & `aiida-core-2.3.0/aiida/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/authinfos.py` & `aiida-core-2.3.0/aiida/orm/authinfos.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,20 +80,20 @@
         """
         self._backend_entity.enabled = enabled
 
     @property
     def computer(self) -> 'Computer':
         """Return the computer associated with this instance."""
         from . import computers  # pylint: disable=cyclic-import
-        return computers.Computer.from_backend_entity(self._backend_entity.computer)
+        return entities.from_backend_entity(computers.Computer, self._backend_entity.computer)
 
     @property
     def user(self) -> 'User':
         """Return the user associated with this instance."""
-        return users.User.from_backend_entity(self._backend_entity.user)
+        return entities.from_backend_entity(users.User, self._backend_entity.user)
 
     def get_auth_params(self) -> Dict[str, Any]:
         """Return the dictionary of authentication parameters
 
         :return: a dictionary with authentication parameters
         """
         return self._backend_entity.get_auth_params()
```

### Comparing `aiida-core-2.2.2/aiida/orm/autogroup.py` & `aiida-core-2.3.0/aiida/orm/autogroup.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/comments.py` & `aiida-core-2.3.0/aiida/orm/comments.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
     @property
     def node(self) -> 'Node':
         return self._backend_entity.node
 
     @property
     def user(self) -> 'User':
-        return users.User.from_backend_entity(self._backend_entity.user)
+        return entities.from_backend_entity(users.User, self._backend_entity.user)
 
     def set_user(self, value: 'User') -> None:
         self._backend_entity.user = value.backend_entity
 
     @property
     def content(self) -> str:
         return self._backend_entity.content
```

### Comparing `aiida-core-2.2.2/aiida/orm/computers.py` & `aiida-core-2.3.0/aiida/orm/computers.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
                 f'Invalid value for def_memory_per_machine, must be a positive int, got: {def_memory_per_machine}'
             )
 
     def copy(self) -> 'Computer':
         """
         Return a copy of the current object to work with, not stored yet.
         """
-        return Computer.from_backend_entity(self._backend_entity.copy())
+        return entities.from_backend_entity(Computer, self._backend_entity.copy())
 
     def store(self) -> 'Computer':
         """
         Store the computer in the DB.
 
         Differently from Nodes, a computer can be re-stored if its properties
         are to be changed (e.g. a new mpirun command, etc.)
```

### Comparing `aiida-core-2.2.2/aiida/orm/convert.py` & `aiida-core-2.3.0/aiida/orm/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 # pylint: disable=cyclic-import
 """Module for converting backend entities into frontend, ORM, entities"""
 from collections.abc import Iterator, Mapping, Sized
 from functools import singledispatch
 
+from aiida.orm.entities import from_backend_entity
 from aiida.orm.implementation import (
     BackendAuthInfo,
     BackendComment,
     BackendComputer,
     BackendGroup,
     BackendLog,
     BackendNode,
@@ -68,52 +69,52 @@
     return converted
 
 
 @get_orm_entity.register(BackendGroup)
 def _(backend_entity):
     from .groups import load_group_class
     group_class = load_group_class(backend_entity.type_string)
-    return group_class.from_backend_entity(backend_entity)
+    return from_backend_entity(group_class, backend_entity)
 
 
 @get_orm_entity.register(BackendComputer)
 def _(backend_entity):
     from . import computers
-    return computers.Computer.from_backend_entity(backend_entity)
+    return from_backend_entity(computers.Computer, backend_entity)
 
 
 @get_orm_entity.register(BackendUser)
 def _(backend_entity):
     from . import users
-    return users.User.from_backend_entity(backend_entity)
+    return from_backend_entity(users.User, backend_entity)
 
 
 @get_orm_entity.register(BackendAuthInfo)
 def _(backend_entity):
     from . import authinfos
-    return authinfos.AuthInfo.from_backend_entity(backend_entity)
+    return from_backend_entity(authinfos.AuthInfo, backend_entity)
 
 
 @get_orm_entity.register(BackendLog)
 def _(backend_entity):
     from . import logs
-    return logs.Log.from_backend_entity(backend_entity)
+    return from_backend_entity(logs.Log, backend_entity)
 
 
 @get_orm_entity.register(BackendComment)
 def _(backend_entity):
     from . import comments
-    return comments.Comment.from_backend_entity(backend_entity)
+    return from_backend_entity(comments.Comment, backend_entity)
 
 
 @get_orm_entity.register(BackendNode)
 def _(backend_entity):
     from .utils.node import load_node_class  # pylint: disable=import-error,no-name-in-module
     node_class = load_node_class(backend_entity.node_type)
-    return node_class.from_backend_entity(backend_entity)
+    return from_backend_entity(node_class, backend_entity)
 
 
 class ConvertIterator(Iterator, Sized):
     """
     Iterator that converts backend entities into frontend ORM entities as needed
 
     See :func:`aiida.orm.Group.nodes` for an example.
```

### Comparing `aiida-core-2.2.2/aiida/orm/entities.py` & `aiida-core-2.3.0/aiida/orm/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,30 +191,14 @@
 
         """
         warn_deprecation(
             f'This method is deprecated, use `{cls.__name__}.collection.get` instead.', version=3, stacklevel=2
         )
         return cls.collection.get(**kwargs)  # pylint: disable=no-member
 
-    @classmethod
-    def from_backend_entity(cls: Type[EntityType], backend_entity: BackendEntityType) -> EntityType:
-        """Construct an entity from a backend entity instance
-
-        :param backend_entity: the backend entity
-
-        :return: an AiiDA entity instance
-        """
-        from .implementation.entities import BackendEntity
-
-        type_check(backend_entity, BackendEntity)
-        entity = cls.__new__(cls)
-        entity._backend_entity = backend_entity
-        call_with_super_check(entity.initialize)
-        return entity
-
     def __init__(self, backend_entity: BackendEntityType) -> None:
         """
         :param backend_entity: the backend model supporting this entity
         """
         self._backend_entity = backend_entity
         call_with_super_check(self.initialize)
 
@@ -267,7 +251,23 @@
         """Get the backend for this entity"""
         return self._backend_entity.backend
 
     @property
     def backend_entity(self) -> BackendEntityType:
         """Get the implementing class for this object"""
         return self._backend_entity
+
+
+def from_backend_entity(cls: Type[EntityType], backend_entity: BackendEntityType) -> EntityType:
+    """Construct an entity from a backend entity instance
+
+    :param backend_entity: the backend entity
+
+    :return: an AiiDA entity instance
+    """
+    from .implementation.entities import BackendEntity
+
+    type_check(backend_entity, BackendEntity)
+    entity = cls.__new__(cls)
+    entity._backend_entity = backend_entity  # pylint: disable=protected-access
+    call_with_super_check(entity.initialize)
+    return entity
```

### Comparing `aiida-core-2.2.2/aiida/orm/extras.py` & `aiida-core-2.3.0/aiida/orm/extras.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/groups.py` & `aiida-core-2.3.0/aiida/orm/groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         if entry_point_group is None or entry_point_group != 'aiida.groups':
             newcls._type_string = None  # type: ignore[attr-defined]
             message = f'no registered entry point for `{mod}:{name}` so its instances will not be storable.'
             warnings.warn(message)  # pylint: disable=no-member
         else:
             assert entry_point is not None
-            newcls._type_string = cast(str, entry_point.name)  # type: ignore[attr-defined]  # pylint: disable=protected-access
+            newcls._type_string = entry_point.name  # type: ignore[attr-defined]  # pylint: disable=protected-access
 
         return newcls
 
 
 class GroupCollection(entities.Collection['Group']):
     """Collection of Groups"""
 
@@ -249,15 +249,15 @@
         return self._backend_entity.type_string
 
     @property
     def user(self) -> 'User':
         """
         :return: the user associated with this group
         """
-        return users.User.from_backend_entity(self._backend_entity.user)
+        return entities.from_backend_entity(users.User, self._backend_entity.user)
 
     @user.setter
     def user(self, user: 'User') -> None:
         """Set the user.
 
         :param user: the user
         """
```

### Comparing `aiida-core-2.2.2/aiida/orm/implementation/__init__.py` & `aiida-core-2.3.0/aiida/orm/implementation/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/implementation/authinfos.py` & `aiida-core-2.3.0/aiida/orm/implementation/authinfos.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/implementation/comments.py` & `aiida-core-2.3.0/aiida/orm/implementation/comments.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/implementation/computers.py` & `aiida-core-2.3.0/aiida/orm/implementation/computers.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/implementation/entities.py` & `aiida-core-2.3.0/aiida/orm/implementation/entities.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/implementation/groups.py` & `aiida-core-2.3.0/aiida/orm/implementation/groups.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/implementation/logs.py` & `aiida-core-2.3.0/aiida/orm/implementation/logs.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/implementation/nodes.py` & `aiida-core-2.3.0/aiida/orm/implementation/nodes.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/implementation/querybuilder.py` & `aiida-core-2.3.0/aiida/orm/implementation/querybuilder.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/implementation/storage_backend.py` & `aiida-core-2.3.0/aiida/orm/implementation/storage_backend.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/implementation/users.py` & `aiida-core-2.3.0/aiida/orm/implementation/users.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/implementation/utils.py` & `aiida-core-2.3.0/aiida/orm/implementation/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/logs.py` & `aiida-core-2.3.0/aiida/orm/logs.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/__init__.py` & `aiida-core-2.3.0/aiida/orm/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/attributes.py` & `aiida-core-2.3.0/aiida/orm/nodes/attributes.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/caching.py` & `aiida-core-2.3.0/aiida/orm/nodes/caching.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/comments.py` & `aiida-core-2.3.0/aiida/orm/nodes/comments.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/__init__.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/array/__init__.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/array/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/array/array.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/array/array.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/array/bands.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/array/bands.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/array/kpoints.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/array/kpoints.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/array/projection.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/array/projection.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/array/trajectory.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/array/trajectory.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/array/xy.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/array/xy.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/base.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/base.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/bool.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/bool.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/cif.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/cif.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/code/abstract.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/code/abstract.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,39 +36,47 @@
     """Abstract data plugin representing an executable code."""
 
     # Should become ``default_calc_job_plugin`` once ``Code`` is dropped in ``aiida-core==3.0``
     _KEY_ATTRIBUTE_DEFAULT_CALC_JOB_PLUGIN: str = 'input_plugin'
     _KEY_ATTRIBUTE_APPEND_TEXT: str = 'append_text'
     _KEY_ATTRIBUTE_PREPEND_TEXT: str = 'prepend_text'
     _KEY_ATTRIBUTE_USE_DOUBLE_QUOTES: str = 'use_double_quotes'
+    _KEY_ATTRIBUTE_WITH_MPI: str = 'with_mpi'
+    _KEY_ATTRIBUTE_WRAP_CMDLINE_PARAMS: str = 'wrap_cmdline_params'
     _KEY_EXTRA_IS_HIDDEN: str = 'hidden'  # Should become ``is_hidden`` once ``Code`` is dropped
 
     def __init__(
         self,
         default_calc_job_plugin: str | None = None,
         append_text: str = '',
         prepend_text: str = '',
         use_double_quotes: bool = False,
+        with_mpi: bool | None = None,
         is_hidden: bool = False,
+        wrap_cmdline_params: bool = False,
         **kwargs
     ):
         """Construct a new instance.
 
         :param default_calc_job_plugin: The entry point name of the default ``CalcJob`` plugin to use.
         :param append_text: The text that should be appended to the run line in the job script.
         :param prepend_text: The text that should be prepended to the run line in the job script.
         :param use_double_quotes: Whether the command line invocation of this code should be escaped with double quotes.
+        :param with_mpi: Whether the command should be run as an MPI program.
+        :param wrap_cmdline_params: Whether to wrap the executable and all its command line parameters into quotes to
+            form a single string. This is required to enable support for Docker with the ``ContainerizedCode``.
         :param is_hidden: Whether the code is hidden.
         """
         super().__init__(**kwargs)
         self.default_calc_job_plugin = default_calc_job_plugin
         self.append_text = append_text
         self.prepend_text = prepend_text
         self.use_double_quotes = use_double_quotes
-        self.use_double_quotes = use_double_quotes
+        self.with_mpi = with_mpi
+        self.wrap_cmdline_params = wrap_cmdline_params
         self.is_hidden = is_hidden
 
     @abc.abstractmethod
     def can_run_on_computer(self, computer: Computer) -> bool:
         """Return whether the code can run on a given computer.
 
         :param computer: The computer.
@@ -218,14 +226,51 @@
 
         :param value: ``True`` if to escape with double quotes, ``False`` otherwise.
         """
         type_check(value, bool)
         self.base.attributes.set(self._KEY_ATTRIBUTE_USE_DOUBLE_QUOTES, value)
 
     @property
+    def with_mpi(self) -> bool | None:
+        """Return whether the command should be run as an MPI program.
+
+        :return: ``True`` if the code should be run as an MPI program, ``False`` if it shouldn't, ``None`` if unknown.
+        """
+        return self.base.attributes.get(self._KEY_ATTRIBUTE_WITH_MPI, None)
+
+    @with_mpi.setter
+    def with_mpi(self, value: bool | None) -> None:
+        """Set whether the command should be run as an MPI program.
+
+        :param value: ``True`` if the code should be run as an MPI program, ``False`` if it shouldn't, ``None`` if
+            unknown.
+        """
+        type_check(value, bool, allow_none=True)
+        self.base.attributes.set(self._KEY_ATTRIBUTE_WITH_MPI, value)
+
+    @property
+    def wrap_cmdline_params(self) -> bool:
+        """Return whether all command line parameters should be wrapped with double quotes to form a single argument.
+
+        ..note:: This is required to support certain containerization technologies, such as Docker.
+
+        :return: ``True`` if command line parameters should be wrapped, ``False`` otherwise.
+        """
+        return self.base.attributes.get(self._KEY_ATTRIBUTE_WRAP_CMDLINE_PARAMS, False)
+
+    @wrap_cmdline_params.setter
+    def wrap_cmdline_params(self, value: bool) -> None:
+        """Set whether all command line parameters should be wrapped with double quotes to form a single argument.
+
+        :param value: ``True`` if command line parameters should be wrapped, ``False`` otherwise.
+        """
+        type_check(value, bool)
+        self.base.attributes.set(self._KEY_ATTRIBUTE_WRAP_CMDLINE_PARAMS, value)
+
+    @property
     def is_hidden(self) -> bool:
         """Return whether the code is hidden.
 
         :return: ``True`` if the code is hidden, ``False`` otherwise, which is also the default.
         """
         return self.base.extras.get(self._KEY_EXTRA_IS_HIDDEN, False)
 
@@ -305,14 +350,31 @@
             },
             'default_calc_job_plugin': {
                 'short_name': '-P',
                 'type': click.STRING,
                 'prompt': 'Default `CalcJob` plugin',
                 'help': 'Entry point name of the default plugin (as listed in `verdi plugin list aiida.calculations`).'
             },
+            'use_double_quotes': {
+                'is_flag': True,
+                'default': False,
+                'help': 'Whether the executable and arguments of the code in the submission script should be escaped '
+                'with single or double quotes.',
+                'prompt': 'Escape using double quotes',
+            },
+            'with_mpi': {
+                'is_flag': True,
+                'default': None,
+                'help': (
+                    'Whether the executable should be run as an MPI program. This option can be left unspecified '
+                    'in which case `None` will be set and it is left up to the calculation job plugin or inputs '
+                    'whether to run with MPI.'
+                ),
+                'prompt': 'Run with MPI',
+            },
             'prepend_text': {
                 'cls': TemplateInteractiveOption,
                 'type': click.STRING,
                 'default': '',
                 'prompt': 'Prepend script',
                 'help': 'Bash commands that should be prepended to the run line in all submit scripts for this code.',
                 'extension': '.bash',
@@ -327,15 +389,8 @@
                 'prompt': 'Append script',
                 'help': 'Bash commands that should be appended to the run line in all submit scripts for this code.',
                 'extension': '.bash',
                 'header': 'APPEND_TEXT: if there is any bash commands that should be appended to the executable call '
                 'in all submit scripts for this code, type that between the equal signs below and save the file.',
                 'footer': 'All lines that start with `#=`: will be ignored.'
             },
-            'use_double_quotes': {
-                'is_flag': True,
-                'default': False,
-                'help': 'Whether the executable and arguments of the code in the submission script should be escaped '
-                'with single or double quotes.',
-                'prompt': 'Escape using double quotes',
-            },
         }
```

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/code/containerized.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/code/containerized.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,49 +54,48 @@
         :param value: The filepath of the executable.
         """
         type_check(value, str)
         self.base.attributes.set(self._KEY_ATTRIBUTE_FILEPATH_EXECUTABLE, value)
 
     @property
     def engine_command(self) -> str:
-        """Return the engine command with image as template field of the containerized code
+        """Return the engine command with image as template field of the containerized code.
 
         :return: The engine command of the containerized code
         """
         return self.base.attributes.get(self._KEY_ATTRIBUTE_ENGINE_COMMAND)
 
     @engine_command.setter
     def engine_command(self, value: str) -> None:
-        """Set the engine command of the containerized code
+        """Set the engine command of the containerized code.
 
         :param value: The engine command of the containerized code
         """
         type_check(value, str)
 
         if '{image_name}' not in value:
             raise ValueError("the '{image_name}' template field should be in engine command.")
 
         self.base.attributes.set(self._KEY_ATTRIBUTE_ENGINE_COMMAND, value)
 
     @property
     def image_name(self) -> str:
-        """The image name of container
+        """The image name of container.
 
         :return: The image name of container.
         """
         return self.base.attributes.get(self._KEY_ATTRIBUTE_IMAGE_NAME)
 
     @image_name.setter
     def image_name(self, value: str) -> None:
-        """Set the image name of container
+        """Set the image name of container.
 
         :param value: The image name of container.
         """
         type_check(value, str)
-
         self.base.attributes.set(self._KEY_ATTRIBUTE_IMAGE_NAME, value)
 
     def get_prepend_cmdline_params(
         self, mpi_args: list[str] | None = None, extra_mpirun_params: list[str] | None = None
     ) -> list[str]:
         """Return the list of prepend cmdline params for mpi seeting
 
@@ -121,11 +120,18 @@
             'image_name': {
                 'short_name': '-I',
                 'required': True,
                 'type': click.STRING,
                 'prompt': 'Image name',
                 'help': 'Name of the image container in which to the run the executable.',
             },
+            'wrap_cmdline_params': {
+                'is_flag': True,
+                'default': False,
+                'help': 'Whether all command line parameters to be passed to the engine command should be wrapped in '
+                'a double quotes to form a single argument. This should be set to `True` for Docker.',
+                'prompt': 'Wrap command line parameters',
+            }
         }
         options.update(**super()._get_cli_options())
 
         return options
```

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/code/installed.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/code/installed.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import click
 
 from aiida.cmdline.params.types import ComputerParamType
 from aiida.common import exceptions
 from aiida.common.lang import type_check
 from aiida.common.log import override_log_level
 from aiida.orm import Computer
+from aiida.orm.entities import from_backend_entity
 
 from .legacy import Code
 
 __all__ = ('InstalledCode',)
 
 
 class InstalledCode(Code):
@@ -64,17 +65,22 @@
     def validate_filepath_executable(self):
         """Validate the ``filepath_executable`` attribute.
 
         Checks whether the executable exists on the remote computer if a transport can be opened to it. This method
         is intentionally not called in ``_validate`` as to allow the creation of ``Code`` instances whose computers can
         not yet be connected to and as to not require the overhead of opening transports in storing a new code.
 
+        .. note:: If the ``filepath_executable`` is not an absolute path, the check is skipped.
+
         :raises `~aiida.common.exceptions.ValidationError`: if no transport could be opened or if the defined executable
             does not exist on the remote computer.
         """
+        if not self.filepath_executable.is_absolute():
+            return
+
         try:
             with override_log_level():  # Temporarily suppress noisy logging
                 with self.computer.get_transport() as transport:
                     file_exists = transport.isfile(str(self.filepath_executable))
         except Exception as exception:  # pylint: disable=broad-except
             raise exceptions.ValidationError(
                 'Could not connect to the configured computer to determine whether the specified executable exists.'
@@ -101,15 +107,15 @@
         """
         return self.filepath_executable
 
     @property  # type: ignore[override]
     def computer(self) -> Computer:
         """Return the computer of this code."""
         assert self.backend_entity.computer is not None
-        return Computer.from_backend_entity(self.backend_entity.computer)
+        return from_backend_entity(Computer, self.backend_entity.computer)
 
     @computer.setter
     def computer(self, computer: Computer) -> None:
         """Set the computer of this code.
 
         :param computer: A `Computer`.
         """
@@ -141,18 +147,14 @@
     @filepath_executable.setter
     def filepath_executable(self, value: str) -> None:
         """Set the absolute filepath of the executable that this code represents.
 
         :param value: The absolute filepath of the executable.
         """
         type_check(value, str)
-
-        if not pathlib.PurePosixPath(value).is_absolute():
-            raise ValueError('the `filepath_executable` should be absolute.')
-
         self.base.attributes.set(self._KEY_ATTRIBUTE_FILEPATH_EXECUTABLE, value)
 
     @staticmethod
     def cli_validate_label_uniqueness(ctx, _, value):
         """Validate the uniqueness of the label of the code."""
         from aiida.orm import load_code
```

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/code/legacy.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/code/legacy.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/code/portable.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/code/portable.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/data.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ###########################################################################
 """Module with `Node` sub class `Data` to be used as a base class for data structures."""
 from typing import Dict
 
 from aiida.common import exceptions
 from aiida.common.lang import override
 from aiida.common.links import LinkType
+from aiida.orm.entities import from_backend_entity
 
 from ..node import Node
 
 __all__ = ('Data',)
 
 
 class Data(Node):
@@ -66,15 +67,15 @@
         """Create a clone of the Data node.
 
         :returns: an unstored clone of this Data node
         """
         import copy
 
         backend_clone = self.backend_entity.clone()
-        clone = self.__class__.from_backend_entity(backend_clone)
+        clone = from_backend_entity(self.__class__, backend_clone)
         clone.base.attributes.reset(copy.deepcopy(self.base.attributes.all))
         clone.base.repository._clone(self.base.repository)  # pylint: disable=protected-access
 
         return clone
 
     @property
     def source(self):
```

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/dict.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/dict.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/enum.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/enum.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/float.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/float.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/folder.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/folder.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/int.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/int.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/jsonable.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/jsonable.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/list.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/list.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/numeric.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/numeric.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,7 +120,16 @@
         return other % self
 
     def __float__(self):
         return float(self.value)
 
     def __int__(self):
         return int(self.value)
+
+    def __pos__(self):
+        return self.value
+
+    def __neg__(self):
+        return self.new(-self.value)
+
+    def __abs__(self):
+        return abs(self.value)
```

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/orbital.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/orbital.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/remote/base.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/remote/base.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/remote/stash/base.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/remote/stash/base.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/remote/stash/folder.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/remote/stash/folder.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/singlefile.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/singlefile.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/str.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/str.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/structure.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1199,27 +1199,45 @@
             ``[ self.get_kind(s.kind_name).get_symbols_string() for s in self.sites]``
             for chemical symbols
 
         :return: a list of strings
         """
         return [this_site.kind_name for this_site in self.sites]
 
-    def get_composition(self):
+    def get_composition(self, mode='full'):
         """
         Returns the chemical composition of this structure as a dictionary,
         where each key is the kind symbol (e.g. H, Li, Ba),
         and each value is the number of occurences of that element in this
-        structure. For BaZrO3 it would return {'Ba':1, 'Zr':1, 'O':3}.
-        No reduction with smallest common divisor!
+        structure.
+
+        :param mode: Specify the mode of the composition to return. Choose from ``full``, ``reduced`` or ``fractional``.
+            For example, given the structure with formula Ba2Zr2O6, the various modes operate as follows.
+            ``full``: The default, the counts are left unnnormalized.
+            ``reduced``: The counts are renormalized to the greatest common denominator.
+            ``fractional``: The counts are renormalized such that the sum equals 1.
 
         :returns: a dictionary with the composition
         """
+        import numpy as np
         symbols_list = [self.get_kind(s.kind_name).get_symbols_string() for s in self.sites]
-        composition = {symbol: symbols_list.count(symbol) for symbol in set(symbols_list)}
-        return composition
+        symbols_set = set(symbols_list)
+
+        if mode == 'full':
+            return {symbol: symbols_list.count(symbol) for symbol in symbols_set}
+
+        if mode == 'reduced':
+            gcd = np.gcd.reduce([symbols_list.count(symbol) for symbol in symbols_set])
+            return {symbol: (symbols_list.count(symbol) / gcd) for symbol in symbols_set}
+
+        if mode == 'fractional':
+            sum_comp = sum(symbols_list.count(symbol) for symbol in symbols_set)
+            return {symbol: symbols_list.count(symbol) / sum_comp for symbol in symbols_set}
+
+        raise ValueError(f'mode `{mode}` is invalid, choose from `full`, `reduced` or `fractional`.')
 
     def get_ase(self):
         """
         Get the ASE object.
         Requires to be able to import ase.
 
         :return: an ASE object corresponding to this
```

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/data/upf.py` & `aiida-core-2.3.0/aiida/orm/nodes/data/upf.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/links.py` & `aiida-core-2.3.0/aiida/orm/nodes/links.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/node.py` & `aiida-core-2.3.0/aiida/orm/nodes/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from aiida.common.links import LinkType
 from aiida.common.warnings import warn_deprecation
 from aiida.manage import get_manager
 from aiida.orm.utils.node import AbstractNodeMeta
 
 from ..computers import Computer
 from ..entities import Collection as EntityCollection
-from ..entities import Entity
+from ..entities import Entity, from_backend_entity
 from ..extras import EntityExtras
 from ..querybuilder import QueryBuilder
 from ..users import User
 from .attributes import NodeAttributes
 from .caching import NodeCaching
 from .comments import NodeComments
 from .links import NodeLinks
@@ -354,15 +354,15 @@
         """
         self.backend_entity.description = value
 
     @property
     def computer(self) -> Optional[Computer]:
         """Return the computer of this node."""
         if self.backend_entity.computer:
-            return Computer.from_backend_entity(self.backend_entity.computer)
+            return from_backend_entity(Computer, self.backend_entity.computer)
 
         return None
 
     @computer.setter
     def computer(self, computer: Optional[Computer]) -> None:
         """Set the computer of this node.
 
@@ -374,15 +374,15 @@
         type_check(computer, Computer, allow_none=True)
 
         self.backend_entity.computer = None if computer is None else computer.backend_entity
 
     @property
     def user(self) -> User:
         """Return the user of this node."""
-        return User.from_backend_entity(self.backend_entity.user)
+        return from_backend_entity(User, self._backend_entity.user)
 
     @user.setter
     def user(self, user: User) -> None:
         """Set the user of this node.
 
         :param user: a `User`
         """
```

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/process/__init__.py` & `aiida-core-2.3.0/aiida/orm/nodes/process/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/process/calculation/__init__.py` & `aiida-core-2.3.0/aiida/orm/nodes/process/calculation/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/process/calculation/calcfunction.py` & `aiida-core-2.3.0/aiida/orm/nodes/process/calculation/calcfunction.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/process/calculation/calcjob.py` & `aiida-core-2.3.0/aiida/orm/nodes/process/calculation/calcjob.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,24 +98,20 @@
         if self._tools is None:
             entry_point_string = self.process_type
 
             if entry_point_string and is_valid_entry_point_string(entry_point_string):
                 entry_point = get_entry_point_from_string(entry_point_string)
 
                 try:
-                    tools_class = load_entry_point(
-                        'aiida.tools.calculations',
-                        entry_point.name  # type: ignore[attr-defined]
-                    )
+                    tools_class = load_entry_point('aiida.tools.calculations', entry_point.name)
                     self._tools = tools_class(self)
                 except exceptions.EntryPointError as exception:
                     self._tools = CalculationTools(self)
-                    entry_point_name = entry_point.name  # type: ignore[attr-defined]
                     self.logger.warning(
-                        f'could not load the calculation tools entry point {entry_point_name}: {exception}'
+                        f'could not load the calculation tools entry point {entry_point.name}: {exception}'
                     )
 
         return self._tools
 
     @classproperty
     def _updatable_attributes(cls) -> Tuple[str, ...]:  # pylint: disable=no-self-argument
         return super()._updatable_attributes + (
@@ -138,29 +134,14 @@
             'account',
             'qos',
             'priority',
             'max_wallclock_seconds',
             'max_memory_kb',
         )
 
-    def get_builder_restart(self) -> 'ProcessBuilder':
-        """Return a `ProcessBuilder` that is ready to relaunch the same `CalcJob` that created this node.
-
-        The process class will be set based on the `process_type` of this node and the inputs of the builder will be
-        prepopulated with the inputs registered for this node. This functionality is very useful if a process has
-        completed and you want to relaunch it with slightly different inputs.
-
-        In addition to prepopulating the input nodes, which is implemented by the base `ProcessNode` class, here we
-        also add the `options` that were passed in the `metadata` input of the `CalcJob` process.
-
-        """
-        builder = super().get_builder_restart()
-        builder.metadata.options = self.get_options()  # type: ignore[attr-defined]
-        return builder
-
     @property
     def is_imported(self) -> bool:
         """Return whether the calculation job was imported instead of being an actual run."""
         return self.base.attributes.get(self.IMMIGRATED_KEY, None) is True
 
     def get_option(self, name: str) -> Optional[Any]:
         """
```

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/process/calculation/calculation.py` & `aiida-core-2.3.0/aiida/orm/nodes/process/calculation/calculation.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/process/process.py` & `aiida-core-2.3.0/aiida/orm/nodes/process/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,14 +139,15 @@
     EXCEPTION_KEY = 'exception'
     EXIT_MESSAGE_KEY = 'exit_message'
     EXIT_STATUS_KEY = 'exit_status'
     PROCESS_PAUSED_KEY = 'paused'
     PROCESS_LABEL_KEY = 'process_label'
     PROCESS_STATE_KEY = 'process_state'
     PROCESS_STATUS_KEY = 'process_status'
+    METADATA_INPUTS_KEY: str = 'metadata_inputs'
 
     _unstorable_message = 'only Data, WorkflowNode, CalculationNode or their subclasses can be stored'
 
     def __str__(self) -> str:
         base = super().__str__()
         if self.process_type:
             return f'{base} ({self.process_type})'
@@ -163,14 +164,22 @@
             cls.EXIT_MESSAGE_KEY,
             cls.EXIT_STATUS_KEY,
             cls.PROCESS_LABEL_KEY,
             cls.PROCESS_STATE_KEY,
             cls.PROCESS_STATUS_KEY,
         )
 
+    def set_metadata_inputs(self, value: Dict[str, Any]) -> None:
+        """Set the mapping of inputs corresponding to ``metadata`` ports that were passed to the process."""
+        return self.base.attributes.set(self.METADATA_INPUTS_KEY, value)
+
+    def get_metadata_inputs(self) -> Optional[Dict[str, Any]]:
+        """Return the mapping of inputs corresponding to ``metadata`` ports that were passed to the process."""
+        return self.base.attributes.get(self.METADATA_INPUTS_KEY, None)
+
     @property
     def logger(self):
         """
         Get the logger of the Calculation object, so that it also logs to the DB.
 
         :return: LoggerAdapter object, that works like a logger, but also has the 'extra' embedded
         """
@@ -184,14 +193,15 @@
         prepopulated with the inputs registered for this node. This functionality is very useful if a process has
         completed and you want to relaunch it with slightly different inputs.
 
         :return: `~aiida.engine.processes.builder.ProcessBuilder` instance
         """
         builder = self.process_class.get_builder()
         builder._update(self.base.links.get_incoming(link_type=(LinkType.INPUT_CALC, LinkType.INPUT_WORK)).nested())  # pylint: disable=protected-access
+        builder._merge(self.get_metadata_inputs() or {})  # pylint: disable=protected-access
 
         return builder
 
     @property
     def process_class(self) -> Type['Process']:
         """Return the process class that was used to create this node.
 
@@ -205,25 +215,36 @@
             raise ValueError(f'no process type for Node<{self.pk}>: cannot recreate process class')
 
         try:
             process_class = load_entry_point_from_string(self.process_type)
         except exceptions.EntryPointError as exception:
             raise ValueError(
                 f'could not load process class for entry point `{self.process_type}` for Node<{self.pk}>: {exception}'
-            )
-        except ValueError:
-            try:
-                import importlib
-                module_name, class_name = self.process_type.rsplit('.', 1)
-                module = importlib.import_module(module_name)
-                process_class = getattr(module, class_name)
-            except (AttributeError, ValueError, ImportError) as exception:
+            ) from exception
+        except ValueError as exception:
+            import importlib
+
+            def str_rsplit_iter(string, sep='.'):
+                components = string.split(sep)
+                for idx in range(1, len(components)):
+                    yield sep.join(components[:-idx]), components[-idx:]
+
+            for module_name, class_names in str_rsplit_iter(self.process_type):
+                try:
+                    module = importlib.import_module(module_name)
+                    process_class = module
+                    for objname in class_names:
+                        process_class = getattr(process_class, objname)
+                    break
+                except (AttributeError, ValueError, ImportError):
+                    pass
+            else:
                 raise ValueError(
-                    f'could not load process class from `{self.process_type}` for Node<{self.pk}>: {exception}'
-                )
+                    f'could not load process class from `{self.process_type}` for Node<{self.pk}>'
+                ) from exception
 
         return process_class
 
     def set_process_type(self, process_type_string: str) -> None:
         """
         Set the process type string.
 
@@ -448,23 +469,23 @@
         """
         if not isinstance(exception, str):
             raise ValueError(f'exception message has to be a string type, got {type(exception)}')
 
         return self.base.attributes.set(self.EXCEPTION_KEY, exception)
 
     @property
-    def checkpoint(self) -> Optional[Dict[str, Any]]:
+    def checkpoint(self) -> Optional[str]:
         """
         Return the checkpoint bundle set for the process
 
         :returns: checkpoint bundle if it exists, None otherwise
         """
         return self.base.attributes.get(self.CHECKPOINT_KEY, None)
 
-    def set_checkpoint(self, checkpoint: Dict[str, Any]) -> None:
+    def set_checkpoint(self, checkpoint: str) -> None:
         """
         Set the checkpoint bundle set for the process
 
         :param state: string representation of the stepper state info
         """
         return self.base.attributes.set(self.CHECKPOINT_KEY, checkpoint)
```

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/process/workflow/__init__.py` & `aiida-core-2.3.0/aiida/orm/nodes/process/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/process/workflow/workchain.py` & `aiida-core-2.3.0/aiida/orm/nodes/process/workflow/workchain.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/process/workflow/workflow.py` & `aiida-core-2.3.0/aiida/orm/nodes/process/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/process/workflow/workfunction.py` & `aiida-core-2.3.0/aiida/orm/nodes/process/workflow/workfunction.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/nodes/repository.py` & `aiida-core-2.3.0/aiida/orm/nodes/repository.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/querybuilder.py` & `aiida-core-2.3.0/aiida/orm/querybuilder.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/users.py` & `aiida-core-2.3.0/aiida/orm/users.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/utils/__init__.py` & `aiida-core-2.3.0/aiida/orm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/utils/builders/__init__.py` & `aiida-core-2.3.0/aiida/orm/utils/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/utils/builders/code.py` & `aiida-core-2.3.0/aiida/orm/utils/builders/code.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/utils/builders/computer.py` & `aiida-core-2.3.0/aiida/orm/utils/builders/computer.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/utils/calcjob.py` & `aiida-core-2.3.0/aiida/orm/utils/calcjob.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/utils/links.py` & `aiida-core-2.3.0/aiida/orm/utils/links.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/utils/loaders.py` & `aiida-core-2.3.0/aiida/orm/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/utils/log.py` & `aiida-core-2.3.0/aiida/orm/utils/log.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/utils/managers.py` & `aiida-core-2.3.0/aiida/orm/utils/managers.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/utils/mixins.py` & `aiida-core-2.3.0/aiida/orm/utils/mixins.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/utils/node.py` & `aiida-core-2.3.0/aiida/orm/utils/node.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/utils/remote.py` & `aiida-core-2.3.0/aiida/orm/utils/remote.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/orm/utils/serialize.py` & `aiida-core-2.3.0/aiida/orm/utils/serialize.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,186 +10,143 @@
 """
 Serialisation functions for AiiDA types
 
 WARNING: Changing the representation of things here may break people's current saved e.g. things like
 checkpoints and messages in the RabbitMQ queue so do so with caution.  It is fine to add representers
 for new types though.
 """
+from __future__ import annotations
+
+from dataclasses import asdict, is_dataclass
 from enum import Enum
 from functools import partial
+import inspect
+from typing import Any, Protocol, Type, overload
 
-from plumpy import Bundle, get_object_loader
+from plumpy import Bundle, get_object_loader  # type: ignore[attr-defined]
 from plumpy.utils import AttributesFrozendict
 import yaml
 
 from aiida import orm
 from aiida.common import AttributeDict
 
 _ENUM_TAG = '!enum'
+_DATACLASS_TAG = '!dataclass'
 _NODE_TAG = '!aiida_node'
 _GROUP_TAG = '!aiida_group'
 _COMPUTER_TAG = '!aiida_computer'
 _ATTRIBUTE_DICT_TAG = '!aiida_attributedict'
 _PLUMPY_ATTRIBUTES_FROZENDICT_TAG = '!plumpy:attributes_frozendict'
 _PLUMPY_BUNDLE = '!plumpy:bundle'
 
 
-def represent_enum(dumper, enum):
-    """Represent an arbitrary enum in yaml.
-
-    :param dumper: the dumper to use.
-    :type dumper: :class:`yaml.dumper.Dumper`
-    :param bundle: the bundle to represent
-    :return: the representation
-    """
+def represent_enum(dumper: yaml.Dumper, enum: Enum) -> yaml.ScalarNode:
+    """Represent an arbitrary enum in yaml."""
     loader = get_object_loader()
     return dumper.represent_scalar(_ENUM_TAG, f'{loader.identify_object(enum)}|{enum.value}')
 
 
-def enum_constructor(loader, serialized):
-    """Construct an enum from the serialized representation.
-
-    :param loader: the yaml loader.
-    :type loader: :class:`yaml.loader.Loader`
-    :param bundle: the enum representation.
-    :return: the enum.
-    """
-    deserialized = loader.construct_scalar(serialized)
+def enum_constructor(loader: yaml.Loader, serialized: yaml.Node) -> Enum:
+    """Construct an enum from the serialized representation."""
+    deserialized: str = loader.construct_scalar(serialized)  # type: ignore[arg-type,assignment]
     identifier, value = deserialized.split('|')
     cls = get_object_loader().load_object(identifier)
     enum = cls(value)
     return enum
 
 
-def represent_node(dumper, node):
-    """Represent a node in yaml.
+def represent_dataclass(dumper: yaml.Dumper, obj: Any) -> yaml.MappingNode:
+    """Represent an arbitrary dataclass in yaml."""
+    loader = get_object_loader()
+    data = {
+        '__type__': loader.identify_object(obj.__class__),
+        '__fields__': asdict(obj),
+    }
+    return dumper.represent_mapping(_DATACLASS_TAG, data)
 
-    :param dumper: the dumper to use
-    :param node: the node to represent
-    :type node: :class:`aiida.orm.nodes.node.Node`
-    :return: the representation
-    """
+
+def dataclass_constructor(loader: yaml.Loader, serialized: yaml.Node) -> Any:
+    """Construct a dataclass from the serialized representation."""
+    deserialized = loader.construct_mapping(serialized, deep=True)  # type: ignore[arg-type]
+    identifier = deserialized['__type__']
+    cls = get_object_loader().load_object(identifier)
+    data = deserialized['__fields__']
+    return cls(**data)
+
+
+def represent_node(dumper: yaml.Dumper, node: orm.Node) -> yaml.ScalarNode:
+    """Represent a node in yaml."""
     if not node.is_stored:
         raise ValueError(f'node {type(node)}<{node.uuid}> cannot be represented because it is not stored')
     return dumper.represent_scalar(_NODE_TAG, f'{node.uuid}')
 
 
-def node_constructor(loader, node):
-    """Load a node from the yaml representation.
-
-    :param loader: the yaml loader
-    :param node: the yaml representation
-    :return: the aiida node
-    :rtype: :class:`aiida.orm.nodes.node.Node`
-    """
-    yaml_node = loader.construct_scalar(node)
+def node_constructor(loader: yaml.Loader, node: yaml.Node) -> orm.Node:
+    """Load a node from the yaml representation."""
+    yaml_node = loader.construct_scalar(node)  # type: ignore[arg-type]
     return orm.load_node(uuid=yaml_node)
 
 
-def represent_group(dumper, group):
-    """Represent a group in yaml.
-
-    :param dumper: the dumper to use
-    :param group: the group to represent
-    :type group: :class:`aiida.orm.Group`
-    :return: the representation
-    """
+def represent_group(dumper: yaml.Dumper, group: orm.Group) -> yaml.ScalarNode:
+    """Represent a group in yaml."""
     if not group.is_stored:
         raise ValueError(f'group {group} cannot be represented because it is not stored')
     return dumper.represent_scalar(_GROUP_TAG, f'{group.uuid}')
 
 
-def group_constructor(loader, group):
-    """Load a group from the yaml representation.
-
-    :param loader: the yaml loader
-    :param group: the yaml representation
-    :return: the aiida group
-    :rtype: :class:`aiida.orm.Group`
-    """
-    yaml_node = loader.construct_scalar(group)
+def group_constructor(loader: yaml.Loader, group: yaml.Node) -> orm.Group:
+    """Load a group from the yaml representation."""
+    yaml_node = loader.construct_scalar(group)  # type: ignore[arg-type]
     return orm.load_group(uuid=yaml_node)
 
 
-def represent_computer(dumper, computer):
-    """Represent a computer in yaml.
-
-    :param dumper: the dumper to use
-    :param computer: the computer to represent
-    :type computer: :class:`aiida.orm.Computer`
-    :return: the representation
-    """
+def represent_computer(dumper: yaml.Dumper, computer: orm.Computer) -> yaml.ScalarNode:
+    """Represent a computer in yaml."""
     if not computer.is_stored:
         raise ValueError(f'computer {computer} cannot be represented because it is not stored')
     return dumper.represent_scalar(_COMPUTER_TAG, f'{computer.uuid}')
 
 
-def computer_constructor(loader, computer):
-    """Load a computer from the yaml representation.
-
-    :param loader: the yaml loader
-    :param computer: the yaml representation
-    :return: the aiida computer
-    :rtype: :class:`aiida.orm.Computer`
-    """
-    yaml_node = loader.construct_scalar(computer)
+def computer_constructor(loader: yaml.Loader, computer: yaml.Node) -> orm.Computer:
+    """Load a computer from the yaml representation."""
+    yaml_node = loader.construct_scalar(computer)  # type: ignore[arg-type]
     return orm.Computer.collection.get(uuid=yaml_node)
 
 
-def represent_mapping(tag, dumper, mapping):
-    """Represent a mapping in yaml.
-
-    :param tag: the yaml tag to use
-    :param dumper: the dumper to use
-    :type dumper: :class:`yaml.dumper.Dumper`
-    :param mapping: the mapping to represent
-    :return: the representation
-    """
+def represent_mapping(tag: str, dumper: yaml.Dumper, mapping: Any) -> yaml.MappingNode:
+    """Represent a mapping in yaml."""
     return dumper.represent_mapping(tag, mapping)
 
 
-def mapping_constructor(mapping_type, loader, mapping):
-    """Construct a mapping from the representation.
+class _MappingType(Protocol):
 
-    :param mapping_type: the class of the mapping to construct, must accept a dictionary as a sole constructor argument
-        to be compatible.
-    :param loader: the yaml loader
-    :type loader: :class:`yaml.loader.Loader`
-    :param mapping: the mapping representation
-    :return: the reconstructed mapping
-    """
+    def __init__(self, mapping: dict) -> None:  # pylint: disable=super-init-not-called
+        ...
+
+
+def mapping_constructor(
+    mapping_type: Type[_MappingType], loader: yaml.Loader, mapping: yaml.MappingNode
+) -> _MappingType:
+    """Construct a mapping from the representation."""
     yaml_node = loader.construct_mapping(mapping, deep=True)
     return mapping_type(yaml_node)
 
 
-def represent_bundle(dumper, bundle):
-    """Represent an `plumpy.Bundle` in yaml
-
-    :param tag: the yaml  tag to use
-    :param dumper: the dumper to use
-    :type dumper: :class:`yaml.dumper.Dumper`
-    :param bundle: the bundle to represent
-    :return: the representation
-    """
+def represent_bundle(dumper: yaml.Dumper, bundle: Bundle) -> yaml.MappingNode:
+    """Represent an `plumpy.Bundle` in yaml."""
     as_dict = dict(bundle)
     return dumper.represent_mapping(_PLUMPY_BUNDLE, as_dict)
 
 
-def bundle_constructor(loader, bundle):
-    """Construct an `plumpy.Bundle` from the representation
-
-    :param loader: the yaml loader
-    :type loader: :class:`yaml.loader.Loader`
-    :param bundle: the bundle representation
-    :return: the mapping type
-    """
-    yaml_node = loader.construct_mapping(bundle)
-    bundle = Bundle.__new__(Bundle)
-    bundle.update(yaml_node)
-    return bundle
+def bundle_constructor(loader: yaml.Loader, bundle: yaml.Node) -> Bundle:
+    """Construct an `plumpy.Bundle` from the representation."""
+    yaml_node = loader.construct_mapping(bundle)  # type: ignore[arg-type]
+    bundle_inst = Bundle.__new__(Bundle)
+    bundle_inst.update(yaml_node)
+    return bundle_inst
 
 
 class AiiDADumper(yaml.Dumper):
     """Custom AiiDA yaml dumper.
 
     Needed so that we don't have to encode each type in the AiiDA graph hierarchy separately using a custom representer.
     """
@@ -197,14 +154,16 @@
     def represent_data(self, data):
         if isinstance(data, orm.Node):
             return represent_node(self, data)
         if isinstance(data, orm.Computer):
             return represent_computer(self, data)
         if isinstance(data, orm.Group):
             return represent_group(self, data)
+        if is_dataclass(data) and not inspect.isclass(data):
+            return represent_dataclass(self, data)
 
         return super().represent_data(data)
 
 
 class AiiDALoader(yaml.Loader):
     """AiiDA specific yaml loader
 
@@ -224,17 +183,28 @@
     _PLUMPY_ATTRIBUTES_FROZENDICT_TAG, partial(mapping_constructor, AttributesFrozendict), Loader=AiiDALoader
 )
 yaml.add_constructor(_PLUMPY_BUNDLE, bundle_constructor, Loader=AiiDALoader)
 yaml.add_constructor(_NODE_TAG, node_constructor, Loader=AiiDALoader)
 yaml.add_constructor(_GROUP_TAG, group_constructor, Loader=AiiDALoader)
 yaml.add_constructor(_COMPUTER_TAG, computer_constructor, Loader=AiiDALoader)
 yaml.add_constructor(_ENUM_TAG, enum_constructor, Loader=AiiDALoader)
+yaml.add_constructor(_DATACLASS_TAG, dataclass_constructor, Loader=AiiDALoader)
+
+
+@overload
+def serialize(data: Any, encoding: None = None) -> str:
+    ...
+
+
+@overload
+def serialize(data: Any, encoding: str) -> bytes:
+    ...
 
 
-def serialize(data, encoding=None):
+def serialize(data: Any, encoding: str | None = None) -> str | bytes:
     """Serialize the given data structure into a yaml dump.
 
     The function supports standard data containers such as maps and lists as well as AiiDA nodes which will be
     serialized into strings, before the whole data structure is dumped into a string using yaml.
 
     :param data: the general data to serialize
     :param encoding: optional encoding for the serialized string
@@ -244,15 +214,15 @@
         serialized = yaml.dump(data, encoding=encoding, Dumper=AiiDADumper)
     else:
         serialized = yaml.dump(data, Dumper=AiiDADumper)
 
     return serialized
 
 
-def deserialize_unsafe(serialized):
+def deserialize_unsafe(serialized: str) -> Any:
     """Deserialize a yaml dump that represents a serialized data structure.
 
     .. note:: This function should not be used on untrusted input, since it is built upon `yaml.Loader` which is unsafe.
 
     :param serialized: a yaml serialized string representation
     :return: the deserialized data structure
     """
```

### Comparing `aiida-core-2.2.2/aiida/parsers/__init__.py` & `aiida-core-2.3.0/aiida/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/parsers/parser.py` & `aiida-core-2.3.0/aiida/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/parsers/plugins/__init__.py` & `aiida-core-2.3.0/aiida/parsers/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/parsers/plugins/arithmetic/__init__.py` & `aiida-core-2.3.0/aiida/parsers/plugins/arithmetic/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/parsers/plugins/arithmetic/add.py` & `aiida-core-2.3.0/aiida/parsers/plugins/arithmetic/add.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/parsers/plugins/diff_tutorial/parsers.py` & `aiida-core-2.3.0/aiida/parsers/plugins/diff_tutorial/parsers.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/parsers/plugins/templatereplacer/__init__.py` & `aiida-core-2.3.0/aiida/parsers/plugins/templatereplacer/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/parsers/plugins/templatereplacer/parser.py` & `aiida-core-2.3.0/aiida/parsers/plugins/templatereplacer/parser.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/plugins/__init__.py` & `aiida-core-2.3.0/aiida/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/plugins/entry_point.py` & `aiida-core-2.3.0/aiida/plugins/entry_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,16 +158,16 @@
     :raises ValueError: if the entry_point_string cannot be split into two parts on the entry point string separator
     """
     if not isinstance(entry_point_string, str):
         raise TypeError('the entry_point_string should be a string')
 
     try:
         group, name = entry_point_string.split(ENTRY_POINT_STRING_SEPARATOR)
-    except ValueError:
-        raise ValueError('invalid entry_point_string format')
+    except ValueError as exc:
+        raise ValueError(f'invalid entry_point_string format: {entry_point_string}') from exc
 
     return group, name
 
 
 def get_entry_point_string_format(entry_point_string: str) -> EntryPointFormat:
     """
     Determine the format of an entry point string. Note that it does not validate the actual entry point
@@ -353,15 +353,15 @@
     :param class_module: module of the class
     :param class_name: name of the class
     :return: the corresponding entry point string or None
     """
     group, entry_point = get_entry_point_from_class(class_module, class_name)
 
     if group and entry_point:
-        return ENTRY_POINT_STRING_SEPARATOR.join([group, entry_point.name])  # type: ignore[attr-defined]
+        return ENTRY_POINT_STRING_SEPARATOR.join([group, entry_point.name])
     return None
 
 
 def is_valid_entry_point_string(entry_point_string: str) -> bool:
     """
     Verify whether the given entry point string is a valid one. For the string to be valid means that it is composed
     of two strings, the entry point group and name, concatenated by the entry point string separator. If that is the
```

### Comparing `aiida-core-2.2.2/aiida/plugins/factories.py` & `aiida-core-2.3.0/aiida/plugins/factories.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/plugins/utils.py` & `aiida-core-2.3.0/aiida/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/repository/__init__.py` & `aiida-core-2.3.0/aiida/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/repository/backend/abstract.py` & `aiida-core-2.3.0/aiida/repository/backend/abstract.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/repository/backend/disk_object_store.py` & `aiida-core-2.3.0/aiida/repository/backend/disk_object_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         :param do_repack:flag for forcing the re-packing of already packed files.
         :param clean_storage:flag for forcing the cleaning of soft-deleted files from the repository.
         :param do_vacuum:flag for forcing the vacuuming of the internal database when cleaning the repository.
         :return:a dictionary with information on the operations performed.
         """
         if live and (do_repack or clean_storage or do_vacuum):
             overrides = {'do_repack': do_repack, 'clean_storage': clean_storage, 'do_vacuum': do_vacuum}
-            keys = ', '.join([key for key, override in overrides if override is True])  # type: ignore
+            keys = ', '.join([key for key, override in overrides.items() if override is True])  # type: ignore
             raise ValueError(f'The following overrides were enabled but cannot be if `live=True`: {keys}')
 
         pack_loose = True if pack_loose is None else pack_loose
 
         if live:
             do_repack = False
             clean_storage = False
```

### Comparing `aiida-core-2.2.2/aiida/repository/backend/sandbox.py` & `aiida-core-2.3.0/aiida/repository/backend/sandbox.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/repository/common.py` & `aiida-core-2.3.0/aiida/repository/common.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/repository/repository.py` & `aiida-core-2.3.0/aiida/repository/repository.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/__init__.py` & `aiida-core-2.3.0/aiida/restapi/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/api.py` & `aiida-core-2.3.0/aiida/restapi/api.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/common/__init__.py` & `aiida-core-2.3.0/aiida/restapi/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/common/config.py` & `aiida-core-2.3.0/aiida/restapi/common/config.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/common/exceptions.py` & `aiida-core-2.3.0/aiida/restapi/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/common/identifiers.py` & `aiida-core-2.3.0/aiida/restapi/common/identifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,22 +185,26 @@
         'node.process.workflow.workchain': 'Work chain',
         'node.process.workflow.workfunction': 'Work function',
     }
 
     # This is a hard-coded mapping to generate the correct full types for process node namespaces of external
     # plugins. The `node_type` in that case is fixed and the `process_type` should start with the entry point group
     # followed by the plugin name and the wildcard.
+    # yapf: disable
     process_full_type_mapping = {
-        'process.calculation.calcjob.': 'process.calculation.calcjob.CalcJobNode.|aiida.calculations:{plugin_name}.%',
+        'process.calculation.calcjob.':
+        'process.calculation.calcjob.CalcJobNode.|aiida.calculations:{plugin_name}.%',
         'process.calculation.calcfunction.':
         'process.calculation.calcfunction.CalcFunctionNode.|aiida.calculations:{plugin_name}.%',
         'process.workflow.workfunction.':
         'process.workflow.workfunction.WorkFunctionNode.|aiida.workflows:{plugin_name}.%',
-        'process.workflow.workchain.': 'process.workflow.workchain.WorkChainNode.|aiida.workflows:{plugin_name}.%',
+        'process.workflow.workchain.':
+        'process.workflow.workchain.WorkChainNode.|aiida.workflows:{plugin_name}.%',
     }
+    # yapf: enable
 
     process_full_type_mapping_unplugged = {
         'process.calculation.calcjob.': 'process.calculation.calcjob.CalcJobNode.|{plugin_name}.%',
         'process.calculation.calcfunction.': 'process.calculation.calcfunction.CalcFunctionNode.|{plugin_name}.%',
         'process.workflow.workfunction.': 'process.workflow.workfunction.WorkFunctionNode.|{plugin_name}.%',
         'process.workflow.workchain.': 'process.workflow.workchain.WorkChainNode.|{plugin_name}.%',
     }
```

### Comparing `aiida-core-2.2.2/aiida/restapi/common/utils.py` & `aiida-core-2.3.0/aiida/restapi/common/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/resources.py` & `aiida-core-2.3.0/aiida/restapi/resources.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/run_api.py` & `aiida-core-2.3.0/aiida/restapi/run_api.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/__init__.py` & `aiida-core-2.3.0/aiida/restapi/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/base.py` & `aiida-core-2.3.0/aiida/restapi/translator/base.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/computer.py` & `aiida-core-2.3.0/aiida/restapi/translator/computer.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/group.py` & `aiida-core-2.3.0/aiida/restapi/translator/group.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/__init__.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/data/__init__.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/data/array/__init__.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/data/array/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/data/array/bands.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/data/array/bands.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/data/cif.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/data/cif.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/data/code.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/data/code.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/data/kpoints.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/data/kpoints.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/data/structure.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/data/structure.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/data/upf.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/data/upf.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/node.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/node.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/process/__init__.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/process/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/process/calculation/__init__.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/process/calculation/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/process/calculation/calcfunction.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/process/calculation/calcfunction.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/process/calculation/calcjob.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/process/calculation/calcjob.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/process/process.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/process/process.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/process/workflow/__init__.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/process/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/process/workflow/workchain.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/process/workflow/workchain.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/nodes/process/workflow/workfunction.py` & `aiida-core-2.3.0/aiida/restapi/translator/nodes/process/workflow/workfunction.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/restapi/translator/user.py` & `aiida-core-2.3.0/aiida/restapi/translator/user.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/schedulers/__init__.py` & `aiida-core-2.3.0/aiida/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/schedulers/datastructures.py` & `aiida-core-2.3.0/aiida/schedulers/datastructures.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,15 @@
       * ``submit_as_hold``: if set, the job will be in a 'hold' status right
         after the submission
       * ``rerunnable``: if the job is rerunnable (boolean)
       * ``job_environment``: a dictionary with environment variables to set
         before the execution of the code.
       * ``environment_variables_double_quotes``: if set to True, use double quotes
         instead of single quotes to escape the environment variables specified
-        in ``environment_variables``.
+        in ``job_environment``.
       * ``working_directory``: the working directory for this job. During
         submission, the transport will first do a 'chdir' to this directory,
         and then possibly set a scheduler parameter, if this is supported
         by the scheduler.
       * ``email``: an email address for sending emails on job events.
       * ``email_on_started``: if True, ask the scheduler to send an email when the
         job starts.
@@ -375,22 +375,27 @@
     `Scheduler.get_submit_script` will pass a list of these objects to `Scheduler._get_run_line` which
     should build up the code execution line based on the parameters specified in this dataclass.
 
     :param preprend_cmdline_params: list of unescaped command line arguments that are to be prepended to the executable.
     :param cmdline_params: list of unescaped command line parameters.
     :param use_double_quotes: list of two booleans. If true, use double quotes to escape command line arguments. The
         first value applies to `prepend_cmdline_params` and the second to `cmdline_params`.
+    :param wrap_cmdline_params: Boolean, by default ``False``. If set to ``True``, all the command line arguments,
+        which includes the ``cmdline_params`` but also all file descriptor redirections (stdin, stderr and stdoout),
+        should be wrapped in double quotes, turning it into a single command line argument. This is necessary to enable
+        support for certain containerization technologies such as Docker.
     :param stdin_name: filename of the the stdin file descriptor.
     :param stdout_name: filename of the the `stdout` file descriptor.
     :param stderr_name: filename of the the `stderr` file descriptor.
     :param join_files: boolean, if true, `stderr` should be redirected to `stdout`.
     """
     prepend_cmdline_params: list[str] = field(default_factory=list)
     cmdline_params: list[str] = field(default_factory=list)
     use_double_quotes: list[bool] = field(default_factory=lambda: [False, False])
+    wrap_cmdline_params: bool = False
     stdin_name: None | str = None
     stdout_name: None | str = None
     stderr_name: None | str = None
     join_files: bool = False
 
 
 class MachineInfo(DefaultFieldsAttributeDict):
```

### Comparing `aiida-core-2.2.2/aiida/schedulers/plugins/__init__.py` & `aiida-core-2.3.0/aiida/schedulers/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/schedulers/plugins/direct.py` & `aiida-core-2.3.0/aiida/schedulers/plugins/direct.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,17 +156,14 @@
 
         if job_tmpl.custom_scheduler_commands:
             lines.append(job_tmpl.custom_scheduler_commands)
 
         if job_tmpl.job_resource and job_tmpl.job_resource.num_cores_per_mpiproc:
             lines.append(f'export OMP_NUM_THREADS={job_tmpl.job_resource.num_cores_per_mpiproc}')
 
-        if job_tmpl.job_environment:
-            lines.append(self._get_submit_script_environment_variables(job_tmpl))
-
         if job_tmpl.rerunnable:
             self.logger.warning(
                 "The 'rerunnable' option is set to 'True', but has no effect when using the direct scheduler."
             )
 
         lines.append(empty_line)
```

### Comparing `aiida-core-2.2.2/aiida/schedulers/plugins/lsf.py` & `aiida-core-2.3.0/aiida/schedulers/plugins/lsf.py`

 * *Files 2% similar despite different names*

```diff
@@ -435,17 +435,14 @@
             # The -M option sets a per-process (soft) memory limit for all the
             # processes that belong to this job
             lines.append(f'#BSUB -M {physical_memory_kb}')
 
         if job_tmpl.custom_scheduler_commands:
             lines.append(job_tmpl.custom_scheduler_commands)
 
-        if job_tmpl.job_environment:
-            lines.append(self._get_submit_script_environment_variables(job_tmpl))
-
         # The following seems to be the only way to copy the input files
         # to the node where the computation are actually launched (the
         # -f option of bsub that does not always work...)
         # TODO: implement the case when LSB_OUTDIR is not properly defined...  # pylint: disable=fixme
         # (need to add the line "#BSUB -outdir PATH_TO_REMOTE_DIRECTORY")
         # IMPORTANT! the -z is needed, because if LSB_OUTDIR is not defined,
         # you would do 'cp -R /* .' basically copying ALL FILES in your
```

### Comparing `aiida-core-2.2.2/aiida/schedulers/plugins/pbsbaseclasses.py` & `aiida-core-2.3.0/aiida/schedulers/plugins/pbsbaseclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,17 +293,14 @@
         )
 
         lines += resource_lines
 
         if job_tmpl.custom_scheduler_commands:
             lines.append(job_tmpl.custom_scheduler_commands)
 
-        if job_tmpl.job_environment:
-            lines.append(self._get_submit_script_environment_variables(job_tmpl))
-
         # Required to change directory to the working directory, that is
         # the one from which the job was submitted
         lines.append('cd "$PBS_O_WORKDIR"')
         lines.append(empty_line)
 
         return '\n'.join(lines)
```

### Comparing `aiida-core-2.2.2/aiida/schedulers/plugins/pbspro.py` & `aiida-core-2.3.0/aiida/schedulers/plugins/pbspro.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
         return_lines = []
 
         select_string = f'select={num_machines}'
         if num_mpiprocs_per_machine:
             select_string += f':mpiprocs={num_mpiprocs_per_machine}'
         if num_cores_per_machine:
-            select_string += f':ppn={num_cores_per_machine}'
+            select_string += f':ncpus={num_cores_per_machine}'
 
         if max_wallclock_seconds is not None:
             try:
                 tot_secs = int(max_wallclock_seconds)
                 if tot_secs <= 0:
                     raise ValueError
             except ValueError:
```

### Comparing `aiida-core-2.2.2/aiida/schedulers/plugins/sge.py` & `aiida-core-2.3.0/aiida/schedulers/plugins/sge.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,17 +261,14 @@
             minutes = tot_minutes // 60
             seconds = tot_minutes % 60
             lines.append(f'#$ -l h_rt={hours:02d}:{minutes:02d}:{seconds:02d}')
 
         if job_tmpl.custom_scheduler_commands:
             lines.append(job_tmpl.custom_scheduler_commands)
 
-        if job_tmpl.job_environment:
-            lines.append(self._get_submit_script_environment_variables(job_tmpl))
-
         return '\n'.join(lines)
 
     def _get_submit_command(self, submit_script):
         """
         Return the string to execute to submit a given script.
 
         Args:
```

### Comparing `aiida-core-2.2.2/aiida/schedulers/plugins/slurm.py` & `aiida-core-2.3.0/aiida/schedulers/plugins/slurm.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,17 +389,14 @@
             # --mem: Specify the real memory required per node in MegaBytes.
             # --mem and  --mem-per-cpu  are  mutually exclusive.
             lines.append(f'#SBATCH --mem={physical_memory_kb // 1024}')
 
         if job_tmpl.custom_scheduler_commands:
             lines.append(job_tmpl.custom_scheduler_commands)
 
-        if job_tmpl.job_environment:
-            lines.append(self._get_submit_script_environment_variables(job_tmpl))
-
         return '\n'.join(lines)
 
     def _get_submit_command(self, submit_script):
         """
         Return the string to execute to submit a given script.
 
         Args:
@@ -418,16 +415,22 @@
         Parse the output of the submit command, as returned by executing the
         command returned by _get_submit_command command.
 
         To be implemented by the plugin.
 
         Return a string with the JobID.
         """
+        from aiida.engine import CalcJob
+
         if retval != 0:
             self.logger.error(f'Error in _parse_submit_output: retval={retval}; stdout={stdout}; stderr={stderr}')
+
+            if 'Invalid account' in stderr:
+                return CalcJob.exit_codes.ERROR_SCHEDULER_INVALID_ACCOUNT
+
             raise SchedulerError(f'Error during submission, retval={retval}\nstdout={stdout}\nstderr={stderr}')
 
         try:
             transport_string = f' for {self.transport}'
         except SchedulerError:
             transport_string = ''
 
@@ -757,14 +760,17 @@
 
             if data['State'] == 'OUT_OF_MEMORY':
                 return CalcJob.exit_codes.ERROR_SCHEDULER_OUT_OF_MEMORY
 
             if data['State'] == 'TIMEOUT':
                 return CalcJob.exit_codes.ERROR_SCHEDULER_OUT_OF_WALLTIME
 
+            if data['State'] == 'NODE_FAIL':
+                return CalcJob.exit_codes.ERROR_SCHEDULER_NODE_FAILURE
+
         # Alternatively, if the ``detailed_job_info`` is not defined or hasn't already determined an error, try to match
         # known error messages from the output written to the ``stderr`` descriptor.
         if stderr is not None:
 
             type_check(stderr, str)
             stderr_lower = stderr.lower()
```

### Comparing `aiida-core-2.2.2/aiida/schedulers/plugins/torque.py` & `aiida-core-2.3.0/aiida/schedulers/plugins/torque.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/schedulers/scheduler.py` & `aiida-core-2.3.0/aiida/schedulers/scheduler.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,26 @@
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 """Implementation of `Scheduler` base class."""
+from __future__ import annotations
+
 import abc
-from typing import Dict, Type
+import typing as t
 
-from aiida.common import exceptions, log
+from aiida.common import exceptions, log, warnings
+from aiida.common.datastructures import CodeRunMode
 from aiida.common.escaping import escape_for_bash
 from aiida.common.lang import classproperty
-from aiida.schedulers.datastructures import JobResource, JobTemplate
+from aiida.engine.processes.exit_code import ExitCode
+from aiida.schedulers.datastructures import JobInfo, JobResource, JobTemplate, JobTemplateCodeInfo
+from aiida.transports import Transport
 
 __all__ = ('Scheduler', 'SchedulerError', 'SchedulerParsingError')
 
 
 class SchedulerError(exceptions.AiidaException):
     pass
 
@@ -33,56 +38,55 @@
     _logger = log.AIIDA_LOGGER.getChild('scheduler')
 
     # A list of features
     # Features that should be defined in the plugins:
     # 'can_query_by_user': True if I can pass the 'user' argument to
     # get_joblist_command (and in this case, no 'jobs' should be given).
     # Otherwise, if False, a list of jobs is passed, and no 'user' is given.
-    _features: Dict[str, bool] = {}
+    _features: dict[str, bool] = {}
 
     # The class to be used for the job resource.
-    _job_resource_class: Type[JobResource] = None  # type: ignore
+    _job_resource_class: t.Type[JobResource] | None = None
 
     def __str__(self):
         return self.__class__.__name__
 
     @classmethod
-    def preprocess_resources(cls, resources, default_mpiprocs_per_machine=None):
+    def preprocess_resources(cls, resources: dict[str, t.Any], default_mpiprocs_per_machine: int | None = None):
         """Pre process the resources.
 
         Add the `num_mpiprocs_per_machine` key to the `resources` if it is not already defined and it cannot be deduced
         from the `num_machines` and `tot_num_mpiprocs` being defined. The value is also not added if the job resource
         class of this scheduler does not accept the `num_mpiprocs_per_machine` keyword. Note that the changes are made
         in place to the `resources` argument passed.
         """
-        num_machines = resources.get('num_machines', None)
-        tot_num_mpiprocs = resources.get('tot_num_mpiprocs', None)
-        num_mpiprocs_per_machine = resources.get('num_mpiprocs_per_machine', None)
+        num_machines: int | None = resources.get('num_machines', None)
+        tot_num_mpiprocs: int | None = resources.get('tot_num_mpiprocs', None)
+        num_mpiprocs_per_machine: int | None = resources.get('num_mpiprocs_per_machine', None)
 
         if (
             num_mpiprocs_per_machine is None and cls.job_resource_class.accepts_default_mpiprocs_per_machine()  # pylint: disable=no-member
             and (num_machines is None or tot_num_mpiprocs is None)
         ):
             resources['num_mpiprocs_per_machine'] = default_mpiprocs_per_machine
 
     @classmethod
     def validate_resources(cls, **resources):
         """Validate the resources against the job resource class of this scheduler.
 
         :param resources: keyword arguments to define the job resources
         :raises ValueError: if the resources are invalid or incomplete
         """
+        assert cls._job_resource_class is not None and issubclass(cls._job_resource_class, JobResource)
         cls._job_resource_class.validate_resources(**resources)
 
     def __init__(self):
+        assert self._job_resource_class is not None and issubclass(self._job_resource_class, JobResource)
         self._transport = None
 
-        if not issubclass(self._job_resource_class, JobResource):
-            raise RuntimeError('the class attribute `_job_resource_class` is not a subclass of `JobResource`.')
-
     @classmethod
     def get_short_doc(cls):
         """Return the first non-empty line of the class docstring, if available."""
         # Remove empty lines
         docstring = cls.__doc__
         if not docstring:
             return 'No documentation available'
@@ -104,24 +108,25 @@
         """Return the internal logger."""
         try:
             return self._logger
         except AttributeError:
             raise exceptions.InternalError('No self._logger configured for {}!')
 
     @classproperty
-    def job_resource_class(cls) -> Type[JobResource]:  # pylint: disable=no-self-argument
+    def job_resource_class(cls) -> t.Type[JobResource]:  # pylint: disable=no-self-argument
+        assert cls._job_resource_class is not None and issubclass(cls._job_resource_class, JobResource)
         return cls._job_resource_class
 
     @classmethod
     def create_job_resource(cls, **kwargs):
         """Create a suitable job resource from the kwargs specified."""
-        # pylint: disable=not-callable
-        return cls._job_resource_class(**kwargs)
+        assert cls._job_resource_class is not None and issubclass(cls._job_resource_class, JobResource)
+        return cls._job_resource_class(**kwargs)  # pylint: disable=not-callable
 
-    def get_submit_script(self, job_tmpl):
+    def get_submit_script(self, job_tmpl: JobTemplate) -> str:
         """Return the submit script as a string.
 
         :parameter job_tmpl: a `aiida.schedulers.datastrutures.JobTemplate` instance.
 
         The plugin returns something like
 
         #!/bin/bash <- this shebang line is configurable to some extent
@@ -146,36 +151,49 @@
             # Here I check whether the shebang was set explicitly as an empty line.
             # In such a case, the first line is empty, if that's what the user wants:
             script_lines.append(job_tmpl.shebang)
         elif job_tmpl.shebang is None:
             script_lines.append('#!/bin/bash')
         else:
             raise ValueError(f'Invalid shebang set: {job_tmpl.shebang}')
-        script_lines.append(self._get_submit_script_header(job_tmpl))
+
+        script_header = self._get_submit_script_header(job_tmpl)
+        script_lines.append(script_header)
         script_lines.append(empty_line)
 
+        if '# ENVIRONMENT VARIABLES BEGIN ###' in script_header:
+            warnings.warn_deprecation(
+                f'Environment variables added by `{self.__class__.__name__}._get_submit_script_environment_variables`, '
+                'however, this is no longer necessary and automatically done by the base `Scheduler` class.',
+                version=3
+            )
+
+        if job_tmpl.job_environment:
+            script_lines.append(self._get_submit_script_environment_variables(job_tmpl))
+            script_lines.append(empty_line)
+
         if job_tmpl.prepend_text:
             script_lines.append(job_tmpl.prepend_text)
             script_lines.append(empty_line)
 
         script_lines.append(self._get_run_line(job_tmpl.codes_info, job_tmpl.codes_run_mode))
         script_lines.append(empty_line)
 
         if job_tmpl.append_text:
             script_lines.append(job_tmpl.append_text)
             script_lines.append(empty_line)
 
-        footer = self._get_submit_script_footer(job_tmpl)  # pylint: disable=assignment-from-none
+        footer = self._get_submit_script_footer(job_tmpl)
         if footer:
             script_lines.append(footer)
             script_lines.append(empty_line)
 
         return '\n'.join(script_lines)
 
-    def _get_submit_script_environment_variables(self, template):  # pylint: disable=no-self-use
+    def _get_submit_script_environment_variables(self, template: JobTemplate) -> str:  # pylint: disable=no-self-use
         """Return the part of the submit script header that defines environment variables.
 
         :parameter template: a `aiida.schedulers.datastrutures.JobTemplate` instance.
         :return: string containing environment variable declarations.
         """
         if not isinstance(template.job_environment, dict):
             raise ValueError('If you provide job_environment, it must be a dictionary')
@@ -186,108 +204,118 @@
             lines.append(f'export {key.strip()}={escape_for_bash(value, template.environment_variables_double_quotes)}')
 
         lines.append('# ENVIRONMENT VARIABLES END ###')
 
         return '\n'.join(lines)
 
     @abc.abstractmethod
-    def _get_submit_script_header(self, job_tmpl):
+    def _get_submit_script_header(self, job_tmpl: JobTemplate) -> str:
         """Return the submit script header, using the parameters from the job template.
 
         :param job_tmpl: a `JobTemplate` instance with relevant parameters set.
+        :return: string with the submission script header.
         """
 
-    def _get_submit_script_footer(self, job_tmpl):
+    def _get_submit_script_footer(self, job_tmpl: JobTemplate) -> str:
         """Return the submit script final part, using the parameters from the job template.
 
         :param job_tmpl: a `JobTemplate` instance with relevant parameters set.
+        :return: string with the submission script footer.
         """
         # pylint: disable=no-self-use,unused-argument
-        return None
+        return ''
 
-    def _get_run_line(self, codes_info, codes_run_mode):
+    def _get_run_line(self, codes_info: list[JobTemplateCodeInfo], codes_run_mode: CodeRunMode) -> str:
         """Return a string with the line to execute a specific code with specific arguments.
 
         :parameter codes_info: a list of `aiida.scheduler.datastructures.JobTemplateCodeInfo` objects.
             Each contains the information needed to run the code. I.e. `cmdline_params`, `stdin_name`,
             `stdout_name`, `stderr_name`, `join_files`. See
             the documentation of `JobTemplate` and `JobTemplateCodeInfo`.
         :parameter codes_run_mode: instance of `aiida.common.datastructures.CodeRunMode` contains the information on how
             to launch the multiple codes.
         :return: string with format: [executable] [args] {[ < stdin ]} {[ < stdout ]} {[2>&1 | 2> stderr]}
         """
-        from aiida.common.datastructures import CodeRunMode
-
+        # pylint: disable=too-many-locals
         list_of_runlines = []
 
         for code_info in codes_info:
             computer_use_double_quotes = code_info.use_double_quotes[0]
             code_use_double_quotes = code_info.use_double_quotes[1]
 
-            command_to_exec_list = []
+            prepend_cmdline_params = []
             for arg in code_info.prepend_cmdline_params:
-                command_to_exec_list.append(escape_for_bash(arg, use_double_quotes=computer_use_double_quotes))
+                prepend_cmdline_params.append(escape_for_bash(arg, use_double_quotes=computer_use_double_quotes))
+
+            cmdline_params = []
             for arg in code_info.cmdline_params:
-                command_to_exec_list.append(escape_for_bash(arg, use_double_quotes=code_use_double_quotes))
-            command_to_exec = ' '.join(command_to_exec_list)
+                cmdline_params.append(escape_for_bash(arg, use_double_quotes=code_use_double_quotes))
 
             escape_stdin_name = escape_for_bash(code_info.stdin_name, use_double_quotes=computer_use_double_quotes)
             escape_stdout_name = escape_for_bash(code_info.stdout_name, use_double_quotes=computer_use_double_quotes)
             escape_sterr_name = escape_for_bash(code_info.stderr_name, use_double_quotes=computer_use_double_quotes)
 
             stdin_str = f'< {escape_stdin_name}' if code_info.stdin_name else ''
             stdout_str = f'> {escape_stdout_name}' if code_info.stdout_name else ''
 
             join_files = code_info.join_files
             if join_files:
                 stderr_str = '2>&1'
             else:
                 stderr_str = f'2> {escape_sterr_name}' if code_info.stderr_name else ''
 
-            output_string = f'{command_to_exec} {stdin_str} {stdout_str} {stderr_str}'
+            cmdline_params.extend([stdin_str, stdout_str, stderr_str])
+
+            prepend_cmdline_params_string = ' '.join(prepend_cmdline_params)
+            cmdline_params_string = ' '.join(cmdline_params)
+
+            if code_info.wrap_cmdline_params:
+                cmdline_params_string = escape_for_bash(cmdline_params_string, use_double_quotes=True)
+
+            run_line = f'{prepend_cmdline_params_string} {cmdline_params_string}'.strip()
 
-            list_of_runlines.append(output_string)
+            list_of_runlines.append(run_line)
 
         self.logger.debug(f'_get_run_line output: {list_of_runlines}')
 
         if codes_run_mode == CodeRunMode.PARALLEL:
             list_of_runlines.append('wait\n')
             return ' &\n\n'.join(list_of_runlines)
 
         if codes_run_mode == CodeRunMode.SERIAL:
             return '\n\n'.join(list_of_runlines)
 
         raise NotImplementedError('Unrecognized code run mode')
 
     @abc.abstractmethod
-    def _get_joblist_command(self, jobs=None, user=None):
+    def _get_joblist_command(self, jobs: list[str] | None = None, user: str | None = None) -> str:
         """Return the command to get the most complete description possible of currently active jobs.
 
         .. note::
 
             Typically one can pass only either jobs or user, depending on the specific plugin. The choice can be done
             according to the value returned by `self.get_feature('can_query_by_user')`
 
         :param jobs: either None to get a list of all jobs in the machine, or a list of jobs.
         :param user: either None, or a string with the username (to show only jobs of the specific user).
         """
 
-    def _get_detailed_job_info_command(self, job_id):
+    def _get_detailed_job_info_command(self, job_id: str) -> dict[str, t.Any]:
         """Return the command to run to get detailed information for a given job.
 
         This is typically called after the job has finished, to retrieve the most detailed information possible about
         the job. This is done because most schedulers just make finished jobs disappear from the `qstat` command, and
         instead sometimes it is useful to know some more detailed information about the job exit status, etc.
 
         :raises: :class:`aiida.common.exceptions.FeatureNotAvailable`
         """
         # pylint: disable=no-self-use,not-callable,unused-argument
         raise exceptions.FeatureNotAvailable('Cannot get detailed job info')
 
-    def get_detailed_job_info(self, job_id):
+    def get_detailed_job_info(self, job_id: str) -> dict[str, str | int]:
         """Return the detailed job info.
 
         This will be a dictionary with the return value, stderr and stdout content returned by calling the command that
         is returned by `_get_detailed_job_info_command`.
 
         :param job_id: the job identifier
         :return: dictionary with `retval`, `stdout` and `stderr`.
@@ -301,21 +329,26 @@
             'stdout': stdout,
             'stderr': stderr,
         }
 
         return detailed_job_info
 
     @abc.abstractmethod
-    def _parse_joblist_output(self, retval, stdout, stderr):
+    def _parse_joblist_output(self, retval: int, stdout: str, stderr: str) -> list[JobInfo]:
         """Parse the joblist output as returned by executing the command returned by `_get_joblist_command` method.
 
         :return: list of `JobInfo` objects, one of each job each with at least its default params implemented.
         """
 
-    def get_jobs(self, jobs=None, user=None, as_dict=False):
+    def get_jobs(
+        self,
+        jobs: list[str] | None = None,
+        user: str | None = None,
+        as_dict: bool = False,
+    ) -> list[JobInfo] | dict[str, JobInfo]:
         """Return the list of currently active jobs.
 
         .. note:: typically, only either jobs or user can be specified. See also comments in `_get_joblist_command`.
 
         :param list jobs: a list of jobs to check; only these are checked
         :param str user: a string with a user: only jobs of this user are checked
         :param list as_dict: if False (default), a list of JobInfo objects is returned. If True, a dictionary is
@@ -338,73 +371,79 @@
     def transport(self):
         """Return the transport set for this scheduler."""
         if self._transport is None:
             raise SchedulerError('Use the set_transport function to set the transport for the scheduler first.')
 
         return self._transport
 
-    def set_transport(self, transport):
+    def set_transport(self, transport: Transport):
         """Set the transport to be used to query the machine or to submit scripts.
 
         This class assumes that the transport is open and active.
         """
         self._transport = transport
 
     @abc.abstractmethod
-    def _get_submit_command(self, submit_script):
+    def _get_submit_command(self, submit_script: str) -> str:
         """Return the string to execute to submit a given script.
 
         .. warning:: the `submit_script` should already have been bash-escaped
 
         :param submit_script: the path of the submit script relative to the working directory.
         :return: the string to execute to submit a given script.
         """
 
     @abc.abstractmethod
-    def _parse_submit_output(self, retval, stdout, stderr):
+    def _parse_submit_output(self, retval: int, stdout: str, stderr: str) -> str | ExitCode:
         """Parse the output of the submit command returned by calling the `_get_submit_command` command.
 
-        :return: a string with the job ID.
+        :return: a string with the job ID or an exit code if the submission failed because the submission script is
+            invalid and the job should be terminated.
         """
 
-    def submit_from_script(self, working_directory, submit_script):
+    def submit_from_script(self, working_directory: str, submit_script: str) -> str | ExitCode:
         """Submit the submission script to the scheduler.
 
         :return: return a string with the job ID in a valid format to be used for querying.
         """
         self.transport.chdir(working_directory)
         result = self.transport.exec_command_wait(self._get_submit_command(escape_for_bash(submit_script)))
         return self._parse_submit_output(*result)
 
-    def kill(self, jobid):
+    def kill(self, jobid: str) -> bool:
         """Kill a remote job and parse the return value of the scheduler to check if the command succeeded.
 
         ..note::
 
             On some schedulers, even if the command is accepted, it may take some seconds for the job to actually
             disappear from the queue.
 
         :param jobid: the job ID to be killed
         :return: True if everything seems ok, False otherwise.
         """
         retval, stdout, stderr = self.transport.exec_command_wait(self._get_kill_command(jobid))
         return self._parse_kill_output(retval, stdout, stderr)
 
     @abc.abstractmethod
-    def _get_kill_command(self, jobid):
+    def _get_kill_command(self, jobid: str) -> str:
         """Return the command to kill the job with specified jobid."""
 
     @abc.abstractmethod
-    def _parse_kill_output(self, retval, stdout, stderr):
+    def _parse_kill_output(self, retval: int, stdout: str, stderr: str) -> bool:
         """Parse the output of the kill command.
 
         :return: True if everything seems ok, False otherwise.
         """
 
-    def parse_output(self, detailed_job_info=None, stdout=None, stderr=None):
+    def parse_output(
+        self,
+        detailed_job_info: dict[str, str | int] | None = None,
+        stdout: str | None = None,
+        stderr: str | None = None
+    ) -> ExitCode | None:
         """Parse the output of the scheduler.
 
         :param detailed_job_info: dictionary with the output returned by the `Scheduler.get_detailed_job_info` command.
             This should contain the keys `retval`, `stdout` and `stderr` corresponding to the return value, stdout and
             stderr returned by the accounting command executed for a specific job id.
         :param stdout: string with the output written by the scheduler to stdout.
         :param stderr: string with the output written by the scheduler to stderr.
```

### Comparing `aiida-core-2.2.2/aiida/sphinxext/__init__.py` & `aiida-core-2.3.0/aiida/sphinxext/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/sphinxext/calcjob.py` & `aiida-core-2.3.0/aiida/sphinxext/calcjob.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/sphinxext/process.py` & `aiida-core-2.3.0/aiida/sphinxext/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,17 @@
         res.append(nodes.Text(', '))
         res.append(nodes.emphasis(text=self.format_valid_types(port.valid_type)))
         res.append(nodes.Text(', '))
         res.append(nodes.Text('required' if port.required else 'optional'))
         if _is_non_db(port):
             res.append(nodes.Text(', '))
             res.append(nodes.emphasis(text='non_db'))
+        if _is_metadata(port):
+            res.append(nodes.Text(', '))
+            res.append(nodes.emphasis(text='is_metadata'))
         if port.help:
             res.append(nodes.Text(' -- '))
             # publish_doctree returns <document: <paragraph...>>.
             # Here we only want the content (children) of the paragraph.
             res.extend(publish_doctree(port.help)[0].children)
         return res
 
@@ -222,7 +225,11 @@
                 for outline_part in outline:
                     res.extend(self.build_outline_lines(outline_part, indent=indent))
         return res
 
 
 def _is_non_db(port):
     return getattr(port, 'non_db', False)
+
+
+def _is_metadata(port):
+    return getattr(port, 'is_metadata', False)
```

### Comparing `aiida-core-2.2.2/aiida/sphinxext/workchain.py` & `aiida-core-2.3.0/aiida/sphinxext/workchain.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/__init__.py` & `aiida-core-2.3.0/aiida/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/log.py` & `aiida-core-2.3.0/aiida/storage/log.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/__init__.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/alembic_cli.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/alembic_cli.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/backend.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/backend.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/__init__.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/env.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/env.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/__init__.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/calc_state.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/calc_state.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/create_dbattribute.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/create_dbattribute.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/dblog_update.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/dblog_update.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/duplicate_uuids.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/duplicate_uuids.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/integrity.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/integrity.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/legacy_workflows.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/legacy_workflows.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/migrate_repository.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/migrate_repository.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/parity.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/parity.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/provenance_redesign.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/provenance_redesign.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/reflect.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/reflect.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/utils/utils.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/041a79fc615f_dblog_cleaning.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/041a79fc615f_dblog_cleaning.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/07fac78e6209_drop_computer_transport_params.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/07fac78e6209_drop_computer_transport_params.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/0aebbeab274d_base_data_plugin_type_string.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/0aebbeab274d_base_data_plugin_type_string.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/0edcdd5a30f0_dbgroup_extras.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/0edcdd5a30f0_dbgroup_extras.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/118349c10896_default_link_label.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/118349c10896_default_link_label.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/12536798d4d3_trajectory_symbols_to_attribute.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/12536798d4d3_trajectory_symbols_to_attribute.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/140c971ae0a3_migrate_builtin_calculations.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/140c971ae0a3_migrate_builtin_calculations.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/162b99bca4a2_drop_dbcalcstate.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/162b99bca4a2_drop_dbcalcstate.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/1830c8430131_drop_node_columns_nodeversion_public.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/1830c8430131_drop_node_columns_nodeversion_public.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/1b8ed3425af9_remove_legacy_workflows.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/1b8ed3425af9_remove_legacy_workflows.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/1de112340b16_django_parity_1.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/1de112340b16_django_parity_1.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/1de112340b17_django_parity_2.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/1de112340b17_django_parity_2.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/1de112340b18_django_parity_3.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/1de112340b18_django_parity_3.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/1feaea71bd5a_migrate_repository.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/1feaea71bd5a_migrate_repository.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/239cea6d2452_provenance_redesign.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/239cea6d2452_provenance_redesign.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/26d561acd560_data_migration_legacy_job_calculations.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/26d561acd560_data_migration_legacy_job_calculations.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/34a831f4286d_entry_point_core_prefix.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/34a831f4286d_entry_point_core_prefix.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/35d4ee9a1b0e_code_hidden_attr_to_extra.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/35d4ee9a1b0e_code_hidden_attr_to_extra.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/375c2db70663_dblog_uuid_uniqueness_constraint.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/375c2db70663_dblog_uuid_uniqueness_constraint.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/37f3d4882837_make_all_uuid_columns_unique.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/37f3d4882837_make_all_uuid_columns_unique.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/3d6190594e19_remove_dbcomputer_enabled.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/3d6190594e19_remove_dbcomputer_enabled.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/535039300e4a_computer_name_to_label.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/535039300e4a_computer_name_to_label.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/59edaf8a8b79_adding_indexes_and_constraints_to_the_.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/59edaf8a8b79_adding_indexes_and_constraints_to_the_.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/5a49629f0d45_dblink_indices.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/5a49629f0d45_dblink_indices.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/5d4d844852b6_invalidating_node_hash.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/5d4d844852b6_invalidating_node_hash.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/5ddd24e52864_dbnode_type_to_dbnode_node_type.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/5ddd24e52864_dbnode_type_to_dbnode_node_type.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/61fc0913fae9_remove_node_prefix.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/61fc0913fae9_remove_node_prefix.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/62fe0d36de90_add_node_uuid_unique_constraint.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/62fe0d36de90_add_node_uuid_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/6a5c2ea1439d_move_data_within_node_module.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/6a5c2ea1439d_move_data_within_node_module.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/6c629c886f84_process_type.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/6c629c886f84_process_type.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/70c7d732f1b2_delete_dbpath.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/70c7d732f1b2_delete_dbpath.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/7536a82b2cc4_add_node_repository_metadata.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/7536a82b2cc4_add_node_repository_metadata.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/7a6587e16f4c_unique_constraints_for_the_db_dbgroup_.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/7a6587e16f4c_unique_constraints_for_the_db_dbgroup_.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/7b38a9e783e7_seal_unsealed_processes.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/7b38a9e783e7_seal_unsealed_processes.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/7ca08c391c49_calc_job_option_attribute_keys.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/7ca08c391c49_calc_job_option_attribute_keys.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/89176227b25_add_indexes_to_dbworkflowdata_table.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/89176227b25_add_indexes_to_dbworkflowdata_table.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/91b573400be5_prepare_schema_reset.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/91b573400be5_prepare_schema_reset.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/__init__.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/a514d673c163_drop_dblock.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/a514d673c163_drop_dblock.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/a603da2cc809_code_sub_class_of_data.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/a603da2cc809_code_sub_class_of_data.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/a6048f0ffca8_update_linktypes.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/a6048f0ffca8_update_linktypes.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/b8b23ddefad4_dbgroup_name_to_label_type_to_type_string.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/b8b23ddefad4_dbgroup_name_to_label_type_to_type_string.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/bf591f31dd12_dbgroup_type_string.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/bf591f31dd12_dbgroup_type_string.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/ce56d84bcc35_delete_trajectory_symbols_array.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/ce56d84bcc35_delete_trajectory_symbols_array.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/d254fdfed416_rename_parameter_data_to_dict.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/d254fdfed416_rename_parameter_data_to_dict.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/de2eaf6978b4_simplify_user_model.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/de2eaf6978b4_simplify_user_model.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0001_initial.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0001_initial.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0002_db_state_change.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0002_db_state_change.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0003_add_link_type.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0003_add_link_type.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0004_add_daemon_and_uuid_indices.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0004_add_daemon_and_uuid_indices.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0005_add_cmtime_indices.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0005_add_cmtime_indices.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0006_delete_dbpath.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0006_delete_dbpath.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0007_update_linktypes.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0007_update_linktypes.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0008_code_hidden_to_extra.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0008_code_hidden_to_extra.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0009_base_data_plugin_type_string.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0009_base_data_plugin_type_string.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0010_process_type.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0010_process_type.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0011_delete_kombu_tables.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0011_delete_kombu_tables.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0012_drop_dblock.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0012_drop_dblock.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0013_django_1_8.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0013_django_1_8.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0014_add_node_uuid_unique_constraint.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0014_add_node_uuid_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0015_invalidating_node_hash.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0015_invalidating_node_hash.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0016_code_sub_class_of_data.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0016_code_sub_class_of_data.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0017_drop_dbcalcstate.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0017_drop_dbcalcstate.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0018_django_1_11.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0018_django_1_11.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0019_migrate_builtin_calculations.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0019_migrate_builtin_calculations.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0020_provenance_redesign.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0020_provenance_redesign.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0021_dbgroup_name_to_label_type_to_type_string.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0021_dbgroup_name_to_label_type_to_type_string.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0022_dbgroup_type_string_change_content.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0022_dbgroup_type_string_change_content.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0023_calc_job_option_attribute_keys.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0023_calc_job_option_attribute_keys.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0024a_dblog_update.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0024a_dblog_update.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0024b_dblog_update.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0024b_dblog_update.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0025_move_data_within_node_module.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0025_move_data_within_node_module.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0026_trajectory_symbols_to_attribute.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0026_trajectory_symbols_to_attribute.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0027_delete_trajectory_symbols_array.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0027_delete_trajectory_symbols_array.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0028_remove_node_prefix.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0028_remove_node_prefix.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0029_rename_parameter_data_to_dict.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0029_rename_parameter_data_to_dict.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0030_dbnode_type_to_dbnode_node_type.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0030_dbnode_type_to_dbnode_node_type.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0031_remove_dbcomputer_enabled.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0031_remove_dbcomputer_enabled.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0032_remove_legacy_workflows.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0032_remove_legacy_workflows.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0033_replace_text_field_with_json_field.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0033_replace_text_field_with_json_field.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0034_drop_node_columns_nodeversion_public.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0034_drop_node_columns_nodeversion_public.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0035_simplify_user_model.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0035_simplify_user_model.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0036_drop_computer_transport_params.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0036_drop_computer_transport_params.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0037_attributes_extras_settings_json.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0037_attributes_extras_settings_json.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0038_data_migration_legacy_job_calculations.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0038_data_migration_legacy_job_calculations.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0039_reset_hash.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0039_reset_hash.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0040_data_migration_legacy_process_attributes.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0040_data_migration_legacy_process_attributes.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0041_seal_unsealed_processes.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0041_seal_unsealed_processes.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0042_prepare_schema_reset.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0042_prepare_schema_reset.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0043_default_link_label.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0043_default_link_label.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0044_dbgroup_type_string.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0044_dbgroup_type_string.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0045_dbgroup_extras.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0045_dbgroup_extras.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0046_add_node_repository_metadata.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0046_add_node_repository_metadata.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0047_migrate_repository.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0047_migrate_repository.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0048_computer_name_to_label.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0048_computer_name_to_label.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0049_entry_point_core_prefix.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0049_entry_point_core_prefix.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/django_0050_sqlalchemy_parity.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/django_0050_sqlalchemy_parity.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/e15ef2630a1b_initial_schema.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/e15ef2630a1b_initial_schema.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/e72ad251bcdb_dbgroup_class_change_type_string_values.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/e72ad251bcdb_dbgroup_class_change_type_string_values.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/e734dd5e50d7_data_migration_legacy_process_attributes.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/e734dd5e50d7_data_migration_legacy_process_attributes.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/e797afa09270_reset_hash.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/e797afa09270_reset_hash.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/ea2f50e7f615_dblog_create_uuid_column.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/ea2f50e7f615_dblog_create_uuid_column.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/f9a69de76a9a_delete_kombu_tables.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/f9a69de76a9a_delete_kombu_tables.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrations/versions/main_0001_initial.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrations/versions/main_0001_initial.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/migrator.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/migrator.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/models/__init__.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/models/authinfo.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/models/authinfo.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/models/base.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/models/base.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/models/comment.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/models/comment.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/models/computer.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/models/computer.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/models/group.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/models/group.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/models/log.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/models/log.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/models/node.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/models/node.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/models/settings.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/models/settings.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/models/user.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/models/user.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/orm/__init__.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/orm/authinfos.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/orm/authinfos.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/orm/comments.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/orm/comments.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/orm/computers.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/orm/computers.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/orm/convert.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/orm/convert.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/orm/entities.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/orm/entities.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/orm/extras_mixin.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/orm/extras_mixin.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/orm/groups.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/orm/groups.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/orm/logs.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/orm/logs.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/orm/nodes.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/orm/nodes.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/orm/querybuilder/__init__.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/orm/querybuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/orm/querybuilder/joiner.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/orm/querybuilder/joiner.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/orm/querybuilder/main.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/orm/querybuilder/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import warnings
 
 from sqlalchemy import and_
 from sqlalchemy import func as sa_func
 from sqlalchemy import not_, or_
 from sqlalchemy.dialects.postgresql import JSONB
 from sqlalchemy.engine import Row
-from sqlalchemy.exc import SAWarning
+from sqlalchemy.exc import CompileError, SAWarning
 from sqlalchemy.orm import aliased
 from sqlalchemy.orm.attributes import InstrumentedAttribute, QueryableAttribute
 from sqlalchemy.orm.query import Query
 from sqlalchemy.orm.session import Session
 from sqlalchemy.orm.util import AliasedClass
 from sqlalchemy.sql.compiler import SQLCompiler
 from sqlalchemy.sql.elements import BinaryExpression, BooleanClauseList, Cast, ColumnClause, ColumnElement, Label
@@ -885,15 +885,16 @@
 
             See https://www.postgresql.org/docs/current/functions-json.html for serialisation specs
             """
             from datetime import date, datetime, timedelta
 
             try:
                 return super().render_literal_value(value, type_)
-            except NotImplementedError:
+            # sqlalchemy<1.4.45 raises NotImplementedError, sqlalchemy>=1.4.45 raises CompileError
+            except (NotImplementedError, CompileError):
                 if isinstance(value, list):
                     values = ','.join(self.render_literal_value(item, type_) for item in value)
                     return f"'[{values}]'"
                 if isinstance(value, int):
                     return str(value)
                 if isinstance(value, (str, date, datetime, timedelta)):
                     escaped = str(value).replace('"', '\\"')
```

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/orm/users.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/orm/users.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/orm/utils.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/orm/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/psql_dos/utils.py` & `aiida-core-2.3.0/aiida/storage/psql_dos/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_temp/__init__.py` & `aiida-core-2.3.0/aiida/storage/sqlite_temp/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_temp/backend.py` & `aiida-core-2.3.0/aiida/storage/sqlite_temp/backend.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/__init__.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/backend.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/backend.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/__init__.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/env.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/env.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/__init__.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v04_to_v05.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v04_to_v05.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v05_to_v06.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v05_to_v06.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v06_to_v07.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v06_to_v07.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v07_to_v08.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v07_to_v08.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v08_to_v09.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v08_to_v09.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v09_to_v10.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v09_to_v10.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v10_to_v11.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v10_to_v11.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v11_to_v12.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v11_to_v12.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy/v12_to_v13.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy/v12_to_v13.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/legacy_to_main.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/legacy_to_main.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/script.py.mako` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/utils.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/v1_db_schema.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/v1_db_schema.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/versions/__init__.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/versions/main_0000_initial.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/versions/main_0000_initial.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/versions/main_0000a_replace_nulls.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/versions/main_0000a_replace_nulls.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/versions/main_0000b_non_nullable.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/versions/main_0000b_non_nullable.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrations/versions/main_0001.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrations/versions/main_0001.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/migrator.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/migrator.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/models.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/models.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/orm.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/orm.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/storage/sqlite_zip/utils.py` & `aiida-core-2.3.0/aiida/storage/sqlite_zip/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/__init__.py` & `aiida-core-2.3.0/aiida/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/archive/__init__.py` & `aiida-core-2.3.0/aiida/tools/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/archive/abstract.py` & `aiida-core-2.3.0/aiida/tools/archive/abstract.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/archive/common.py` & `aiida-core-2.3.0/aiida/tools/archive/common.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/archive/create.py` & `aiida-core-2.3.0/aiida/tools/archive/create.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/archive/exceptions.py` & `aiida-core-2.3.0/aiida/tools/archive/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/archive/implementations/__init__.py` & `aiida-core-2.3.0/aiida/tools/archive/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/archive/implementations/sqlite_zip/__init__.py` & `aiida-core-2.3.0/aiida/tools/archive/implementations/sqlite_zip/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/archive/implementations/sqlite_zip/main.py` & `aiida-core-2.3.0/aiida/tools/archive/implementations/sqlite_zip/main.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/archive/implementations/sqlite_zip/reader.py` & `aiida-core-2.3.0/aiida/tools/archive/implementations/sqlite_zip/reader.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/archive/implementations/sqlite_zip/writer.py` & `aiida-core-2.3.0/aiida/tools/archive/implementations/sqlite_zip/writer.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/archive/imports.py` & `aiida-core-2.3.0/aiida/tools/archive/imports.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/calculations/__init__.py` & `aiida-core-2.3.0/aiida/tools/calculations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/calculations/base.py` & `aiida-core-2.3.0/aiida/tools/calculations/base.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/data/__init__.py` & `aiida-core-2.3.0/aiida/tools/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/data/array/__init__.py` & `aiida-core-2.3.0/aiida/tools/data/array/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/data/array/kpoints/__init__.py` & `aiida-core-2.3.0/aiida/tools/data/array/kpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/data/array/kpoints/legacy.py` & `aiida-core-2.3.0/aiida/tools/data/array/kpoints/legacy.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/data/array/kpoints/main.py` & `aiida-core-2.3.0/aiida/tools/data/array/kpoints/main.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/data/array/kpoints/seekpath.py` & `aiida-core-2.3.0/aiida/tools/data/array/kpoints/seekpath.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/data/array/trajectory.py` & `aiida-core-2.3.0/aiida/tools/data/array/trajectory.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/data/cif.py` & `aiida-core-2.3.0/aiida/tools/data/cif.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/data/orbital/__init__.py` & `aiida-core-2.3.0/aiida/tools/data/orbital/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/data/orbital/orbital.py` & `aiida-core-2.3.0/aiida/tools/data/orbital/orbital.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/data/orbital/realhydrogen.py` & `aiida-core-2.3.0/aiida/tools/data/orbital/realhydrogen.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/data/structure.py` & `aiida-core-2.3.0/aiida/tools/data/structure.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/dbexporters/__init__.py` & `aiida-core-2.3.0/aiida/tools/dbexporters/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/dbimporters/__init__.py` & `aiida-core-2.3.0/aiida/tools/dbimporters/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/dbimporters/baseclasses.py` & `aiida-core-2.3.0/aiida/tools/dbimporters/baseclasses.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/dbimporters/plugins/__init__.py` & `aiida-core-2.3.0/aiida/tools/dbimporters/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/dbimporters/plugins/cod.py` & `aiida-core-2.3.0/aiida/tools/dbimporters/plugins/cod.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/dbimporters/plugins/icsd.py` & `aiida-core-2.3.0/aiida/tools/dbimporters/plugins/icsd.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 # pylint: disable=no-self-use
-""""Implementation of `DbImporter` for the CISD database."""
+"""Implementation of `DbImporter` for the ICSD database.
+
+Note: The implementation in this file is not compatible with the recent versions
+of ICSD, which are built with Apache Lucene and Tomcat. Older ICSD versions are
+supported, which included a MySQL database and a php-based web interface. The
+last confirmed compatible version was released in 2020.
+"""
 import io
 
 from aiida.tools.dbimporters.baseclasses import CifEntry, DbImporter, DbSearchResults
 
 
 class IcsdImporterExp(Exception):
     """Base class for ICSD exceptions."""
@@ -464,20 +470,19 @@
         self.db = None  # pylint: disable=invalid-name
         self.cursor = None
         self.db_parameters = db_parameters
         self.query = query
         self.number_of_results = None
         self._results = []
         self.cif_numbers = []
+        self.is_theoretical = []
         self.entries = {}
         self.page = 1
         self.position = 0
         self.db_version = None
-        self.sql_select_query = 'SELECT SQL_CALC_FOUND_ROWS icsd.IDNUM, icsd.COLL_CODE, icsd.STRUCT_FORM '
-        self.sql_from_query = 'FROM icsd '
 
         if self.db_parameters['querydb']:
             self.query_db_version()
         self.query_page()
 
     @property
     def results(self):
@@ -512,15 +517,18 @@
             if self.db_parameters['querydb']:
                 self.entries[position] = IcsdEntry(
                     self.db_parameters['server'] + self.db_parameters['dl_db'] +
                     self.cif_url.format(self._results[position]),
                     db_name=self.db_name,
                     id=self.cif_numbers[position],
                     version=self.db_version,
-                    extras={'idnum': self._results[position]}
+                    extras={
+                        'idnum': self._results[position],
+                        'is_theoretical': self.is_theoretical[position]
+                    }
                 )
             else:
                 self.entries[position] = IcsdEntry(
                     self.db_parameters['server'] + self.db_parameters['dl_db'] +
                     self.cif_url.format(self._results[position]),
                     db_name=self.db_name,
                     extras={'idnum': self._results[position]}
@@ -555,29 +563,44 @@
             raise NotImplementedError('Cannot query the database version with a web query.')
 
     def query_page(self):
         """
         Query the mysql or web page database, depending on the db_parameters.
         Store the number_of_results, cif file number and the corresponding icsd number.
 
+        Additionally, for the mysql case, determine if the origin of the structure is theoretical.
+        This information is stored in the `icsd_remarks` mysql table. If the crystal has either "THE"
+        or "ZTHE" tags, then it's classified as theoretical.
+
         :note: Icsd uses its own number system, different from the CIF
                 file numbers.
         """
         if self.db_parameters['querydb']:
 
-            self._connect_db()
-            query_statement = '{}{}{} LIMIT {}, 100'.format(
-                self.sql_select_query, self.sql_from_query, self.query, (self.page - 1) * 100
+            # Build the "THEORY" column based on the icsd_remarks table
+            sql_theory_column_query = (
+                "SELECT IDNUM, count(case when STD_REM_CODE IN ('THE', 'ZTHE') then 1 end) >= 1 AS THEORY " +
+                'FROM icsd_remarks GROUP BY IDNUM'
             )
+
+            # call it `tt` and join it with the main table based on IDNUM
+            sql_from_query = f'FROM icsd INNER JOIN ({sql_theory_column_query}) AS tt ON icsd.IDNUM=tt.IDNUM '
+
+            # Select the following columns
+            sql_select_query = 'SELECT SQL_CALC_FOUND_ROWS icsd.IDNUM, icsd.COLL_CODE, icsd.STRUCT_FORM, tt.THEORY '
+
+            self._connect_db()
+            query_statement = f'{sql_select_query}{sql_from_query}{self.query} LIMIT {(self.page - 1) * 100}, 100'
             self.cursor.execute(query_statement)
             self.db.commit()
 
             for row in self.cursor.fetchall():
                 self._results.append(str(row[0]))
                 self.cif_numbers.append(str(row[1]))
+                self.is_theoretical.append(bool(row[3]))
 
             if self.number_of_results is None:
                 self.cursor.execute('SELECT FOUND_ROWS()')
                 self.number_of_results = int(self.cursor.fetchone()[0])
 
             self._disconnect_db()
 
@@ -643,22 +666,24 @@
     _license = 'ICSD'
 
     def __init__(self, uri, **kwargs):
         """
         Create an instance of IcsdEntry, related to the supplied URI.
         """
         super().__init__(**kwargs)
+        _extras = kwargs.get('extras', {})
         self.source = {
             'db_name': kwargs.get('db_name', 'Icsd'),
             'db_uri': None,
             'id': kwargs.get('id', None),
             'version': kwargs.get('version', None),
             'uri': uri,
             'extras': {
-                'idnum': kwargs.get('extras', {}).get('idnum', None)
+                'idnum': _extras.get('idnum', None),
+                'is_theoretical': _extras.get('is_theoretical', None)
             },
             'license': self._license,
         }
 
     @property
     def contents(self):
         """
```

### Comparing `aiida-core-2.2.2/aiida/tools/dbimporters/plugins/materialsproject.py` & `aiida-core-2.3.0/aiida/tools/dbimporters/plugins/materialsproject.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/dbimporters/plugins/mpds.py` & `aiida-core-2.3.0/aiida/tools/dbimporters/plugins/mpds.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/dbimporters/plugins/mpod.py` & `aiida-core-2.3.0/aiida/tools/dbimporters/plugins/mpod.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/dbimporters/plugins/nninc.py` & `aiida-core-2.3.0/aiida/tools/dbimporters/plugins/nninc.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/dbimporters/plugins/oqmd.py` & `aiida-core-2.3.0/aiida/tools/dbimporters/plugins/oqmd.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/dbimporters/plugins/pcod.py` & `aiida-core-2.3.0/aiida/tools/dbimporters/plugins/pcod.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/dbimporters/plugins/tcod.py` & `aiida-core-2.3.0/aiida/tools/dbimporters/plugins/tcod.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/graph/__init__.py` & `aiida-core-2.3.0/aiida/tools/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/graph/age_entities.py` & `aiida-core-2.3.0/aiida/tools/graph/age_entities.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/graph/age_rules.py` & `aiida-core-2.3.0/aiida/tools/graph/age_rules.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/graph/deletions.py` & `aiida-core-2.3.0/aiida/tools/graph/deletions.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/graph/graph_traversers.py` & `aiida-core-2.3.0/aiida/tools/graph/graph_traversers.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/groups/__init__.py` & `aiida-core-2.3.0/aiida/tools/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/groups/paths.py` & `aiida-core-2.3.0/aiida/tools/groups/paths.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/ipython/__init__.py` & `aiida-core-2.3.0/aiida/tools/ipython/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/ipython/aiida_magic_register.py` & `aiida-core-2.3.0/aiida/tools/ipython/aiida_magic_register.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/query/calculation.py` & `aiida-core-2.3.0/aiida/tools/query/calculation.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     """Utility class to construct a QueryBuilder instance for Calculation nodes and project the query set."""
 
     # This tuple serves to mark compound projections that cannot explicitly be projected in the QueryBuilder, but will
     # have to be manually projected from composing its individual projection constituents
     _compound_projections = ('state',)
     _default_projections = ('pk', 'ctime', 'process_label', 'state', 'process_status')
     _valid_projections = (
-        'pk', 'uuid', 'ctime', 'mtime', 'state', 'process_state', 'process_status', 'exit_status', 'sealed',
-        'process_label', 'label', 'description', 'node_type', 'paused', 'process_type', 'job_state', 'scheduler_state',
-        'exception'
+        'pk', 'uuid', 'ctime', 'mtime', 'state', 'process_state', 'process_status', 'exit_status', 'exit_message',
+        'sealed', 'process_label', 'label', 'description', 'node_type', 'paused', 'process_type', 'job_state',
+        'scheduler_state', 'exception'
     )
 
     def __init__(self, mapper=None):
         if mapper is None:
             self._mapper = CalculationProjectionMapper(self._valid_projections)
         else:
             self._mapper = mapper
```

### Comparing `aiida-core-2.2.2/aiida/tools/query/formatting.py` & `aiida-core-2.3.0/aiida/tools/query/formatting.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/query/mapping.py` & `aiida-core-2.3.0/aiida/tools/query/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     attributes. This mapper class serves to map these projections onto the corresponding label and attribute names, as
     well as formatter functions to format the attribute values into strings, suitable to be printed by the CLI.
     """
 
     _valid_projections = []
 
     def __init__(self, projection_labels=None, projection_attributes=None, projection_formatters=None):
+        """Construct new instance."""
         if not self._valid_projections:
             raise NotImplementedError('no valid projections were specified by the sub class')
 
         self._projection_labels = {}
         self._projection_attributes = {}
         self._projection_formatters = {}
 
@@ -87,43 +88,40 @@
         job_state_key = 'attributes.state'
         scheduler_state_key = 'attributes.scheduler_state'
         process_paused_key = f'attributes.{ProcessNode.PROCESS_PAUSED_KEY}'
         process_label_key = f'attributes.{ProcessNode.PROCESS_LABEL_KEY}'
         process_state_key = f'attributes.{ProcessNode.PROCESS_STATE_KEY}'
         process_status_key = f'attributes.{ProcessNode.PROCESS_STATUS_KEY}'
         exit_status_key = f'attributes.{ProcessNode.EXIT_STATUS_KEY}'
+        exit_message_key = f'attributes.{ProcessNode.EXIT_MESSAGE_KEY}'
         exception_key = f'attributes.{ProcessNode.EXCEPTION_KEY}'
 
         default_labels = {'pk': 'PK', 'uuid': 'UUID', 'ctime': 'Created', 'mtime': 'Modified', 'state': 'Process State'}
 
         default_attributes = {
             'pk': 'id',
             'job_state': job_state_key,
             'scheduler_state': scheduler_state_key,
             'sealed': sealed_key,
             'paused': process_paused_key,
             'process_label': process_label_key,
             'process_state': process_state_key,
             'process_status': process_status_key,
             'exit_status': exit_status_key,
+            'exit_message': exit_message_key,
             'exception': exception_key,
         }
 
         default_formatters = {
-            'ctime':
-            lambda value: formatting.format_relative_time(value['ctime']),
-            'mtime':
-            lambda value: formatting.format_relative_time(value['mtime']),
-            'state':
-            lambda value: formatting.
+            'ctime': lambda value: formatting.format_relative_time(value['ctime']),
+            'mtime': lambda value: formatting.format_relative_time(value['mtime']),
+            'state': lambda value: formatting.
             format_state(value[process_state_key], value[process_paused_key], value[exit_status_key]),
-            'process_state':
-            lambda value: formatting.format_process_state(value[process_state_key]),
-            'sealed':
-            lambda value: formatting.format_sealed(value[sealed_key]),
+            'process_state': lambda value: formatting.format_process_state(value[process_state_key]),
+            'sealed': lambda value: formatting.format_sealed(value[sealed_key]),
         }
 
         if projection_labels is not None:
             for projection, label in projection_labels.items():
                 if projection not in self.valid_projections:
                     raise ValueError(f'{projection} is not a valid projection')
                 else:
```

### Comparing `aiida-core-2.2.2/aiida/tools/visualization/__init__.py` & `aiida-core-2.3.0/aiida/tools/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/tools/visualization/graph.py` & `aiida-core-2.3.0/aiida/tools/visualization/graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,43 +6,48 @@
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 """ provides functionality to create graphs of the AiiDa data providence,
 *via* graphviz.
 """
+from __future__ import annotations
+
 import os
-from types import MappingProxyType  # pylint: disable=no-name-in-module,useless-suppression
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Any, Callable, Literal, Mapping, Protocol, Sequence
 
 from graphviz import Digraph
 
 from aiida import orm
 from aiida.common import LinkType
 from aiida.manage import get_manager
 from aiida.orm.utils.links import LinkPair
 from aiida.tools.graph.graph_traversers import traverse_graph
 
 if TYPE_CHECKING:
     from aiida.orm.implementation import StorageBackend
 
 __all__ = ('Graph', 'default_link_styles', 'default_node_styles', 'pstate_node_styles', 'default_node_sublabels')
 
+LinkAnnotateType = Literal[None, 'label', 'type', 'both']
+
+
+class LinkStyleFunc(Protocol):
+    """Protocol for a link style function"""
+
+    def __call__(self, link_pair: LinkPair, add_label: bool, add_type: bool) -> dict:
+        ...
 
-def default_link_styles(link_pair, add_label, add_type):
-    # type: (LinkPair, bool, bool) -> dict
-    """map link_pair to a graphviz edge style
+
+def default_link_styles(link_pair: LinkPair, add_label: bool, add_type: bool) -> dict:
+    """Map link_pair to a graphviz edge style
 
     :param link_type: a LinkPair attribute
-    :type link_type: aiida.orm.utils.links.LinkPair
     :param add_label: include link label
-    :type add_label: bool
     :param add_type: include link type
-    :type add_type: bool
-    :rtype: dict
     """
 
     style = {
         LinkType.INPUT_CALC: {
             'style': 'solid',
             'color': '#000000'  # black
         },
@@ -74,20 +79,18 @@
         style['label'] = link_pair.link_type.name
     elif add_label and add_type:
         style['label'] = f'{link_pair.link_type.name}\n{link_pair.link_label}'
 
     return style
 
 
-def default_node_styles(node):
-    """map a node to a graphviz node style
+def default_node_styles(node: orm.Node) -> dict:
+    """Map a node to a graphviz node style
 
     :param node: the node to map
-    :type node: aiida.orm.nodes.node.Node
-    :rtype: dict
     """
 
     class_node_type = node.class_node_type
 
     try:
         default = node.get_style_default()
     except AttributeError:
@@ -132,20 +135,18 @@
     }
 
     node_style = node_type_map.get(class_node_type, default)
 
     return node_style
 
 
-def pstate_node_styles(node):
-    """map a process node to a graphviz node style
+def pstate_node_styles(node: orm.Node) -> dict:
+    """Map a process node to a graphviz node style
 
     :param node: the node to map
-    :type node: aiida.orm.nodes.node.Node
-    :rtype: dict
     """
 
     class_node_type = node.class_node_type
 
     default = {'shape': 'rectangle', 'pencolor': 'black'}
 
     process_map = {
@@ -188,126 +189,131 @@
         else:
             # Note: this conditional will hit the states CREATED, WAITING and RUNNING
             node_style['fillcolor'] = '#e38851ff'  # orange
 
     return node_style
 
 
-_OVERRIDE_STYLES_DICT = {
-    'ignore_node': {
+def _default_ignore_node_styles() -> dict:
+    """Return the default style for ignored nodes."""
+    return {
         'color': 'lightgray',
         'fillcolor': 'white',
         'penwidth': 2,
-    },
-    'origin_node': {
+    }
+
+
+def _default_origin_node_styles() -> dict:
+    """Return the default style for origin nodes."""
+    return {
         'color': 'red',
         'penwidth': 6,
-    },
-}
+    }
 
 
-def default_node_sublabels(node):
-    """function mapping nodes to a sublabel
+def default_node_sublabels(node: orm.Node) -> str:
+    """Function mapping nodes to a sub-label
     (e.g. specifying some attribute values)
 
     :param node: the node to map
-    :type node: aiida.orm.nodes.node.Node
-    :rtype: str
     """
     # pylint: disable=too-many-branches
 
     class_node_type = node.class_node_type
     if class_node_type == 'data.core.int.Int.':
         sublabel = f"value: {node.base.attributes.get('value', '')}"
     elif class_node_type == 'data.core.float.Float.':
         sublabel = f"value: {node.base.attributes.get('value', '')}"
     elif class_node_type == 'data.core.str.Str.':
         sublabel = f"{node.base.attributes.get('value', '')}"
     elif class_node_type == 'data.core.bool.Bool.':
         sublabel = f"{node.base.attributes.get('value', '')}"
     elif class_node_type == 'data.core.code.Code.':
-        sublabel = f'{os.path.basename(node.get_execname())}@{node.computer.label}'
+        label = '?' if node.computer is None else node.computer.label
+        sublabel = f'{os.path.basename(node.get_execname())}@{label}'
     elif class_node_type == 'data.core.singlefile.SinglefileData.':
         sublabel = node.filename
     elif class_node_type == 'data.core.remote.RemoteData.':
-        sublabel = f'@{node.computer.label}'
+        sublabel = f'@{node.computer.label}' if node.computer is not None else '@?'
     elif class_node_type == 'data.core.structure.StructureData.':
         sublabel = node.get_formula()
     elif class_node_type == 'data.core.cif.CifData.':
         formulae = [str(f).replace(' ', '') for f in node.get_formulae() or []]
         sg_numbers = [str(s) for s in node.get_spacegroup_numbers() or []]
         sublabel_lines = []
         if formulae:
             sublabel_lines.append(', '.join(formulae))
         if sg_numbers:
             sublabel_lines.append(', '.join(sg_numbers))
         sublabel = '; '.join(sublabel_lines)
     elif class_node_type == 'data.core.upf.UpfData.':
         sublabel = f"{node.base.attributes.get('element', '')}"
     elif isinstance(node, orm.ProcessNode):
-        sublabel = []
+        sublabel_list = []
         if node.process_state is not None:
-            sublabel.append(f'State: {node.process_state.value}')
+            sublabel_list.append(f'State: {node.process_state.value}')
         if node.exit_status is not None:
-            sublabel.append(f'Exit Code: {node.exit_status}')
-        sublabel = '\n'.join(sublabel)
+            sublabel_list.append(f'Exit Code: {node.exit_status}')
+        sublabel = '\n'.join(sublabel_list)
     else:
         sublabel = node.get_description()
 
     return sublabel
 
 
-def get_node_id_label(node, id_type):
-    """return an identifier str for the node """
+def get_node_id_label(node: orm.Node, id_type: Literal['pk', 'uuid', 'label']) -> str:
+    """Return an identifier str for the node """
     if id_type == 'pk':
-        return node.pk
+        return str(node.pk)
     if id_type == 'uuid':
         return node.uuid.split('-')[0]
     if id_type == 'label':
         return node.label
     raise ValueError(f'node_id_type not recognised: {id_type}')
 
 
-def _get_node_label(node, id_type='pk'):
-    """return a label text of node and the return format is '<NodeType> (<id>)'."""
+def _get_node_label(node: orm.Node, id_type: Literal['pk', 'uuid', 'label'] = 'pk') -> str:
+    """Return a label text of node and the return format is '<NodeType> (<id>)'."""
     if isinstance(node, orm.Data):
         label = f'{node.__class__.__name__} ({get_node_id_label(node, id_type)})'
     elif isinstance(node, orm.ProcessNode):
         label = '{} ({})'.format(
             node.__class__.__name__ if node.process_label is None else node.process_label,
             get_node_id_label(node, id_type)
         )
     else:
         raise TypeError(f'Unknown type: {type(node)}')
 
     return label
 
 
 def _add_graphviz_node(
-    graph, node, node_style_func, node_sublabel_func, style_override=None, include_sublabels=True, id_type='pk'
+    graph: Digraph,
+    node: orm.Node,
+    node_style_func,
+    node_sublabel_func,
+    style_override: None | dict = None,
+    include_sublabels: bool = True,
+    id_type: Literal['pk', 'uuid', 'label'] = 'pk'
 ):
-    """create a node in the graph
+    """Create a node in the graph
 
     The first line of the node text is always '<node.name> (<node.pk>)'.
     Then, if ``include_sublabels=True``, subsequent lines are added,
     which are node type dependant.
 
     :param graph: the graphviz.Digraph to add the node to
     :param node: the node to add
-    :type node: aiida.orm.nodes.node.Node
     :param node_style_func: callable mapping a node instance to a dictionary defining the graphviz node style
     :param node_sublabel_func: callable mapping a node instance to a sub-label for the node text
     :param style_override: style dictionary, whose keys will override the final computed style
-    :type style_override: None or dict
     :param include_sublabels: whether to include the sublabels for nodes
-    :type include_sublabels: bool
-    :param id_type: the type of identifier to use for node labels ('pk' or 'uuid')
-    :type id_type: str
+    :param id_type: the type of identifier to use for node labels
 
-    nodes are styled based on the node type
+    Nodes are styled based on the node type
 
     For subclasses of Data, the ``class_node_type`` attribute is used
     for mapping to type specific styles
 
     For subclasses of ProcessNode, we choose styles to distinguish between
     types, and also color the nodes for successful/failed processes
     """
@@ -327,151 +333,123 @@
 
     # coerce node style values to strings, required by graphviz
     node_style = {k: str(v) for k, v in node_style.items()}
 
     return graph.node(f'N{node.pk}', **node_style)
 
 
-def _add_graphviz_edge(graph, in_node, out_node, style=None):
-    """add graphviz edge between two nodes
+def _add_graphviz_edge(graph: Digraph, in_node: orm.Node, out_node: orm.Node, style: dict | None = None) -> dict:
+    """Add graphviz edge between two nodes
 
     :param graph: the graphviz.DiGraph to add the edge to
     :param in_node: the head node
     :param out_node: the tail node
-    :param style: the graphviz style (Default value = None)
-    :type style: dict or None
+    :param style: the graphviz style
     """
 
     if style is None:
         style = {}
 
     # coerce node style values to strings
     style = {k: str(v) for k, v in style.items()}
 
     return graph.edge(f'N{in_node.pk}', f'N{out_node.pk}', **style)
 
 
 class Graph:
-    """a class to create graphviz graphs of the AiiDA node provenance"""
+    """A class to create graphviz graphs of the AiiDA node provenance."""
 
     def __init__(
         self,
-        engine=None,
-        graph_attr=None,
-        global_node_style=None,
-        global_edge_style=None,
-        include_sublabels=True,
-        link_style_fn=None,
-        node_style_fn=None,
-        node_sublabel_fn=None,
-        node_id_type='pk',
-        backend: Optional['StorageBackend'] = None
+        engine: str | None = None,
+        graph_attr: dict | None = None,
+        global_node_style: dict | None = None,
+        global_edge_style: dict | None = None,
+        include_sublabels: bool = True,
+        link_style_fn: LinkStyleFunc | None = None,
+        node_style_fn: Callable[[orm.Node], dict] | None = None,
+        node_sublabel_fn: Callable[[orm.Node], str] | None = None,
+        node_id_type: Literal['pk', 'uuid', 'label'] = 'pk',
+        backend: StorageBackend | None = None
     ):
-        """a class to create graphviz graphs of the AiiDA node provenance
+        """A class to create graphviz graphs of the AiiDA node provenance
 
         Nodes and edges, are cached, so that they are only created once
 
-        :param engine: the graphviz engine, e.g. dot, circo (Default value = None)
-        :type engine: str or None
-        :param graph_attr: attributes for the graphviz graph (Default value = None)
-        :type graph_attr: dict or None
+        :param engine: the graphviz engine, e.g. dot, circo
+        :param graph_attr: attributes for the graphviz graph
         :param global_node_style: styles which will be added to all nodes.
-            Note this will override any builtin attributes (Default value = None)
-        :type global_node_style: dict or None
+            Note this will override any builtin attributes
         :param global_edge_style: styles which will be added to all edges.
-            Note this will override any builtin attributes (Default value = None)
-        :type global_edge_style: dict or None
-        :param include_sublabels: if True, the note text will include node dependant sub-labels (Default value = True)
-        :type include_sublabels: bool
+            Note this will override any builtin attributes
+        :param include_sublabels: if True, the note text will include node dependant sub-labels
         :param link_style_fn: callable mapping LinkType to graphviz style dict;
-            link_style_fn(link_type) -> dict (Default value = None)
+            link_style_fn(link_type, add_label, add_type) -> dict
         :param node_sublabel_fn: callable mapping nodes to a graphviz style dict;
-            node_sublabel_fn(node) -> dict (Default value = None)
+            node_sublabel_fn(node) -> dict
         :param node_sublabel_fn: callable mapping data node to a sublabel (e.g. specifying some attribute values)
-            node_sublabel_fn(node) -> str (Default value = None)
-        :param node_id_type: the type of identifier to within the node text ('pk', 'uuid' or 'label')
-        :type node_id_type: str
+            node_sublabel_fn(node) -> str
+        :param node_id_type: the type of identifier to within the node text
         """
         # pylint: disable=too-many-arguments
 
         self._graph = Digraph(engine=engine, graph_attr=graph_attr)
-        self._nodes = set()
-        self._edges = set()
+        self._nodes: set[int] = set()
+        self._edges: set[tuple[int, int, None | LinkPair]] = set()
         self._global_node_style = global_node_style or {}
         self._global_edge_style = global_edge_style or {}
         self._include_sublabels = include_sublabels
         self._link_styles = link_style_fn or default_link_styles
         self._node_styles = node_style_fn or default_node_styles
         self._node_sublabels = node_sublabel_fn or default_node_sublabels
         self._node_id_type = node_id_type
         self._backend = backend or get_manager().get_profile_storage()
 
-        self._ignore_node_style = _OVERRIDE_STYLES_DICT['ignore_node']
-        self._origin_node_style = _OVERRIDE_STYLES_DICT['origin_node']
+        self._ignore_node_style = _default_ignore_node_styles()
+        self._origin_node_style = _default_origin_node_styles()
 
     @property
-    def backend(self) -> 'StorageBackend':
+    def backend(self) -> StorageBackend:
         """The backend used to create the graph"""
         return self._backend
 
     @property
-    def graphviz(self):
-        """return a copy of the graphviz.Digraph"""
+    def graphviz(self) -> Digraph:
+        """Return a copy of the graphviz.Digraph"""
         return self._graph.copy()
 
     @property
-    def nodes(self):
-        """return a copy of the nodes"""
+    def nodes(self) -> set[int]:
+        """Return a copy of the nodes"""
         return self._nodes.copy()
 
     @property
-    def edges(self):
-        """return a copy of the edges"""
+    def edges(self) -> set[tuple[int, int, None | LinkPair]]:
+        """Return a copy of the edges"""
         return self._edges.copy()
 
-    def _load_node(self, node):
-        """ load a node (if not already loaded)
+    def _load_node(self, node: int | str | orm.Node) -> orm.Node:
+        """Load a node (if not already loaded)
 
         :param node: node or node pk/uuid
-        :type node: int or str or aiida.orm.nodes.node.Node
-        :returns: aiida.orm.nodes.node.Node
         """
         if isinstance(node, int):
             return orm.Node.collection(self._backend).get(pk=node)
         if isinstance(node, str):
             return orm.Node.collection(self._backend).get(uuid=node)
         return node
 
-    @staticmethod
-    def _default_link_types(link_types):
-        """If link_types is empty, it will return all the links_types
-
-        :param links: iterable with the link_types ()
-        :returns: list of :py:class:`aiida.common.links.LinkType`
-        """
-        if not link_types:
-            all_link_types = [LinkType.CREATE]
-            all_link_types.append(LinkType.RETURN)
-            all_link_types.append(LinkType.INPUT_CALC)
-            all_link_types.append(LinkType.INPUT_WORK)
-            all_link_types.append(LinkType.CALL_CALC)
-            all_link_types.append(LinkType.CALL_WORK)
-            return all_link_types
-
-        return link_types
-
-    def add_node(self, node, style_override=None, overwrite=False):
-        """add single node to the graph
+    def add_node(
+        self, node: int | str | orm.Node, style_override: dict | None = None, overwrite: bool = False
+    ) -> orm.Node:
+        """Add single node to the graph
 
         :param node: node or node pk/uuid
-        :type node: int or str or aiida.orm.nodes.node.Node
         :param style_override: graphviz style parameters that will override default values
-        :type style_override: dict or None
-        :param overwrite: whether to overrite an existing node (Default value = False)
-        :type overwrite: bool
+        :param overwrite: whether to overwrite an existing node
         """
         node = self._load_node(node)
         style = {} if style_override is None else dict(style_override)
         style.update(self._global_node_style)
         if node.pk not in self._nodes or overwrite:
             _add_graphviz_node(
                 self._graph,
@@ -481,27 +459,29 @@
                 style_override=style,
                 include_sublabels=self._include_sublabels,
                 id_type=self._node_id_type
             )
             self._nodes.add(node.pk)
         return node
 
-    def add_edge(self, in_node, out_node, link_pair=None, style=None, overwrite=False):
-        """add single node to the graph
+    def add_edge(
+        self,
+        in_node: int | str | orm.Node,
+        out_node: int | str | orm.Node,
+        link_pair: LinkPair | None = None,
+        style: dict | None = None,
+        overwrite: bool = False
+    ) -> None:
+        """Add single node to the graph
 
         :param in_node: node or node pk/uuid
-        :type in_node: int or aiida.orm.nodes.node.Node
         :param out_node: node or node pk/uuid
-        :type out_node: int or str or aiida.orm.nodes.node.Node
         :param link_pair: defining the relationship between the nodes
-        :type link_pair: None or aiida.orm.utils.links.LinkPair
-        :param style: graphviz style parameters (Default value = None)
-        :type style: dict or None
-        :param overwrite: whether to overrite existing edge (Default value = False)
-        :type overwrite: bool
+        :param style: graphviz style parameters
+        :param overwrite: whether to overwrite existing edge
         """
         in_node = self._load_node(in_node)
         if in_node.pk not in self._nodes:
             raise AssertionError(f'in_node pk={in_node.pk} must have already been added to the graph')
         out_node = self._load_node(out_node)
         if out_node.pk not in self._nodes:
             raise AssertionError(f'out_node pk={out_node.pk} must have already been added to the graph')
@@ -512,124 +492,133 @@
         style = {} if style is None else style
         self._edges.add((in_node.pk, out_node.pk, link_pair))
         style.update(self._global_edge_style)
 
         _add_graphviz_edge(self._graph, in_node, out_node, style)
 
     @staticmethod
-    def _convert_link_types(link_types):
-        """convert link types, which may be strings, to a member of LinkType"""
-        if link_types is None:
-            return None
-        if isinstance(link_types, str):
-            link_types = [link_types]
-        link_types = tuple(getattr(LinkType, l.upper()) if isinstance(l, str) else l for l in link_types)
-        return link_types
+    def _convert_link_types(
+        link_types: None | str | LinkType | Sequence[str] | Sequence[LinkType]
+    ) -> tuple[LinkType, ...]:
+        """Convert link types, which may be strings, to a member of LinkType"""
+        link_types_list: Sequence[LinkType] | Sequence[str]
+        if not link_types:
+            link_types_list = [
+                LinkType.CREATE, LinkType.RETURN, LinkType.INPUT_CALC, LinkType.INPUT_WORK, LinkType.CALL_CALC,
+                LinkType.CALL_WORK
+            ]
+        elif isinstance(link_types, (str, LinkType)):
+            link_types_list = [link_types]  # type: ignore
+        else:
+            link_types_list = link_types
+        return tuple(getattr(LinkType, l.upper()) if isinstance(l, str) else l for l in link_types_list)
 
-    def add_incoming(self, node, link_types=(), annotate_links=None, return_pks=True):
-        """add nodes and edges for incoming links to a node
+    def add_incoming(
+        self,
+        node: int | str | orm.Node,
+        link_types: None | str | Sequence[str] | LinkType | Sequence[LinkType] = None,
+        annotate_links: LinkAnnotateType = None,
+        return_pks: bool = True
+    ) -> list[int] | list[orm.Node]:
+        """Add nodes and edges for incoming links to a node
 
         :param node: node or node pk/uuid
-        :type node: aiida.orm.nodes.node.Node or int
-        :param link_types: filter by link types (Default value = ())
-        :type link_types: str or tuple[str] or aiida.common.links.LinkType or tuple[aiida.common.links.LinkType]
-        :param annotate_links: label edges with the link 'label', 'type' or 'both' (Default value = None)
-        :type annotate_links: bool or str
-        :param return_pks: whether to return a list of nodes, or list of node pks (Default value = True)
-        :type return_pks: bool
+        :param link_types: filter by link types
+        :param annotate_links: label edges with the link 'label', 'type' or 'both'
+        :param return_pks: whether to return a list of nodes, or list of node pks
         :returns: list of nodes or node pks
         """
         if annotate_links not in [None, False, 'label', 'type', 'both']:
             raise ValueError(
                 f'annotate_links must be one of False, "label", "type" or "both"\ninstead, it is: {annotate_links}'
             )
 
         # incoming nodes are found traversing backwards
         node_pk = self._load_node(node).pk
-        valid_link_types = self._default_link_types(link_types)
-        valid_link_types = self._convert_link_types(valid_link_types)
+        valid_link_types = self._convert_link_types(link_types)
         traversed_graph = traverse_graph(
             (node_pk,),
             max_iterations=1,
             get_links=True,
             backend=self.backend,
             links_backward=valid_link_types,
         )
 
-        traversed_nodes = orm.QueryBuilder(backend=self.backend).append(
+        query = orm.QueryBuilder(backend=self.backend).append(
             orm.Node,
             filters={'id': {
                 'in': traversed_graph['nodes']
             }},
             project=['id', '*'],
             tag='node',
         )
-        traversed_nodes = {query_result[0]: query_result[1] for query_result in traversed_nodes.all()}
+        traversed_nodes = {query_result[0]: query_result[1] for query_result in query.all()}
 
         for _, traversed_node in traversed_nodes.items():
             self.add_node(traversed_node, style_override=None)
 
-        for link in traversed_graph['links']:
+        for link in (traversed_graph['links'] or []):
             source_node = traversed_nodes[link.source_id]
             target_node = traversed_nodes[link.target_id]
             link_pair = LinkPair(self._convert_link_types(link.link_type)[0], link.link_label)
             link_style = self._link_styles(
                 link_pair, add_label=annotate_links in ['label', 'both'], add_type=annotate_links in ['type', 'both']
             )
             self.add_edge(source_node, target_node, link_pair, style=link_style)
 
         if return_pks:
             return list(traversed_nodes.keys())
         # else:
         return list(traversed_nodes.values())
 
-    def add_outgoing(self, node, link_types=(), annotate_links=None, return_pks=True):
-        """add nodes and edges for outgoing links to a node
+    def add_outgoing(
+        self,
+        node: int | str | orm.Node,
+        link_types: None | str | Sequence[str] | LinkType | Sequence[LinkType] = None,
+        annotate_links: LinkAnnotateType = None,
+        return_pks: bool = True
+    ) -> list[int] | list[orm.Node]:
+        """Add nodes and edges for outgoing links to a node
 
         :param node: node or node pk
-        :type node: aiida.orm.nodes.node.Node or int
-        :param link_types: filter by link types (Default value = ())
-        :type link_types: str or tuple[str] or aiida.common.links.LinkType or tuple[aiida.common.links.LinkType]
-        :param annotate_links: label edges with the link 'label', 'type' or 'both' (Default value = None)
-        :type annotate_links: bool or str
-        :param return_pks: whether to return a list of nodes, or list of node pks (Default value = True)
-        :type return_pks: bool
+        :param link_types: filter by link types
+        :param annotate_links: label edges with the link 'label', 'type' or 'both'
+        :param return_pks: whether to return a list of nodes, or list of node pks
         :returns: list of nodes or node pks
         """
         if annotate_links not in [None, False, 'label', 'type', 'both']:
             raise ValueError(
                 f'annotate_links must be one of False, "label", "type" or "both"\ninstead, it is: {annotate_links}'
             )
 
         # outgoing nodes are found traversing forwards
         node_pk = self._load_node(node).pk
-        valid_link_types = self._default_link_types(link_types)
-        valid_link_types = self._convert_link_types(valid_link_types)
+        valid_link_types = self._convert_link_types(link_types)
         traversed_graph = traverse_graph(
             (node_pk,),
             max_iterations=1,
             get_links=True,
             backend=self.backend,
             links_forward=valid_link_types,
         )
 
-        traversed_nodes = orm.QueryBuilder(backend=self.backend).append(
+        query = orm.QueryBuilder(backend=self.backend).append(
             orm.Node,
             filters={'id': {
                 'in': traversed_graph['nodes']
             }},
             project=['id', '*'],
             tag='node',
         )
-        traversed_nodes = {query_result[0]: query_result[1] for query_result in traversed_nodes.all()}
+        traversed_nodes = {query_result[0]: query_result[1] for query_result in query.all()}
 
         for _, traversed_node in traversed_nodes.items():
             self.add_node(traversed_node, style_override=None)
 
-        for link in traversed_graph['links']:
+        for link in (traversed_graph['links'] or []):
             source_node = traversed_nodes[link.source_id]
             target_node = traversed_nodes[link.target_id]
             link_pair = LinkPair(self._convert_link_types(link.link_type)[0], link.link_label)
             link_style = self._link_styles(
                 link_pair, add_label=annotate_links in ['label', 'both'], add_type=annotate_links in ['type', 'both']
             )
             self.add_edge(source_node, target_node, link_pair, style=link_style)
@@ -637,47 +626,39 @@
         if return_pks:
             return list(traversed_nodes.keys())
         # else:
         return list(traversed_nodes.values())
 
     def recurse_descendants(
         self,
-        origin,
-        depth=None,
-        link_types=(),
-        annotate_links=False,
-        origin_style=MappingProxyType(_OVERRIDE_STYLES_DICT['origin_node']),
-        include_process_inputs=False,
-        highlight_classes=None,
-    ):
-        """add nodes and edges from an origin recursively,
+        origin: int | str | orm.Node,
+        depth: int | None = None,
+        link_types: None | str | Sequence[str] | LinkType | Sequence[LinkType] = None,
+        annotate_links: LinkAnnotateType = None,
+        origin_style: dict | None = None,
+        include_process_inputs: bool = False,
+        highlight_classes: None | Sequence[str] = None,
+    ) -> None:
+        """Add nodes and edges from an origin recursively,
         following outgoing links
 
         :param origin: node or node pk/uuid
-        :type origin: aiida.orm.nodes.node.Node or int
-        :param depth: if not None, stop after travelling a certain depth into the graph (Default value = None)
-        :type depth: None or int
-        :param link_types: filter by subset of link types (Default value = ())
-        :type link_types: tuple or str
-        :param annotate_links: label edges with the link 'label', 'type' or 'both' (Default value = False)
-        :type annotate_links: bool or str
-        :param origin_style: node style map for origin node (Default value = None)
-        :type origin_style: None or dict
-        :param include_calculation_inputs: include incoming links for all processes (Default value = False)
-        :type include_calculation_inputs: bool
+        :param depth: if not None, stop after travelling a certain depth into the graph
+        :param link_types: filter by subset of link types
+        :param annotate_links: label edges with the link 'label', 'type' or 'both'
+        :param origin_style: node style map for origin node
+        :param include_calculation_inputs: include incoming links for all processes
         :param highlight_classes: target class in exported graph expected to be highlight and
-            other nodes are decolorized (Default value = None)
-        :typle highlight_classes: tuple of class or class
+            other nodes are decolorized
         """
         # pylint: disable=too-many-arguments,too-many-locals
         # Get graph traversal rules where the given link types and direction are all set to True,
         # and all others are set to False
         origin_pk = self._load_node(origin).pk
-        valid_link_types = self._default_link_types(link_types)
-        valid_link_types = self._convert_link_types(valid_link_types)
+        valid_link_types = self._convert_link_types(link_types)
         traversed_graph = traverse_graph(
             (origin_pk,),
             max_iterations=depth,
             get_links=True,
             backend=self.backend,
             links_forward=valid_link_types,
         )
@@ -689,88 +670,80 @@
                 traversed_graph['nodes'],
                 max_iterations=1,
                 get_links=True,
                 backend=self.backend,
                 links_backward=[LinkType.INPUT_WORK, LinkType.INPUT_CALC]
             )
             traversed_graph['nodes'] = traversed_graph['nodes'].union(traversed_outputs['nodes'])
-            traversed_graph['links'] = traversed_graph['links'].union(traversed_outputs['links'])
+            traversed_graph['links'] = (traversed_graph['links'] or set()).union(traversed_outputs['links'] or set())
 
         # Do one central query for all nodes in the Graph and generate a {id: Node} dictionary
-        traversed_nodes = orm.QueryBuilder(backend=self.backend).append(
+        query = orm.QueryBuilder(backend=self.backend).append(
             orm.Node,
             filters={'id': {
                 'in': traversed_graph['nodes']
             }},
             project=['id', '*'],
             tag='node',
         )
-        traversed_nodes = {query_result[0]: query_result[1] for query_result in traversed_nodes.all()}
+        traversed_nodes = {query_result[0]: query_result[1] for query_result in query.all()}
 
         # Pop the origin node and add it to the graph, applying custom styling
         origin_node = traversed_nodes.pop(origin_pk)
-        self.add_node(origin_node, style_override=origin_style)
+        self.add_node(origin_node, style_override=origin_style or _default_origin_node_styles())
 
         # Add all traversed nodes to the graph with default styling
         for _, traversed_node in traversed_nodes.items():
             node_label = _get_node_label(traversed_node)
             if highlight_classes and not node_label.split()[0] in highlight_classes:
                 self.add_node(traversed_node, style_override=self._ignore_node_style)
             else:
                 self.add_node(traversed_node, style_override=None)
 
         # Add the origin node back into traversed nodes so it can be found for adding edges
         traversed_nodes[origin_pk] = origin_node
 
         # Add all links to the Graph, using the {id: Node} dictionary for queryless Node retrieval, applying
         # appropriate styling
-        for link in traversed_graph['links']:
+        for link in (traversed_graph['links'] or []):
             source_node = traversed_nodes[link.source_id]
             target_node = traversed_nodes[link.target_id]
             link_pair = LinkPair(self._convert_link_types(link.link_type)[0], link.link_label)
             link_style = self._link_styles(
                 link_pair, add_label=annotate_links in ['label', 'both'], add_type=annotate_links in ['type', 'both']
             )
             self.add_edge(source_node, target_node, link_pair, style=link_style)
 
     def recurse_ancestors(
         self,
-        origin,
-        depth=None,
-        link_types=(),
-        annotate_links=False,
-        origin_style=MappingProxyType(_OVERRIDE_STYLES_DICT['origin_node']),
-        include_process_outputs=False,
-        highlight_classes=None,
-    ):
-        """add nodes and edges from an origin recursively,
+        origin: int | str | orm.Node,
+        depth: int | None = None,
+        link_types: None | str | Sequence[str] | LinkType | Sequence[LinkType] = None,
+        annotate_links: LinkAnnotateType = None,
+        origin_style: dict | None = None,
+        include_process_outputs: bool = False,
+        highlight_classes: None | Sequence[str] = None,
+    ) -> None:
+        """Add nodes and edges from an origin recursively,
         following incoming links
 
         :param origin: node or node pk/uuid
-        :type origin: aiida.orm.nodes.node.Node or int
-        :param depth: if not None, stop after travelling a certain depth into the graph (Default value = None)
-        :type depth: None or int
-        :param link_types: filter by subset of link types (Default value = ())
-        :type link_types: tuple or str
-        :param annotate_links: label edges with the link 'label', 'type' or 'both' (Default value = False)
-        :type annotate_links: bool
-        :param origin_style: node style map for origin node (Default value = None)
-        :type origin_style: None or dict
-        :param include_process_outputs:  include outgoing links for all processes (Default value = False)
-        :type include_process_outputs: bool
+        :param depth: if not None, stop after travelling a certain depth into the graph
+        :param link_types: filter by subset of link types
+        :param annotate_links: label edges with the link 'label', 'type' or 'both'
+        :param origin_style: node style map for origin node
+        :param include_process_outputs: include outgoing links for all processes
         :param highlight_classes:  class label (as displayed in the graph, e.g. 'StructureData', 'FolderData', etc.)
-            to be highlight and other nodes are decolorized (Default value = None)
-        :typle highlight_classes: list or tuple of str
+            to be highlight and other nodes are decolorized
         """
         # pylint: disable=too-many-arguments,too-many-locals
         # Get graph traversal rules where the given link types and direction are all set to True,
         # and all others are set to False
         origin_pk = self._load_node(origin).pk
-        valid_link_types = self._default_link_types(link_types)
-        valid_link_types = self._convert_link_types(valid_link_types)
+        valid_link_types = self._convert_link_types(link_types)
         traversed_graph = traverse_graph(
             (origin_pk,),
             max_iterations=depth,
             get_links=True,
             backend=self.backend,
             links_backward=valid_link_types,
         )
@@ -782,156 +755,142 @@
                 traversed_graph['nodes'],
                 max_iterations=1,
                 get_links=True,
                 backend=self.backend,
                 links_forward=[LinkType.CREATE, LinkType.RETURN]
             )
             traversed_graph['nodes'] = traversed_graph['nodes'].union(traversed_outputs['nodes'])
-            traversed_graph['links'] = traversed_graph['links'].union(traversed_outputs['links'])
+            traversed_graph['links'] = (traversed_graph['links'] or set()).union(traversed_outputs['links'] or set())
 
         # Do one central query for all nodes in the Graph and generate a {id: Node} dictionary
-        traversed_nodes = orm.QueryBuilder(backend=self.backend).append(
+        query = orm.QueryBuilder(backend=self.backend).append(
             orm.Node,
             filters={'id': {
                 'in': traversed_graph['nodes']
             }},
             project=['id', '*'],
             tag='node',
         )
-        traversed_nodes = {query_result[0]: query_result[1] for query_result in traversed_nodes.all()}
+        traversed_nodes = {query_result[0]: query_result[1] for query_result in query.all()}
 
         # Pop the origin node and add it to the graph, applying custom styling
         origin_node = traversed_nodes.pop(origin_pk)
-        self.add_node(origin_node, style_override=origin_style)
+        self.add_node(origin_node, style_override=(origin_style or _default_origin_node_styles()))
 
         # Add all traversed nodes to the graph with default styling
         for _, traversed_node in traversed_nodes.items():
             node_label = _get_node_label(traversed_node)
             if highlight_classes and not node_label.split()[0] in highlight_classes:
                 self.add_node(traversed_node, style_override=self._ignore_node_style)
             else:
                 self.add_node(traversed_node, style_override=None)
 
         # Add the origin node back into traversed nodes so it can be found for adding edges
         traversed_nodes[origin_pk] = origin_node
 
         # Add all links to the Graph, using the {id: Node} dictionary for queryless Node retrieval, applying
         # appropriate styling
-        for link in traversed_graph['links']:
+        for link in (traversed_graph['links'] or []):
             source_node = traversed_nodes[link.source_id]
             target_node = traversed_nodes[link.target_id]
             link_pair = LinkPair(self._convert_link_types(link.link_type)[0], link.link_label)
             link_style = self._link_styles(
                 link_pair, add_label=annotate_links in ['label', 'both'], add_type=annotate_links in ['type', 'both']
             )
             self.add_edge(source_node, target_node, link_pair, style=link_style)
 
     def add_origin_to_targets(
         self,
-        origin,
-        target_cls,
-        target_filters=None,
-        include_target_inputs=False,
-        include_target_outputs=False,
-        origin_style=(),
-        annotate_links=False
-    ):
+        origin: int | str | orm.Node,
+        target_cls: type[orm.Node],
+        target_filters: dict | None = None,
+        include_target_inputs: bool = False,
+        include_target_outputs: bool = False,
+        origin_style: Mapping[str, Any] | None = None,
+        annotate_links: LinkAnnotateType = None
+    ) -> None:
         """Add nodes and edges from an origin node to all nodes of a target node class.
 
         :param origin: node or node pk/uuid
-        :type origin: aiida.orm.nodes.node.Node or int
         :param target_cls: target node class
-        :param target_filters:  (Default value = None)
-        :type target_filters: dict or None
-        :param include_target_inputs:  (Default value = False)
-        :type include_target_inputs: bool
-        :param include_target_outputs:  (Default value = False)
-        :type include_target_outputs: bool
-        :param origin_style: node style map for origin node (Default value = ())
-        :type origin_style: dict or tuple
-        :param annotate_links: label edges with the link 'label', 'type' or 'both' (Default value = False)
-        :type annotate_links: bool
+        :param target_filters: filters for query of target nodes
+        :param include_target_inputs: Include incoming links for all target nodes
+        :param include_target_outputs: Include outgoing links for all target nodes
+        :param origin_style: node style map for origin node
+        :param annotate_links: label edges with the link 'label', 'type' or 'both'
         """
         # pylint: disable=too-many-arguments
         origin_node = self._load_node(origin)
 
         if target_filters is None:
             target_filters = {}
 
-        self.add_node(origin_node, style_override=dict(origin_style))
+        self.add_node(origin_node, style_override=dict(origin_style or {}))
 
         query = orm.QueryBuilder(
             backend=self.backend,
-            **{
-                'path': [{
-                    'cls': origin_node.__class__,
-                    'filters': {
-                        'id': origin_node.pk
-                    },
-                    'tag': 'origin'
-                }, {
-                    'cls': target_cls,
-                    'filters': target_filters,
-                    'with_ancestors': 'origin',
-                    'tag': 'target',
-                    'project': '*'
-                }]
-            }
+            path=[{
+                'cls': origin_node.__class__,
+                'filters': {
+                    'id': origin_node.pk
+                },
+                'tag': 'origin'
+            }, {
+                'cls': target_cls,
+                'filters': target_filters,
+                'with_ancestors': 'origin',
+                'tag': 'target',
+                'project': '*'
+            }]
         )
 
         for (target_node,) in query.iterall():
             self.add_node(target_node)
             self.add_edge(origin_node, target_node, style={'style': 'dashed', 'color': 'grey'})
 
             if include_target_inputs:
                 self.add_incoming(target_node, annotate_links=annotate_links)
 
             if include_target_outputs:
                 self.add_outgoing(target_node, annotate_links=annotate_links)
 
     def add_origins_to_targets(
         self,
-        origin_cls,
-        target_cls,
-        origin_filters=None,
-        target_filters=None,
-        include_target_inputs=False,
-        include_target_outputs=False,
-        origin_style=(),
-        annotate_links=False
-    ):
+        origin_cls: type[orm.Node],
+        target_cls: type[orm.Node],
+        origin_filters: dict | None = None,
+        target_filters: dict | None = None,
+        include_target_inputs: bool = False,
+        include_target_outputs: bool = False,
+        origin_style: Mapping[str, Any] | None = None,
+        annotate_links: LinkAnnotateType = None
+    ) -> None:
         """Add nodes and edges from all nodes of an origin class to all node of a target node class.
 
         :param origin_cls: origin node class
         :param target_cls: target node class
-        :param origin_filters:  (Default value = None)
-        :type origin_filters: dict or None
-        :param target_filters:  (Default value = None)
-        :type target_filters: dict or None
-        :param include_target_inputs:  (Default value = False)
-        :type include_target_inputs: bool
-        :param include_target_outputs:  (Default value = False)
-        :type include_target_outputs: bool
-        :param origin_style: node style map for origin node (Default value = ())
-        :type origin_style: dict or tuple
-        :param annotate_links: label edges with the link 'label', 'type' or 'both' (Default value = False)
-        :type annotate_links: bool
+        :param origin_filters: filters for origin nodes
+        :param target_filters: filters for target nodes
+        :param include_target_inputs: Include incoming links for all target nodes
+        :param include_target_outputs: Include outgoing links for all target nodes
+        :param origin_style: node style map for origin node
+        :param annotate_links: label edges with the link 'label', 'type' or 'both'
         """
         # pylint: disable=too-many-arguments
         if origin_filters is None:
             origin_filters = {}
 
         query = orm.QueryBuilder(
             backend=self.backend,
-            **{'path': [{
+            path=[{
                 'cls': origin_cls,
                 'filters': origin_filters,
                 'tag': 'origin',
                 'project': '*'
-            }]}
+            }]
         )
 
         for (node,) in query.iterall():
             self.add_origin_to_targets(
                 node,
                 target_cls,
                 target_filters=target_filters,
```

### Comparing `aiida-core-2.2.2/aiida/transports/__init__.py` & `aiida-core-2.3.0/aiida/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/transports/cli.py` & `aiida-core-2.3.0/aiida/transports/cli.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/transports/plugins/__init__.py` & `aiida-core-2.3.0/aiida/transports/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/transports/plugins/local.py` & `aiida-core-2.3.0/aiida/transports/plugins/local.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/transports/plugins/ssh.py` & `aiida-core-2.3.0/aiida/transports/plugins/ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,35 +118,29 @@
                 'prompt': 'Allow ssh agent',
                 'help': 'Switch to allow or disallow using an SSH agent.',
                 'non_interactive_default': True
             }
         ),
         (
             'proxy_jump', {
-                'prompt':
-                'SSH proxy jump',
-                'help':
-                'SSH proxy jump for tunneling through other SSH hosts.'
+                'prompt': 'SSH proxy jump',
+                'help': 'SSH proxy jump for tunneling through other SSH hosts.'
                 ' Use a comma-separated list of hosts of the form [user@]host[:port].'
                 ' If user or port are not specified for a host, the user & port values from the target host are used.'
                 ' This option must be provided explicitly and is not parsed from the SSH config file when left empty.',
-                'non_interactive_default':
-                True
+                'non_interactive_default': True
             }
         ),  # Managed 'manually' in connect
         (
             'proxy_command', {
-                'prompt':
-                'SSH proxy command',
-                'help':
-                'SSH proxy command for tunneling through a proxy server.'
+                'prompt': 'SSH proxy command',
+                'help': 'SSH proxy command for tunneling through a proxy server.'
                 ' For tunneling through another SSH host, consider using the "SSH proxy jump" option instead!'
                 ' Leave empty to parse the proxy command from the SSH config file.',
-                'non_interactive_default':
-                True
+                'non_interactive_default': True
             }
         ),  # Managed 'manually' in connect
         (
             'compress', {
                 'default': True,
                 'switch': True,
                 'prompt': 'Compress file transfers',
```

### Comparing `aiida-core-2.2.2/aiida/transports/transport.py` & `aiida-core-2.3.0/aiida/transports/transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,26 +51,21 @@
     # See the ssh or local plugin to see the format
     _valid_auth_params = None
     _MAGIC_CHECK = re.compile('[*?[]')
     _valid_auth_options: list = []
     _common_auth_options = [
         (
             'use_login_shell', {
-                'default':
-                True,
-                'switch':
-                True,
-                'prompt':
-                'Use login shell when executing command',
-                'help':
-                ' Not using a login shell can help suppress potential'
+                'default': True,
+                'switch': True,
+                'prompt': 'Use login shell when executing command',
+                'help': ' Not using a login shell can help suppress potential'
                 ' spurious text output that can prevent AiiDA from parsing the output of commands,'
                 ' but may result in some startup files (.profile) not being sourced.',
-                'non_interactive_default':
-                True
+                'non_interactive_default': True
             }
         ),
         (
             'safe_interval', {
                 'type': float,
                 'prompt': 'Connection cooldown time (s)',
                 'help': 'Minimum time interval in seconds between opening new connections.',
```

### Comparing `aiida-core-2.2.2/aiida/transports/util.py` & `aiida-core-2.3.0/aiida/transports/util.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/workflows/__init__.py` & `aiida-core-2.3.0/aiida/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/workflows/arithmetic/__init__.py` & `aiida-core-2.3.0/aiida/workflows/arithmetic/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/workflows/arithmetic/add_multiply.py` & `aiida-core-2.3.0/aiida/workflows/arithmetic/add_multiply.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/aiida/workflows/arithmetic/multiply_add.py` & `aiida-core-2.3.0/aiida/workflows/arithmetic/multiply_add.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/environment.yml` & `aiida-core-2.3.0/environment.yml`

 * *Files 8% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 - defaults
 dependencies:
 - python~=3.8
 - alembic~=1.2
 - archive-path~=0.4.2
 - aio-pika~=6.6
 - circus~=0.18.0
-- click-config-file~=0.6.0
 - click-spinner~=0.1.8
 - click~=8.1
 - disk-objectstore~=0.6.0
-- python-graphviz~=0.13
-- ipython~=7.20
+- docstring_parser
+- get-annotations~=0.1
+- python-graphviz~=0.19
+- ipython<9,>=7
 - jinja2~=3.0
 - jsonschema~=3.0
 - kiwipy[rmq]~=0.7.7
-- importlib-metadata~=4.3
+- importlib-metadata~=4.13
 - importlib-resources~=5.0
 - numpy~=1.19
 - paramiko>=2.7.2,~=2.7
-- plumpy~=0.21.3
+- plumpy~=0.21.6
 - pgsu~=0.2.1
 - psutil~=5.6
 - psycopg2-binary~=2.8
 - pytz~=2021.1
 - pyyaml~=6.0
 - requests~=2.0
 - sqlalchemy~=1.4.22
 - tabulate~=0.8.5
 - tqdm~=4.45
 - upf_to_json~=0.9.2
-- werkzeug<2.2
 - wrapt~=1.11
```

### Comparing `aiida-core-2.2.2/open_source_licenses.txt` & `aiida-core-2.3.0/open_source_licenses.txt`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/pyproject.toml` & `aiida-core-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,39 +25,39 @@
 keywords = ["aiida", "workflows"]
 requires-python = ">=3.8"
 dependencies = [
     "alembic~=1.2",
     "archive-path~=0.4.2",
     "aio-pika~=6.6",
     "circus~=0.18.0",
-    "click-config-file~=0.6.0",
     "click-spinner~=0.1.8",
     "click~=8.1",
     "disk-objectstore~=0.6.0",
-    "graphviz~=0.13",
-    "ipython~=7.20",
+    "docstring-parser",
+    "get-annotations~=0.1;python_version<'3.10'",
+    "graphviz~=0.19",
+    "ipython>=7,<9",
     "jinja2~=3.0",
     "jsonschema~=3.0",
     "kiwipy[rmq]~=0.7.7",
-    "importlib-metadata~=4.3",
+    "importlib-metadata~=4.13",
     "importlib-resources~=5.0;python_version<'3.9'",
     "numpy~=1.19",
     "paramiko~=2.7,>=2.7.2",
-    "plumpy~=0.21.3",
+    "plumpy~=0.21.6",
     "pgsu~=0.2.1",
     "psutil~=5.6",
     "psycopg2-binary~=2.8",
     "pytz~=2021.1",
     "pyyaml~=6.0",
     "requests~=2.0",
     "sqlalchemy~=1.4.22",
     "tabulate~=0.8.5",
     "tqdm~=4.45",
     "upf_to_json~=0.9.2",
-    "werkzeug<2.2",
     "wrapt~=1.11"
 ]
 
 [project.urls]
 Home = "http://www.aiida.net/"
 Documentation = "https://aiida.readthedocs.io"
 Source = "https://github.com/aiidateam/aiida-core"
@@ -80,15 +80,15 @@
     "sphinx~=4.1",
     "sphinxcontrib-details-directive~=0.1.0",
     "sphinx-copybutton~=0.5.0",
     "sphinx-design~=0.0.13",
     "sphinx-notfound-page~=0.5",
     "sphinxext-rediraffe~=0.2.4",
     "sphinx-sqlalchemy~=0.1.1",
-    "sphinx-intl[transifex]~=2.0.1",
+    "sphinx-intl~=2.1.0",
     "myst-nb~=0.17.0",
 ]
 atomic_tools = [
     "PyCifRW~=4.4",
     "ase~=3.18",
     "matplotlib~=3.3,>=3.3.4",
     "pymatgen>=2022.1.20",
@@ -348,14 +348,15 @@
 based_on_style = "google"
 column_limit = 120
 dedent_closing_brackets = true
 coalesce_brackets = true
 align_closing_bracket_with_visual_indent = true
 split_arguments_when_comma_terminated = true
 indent_dictionary_value = false
+allow_split_before_dict_value = false
 
 [tool.mypy]
 show_error_codes = true
 scripts_are_modules = true
 show_traceback = true
 plugins = ["sqlalchemy.ext.mypy.plugin"]
 
@@ -389,14 +390,15 @@
     'CifFile.*',
     'circus.*',
     'click_config_file.*',
     'click_spinner.*',
     'docutils.*',
     'flask_cors.*',
     'flask_restful.*',
+    'get_annotations.*',
     'graphviz.*',
     'importlib._bootstrap.*',
     'IPython.*',
     'jsonschema.*',
     'kiwipy.*',
     'matplotlib.*',
     'mayavi.*',
```

### Comparing `aiida-core-2.2.2/requirements/requirements-py-3.10.txt` & `aiida-core-2.3.0/requirements/requirements-py-3.8.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,40 +16,42 @@
 beautifulsoup4==4.10.0
 bleach==4.1.0
 certifi==2022.12.7
 cffi==1.15.0
 charset-normalizer==2.0.8
 circus==0.18.0
 click==8.1.0
-click-config-file==0.6.0
 click-spinner==0.1.10
 configobj==5.0.6
 coverage==6.5.0
-cryptography==36.0.0
+cryptography==39.0.1
 cycler==0.11.0
 debugpy==1.5.1
 decorator==5.1.0
 defusedxml==0.7.1
 deprecation==2.1.0
 disk-objectstore==0.6.0
+docstring-parser==0.15.0
 docutils==0.16
 entrypoints==0.3
 Flask==2.0.3
 Flask-Cors==3.0.10
 Flask-RESTful==0.3.9
 fonttools==4.28.2
-future==0.18.2
+future==0.18.3
+get-annotations==0.1.2
 graphviz==0.19
 greenlet==1.1.2
 idna==3.3
 imagesize==1.3.0
-importlib-metadata==4.8.2
+importlib-metadata==4.13.0
+importlib-resources==5.4.0
 iniconfig==1.1.1
 ipykernel==6.5.1
-ipython==7.31.1
+ipython==8.10.0
 ipython-genutils==0.2.0
 ipywidgets==7.6.5
 itsdangerous==2.0.1
 jedi==0.18.1
 Jinja2==3.0.3
 jsonschema==3.2.0
 jupyter==1.0.0
@@ -57,15 +59,15 @@
 jupyter-console==6.4.0
 jupyter-core==4.11.2
 jupyterlab-pygments==0.1.2
 jupyterlab-widgets==1.0.2
 kiwipy==0.7.7
 kiwisolver==1.3.2
 Mako==1.2.2
-MarkupSafe==2.0.1
+MarkupSafe==2.1.1
 matplotlib==3.5.0
 matplotlib-inline==0.1.3
 mistune==0.8.4
 monty==2021.8.17
 mpmath==1.2.1
 multidict==5.2.0
 myst-nb==0.17.1
@@ -86,17 +88,17 @@
 pg8000==1.23.0
 pgsu==0.2.1
 pgtest==1.3.2
 pickleshare==0.7.5
 Pillow==9.3.0
 plotly==5.4.0
 pluggy==1.0.0
-plumpy==0.21.3
+plumpy==0.21.6
 prometheus-client==0.12.0
-prompt-toolkit==3.0.23
+prompt-toolkit==3.0.37
 psutil==5.8.0
 psycopg2-binary==2.9.1
 ptyprocess==0.7.0
 py==1.11.0
 py-cpuinfo==8.0.0
 PyCifRW==4.4.3
 pycparser==2.21
@@ -121,28 +123,29 @@
 pytz==2021.3
 PyYAML==6.0.0
 pyzmq==22.3.0
 qtconsole==5.2.1
 QtPy==1.11.2
 requests==2.26.0
 ruamel.yaml==0.17.17
+ruamel.yaml.clib==0.2.6
 scipy==1.7.3
 scramp==1.4.1
 seekpath==1.9.7
 Send2Trash==1.8.0
 setuptools-scm==6.3.2
 shortuuid==1.0.8
 six==1.16.0
 snowballstemmer==2.2.0
 soupsieve==2.3.1
 spglib==2.0.2
 sphinx==4.4.0
 sphinx-copybutton==0.5.0
 sphinx-design==0.0.13
-sphinx-intl==2.0.1
+sphinx-intl==2.1.0
 sphinx-notfound-page==0.8
 sphinx-sqlalchemy==0.1.1
 sphinxcontrib-applehelp==1.0.2
 sphinxcontrib-details-directive==0.1.0
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.0
 sphinxcontrib-jsmath==1.0.1
@@ -162,12 +165,12 @@
 tqdm==4.62.3
 traitlets==5.1.1
 uncertainties==3.1.6
 upf-to-json==0.9.3
 urllib3==1.26.7
 wcwidth==0.2.5
 webencodings==0.5.1
-Werkzeug==2.0.2
+Werkzeug==2.2.3
 widgetsnbextension==3.5.2
 wrapt==1.11.2
 yarl==1.7.2
 zipp==3.6.0
```

### Comparing `aiida-core-2.2.2/requirements/requirements-py-3.11.txt` & `aiida-core-2.3.0/requirements/requirements-py-3.11.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,42 +18,42 @@
 beautifulsoup4==4.11.1
 bleach==5.0.1
 certifi==2022.12.7
 cffi==1.15.1
 charset-normalizer==2.1.1
 circus==0.18.0
 click==8.1.3
-click-config-file==0.6.0
 click-spinner==0.1.10
 configobj==5.0.6
 contourpy==1.0.6
 coverage==6.5.0
-cryptography==38.0.4
+cryptography==39.0.1
 cycler==0.11.0
 debugpy==1.6.4
 decorator==5.1.1
 defusedxml==0.7.1
 deprecation==2.1.0
 disk-objectstore==0.6.0
+docstring-parser==0.15.0
 docutils==0.16
 emmet-core==0.39.0
 fastjsonschema==2.16.2
 Flask==2.1.3
 Flask-Cors==3.0.10
 Flask-RESTful==0.3.9
 fonttools==4.38.0
-future==0.18.2
+future==0.18.3
 graphviz==0.20.1
 greenlet==2.0.1
 idna==3.4
 imagesize==1.4.1
 importlib-metadata==4.13.0
 iniconfig==1.1.1
 ipykernel==6.17.1
-ipython==7.34.0
+ipython==8.10.0
 ipython-genutils==0.2.0
 ipywidgets==8.0.2
 itsdangerous==2.1.2
 jedi==0.18.2
 Jinja2==3.1.2
 jsonschema==3.2.0
 jupyter==1.0.0
@@ -103,17 +103,17 @@
 pgsu==0.2.3
 pgtest==1.3.2
 pickleshare==0.7.5
 Pillow==9.3.0
 platformdirs==2.5.4
 plotly==5.11.0
 pluggy==1.0.0
-plumpy==0.21.3
+plumpy==0.21.6
 prometheus-client==0.15.0
-prompt-toolkit==3.0.33
+prompt-toolkit==3.0.37
 psutil==5.9.4
 psycopg2-binary==2.9.5
 ptyprocess==0.7.0
 py==1.11.0
 py-cpuinfo==9.0.0
 pybtex==0.24.0
 PyCifRW==4.4.5
@@ -154,15 +154,15 @@
 sniffio==1.3.0
 snowballstemmer==2.2.0
 soupsieve==2.3.2.post1
 spglib==2.0.2
 Sphinx==4.5.0
 sphinx-copybutton==0.5.1
 sphinx-design==0.0.13
-sphinx-intl==2.0.1
+sphinx-intl==2.1.0
 sphinx-notfound-page==0.8.3
 sphinx-sqlalchemy==0.1.1
 sphinxcontrib-applehelp==1.0.2
 sphinxcontrib-details-directive==0.1.0
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.0
 sphinxcontrib-jsmath==1.0.1
@@ -184,12 +184,12 @@
 typing_extensions==4.4.0
 uncertainties==3.1.7
 upf-to-json==0.9.5
 urllib3==1.26.13
 wcwidth==0.2.5
 webencodings==0.5.1
 websocket-client==1.4.2
-Werkzeug==2.1.2
+Werkzeug==2.2.3
 widgetsnbextension==4.0.3
 wrapt==1.14.1
 yarl==1.8.1
 zipp==3.11.0
```

### Comparing `aiida-core-2.2.2/requirements/requirements-py-3.8.txt` & `aiida-core-2.3.0/requirements/requirements-py-3.9.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,41 +16,41 @@
 beautifulsoup4==4.10.0
 bleach==4.1.0
 certifi==2022.12.7
 cffi==1.15.0
 charset-normalizer==2.0.8
 circus==0.18.0
 click==8.1.0
-click-config-file==0.6.0
 click-spinner==0.1.10
 configobj==5.0.6
 coverage==6.5.0
-cryptography==36.0.0
+cryptography==39.0.1
 cycler==0.11.0
 debugpy==1.5.1
 decorator==5.1.0
 defusedxml==0.7.1
 deprecation==2.1.0
 disk-objectstore==0.6.0
+docstring-parser==0.15.0
 docutils==0.16
 entrypoints==0.3
 Flask==2.0.3
 Flask-Cors==3.0.10
 Flask-RESTful==0.3.9
 fonttools==4.28.2
-future==0.18.2
+future==0.18.3
+get-annotations==0.1.2
 graphviz==0.19
 greenlet==1.1.2
 idna==3.3
 imagesize==1.3.0
-importlib-metadata==4.8.2
-importlib-resources==5.4.0
+importlib-metadata==4.13.0
 iniconfig==1.1.1
 ipykernel==6.5.1
-ipython==7.31.1
+ipython==8.10.0
 ipython-genutils==0.2.0
 ipywidgets==7.6.5
 itsdangerous==2.0.1
 jedi==0.18.1
 Jinja2==3.0.3
 jsonschema==3.2.0
 jupyter==1.0.0
@@ -58,15 +58,15 @@
 jupyter-console==6.4.0
 jupyter-core==4.11.2
 jupyterlab-pygments==0.1.2
 jupyterlab-widgets==1.0.2
 kiwipy==0.7.7
 kiwisolver==1.3.2
 Mako==1.2.2
-MarkupSafe==2.0.1
+MarkupSafe==2.1.1
 matplotlib==3.5.0
 matplotlib-inline==0.1.3
 mistune==0.8.4
 monty==2021.8.17
 mpmath==1.2.1
 multidict==5.2.0
 myst-nb==0.17.1
@@ -87,17 +87,17 @@
 pg8000==1.23.0
 pgsu==0.2.1
 pgtest==1.3.2
 pickleshare==0.7.5
 Pillow==9.3.0
 plotly==5.4.0
 pluggy==1.0.0
-plumpy==0.21.3
+plumpy==0.21.6
 prometheus-client==0.12.0
-prompt-toolkit==3.0.23
+prompt-toolkit==3.0.37
 psutil==5.8.0
 psycopg2-binary==2.9.1
 ptyprocess==0.7.0
 py==1.11.0
 py-cpuinfo==8.0.0
 PyCifRW==4.4.3
 pycparser==2.21
@@ -136,15 +136,15 @@
 six==1.16.0
 snowballstemmer==2.2.0
 soupsieve==2.3.1
 spglib==2.0.2
 sphinx==4.4.0
 sphinx-copybutton==0.5.0
 sphinx-design==0.0.13
-sphinx-intl==2.0.1
+sphinx-intl==2.1.0
 sphinx-notfound-page==0.8
 sphinx-sqlalchemy==0.1.1
 sphinxcontrib-applehelp==1.0.2
 sphinxcontrib-details-directive==0.1.0
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.0
 sphinxcontrib-jsmath==1.0.1
@@ -164,12 +164,12 @@
 tqdm==4.62.3
 traitlets==5.1.1
 uncertainties==3.1.6
 upf-to-json==0.9.3
 urllib3==1.26.7
 wcwidth==0.2.5
 webencodings==0.5.1
-Werkzeug==2.0.2
+Werkzeug==2.2.3
 widgetsnbextension==3.5.2
 wrapt==1.11.2
 yarl==1.7.2
 zipp==3.6.0
```

### Comparing `aiida-core-2.2.2/requirements/requirements-py-3.9.txt` & `aiida-core-2.3.0/requirements/requirements-py-3.10.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,40 +16,40 @@
 beautifulsoup4==4.10.0
 bleach==4.1.0
 certifi==2022.12.7
 cffi==1.15.0
 charset-normalizer==2.0.8
 circus==0.18.0
 click==8.1.0
-click-config-file==0.6.0
 click-spinner==0.1.10
 configobj==5.0.6
 coverage==6.5.0
-cryptography==36.0.0
+cryptography==39.0.1
 cycler==0.11.0
 debugpy==1.5.1
 decorator==5.1.0
 defusedxml==0.7.1
 deprecation==2.1.0
 disk-objectstore==0.6.0
+docstring-parser==0.15.0
 docutils==0.16
 entrypoints==0.3
 Flask==2.0.3
 Flask-Cors==3.0.10
 Flask-RESTful==0.3.9
 fonttools==4.28.2
-future==0.18.2
+future==0.18.3
 graphviz==0.19
 greenlet==1.1.2
 idna==3.3
 imagesize==1.3.0
-importlib-metadata==4.8.2
+importlib-metadata==4.13.0
 iniconfig==1.1.1
 ipykernel==6.5.1
-ipython==7.31.1
+ipython==8.10.0
 ipython-genutils==0.2.0
 ipywidgets==7.6.5
 itsdangerous==2.0.1
 jedi==0.18.1
 Jinja2==3.0.3
 jsonschema==3.2.0
 jupyter==1.0.0
@@ -57,15 +57,15 @@
 jupyter-console==6.4.0
 jupyter-core==4.11.2
 jupyterlab-pygments==0.1.2
 jupyterlab-widgets==1.0.2
 kiwipy==0.7.7
 kiwisolver==1.3.2
 Mako==1.2.2
-MarkupSafe==2.0.1
+MarkupSafe==2.1.1
 matplotlib==3.5.0
 matplotlib-inline==0.1.3
 mistune==0.8.4
 monty==2021.8.17
 mpmath==1.2.1
 multidict==5.2.0
 myst-nb==0.17.1
@@ -86,17 +86,17 @@
 pg8000==1.23.0
 pgsu==0.2.1
 pgtest==1.3.2
 pickleshare==0.7.5
 Pillow==9.3.0
 plotly==5.4.0
 pluggy==1.0.0
-plumpy==0.21.3
+plumpy==0.21.6
 prometheus-client==0.12.0
-prompt-toolkit==3.0.23
+prompt-toolkit==3.0.37
 psutil==5.8.0
 psycopg2-binary==2.9.1
 ptyprocess==0.7.0
 py==1.11.0
 py-cpuinfo==8.0.0
 PyCifRW==4.4.3
 pycparser==2.21
@@ -121,29 +121,28 @@
 pytz==2021.3
 PyYAML==6.0.0
 pyzmq==22.3.0
 qtconsole==5.2.1
 QtPy==1.11.2
 requests==2.26.0
 ruamel.yaml==0.17.17
-ruamel.yaml.clib==0.2.6
 scipy==1.7.3
 scramp==1.4.1
 seekpath==1.9.7
 Send2Trash==1.8.0
 setuptools-scm==6.3.2
 shortuuid==1.0.8
 six==1.16.0
 snowballstemmer==2.2.0
 soupsieve==2.3.1
 spglib==2.0.2
 sphinx==4.4.0
 sphinx-copybutton==0.5.0
 sphinx-design==0.0.13
-sphinx-intl==2.0.1
+sphinx-intl==2.1.0
 sphinx-notfound-page==0.8
 sphinx-sqlalchemy==0.1.1
 sphinxcontrib-applehelp==1.0.2
 sphinxcontrib-details-directive==0.1.0
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.0
 sphinxcontrib-jsmath==1.0.1
@@ -163,12 +162,12 @@
 tqdm==4.62.3
 traitlets==5.1.1
 uncertainties==3.1.6
 upf-to-json==0.9.3
 urllib3==1.26.7
 wcwidth==0.2.5
 webencodings==0.5.1
-Werkzeug==2.0.2
+Werkzeug==2.2.3
 widgetsnbextension==3.5.2
 wrapt==1.11.2
 yarl==1.7.2
 zipp==3.6.0
```

### Comparing `aiida-core-2.2.2/utils/__init__.py` & `aiida-core-2.3.0/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/utils/dependency_management.py` & `aiida-core-2.3.0/utils/dependency_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import tomli
 import yaml
 
 ROOT = Path(__file__).resolve().parent.parent  # repository root
 
 SETUPTOOLS_CONDA_MAPPINGS = {
     'graphviz': 'python-graphviz',
+    'docstring-parser': 'docstring_parser',
 }
 
 CONDA_IGNORE = []
 
 GITHUB_ACTIONS = os.environ.get('GITHUB_ACTIONS') == 'true'
```

### Comparing `aiida-core-2.2.2/utils/make_all.py` & `aiida-core-2.3.0/utils/make_all.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/utils/validate_consistency.py` & `aiida-core-2.3.0/utils/validate_consistency.py`

 * *Files identical despite different names*

### Comparing `aiida-core-2.2.2/PKG-INFO` & `aiida-core-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-core
-Version: 2.2.2
+Version: 2.3.0
 Summary: AiiDA is a workflow manager for computational science with a strong focus on provenance, performance and extensibility.
 Keywords: aiida,workflows
 Author-email: The AiiDA team <developers@aiida.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
@@ -17,39 +17,39 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: alembic~=1.2
 Requires-Dist: archive-path~=0.4.2
 Requires-Dist: aio-pika~=6.6
 Requires-Dist: circus~=0.18.0
-Requires-Dist: click-config-file~=0.6.0
 Requires-Dist: click-spinner~=0.1.8
 Requires-Dist: click~=8.1
 Requires-Dist: disk-objectstore~=0.6.0
-Requires-Dist: graphviz~=0.13
-Requires-Dist: ipython~=7.20
+Requires-Dist: docstring-parser
+Requires-Dist: get-annotations~=0.1;python_version<'3.10'
+Requires-Dist: graphviz~=0.19
+Requires-Dist: ipython>=7,<9
 Requires-Dist: jinja2~=3.0
 Requires-Dist: jsonschema~=3.0
 Requires-Dist: kiwipy[rmq]~=0.7.7
-Requires-Dist: importlib-metadata~=4.3
+Requires-Dist: importlib-metadata~=4.13
 Requires-Dist: importlib-resources~=5.0;python_version<'3.9'
 Requires-Dist: numpy~=1.19
 Requires-Dist: paramiko~=2.7,>=2.7.2
-Requires-Dist: plumpy~=0.21.3
+Requires-Dist: plumpy~=0.21.6
 Requires-Dist: pgsu~=0.2.1
 Requires-Dist: psutil~=5.6
 Requires-Dist: psycopg2-binary~=2.8
 Requires-Dist: pytz~=2021.1
 Requires-Dist: pyyaml~=6.0
 Requires-Dist: requests~=2.0
 Requires-Dist: sqlalchemy~=1.4.22
 Requires-Dist: tabulate~=0.8.5
 Requires-Dist: tqdm~=4.45
 Requires-Dist: upf_to_json~=0.9.2
-Requires-Dist: werkzeug<2.2
 Requires-Dist: wrapt~=1.11
 Requires-Dist: PyCifRW~=4.4 ; extra == "atomic_tools"
 Requires-Dist: ase~=3.18 ; extra == "atomic_tools"
 Requires-Dist: matplotlib~=3.3,>=3.3.4 ; extra == "atomic_tools"
 Requires-Dist: pymatgen>=2022.1.20 ; extra == "atomic_tools"
 Requires-Dist: pymysql~=0.9.3 ; extra == "atomic_tools"
 Requires-Dist: seekpath~=1.9,>=1.9.3 ; extra == "atomic_tools"
@@ -59,15 +59,15 @@
 Requires-Dist: sphinx~=4.1 ; extra == "docs"
 Requires-Dist: sphinxcontrib-details-directive~=0.1.0 ; extra == "docs"
 Requires-Dist: sphinx-copybutton~=0.5.0 ; extra == "docs"
 Requires-Dist: sphinx-design~=0.0.13 ; extra == "docs"
 Requires-Dist: sphinx-notfound-page~=0.5 ; extra == "docs"
 Requires-Dist: sphinxext-rediraffe~=0.2.4 ; extra == "docs"
 Requires-Dist: sphinx-sqlalchemy~=0.1.1 ; extra == "docs"
-Requires-Dist: sphinx-intl[transifex]~=2.0.1 ; extra == "docs"
+Requires-Dist: sphinx-intl~=2.1.0 ; extra == "docs"
 Requires-Dist: myst-nb~=0.17.0 ; extra == "docs"
 Requires-Dist: jupyter-client~=6.1,<6.1.13 ; extra == "notebook"
 Requires-Dist: jupyter~=1.0 ; extra == "notebook"
 Requires-Dist: notebook~=6.1,>=6.1.5 ; extra == "notebook"
 Requires-Dist: mypy==0.991 ; extra == "pre-commit"
 Requires-Dist: packaging==20.3 ; extra == "pre-commit"
 Requires-Dist: pre-commit~=2.2 ; extra == "pre-commit"
@@ -107,23 +107,23 @@
 Provides-Extra: docs
 Provides-Extra: notebook
 Provides-Extra: pre-commit
 Provides-Extra: rest
 Provides-Extra: ssh_kerberos
 Provides-Extra: tests
 
-# <img src="http://www.aiida.net/wp-content/uploads/2020/06/logo_aiida.png" alt="AiiDA" width="200"/>
+# <img src="https://raw.githubusercontent.com/aiidateam/aiida-core/main/docs/source/images/aiida-logo.svg" alt="AiiDA" width="200"/>
 
 AiiDA (www.aiida.net) is a workflow manager for computational science with a strong focus on provenance, performance and extensibility.
 
 |    | |
 |-----|----------------------------------------------------------------------------|
 |Latest release| [![PyPI version](https://badge.fury.io/py/aiida-core.svg)](https://badge.fury.io/py/aiida-core) [![conda-forge](https://img.shields.io/conda/vn/conda-forge/aiida-core.svg?style=flat)](https://anaconda.org/conda-forge/aiida-core) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-core.svg)](https://pypi.python.org/pypi/aiida-core/) |
 |Getting help| [![Docs status](https://readthedocs.org/projects/aiida-core/badge)](http://aiida-core.readthedocs.io/) [![Google Group](https://img.shields.io/badge/-Google%20Group-lightgrey.svg)](https://groups.google.com/forum/#!forum/aiidausers)
-|Build status| [![Build Status](https://github.com/aiidateam/aiida-core/workflows/aiida-core/badge.svg)](https://github.com/aiidateam/aiida-core/actions) [![Coverage Status](https://codecov.io/gh/aiidateam/aiida-core/branch/main/graph/badge.svg)](https://codecov.io/gh/aiidateam/aiida-core) |
+|Build status| [![Build Status](https://github.com/aiidateam/aiida-core/actions/workflows/ci-code.yml/badge.svg)](https://github.com/aiidateam/aiida-core/actions) [![Coverage Status](https://codecov.io/gh/aiidateam/aiida-core/branch/main/graph/badge.svg)](https://codecov.io/gh/aiidateam/aiida-core) [Benchmarks](https://aiidateam.github.io/aiida-core/dev/bench/ubuntu-22.04/psql_dos/) |
 |Activity| [![PyPI-downloads](https://img.shields.io/pypi/dm/aiida-core.svg?style=flat)](https://pypistats.org/packages/aiida-core) [![Commit Activity](https://img.shields.io/github/commit-activity/m/aiidateam/aiida-core.svg)](https://github.com/aiidateam/aiida-core/pulse)
 |Community| [![Affiliated with NumFOCUS](https://img.shields.io/badge/NumFOCUS-affiliated%20project-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org/sponsored-projects/affiliated-projects) [![Twitter](https://img.shields.io/twitter/follow/aiidateam.svg?style=social&label=Follow)](https://twitter.com/aiidateam)
 
 
 ## Features
 
  -   **Workflows:** Write complex, auto-documenting workflows in
```

