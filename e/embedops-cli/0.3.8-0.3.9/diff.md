# Comparing `tmp/embedops-cli-0.3.8.tar.gz` & `tmp/embedops-cli-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedops-cli-0.3.8.tar", last modified: Sat Aug 13 07:44:01 2022, max compression
+gzip compressed data, was "embedops-cli-0.3.9.tar", last modified: Mon Aug 29 15:43:47 2022, max compression
```

## Comparing `embedops-cli-0.3.8.tar` & `embedops-cli-0.3.9.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-13 07:44:01.592829 embedops-cli-0.3.8/
--rw-rw-rw-   0 root         (0) root         (0)       33 2021-10-15 01:50:36.000000 embedops-cli-0.3.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4773 2022-08-13 07:44:01.592829 embedops-cli-0.3.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4187 2022-05-11 19:59:10.000000 embedops-cli-0.3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-13 07:44:01.576829 embedops-cli-0.3.8/embedops_cli/
--rw-rw-rw-   0 root         (0) root         (0)      252 2022-08-13 07:38:12.000000 embedops-cli-0.3.8/embedops_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-13 07:44:01.580829 embedops-cli-0.3.8/embedops_cli/api/
--rw-rw-rw-   0 root         (0) root         (0)     5045 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-13 07:44:01.580829 embedops-cli-0.3.8/embedops_cli/api/api/
--rw-rw-rw-   0 root         (0) root         (0)      143 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   172153 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/api/default_api.py
--rw-rw-rw-   0 root         (0) root         (0)    24581 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     8437 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)   172153 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/default_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-13 07:44:01.588829 embedops-cli-0.3.8/embedops_cli/api/models/
--rw-rw-rw-   0 root         (0) root         (0)     4451 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6424 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/aws_access_key.py
--rw-rw-rw-   0 root         (0) root         (0)     6718 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/aws_access_key_access_key.py
--rw-rw-rw-   0 root         (0) root         (0)     2518 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/branch_names.py
--rw-rw-rw-   0 root         (0) root         (0)     3932 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/ci_o_auth_token_update_props.py
--rw-rw-rw-   0 root         (0) root         (0)     3187 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/ci_o_auth_tokens.py
--rw-rw-rw-   0 root         (0) root         (0)     2626 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/ci_provider.py
--rw-rw-rw-   0 root         (0) root         (0)     9901 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/ci_run.py
--rw-rw-rw-   0 root         (0) root         (0)     7880 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/ci_run_artifact.py
--rw-rw-rw-   0 root         (0) root         (0)     3175 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/ci_run_artifact_create_props.py
--rw-rw-rw-   0 root         (0) root         (0)     6907 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/ci_run_create_props.py
--rw-rw-rw-   0 root         (0) root         (0)     3962 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/ci_run_id_artifacts_body.py
--rw-rw-rw-   0 root         (0) root         (0)     6561 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/ci_run_update_props.py
--rw-rw-rw-   0 root         (0) root         (0)     3634 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/created_at.py
--rw-rw-rw-   0 root         (0) root         (0)     6443 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/gitlab_access_token.py
--rw-rw-rw-   0 root         (0) root         (0)    10394 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/gitlab_access_token_token.py
--rw-rw-rw-   0 root         (0) root         (0)     6431 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/group.py
--rw-rw-rw-   0 root         (0) root         (0)     4309 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/group_create_props.py
--rw-rw-rw-   0 root         (0) root         (0)     4079 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/group_update_props.py
--rw-rw-rw-   0 root         (0) root         (0)     3179 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/inline_response400.py
--rw-rw-rw-   0 root         (0) root         (0)     3474 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/inline_response404.py
--rw-rw-rw-   0 root         (0) root         (0)     7184 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/job_def.py
--rw-rw-rw-   0 root         (0) root         (0)     4912 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/job_def_create_props.py
--rw-rw-rw-   0 root         (0) root         (0)     4685 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/job_def_update_props.py
--rw-rw-rw-   0 root         (0) root         (0)     5578 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/job_template.py
--rw-rw-rw-   0 root         (0) root         (0)     3239 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/job_template_update_props.py
--rw-rw-rw-   0 root         (0) root         (0)     7714 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/metric.py
--rw-rw-rw-   0 root         (0) root         (0)     5552 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/metric_create_props.py
--rw-rw-rw-   0 root         (0) root         (0)     6936 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/metric_result.py
--rw-rw-rw-   0 root         (0) root         (0)     7538 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/metric_result_ci_run.py
--rw-rw-rw-   0 root         (0) root         (0)     4471 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/metric_result_ci_run_repo.py
--rw-rw-rw-   0 root         (0) root         (0)     4512 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/metric_result_ci_run_repo_project.py
--rw-rw-rw-   0 root         (0) root         (0)     3828 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/metric_result_ci_run_repo_project_org.py
--rw-rw-rw-   0 root         (0) root         (0)     4215 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/myself_clitelemetry_body.py
--rw-rw-rw-   0 root         (0) root         (0)     6032 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/org.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/org_create_props.py
--rw-rw-rw-   0 root         (0) root         (0)     3095 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/org_update_props.py
--rw-rw-rw-   0 root         (0) root         (0)     6828 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/project.py
--rw-rw-rw-   0 root         (0) root         (0)     3240 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/project_create_props.py
--rw-rw-rw-   0 root         (0) root         (0)     4374 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/project_group_create_props.py
--rw-rw-rw-   0 root         (0) root         (0)     3771 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/project_group_update_props.py
--rw-rw-rw-   0 root         (0) root         (0)     3127 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/project_update_props.py
--rw-rw-rw-   0 root         (0) root         (0)     9980 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/repo.py
--rw-rw-rw-   0 root         (0) root         (0)     6973 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/repo_api_key.py
--rw-rw-rw-   0 root         (0) root         (0)     7414 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/repo_create_props.py
--rw-rw-rw-   0 root         (0) root         (0)     6518 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/repo_pipeline_config.py
--rw-rw-rw-   0 root         (0) root         (0)     3436 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/repo_pipeline_config_create_props.py
--rw-rw-rw-   0 root         (0) root         (0)     3436 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/repo_pipeline_config_update_props.py
--rw-rw-rw-   0 root         (0) root         (0)     4046 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/repo_pipeline_config_update_props_jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     7066 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/repo_update_props.py
--rw-rw-rw-   0 root         (0) root         (0)    12215 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/user.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/user_group_invite_props.py
--rw-rw-rw-   0 root         (0) root         (0)     4146 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/user_group_props.py
--rw-rw-rw-   0 root         (0) root         (0)     4154 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/user_group_props_group.py
--rw-rw-rw-   0 root         (0) root         (0)     3675 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/models/user_group_update_props.py
--rw-rw-rw-   0 root         (0) root         (0)     4220 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/api/models/user_update_props.py
--rw-rw-rw-   0 root         (0) root         (0)    13278 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/api/rest.py
--rw-rw-rw-   0 root         (0) root         (0)     2537 2022-03-04 23:30:50.000000 embedops-cli-0.3.8/embedops_cli/ci_config_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2022-03-04 23:30:50.000000 embedops-cli-0.3.8/embedops_cli/config.py
--rw-rw-rw-   0 root         (0) root         (0)     4596 2022-08-13 07:38:12.000000 embedops-cli-0.3.8/embedops_cli/docker_run.py
--rw-rw-rw-   0 root         (0) root         (0)     9750 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/embedops_cli/embedops_authorization.py
--rw-rw-rw-   0 root         (0) root         (0)    13167 2022-08-13 07:38:12.000000 embedops-cli-0.3.8/embedops_cli/embedops_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1905 2022-03-17 19:46:44.000000 embedops-cli-0.3.8/embedops_cli/environment_utilities.py
--rw-rw-rw-   0 root         (0) root         (0)     8990 2022-03-18 14:38:29.000000 embedops-cli-0.3.8/embedops_cli/eo_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-13 07:44:01.588829 embedops-cli-0.3.8/embedops_cli/eotools/
--rwxrwxrwx   0 root         (0) root         (0)     1536 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/eotools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4247 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/eotools/ci_run.py
--rwxrwxrwx   0 root         (0) root         (0)      331 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/eotools/create_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-13 07:44:01.588829 embedops-cli-0.3.8/embedops_cli/eotools/log_parser/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/eotools/log_parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/eotools/log_parser/gnu_size_berkeley.py
--rw-rw-rw-   0 root         (0) root         (0)      688 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/eotools/log_parser/iar.py
--rwxrwxrwx   0 root         (0) root         (0)     5171 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/eotools/parse.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/eotools/puller.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/eotools/sender.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/eotools/update_run.py
--rw-rw-rw-   0 root         (0) root         (0)      483 2022-05-27 11:55:24.000000 embedops-cli-0.3.8/embedops_cli/settings.toml
--rw-rw-rw-   0 root         (0) root         (0)      946 2022-06-21 20:56:56.000000 embedops-cli-0.3.8/embedops_cli/telemetry.py
--rw-rw-rw-   0 root         (0) root         (0)     3221 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/embedops_cli/utilities.py
--rw-rw-rw-   0 root         (0) root         (0)       67 2022-08-13 07:41:56.000000 embedops-cli-0.3.8/embedops_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-13 07:44:01.592829 embedops-cli-0.3.8/embedops_cli/yaml_tools/
--rw-rw-rw-   0 root         (0) root         (0)      452 2022-03-17 19:46:44.000000 embedops-cli-0.3.8/embedops_cli/yaml_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3088 2022-03-18 14:38:29.000000 embedops-cli-0.3.8/embedops_cli/yaml_tools/bb_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     3385 2022-03-17 19:46:44.000000 embedops-cli-0.3.8/embedops_cli/yaml_tools/gh_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     5150 2022-03-18 14:38:29.000000 embedops-cli-0.3.8/embedops_cli/yaml_tools/gl_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     3249 2022-03-17 19:46:44.000000 embedops-cli-0.3.8/embedops_cli/yaml_tools/yaml_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-13 07:44:01.580829 embedops-cli-0.3.8/embedops_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4773 2022-08-13 07:44:01.000000 embedops-cli-0.3.8/embedops_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4311 2022-08-13 07:44:01.000000 embedops-cli-0.3.8/embedops_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-13 07:44:01.000000 embedops-cli-0.3.8/embedops_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      303 2022-08-13 07:44:01.000000 embedops-cli-0.3.8/embedops_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      210 2022-08-13 07:44:01.000000 embedops-cli-0.3.8/embedops_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-08-13 07:44:01.000000 embedops-cli-0.3.8/embedops_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      260 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1299 2022-08-13 07:44:01.592829 embedops-cli-0.3.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-13 07:44:01.592829 embedops-cli-0.3.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)      202 2022-01-13 00:53:26.000000 embedops-cli-0.3.8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1685 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/tests/api_interface_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5280 2022-03-18 14:38:29.000000 embedops-cli-0.3.8/tests/bb_parser_test.py
--rwxrwxrwx   0 root         (0) root         (0)     1685 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/tests/check_api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     8594 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/tests/create_run_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5738 2022-03-18 14:38:29.000000 embedops-cli-0.3.8/tests/docker_run_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4495 2022-07-26 20:16:30.000000 embedops-cli-0.3.8/tests/embedops_authorization_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5004 2022-04-13 15:23:36.000000 embedops-cli-0.3.8/tests/embedops_cli_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1924 2022-03-17 19:46:44.000000 embedops-cli-0.3.8/tests/environment_utilities_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3336 2022-03-29 18:37:59.000000 embedops-cli-0.3.8/tests/eotools_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5962 2022-02-15 22:14:25.000000 embedops-cli-0.3.8/tests/gh_parser_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5414 2022-03-18 14:38:29.000000 embedops-cli-0.3.8/tests/gl_parser_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2595 2022-03-04 23:30:50.000000 embedops-cli-0.3.8/tests/utilities_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-29 15:43:47.384812 embedops-cli-0.3.9/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4773 2022-08-29 15:43:47.384812 embedops-cli-0.3.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4187 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-29 15:43:47.356812 embedops-cli-0.3.9/embedops_cli/
+-rw-rw-rw-   0 root         (0) root         (0)      252 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-29 15:43:47.360812 embedops-cli-0.3.9/embedops_cli/api/
+-rw-rw-rw-   0 root         (0) root         (0)     5045 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-29 15:43:47.360812 embedops-cli-0.3.9/embedops_cli/api/api/
+-rw-rw-rw-   0 root         (0) root         (0)      143 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   172153 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/api/default_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    24581 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)   172153 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/default_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-29 15:43:47.376812 embedops-cli-0.3.9/embedops_cli/api/models/
+-rw-rw-rw-   0 root         (0) root         (0)     4451 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6424 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/aws_access_key.py
+-rw-rw-rw-   0 root         (0) root         (0)     6718 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/aws_access_key_access_key.py
+-rw-rw-rw-   0 root         (0) root         (0)     2518 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/branch_names.py
+-rw-rw-rw-   0 root         (0) root         (0)     3932 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/ci_o_auth_token_update_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     3187 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/ci_o_auth_tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)     2626 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/ci_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     9901 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/ci_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     7880 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/ci_run_artifact.py
+-rw-rw-rw-   0 root         (0) root         (0)     3175 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/ci_run_artifact_create_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     6907 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/ci_run_create_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     3962 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/ci_run_id_artifacts_body.py
+-rw-rw-rw-   0 root         (0) root         (0)     6561 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/ci_run_update_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     3634 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/created_at.py
+-rw-rw-rw-   0 root         (0) root         (0)     6443 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/gitlab_access_token.py
+-rw-rw-rw-   0 root         (0) root         (0)    10394 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/gitlab_access_token_token.py
+-rw-rw-rw-   0 root         (0) root         (0)     6431 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/group.py
+-rw-rw-rw-   0 root         (0) root         (0)     4309 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/group_create_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     4079 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/group_update_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     3179 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/inline_response400.py
+-rw-rw-rw-   0 root         (0) root         (0)     3474 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/inline_response404.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/job_def.py
+-rw-rw-rw-   0 root         (0) root         (0)     4912 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/job_def_create_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     4685 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/job_def_update_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     5578 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/job_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     3239 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/job_template_update_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     7714 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/metric.py
+-rw-rw-rw-   0 root         (0) root         (0)     5552 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/metric_create_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     6936 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/metric_result.py
+-rw-rw-rw-   0 root         (0) root         (0)     7538 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/metric_result_ci_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     4471 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/metric_result_ci_run_repo.py
+-rw-rw-rw-   0 root         (0) root         (0)     4512 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/metric_result_ci_run_repo_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     3828 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/metric_result_ci_run_repo_project_org.py
+-rw-rw-rw-   0 root         (0) root         (0)     4215 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/myself_clitelemetry_body.py
+-rw-rw-rw-   0 root         (0) root         (0)     6032 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/org.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/org_create_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     3095 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/org_update_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     6828 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     3240 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/project_create_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     4374 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/project_group_create_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     3771 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/project_group_update_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     3127 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/project_update_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     9980 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/repo.py
+-rw-rw-rw-   0 root         (0) root         (0)     6973 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/repo_api_key.py
+-rw-rw-rw-   0 root         (0) root         (0)     7414 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/repo_create_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     6518 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/repo_pipeline_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3436 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/repo_pipeline_config_create_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     3436 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/repo_pipeline_config_update_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     4046 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/repo_pipeline_config_update_props_jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     7066 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/repo_update_props.py
+-rw-rw-rw-   0 root         (0) root         (0)    12215 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/user.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/user_group_invite_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     4146 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/user_group_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     4154 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/user_group_props_group.py
+-rw-rw-rw-   0 root         (0) root         (0)     3675 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/user_group_update_props.py
+-rw-rw-rw-   0 root         (0) root         (0)     4220 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/models/user_update_props.py
+-rw-rw-rw-   0 root         (0) root         (0)    13278 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/api/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/ci_config_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     4596 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/docker_run.py
+-rw-rw-rw-   0 root         (0) root         (0)    11716 2022-08-25 14:30:42.000000 embedops-cli-0.3.9/embedops_cli/embedops_authorization.py
+-rw-rw-rw-   0 root         (0) root         (0)    13348 2022-08-24 13:17:22.000000 embedops-cli-0.3.9/embedops_cli/embedops_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/environment_utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     8990 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/eo_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-29 15:43:47.380812 embedops-cli-0.3.9/embedops_cli/eotools/
+-rwxrwxrwx   0 root         (0) root         (0)     1536 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/eotools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4247 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/eotools/ci_run.py
+-rwxrwxrwx   0 root         (0) root         (0)      331 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/eotools/create_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-29 15:43:47.380812 embedops-cli-0.3.9/embedops_cli/eotools/log_parser/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/eotools/log_parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/eotools/log_parser/gnu_size_berkeley.py
+-rw-rw-rw-   0 root         (0) root         (0)      688 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/eotools/log_parser/iar.py
+-rwxrwxrwx   0 root         (0) root         (0)     5171 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/eotools/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/eotools/puller.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/eotools/sender.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/eotools/update_run.py
+-rw-rw-rw-   0 root         (0) root         (0)      483 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/settings.toml
+-rw-rw-rw-   0 root         (0) root         (0)      946 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/telemetry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3221 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)       67 2022-08-29 15:40:21.000000 embedops-cli-0.3.9/embedops_cli/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-29 15:43:47.380812 embedops-cli-0.3.9/embedops_cli/yaml_tools/
+-rw-rw-rw-   0 root         (0) root         (0)      452 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/yaml_tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3088 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/yaml_tools/bb_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     3385 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/yaml_tools/gh_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     5150 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/yaml_tools/gl_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     3249 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/embedops_cli/yaml_tools/yaml_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-29 15:43:47.360812 embedops-cli-0.3.9/embedops_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4773 2022-08-29 15:43:47.000000 embedops-cli-0.3.9/embedops_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4311 2022-08-29 15:43:47.000000 embedops-cli-0.3.9/embedops_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-29 15:43:47.000000 embedops-cli-0.3.9/embedops_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      303 2022-08-29 15:43:47.000000 embedops-cli-0.3.9/embedops_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      210 2022-08-29 15:43:47.000000 embedops-cli-0.3.9/embedops_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-08-29 15:43:47.000000 embedops-cli-0.3.9/embedops_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      260 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2022-08-29 15:43:47.384812 embedops-cli-0.3.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-29 15:43:47.384812 embedops-cli-0.3.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      202 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2022-08-24 13:17:22.000000 embedops-cli-0.3.9/tests/api_interface_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5280 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/tests/bb_parser_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     1685 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/tests/check_api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     8593 2022-08-24 13:17:22.000000 embedops-cli-0.3.9/tests/create_run_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5738 2022-08-24 13:11:27.000000 embedops-cli-0.3.9/tests/docker_run_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     6932 2022-08-25 14:34:24.000000 embedops-cli-0.3.9/tests/embedops_authorization_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5033 2022-08-24 13:17:22.000000 embedops-cli-0.3.9/tests/embedops_cli_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1924 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/tests/environment_utilities_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3355 2022-08-24 13:17:22.000000 embedops-cli-0.3.9/tests/eotools_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5962 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/tests/gh_parser_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5414 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/tests/gl_parser_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2022-08-22 21:47:22.000000 embedops-cli-0.3.9/tests/utilities_test.py
```

### Comparing `embedops-cli-0.3.8/PKG-INFO` & `embedops-cli-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedops-cli
-Version: 0.3.8
+Version: 0.3.9
 Summary: EmbedOps Command Line Tools
 Home-page: https://embedops.io
 Author: Dojo Five, LLC
 Author-email: embedops@dojofive.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
```

### Comparing `embedops-cli-0.3.8/README.md` & `embedops-cli-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/__init__.py` & `embedops-cli-0.3.9/embedops_cli/api/__init__.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/api/default_api.py` & `embedops-cli-0.3.9/embedops_cli/api/api/default_api.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/api_client.py` & `embedops-cli-0.3.9/embedops_cli/api/api_client.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/configuration.py` & `embedops-cli-0.3.9/embedops_cli/api/configuration.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/default_api.py` & `embedops-cli-0.3.9/embedops_cli/api/default_api.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/__init__.py` & `embedops-cli-0.3.9/embedops_cli/api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/aws_access_key.py` & `embedops-cli-0.3.9/embedops_cli/api/models/aws_access_key.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/aws_access_key_access_key.py` & `embedops-cli-0.3.9/embedops_cli/api/models/aws_access_key_access_key.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/branch_names.py` & `embedops-cli-0.3.9/embedops_cli/api/models/branch_names.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/ci_o_auth_token_update_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/ci_o_auth_token_update_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/ci_o_auth_tokens.py` & `embedops-cli-0.3.9/embedops_cli/api/models/ci_o_auth_tokens.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/ci_provider.py` & `embedops-cli-0.3.9/embedops_cli/api/models/ci_provider.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/ci_run.py` & `embedops-cli-0.3.9/embedops_cli/api/models/ci_run.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/ci_run_artifact.py` & `embedops-cli-0.3.9/embedops_cli/api/models/ci_run_artifact.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/ci_run_artifact_create_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/ci_run_artifact_create_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/ci_run_create_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/ci_run_create_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/ci_run_id_artifacts_body.py` & `embedops-cli-0.3.9/embedops_cli/api/models/ci_run_id_artifacts_body.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/ci_run_update_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/ci_run_update_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/created_at.py` & `embedops-cli-0.3.9/embedops_cli/api/models/created_at.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/gitlab_access_token.py` & `embedops-cli-0.3.9/embedops_cli/api/models/gitlab_access_token.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/gitlab_access_token_token.py` & `embedops-cli-0.3.9/embedops_cli/api/models/gitlab_access_token_token.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/group.py` & `embedops-cli-0.3.9/embedops_cli/api/models/group.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/group_create_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/group_create_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/group_update_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/group_update_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/inline_response400.py` & `embedops-cli-0.3.9/embedops_cli/api/models/inline_response400.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/inline_response404.py` & `embedops-cli-0.3.9/embedops_cli/api/models/inline_response404.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/job_def.py` & `embedops-cli-0.3.9/embedops_cli/api/models/job_def.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/job_def_create_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/job_def_create_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/job_def_update_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/job_def_update_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/job_template.py` & `embedops-cli-0.3.9/embedops_cli/api/models/job_template.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/job_template_update_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/job_template_update_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/metric.py` & `embedops-cli-0.3.9/embedops_cli/api/models/metric.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/metric_create_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/metric_create_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/metric_result.py` & `embedops-cli-0.3.9/embedops_cli/api/models/metric_result.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/metric_result_ci_run.py` & `embedops-cli-0.3.9/embedops_cli/api/models/metric_result_ci_run.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/metric_result_ci_run_repo.py` & `embedops-cli-0.3.9/embedops_cli/api/models/metric_result_ci_run_repo.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/metric_result_ci_run_repo_project.py` & `embedops-cli-0.3.9/embedops_cli/api/models/metric_result_ci_run_repo_project.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/metric_result_ci_run_repo_project_org.py` & `embedops-cli-0.3.9/embedops_cli/api/models/metric_result_ci_run_repo_project_org.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/myself_clitelemetry_body.py` & `embedops-cli-0.3.9/embedops_cli/api/models/myself_clitelemetry_body.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/org.py` & `embedops-cli-0.3.9/embedops_cli/api/models/org.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/org_create_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/org_create_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/org_update_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/org_update_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/project.py` & `embedops-cli-0.3.9/embedops_cli/api/models/project.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/project_create_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/project_create_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/project_group_create_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/project_group_create_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/project_group_update_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/project_group_update_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/project_update_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/project_update_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/repo.py` & `embedops-cli-0.3.9/embedops_cli/api/models/repo.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/repo_api_key.py` & `embedops-cli-0.3.9/embedops_cli/api/models/repo_api_key.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/repo_create_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/repo_create_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/repo_pipeline_config.py` & `embedops-cli-0.3.9/embedops_cli/api/models/repo_pipeline_config.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/repo_pipeline_config_create_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/repo_pipeline_config_create_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/repo_pipeline_config_update_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/repo_pipeline_config_update_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/repo_pipeline_config_update_props_jobs.py` & `embedops-cli-0.3.9/embedops_cli/api/models/repo_pipeline_config_update_props_jobs.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/repo_update_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/repo_update_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/user.py` & `embedops-cli-0.3.9/embedops_cli/api/models/user.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/user_group_invite_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/user_group_invite_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/user_group_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/user_group_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/user_group_props_group.py` & `embedops-cli-0.3.9/embedops_cli/api/models/user_group_props_group.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/user_group_update_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/user_group_update_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/models/user_update_props.py` & `embedops-cli-0.3.9/embedops_cli/api/models/user_update_props.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/api/rest.py` & `embedops-cli-0.3.9/embedops_cli/api/rest.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/ci_config_loader.py` & `embedops-cli-0.3.9/embedops_cli/ci_config_loader.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/config.py` & `embedops-cli-0.3.9/embedops_cli/config.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/docker_run.py` & `embedops-cli-0.3.9/embedops_cli/docker_run.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/embedops_authorization.py` & `embedops-cli-0.3.9/embedops_cli/embedops_authorization.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import base64
 import pathlib
 import webbrowser
 from time import sleep
 import logging
 import subprocess
+from datetime import datetime
 from operator import itemgetter
 from urllib.parse import urlparse
 import requests
 import dotenv
 import click
 from dynaconf import Dynaconf
 from dynaconf.loaders import toml_loader
@@ -56,14 +57,26 @@
     """Set the Auth0 token in user secrets"""
     try:
         toml_loader.write(secrets_file, {"EMBEDOPS_AUTH_TOKEN": auth_token}, merge=True)
     except (IOError) as exc:
         raise LoginFailureException from exc
 
 
+def set_docker_expiration_time(expires_at, secrets_file=user_secrets):
+    """Set the Auth0 token in user secrets"""
+    try:
+        toml_loader.write(
+            secrets_file,
+            {"EMBEDOPS_ECR_TOKEN_EXPIRES_AT": expires_at.timestamp()},
+            merge=True,
+        )
+    except (IOError) as exc:
+        raise LoginFailureException from exc
+
+
 def fetch_registry_token() -> str:
     """Retrieve a GitLab token for the user's group and store it"""
     user_client = get_user_client()
 
     user = user_client.get_my_user()
     if len(user.groups) < 1:
         raise UnauthorizedUserException
@@ -73,27 +86,48 @@
 
     token_record = user_client.get_aws_access_key_for_org(org_id)
     set_registry_token(
         token_record.access_key.access_key_id, token_record.access_key.secret_access_key
     )
 
 
+def get_docker_expiration_time(secrets_file=user_secrets):
+    """Retrieve docker exp date"""
+    registry_token_expires_at = None
+
+    # Return false since variable is not set
+    if not os.path.exists(secrets_file):
+        return registry_token_expires_at
+
+    secrets_file_settings = Dynaconf(SETTINGS_FILES=[secrets_file])
+    try:
+        registry_token_expires_at = secrets_file_settings.EMBEDOPS_ECR_TOKEN_EXPIRES_AT
+    except AttributeError as exc:
+        raise UnauthorizedUserException from exc
+
+    return registry_token_expires_at
+
+
 def get_registry_token(secrets_file=user_secrets):
     """Retrieve the Auth0 token from user secrets"""
     if not os.path.exists(secrets_file):
         raise UnauthorizedUserException
     secrets_file_settings = Dynaconf(SETTINGS_FILES=[secrets_file])
     try:
         registry_token_id = secrets_file_settings.EMBEDOPS_ECR_TOKEN_ID
         registry_token_secret = secrets_file_settings.EMBEDOPS_ECR_TOKEN_SECRET
     except AttributeError as exc:
         raise UnauthorizedUserException from exc
     if not registry_token_id or not registry_token_secret:
         raise UnauthorizedUserException
-    return registry_token_id, registry_token_secret
+
+    return {
+        "registry_token_id": registry_token_id,
+        "registry_token_secret": registry_token_secret,
+    }
 
 
 def set_registry_token(
     registry_access_key_id: str,
     registry_secret_access_key: str,
     secrets_file=user_secrets,
 ):
@@ -124,15 +158,19 @@
 def request_authorization():  # pylint: disable=too-many-locals
     """start the routine for the user to authenticate with Auth0"""
 
     ############## Setup request bits ################
     env_path = pathlib.Path(".") / ".env"
     dotenv.load_dotenv(dotenv_path=env_path)
 
-    # TODO: we'll need to set this to where the .env are stored in the application
+    # Uncomment to connect to platform in dev environment
+    # todo: Need a make setting for switching between dev & prod env ticket: EO-473
+    # client_id = "6Sm3VSVQ15B9IxTFKmwrjcPzXaH0oC1P"
+    # base_url = "https://embedops-dev.us.auth0.com/oauth"
+
     client_id = "wBgMNZyLb76QRZe3eDRsCnoBLBy4qMQh"
     base_url = "https://embedops.us.auth0.com/oauth"
 
     code_obj = request_user_code(client_id, base_url)
 
     # Request the user code and verification url, show instructions to user
     user_code = code_obj["user_code"]
@@ -145,19 +183,26 @@
 
     return launch_login_url(verification_url, base_url, device_code, client_id)
 
 
 def request_user_code(client_id, base_url):
     """Request the code to show to the user"""
     # We generate a nonce (state) that is used to protect against attackers invoking the callback
+
+    # Uncomment to connect to platform in dev environment
+    # todo: Need a make setting for switching between dev & prod env ticket: EO-473
+    # audience = "https://app-dev.embedops.com"
+    audience = "https://app.embedops.com"
+
     data = {
-        "audience": "https://app.embedops.com",
+        "audience": audience,
         "scope": "openid email profile offline_access",
         "client_id": client_id,
     }
+
     url = f"{base_url}/device/code"
 
     code_req_response = requests.post(url, data=data)
     return code_req_response.json()
 
 
 def show_login_instructions(user_code):
@@ -247,17 +292,21 @@
     )(assume_role_response["Credentials"])
     ecr_client = boto3.client(
         "ecr",
         aws_access_key_id=aws_access_key_id,
         aws_secret_access_key=aws_secret_access_key,
         aws_session_token=aws_session_token,
     )
+
     ecr_authorization_data = ecr_client.get_authorization_token()["authorizationData"][
         0
     ]
+    # We need to save this for later to check if the token is valid when we use 'docker run ...'
+    set_docker_expiration_time(ecr_authorization_data["expiresAt"])
+
     authorization_token, registry_server = itemgetter(
         "authorizationToken", "proxyEndpoint"
     )(ecr_authorization_data)
     registry_token = base64.b64decode(authorization_token).decode().replace("AWS:", "")
     try:
         subprocess.check_output(
             f"echo {registry_token} | \
@@ -274,16 +323,33 @@
 
         return err.returncode
 
 
 def login_to_registry(secrets_file=user_secrets):
     """Log into a docker registry"""
     try:
-        registry_token_id, registry_token_secret = get_registry_token(secrets_file)
+        registry_token_data = get_registry_token(secrets_file)
+
     except UnauthorizedUserException as exc:
         raise UnauthorizedUserException from exc
-    return_code = docker_cli_login(registry_token_id, registry_token_secret)
+    return_code = docker_cli_login(
+        registry_token_data["registry_token_id"],
+        registry_token_data["registry_token_secret"],
+    )
     if return_code == 1:
         raise DockerRegistryException
     if return_code > 0:
         raise UnknownDockerException
     return return_code
+
+
+def is_registery_token_valid(secrets_file=user_secrets):
+    """Check if register token has expired"""
+    registry_token_expires_at = get_docker_expiration_time(secrets_file)
+    is_valid = False
+
+    if registry_token_expires_at:
+
+        if registry_token_expires_at > datetime.now().timestamp():
+            is_valid = True
+
+    return is_valid
```

### Comparing `embedops-cli-0.3.8/embedops_cli/embedops_cli.py` & `embedops-cli-0.3.9/embedops_cli/embedops_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,18 @@
 @click.argument("job_name")
 def run(ctx: click.Context, job_name):
     """Run a job defined in a CI YAML file.
     JOB_NAME is the name of the job or step in your CI YAML file"""
 
     telemetry.command_event("jobs_run", {"job_name": job_name})
 
+    # check if token has expired if so try to get a new token
+    if embedops_authorization.is_registery_token_valid() is False:
+        embedops_authorization.login_to_registry()
+
     filename = ctx.obj
     _logger.debug(f"jobs run called with file '{filename}' and job '{job_name}")
 
     try:
         job_list = yaml_utilities.get_job_list(filename)
     except (
         UnsupportedYamlTypeException,
```

### Comparing `embedops-cli-0.3.8/embedops_cli/environment_utilities.py` & `embedops-cli-0.3.9/embedops_cli/environment_utilities.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/eo_types.py` & `embedops-cli-0.3.9/embedops_cli/eo_types.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/eotools/__init__.py` & `embedops-cli-0.3.9/embedops_cli/eotools/__init__.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/eotools/ci_run.py` & `embedops-cli-0.3.9/embedops_cli/eotools/ci_run.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/eotools/log_parser/gnu_size_berkeley.py` & `embedops-cli-0.3.9/embedops_cli/eotools/log_parser/gnu_size_berkeley.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/eotools/log_parser/iar.py` & `embedops-cli-0.3.9/embedops_cli/eotools/log_parser/iar.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/eotools/parse.py` & `embedops-cli-0.3.9/embedops_cli/eotools/parse.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/eotools/update_run.py` & `embedops-cli-0.3.9/embedops_cli/eotools/update_run.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/telemetry.py` & `embedops-cli-0.3.9/embedops_cli/telemetry.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/utilities.py` & `embedops-cli-0.3.9/embedops_cli/utilities.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/yaml_tools/bb_parser.py` & `embedops-cli-0.3.9/embedops_cli/yaml_tools/bb_parser.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/yaml_tools/gh_parser.py` & `embedops-cli-0.3.9/embedops_cli/yaml_tools/gh_parser.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/yaml_tools/gl_parser.py` & `embedops-cli-0.3.9/embedops_cli/yaml_tools/gl_parser.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli/yaml_tools/yaml_utilities.py` & `embedops-cli-0.3.9/embedops_cli/yaml_tools/yaml_utilities.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/embedops_cli.egg-info/PKG-INFO` & `embedops-cli-0.3.9/embedops_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedops-cli
-Version: 0.3.8
+Version: 0.3.9
 Summary: EmbedOps Command Line Tools
 Home-page: https://embedops.io
 Author: Dojo Five, LLC
 Author-email: embedops@dojofive.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
```

### Comparing `embedops-cli-0.3.8/embedops_cli.egg-info/SOURCES.txt` & `embedops-cli-0.3.9/embedops_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/setup.cfg` & `embedops-cli-0.3.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/tests/api_interface_test.py` & `embedops-cli-0.3.9/tests/api_interface_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 Unit tests for code to upload XML files to the API
 * Author(s): Bryan Siepert
 """
 from embedops_cli.config import settings
 from embedops_cli.eotools import post_test_report
 import pytest
 
+
 class FakeResponse(object):
     """Fake http response for test use"""
 
     status_code = 200
 
     def json(self):
         """Empty JSON object"""
         return "{}"
 
 
 # test the cli/click to report_test fn call
 class APIInterfaceTest:
-
     @pytest.fixture(autouse=True)
     def configure_env(self, monkeypatch, mocker):
         monkeypatch.setenv("CI", "true")
         monkeypatch.setenv("EMBEDOPS_API_REPO_KEY", "special_pwefix")
         self.logger_mock = mocker.patch("embedops_cli.eotools.ci_run._logger")
 
     def test_report_file_contents_sent(self, mocker):
@@ -47,9 +47,12 @@
                 file_obj,
                 "application/xml+junit",
             )
         }
 
         post_test_report(report_filename)
         req_mock.assert_called_with(
-            settings.ci_artifact_endpoint, data_dict=data, file_dict=files, headers=headers
-    )
+            settings.ci_artifact_endpoint,
+            data_dict=data,
+            file_dict=files,
+            headers=headers,
+        )
```

### Comparing `embedops-cli-0.3.8/tests/bb_parser_test.py` & `embedops-cli-0.3.9/tests/bb_parser_test.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/tests/check_api_client.py` & `embedops-cli-0.3.9/tests/check_api_client.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/tests/create_run_test.py` & `embedops-cli-0.3.9/tests/create_run_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,14 @@
         monkeypatch.setenv("BITBUCKET_STEP_UUID", "yoo-yoo-eye-de")
         self.logger_mock = mocker.patch("embedops_cli.eotools.ci_run._logger")
 
         self.ci_run = CIRun()
         yield
         del self.ci_run
 
-
     def test_successful_create_response(self, mocker):
         mocked_id = "123123"
         ci_run = MagicMock()
         ci_run.id = mocked_id
 
         get_client = mocker.patch("embedops_cli.eotools.ci_run.get_client")
```

### Comparing `embedops-cli-0.3.8/tests/docker_run_test.py` & `embedops-cli-0.3.9/tests/docker_run_test.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/tests/embedops_cli_test.py` & `embedops-cli-0.3.9/tests/embedops_cli_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,24 +135,28 @@
     runner = CliRunner()
     result = runner.invoke(
         embedops_cli.embedops_cli,
         ["jobs", "--filename", "tests/README.md", "run", "build"],
     )
     assert result.exit_code == 1
 
+
 def test_stale_token_prompts_login(mocker):
     """Test that a no-longer-valid auth token prompts"""
-    token_status = mocker.patch("embedops_cli.embedops_cli.embedops_authorization.check_token")
+    token_status = mocker.patch(
+        "embedops_cli.embedops_cli.embedops_authorization.check_token"
+    )
     token_status.return_value = False
 
-
-    do_login = mocker.patch("embedops_cli.embedops_cli.embedops_authorization.request_authorization")
+    do_login = mocker.patch(
+        "embedops_cli.embedops_cli.embedops_authorization.request_authorization"
+    )
     do_login.side_effect = UnauthorizedUserException()
     runner = CliRunner()
     result = runner.invoke(embedops_cli.embedops_cli, "login")
     do_login.assert_called()
 
     assert result.exit_code != 0
 
     # mock `check user` to return false
     # verify that "do login" is called
-    # verify that if "do login" is successful that the return value is 0
+    # verify that if "do login" is successful that the return value is 0
```

### Comparing `embedops-cli-0.3.8/tests/environment_utilities_test.py` & `embedops-cli-0.3.9/tests/environment_utilities_test.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/tests/eotools_test.py` & `embedops-cli-0.3.9/tests/eotools_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,27 +30,30 @@
         self._run_id = uuid.uuid1()
 
     @property
     def run_id(self):
         """Run id for fake config class"""
         return self._run_id
 
+
 class EOToolsTests:
     @pytest.fixture(autouse=True)
     def configure_env(self, monkeypatch, mocker):
         monkeypatch.setenv("CI", "true")
         monkeypatch.setenv("EMBEDOPS_API_REPO_KEY", "special_pwefix")
         monkeypatch.setenv("EMBEDOPS_ANALYSIS_TYPE", "memusage")
         monkeypatch.setenv("BITBUCKET_COMMIT", "abcd1234")
         monkeypatch.setenv("BITBUCKET_BRANCH", "main")
-        self.ci_run_caller = mocker.patch("embedops_cli.eotools.create_run.CIRun.create_run")
+        self.ci_run_caller = mocker.patch(
+            "embedops_cli.eotools.create_run.CIRun.create_run"
+        )
         self.logger_mock = mocker.patch("embedops_cli.eotools.create_run._logger")
         self.ci_run = CIRun()
         yield
-        del(self.ci_run)
+        del self.ci_run
 
     def test_successful_job_sets_ci_url(self, mocker):
 
         mocker.patch(
             "embedops_cli.eotools.update_run.CiRun._previous_return", return_value=0
         )
 
@@ -72,15 +75,15 @@
         ci_run_id = call_args[1]
 
         assert isinstance(ci_properties, CIRunUpdateProps)
         assert ci_run_id == settings.run_id
         assert ci_properties.pipeline_url == settings.job_url
 
     def test_api_client_configured(self, mocker):
-    
+
         self.config_dict = mocker.patch.dict(
             self.config_class.api_key, {"X-API-Key": None}
         )
         api_client = mocker.patch("embedops_cli.api.get_client")
         with pytest.raises(SystemExit) as pytest_wrapped_e:
             create_entry()
         assert pytest_wrapped_e.type == SystemExit
@@ -93,8 +96,8 @@
         )
         assert self.config_class().host == self.expected_host + "/api/v1"
 
         args, _kwargs = api_client().create_ci_run_from_ci.call_args
         first_call = args[0]
         assert first_call.type == self.expected_type
         assert first_call.commit_id == self.expected_commit_id
-        assert first_call.branch == self.expected_branch
+        assert first_call.branch == self.expected_branch
```

### Comparing `embedops-cli-0.3.8/tests/gh_parser_test.py` & `embedops-cli-0.3.9/tests/gh_parser_test.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/tests/gl_parser_test.py` & `embedops-cli-0.3.9/tests/gl_parser_test.py`

 * *Files identical despite different names*

### Comparing `embedops-cli-0.3.8/tests/utilities_test.py` & `embedops-cli-0.3.9/tests/utilities_test.py`

 * *Files identical despite different names*

