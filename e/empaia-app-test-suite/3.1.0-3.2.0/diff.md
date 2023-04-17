# Comparing `tmp/empaia_app_test_suite-3.1.0.tar.gz` & `tmp/empaia_app_test_suite-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empaia_app_test_suite-3.1.0.tar", max compression
+gzip compressed data, was "empaia_app_test_suite-3.2.0.tar", max compression
```

## Comparing `empaia_app_test_suite-3.1.0.tar` & `empaia_app_test_suite-3.2.0.tar`

### file list

```diff
@@ -1,152 +1,154 @@
--rw-r--r--   0        0        0     1288 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/LICENSE
--rw-r--r--   0        0        0     6610 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/README.md
--rw-r--r--   0        0        0       87 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/__init__.py
--rw-r--r--   0        0        0     2624 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/cli.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/cli_definitions/__init__.py
--rw-r--r--   0        0        0     2944 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/cli_definitions/apps_cli.py
--rw-r--r--   0        0        0     1305 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/cli_definitions/cases_cli.py
--rw-r--r--   0        0        0     5646 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.1.0/empaia_app_test_suite/cli_definitions/jobs_cli.py
--rw-r--r--   0        0        0     4444 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/cli_definitions/main_cli.py
--rw-r--r--   0        0        0     3764 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/cli_definitions/services_cli.py
--rw-r--r--   0        0        0     2386 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.1.0/empaia_app_test_suite/cli_definitions/slides_cli.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/__init__.py
--rw-r--r--   0        0        0     5244 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/apps_commands.py
--rw-r--r--   0        0        0      921 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/cases_commands.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/helper/__init__.py
--rw-r--r--   0        0        0     4204 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/helper/app_helper.py
--rw-r--r--   0        0        0     4324 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/helper/data_helper.py
--rw-r--r--   0        0        0     2784 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/helper/job_helper.py
--rw-r--r--   0        0        0    10601 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/helper/job_validation_helper.py
--rw-r--r--   0        0        0     4201 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/helper/wsi_helper.py
--rw-r--r--   0        0        0    13309 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/jobs_commands.py
--rw-r--r--   0        0        0     8678 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/services_commands.py
--rw-r--r--   0        0        0     2973 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/slides_commands.py
--rw-r--r--   0        0        0     4740 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.1.0/empaia_app_test_suite/constants.py
--rw-r--r--   0        0        0     3881 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/custom_models.py
--rw-r--r--   0        0        0       56 2022-11-30 10:14:50.710744 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/.git
--rw-r--r--   0        0        0       32 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/.gitignore
--rw-r--r--   0        0        0      845 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/.gitlab/issue_templates/story_qa_level_1.md
--rw-r--r--   0        0        0      699 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/.gitlab/merge_request_templates/merge_request_qa_level_1.md
--rw-r--r--   0        0        0     1447 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/.gitlab-ci.yml
--rw-r--r--   0        0        0     2258 2023-03-30 12:45:35.128584 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/CHANGELOG.md
--rw-r--r--   0        0        0     1064 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/LICENSE
--rw-r--r--   0        0        0      302 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/README.md
--rw-r--r--   0        0        0        0 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/__init__.py
--rw-r--r--   0        0        0      692 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/commons.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/marketplace/__init__.py
--rw-r--r--   0        0        0    17434 2023-03-30 12:45:35.128584 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/marketplace/app.py
--rw-r--r--   0        0        0    36937 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/poetry.lock
--rw-r--r--   0        0        0      780 2023-03-30 12:45:35.128584 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/pyproject.toml
--rw-r--r--   0        0        0       36 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/setup.cfg
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/utils/__init__.py
--rw-r--r--   0        0        0     3983 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/utils/access_token_tools.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/utils/tests/__init__.py
--rw-r--r--   0        0        0     8405 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/utils/tests/test_access_token_tools.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/__init__.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/annotation/__init__.py
--rw-r--r--   0        0        0    12040 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/annotation/annotations.py
--rw-r--r--   0        0        0     3587 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/annotation/classes.py
--rw-r--r--   0        0        0    11262 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/annotation/collections.py
--rw-r--r--   0        0        0     2341 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/annotation/jobs.py
--rw-r--r--   0        0        0     5884 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/annotation/primitives.py
--rw-r--r--   0        0        0      423 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/annotation/server_settings.py
--rw-r--r--   0        0        0     6052 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/clinical.py
--rw-r--r--   0        0        0     3305 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/commons.py
--rw-r--r--   0        0        0     3826 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/examination.py
--rw-r--r--   0        0        0      922 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/id_mapper.py
--rw-r--r--   0        0        0     7516 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/job.py
--rw-r--r--   0        0        0     2156 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/slide.py
--rw-r--r--   0        0        0     2661 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/storage.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/tests/__init__.py
--rw-r--r--   0        0        0      448 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/tests/test_job_creator_type.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/__init__.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/annotation/__init__.py
--rw-r--r--   0        0        0    13252 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/annotation/annotations.py
--rw-r--r--   0        0        0     3747 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/annotation/classes.py
--rw-r--r--   0        0        0    17090 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/annotation/collections.py
--rw-r--r--   0        0        0      397 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/annotation/jobs.py
--rw-r--r--   0        0        0     6657 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/annotation/primitives.py
--rw-r--r--   0        0        0      423 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/annotation/server_settings.py
--rw-r--r--   0        0        0     6052 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/clinical.py
--rw-r--r--   0        0        0     3683 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/commons.py
--rw-r--r--   0        0        0     8591 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/examination.py
--rw-r--r--   0        0        0      922 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/id_mapper.py
--rw-r--r--   0        0        0    11686 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/job.py
--rw-r--r--   0        0        0     2329 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/slide.py
--rw-r--r--   0        0        0     2661 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/storage.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/tests/__init__.py
--rw-r--r--   0        0        0      373 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/tests/test_examination.py
--rw-r--r--   0        0        0      500 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/tests/test_job_creator_type.py
--rw-r--r--   0        0        0     2829 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/tests/test_job_mode.py
--rw-r--r--   0        0        0     1816 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/tests/test_job_progress.py
--rw-r--r--   0        0        0     2445 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/tests/test_job_validation_fields.py
--rw-r--r--   0        0        0       67 2022-11-30 10:14:51.720744 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/.git
--rw-r--r--   0        0        0       31 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/.gitignore
--rw-r--r--   0        0        0      845 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/.gitlab/issue_templates/story_qa_level_1.md
--rw-r--r--   0        0        0      699 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/.gitlab/merge_request_templates/merge_request_qa_level_1.md
--rw-r--r--   0        0        0      791 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/.gitlab-ci.yml
--rw-r--r--   0        0        0      224 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/.gitmodules
--rw-r--r--   0        0        0     1115 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/CHANGELOG.md
--rw-r--r--   0        0        0     6254 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/README.md
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/__init__.py
--rw-r--r--   0        0        0     3482 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/docker-compose.yml
--rw-r--r--   0        0        0    16228 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/poetry.lock
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/__init__.py
--rw-r--r--   0        0        0     1232 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/__main__.py
--rw-r--r--   0        0        0      111 2022-11-30 10:14:56.020743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.git
--rw-r--r--   0        0        0        8 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitignore
--rw-r--r--   0        0        0      845 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/issue_templates/story_qa_level_1.md
--rw-r--r--   0        0        0      697 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/merge_request_templates/merge_request_qa_level_1.md
--rw-r--r--   0        0        0     1505 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/README.md
--rw-r--r--   0        0        0    12338 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft1.json
--rw-r--r--   0        0        0    17247 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft3.json
--rw-r--r--   0        0        0    18941 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v3.json
--rw-r--r--   0        0        0      283 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead-settings.json
--rw-r--r--   0        0        0      170 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/namespaces/org.empaia.global.v1.json
--rw-r--r--   0        0        0     9133 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/tags/tags.csv
--rw-r--r--   0        0        0     5744 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/ead_validator.py
--rw-r--r--   0        0        0      457 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/exceptions.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/__init__.py
--rw-r--r--   0        0        0     2230 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/common.py
--rw-r--r--   0        0        0        0 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/__init__.py
--rw-r--r--   0        0        0     2674 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/ead.py
--rw-r--r--   0        0        0        0 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/__init__.py
--rw-r--r--   0        0        0     4439 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/ead.py
--rw-r--r--   0        0        0    16713 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/job.py
--rw-r--r--   0        0        0     2149 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/job_validator.py
--rw-r--r--   0        0        0      869 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/pyproject.toml
--rw-r--r--   0        0        0      260 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/sample.env
--rw-r--r--   0        0        0       36 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/setup.cfg
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/__init__.py
--rw-r--r--   0        0        0     9099 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/test_ead_validator.py
--rw-r--r--   0        0        0    23309 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead.py
--rw-r--r--   0        0        0    10278 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead_with_config.py
--rw-r--r--   0        0        0    35567 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3.py
--rw-r--r--   0        0        0    10465 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3_with_config.py
--rw-r--r--   0        0        0        0 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/__init__.py
--rw-r--r--   0        0        0    43792 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/conftest.py
--rw-r--r--   0        0        0     2186 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_completeness.py
--rw-r--r--   0        0        0    34033 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_compliance.py
--rw-r--r--   0        0        0     2345 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_completeness.py
--rw-r--r--   0        0        0    42502 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_compliance.py
--rw-r--r--   0        0        0     3024 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_suitable_job_status.py
--rw-r--r--   0        0        0      864 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/test_exceptions.py
--rw-r--r--   0        0        0     3000 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.1.0/empaia_app_test_suite/services/docker-compose.yml
--rw-r--r--   0        0        0       48 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/services/nginx/Dockerfile
--rw-r--r--   0        0        0     1134 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/services/nginx/nginx.conf
--rw-r--r--   0        0        0     1256 2023-03-30 05:35:46.188277 empaia_app_test_suite-3.1.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/Dockerfile
--rw-r--r--   0        0        0        0 2022-11-30 10:14:58.080743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/__init__.py
--rw-r--r--   0        0        0     5688 2022-11-30 10:14:58.080743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/__main__.py
--rw-r--r--   0        0        0     9365 2022-11-30 10:14:58.080743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/isyntax_reader.py
--rw-r--r--   0        0        0      362 2023-03-30 05:35:46.188277 empaia_app_test_suite-3.1.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/pyproject.toml
--rw-r--r--   0        0        0    16186 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.1.0/empaia_app_test_suite/settings.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/utils/__init__.py
--rw-r--r--   0        0        0      511 2023-03-31 14:14:09.315022 empaia_app_test_suite-3.1.0/empaia_app_test_suite/utils/utils_aaa.py
--rw-r--r--   0        0        0     2448 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/utils/utils_commons.py
--rw-r--r--   0        0        0     8016 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.1.0/empaia_app_test_suite/utils/utils_mds.py
--rw-r--r--   0        0        0     2158 2023-03-23 08:17:05.515364 empaia_app_test_suite-3.1.0/empaia_app_test_suite/utils/utils_mps.py
--rw-r--r--   0        0        0     5671 2023-03-31 14:14:09.315022 empaia_app_test_suite-3.1.0/empaia_app_test_suite/utils/utils_print.py
--rw-r--r--   0        0        0     2870 2023-03-31 14:14:09.315022 empaia_app_test_suite-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     8304 1970-01-01 00:00:00.000000 empaia_app_test_suite-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1288 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/LICENSE
+-rw-r--r--   0        0        0     6610 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/README.md
+-rw-r--r--   0        0        0       87 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/__init__.py
+-rw-r--r--   0        0        0     2624 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli.py
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/__init__.py
+-rw-r--r--   0        0        0     2944 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/apps_cli.py
+-rw-r--r--   0        0        0     1305 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/cases_cli.py
+-rw-r--r--   0        0        0     5646 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/jobs_cli.py
+-rw-r--r--   0        0        0     4579 2023-04-17 13:48:35.451634 empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/main_cli.py
+-rw-r--r--   0        0        0     3899 2023-04-17 13:48:35.451634 empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/services_cli.py
+-rw-r--r--   0        0        0     2386 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/slides_cli.py
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/__init__.py
+-rw-r--r--   0        0        0     5244 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/apps_commands.py
+-rw-r--r--   0        0        0      921 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/cases_commands.py
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/__init__.py
+-rw-r--r--   0        0        0     4204 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/app_helper.py
+-rw-r--r--   0        0        0     4324 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/data_helper.py
+-rw-r--r--   0        0        0     2784 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/job_helper.py
+-rw-r--r--   0        0        0    10601 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/job_validation_helper.py
+-rw-r--r--   0        0        0     4201 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/wsi_helper.py
+-rw-r--r--   0        0        0    13309 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/jobs_commands.py
+-rw-r--r--   0        0        0     8804 2023-04-17 13:48:35.451634 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/services_commands.py
+-rw-r--r--   0        0        0     2973 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/slides_commands.py
+-rw-r--r--   0        0        0     4818 2023-04-17 13:48:35.451634 empaia_app_test_suite-3.2.0/empaia_app_test_suite/constants.py
+-rw-r--r--   0        0        0     3881 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/custom_models.py
+-rw-r--r--   0        0        0       56 2022-11-30 10:14:50.710744 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/.git
+-rw-r--r--   0        0        0       32 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/.gitignore
+-rw-r--r--   0        0        0      845 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/.gitlab/issue_templates/story_qa_level_1.md
+-rw-r--r--   0        0        0      699 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/.gitlab/merge_request_templates/merge_request_qa_level_1.md
+-rw-r--r--   0        0        0     1447 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2258 2023-03-30 12:45:35.128584 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/CHANGELOG.md
+-rw-r--r--   0        0        0     1064 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/LICENSE
+-rw-r--r--   0        0        0      302 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/README.md
+-rw-r--r--   0        0        0        0 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/__init__.py
+-rw-r--r--   0        0        0      692 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/commons.py
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/marketplace/__init__.py
+-rw-r--r--   0        0        0    17434 2023-03-30 12:45:35.128584 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/marketplace/app.py
+-rw-r--r--   0        0        0    36937 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/poetry.lock
+-rw-r--r--   0        0        0      780 2023-03-30 12:45:35.128584 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/pyproject.toml
+-rw-r--r--   0        0        0       36 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/setup.cfg
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/utils/__init__.py
+-rw-r--r--   0        0        0     3983 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/utils/access_token_tools.py
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/utils/tests/__init__.py
+-rw-r--r--   0        0        0     8405 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/utils/tests/test_access_token_tools.py
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/__init__.py
+-rw-r--r--   0        0        0    12040 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/annotations.py
+-rw-r--r--   0        0        0     3587 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/classes.py
+-rw-r--r--   0        0        0    11262 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/collections.py
+-rw-r--r--   0        0        0     2341 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/jobs.py
+-rw-r--r--   0        0        0     5884 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/primitives.py
+-rw-r--r--   0        0        0      423 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/server_settings.py
+-rw-r--r--   0        0        0     6052 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/clinical.py
+-rw-r--r--   0        0        0     3305 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/commons.py
+-rw-r--r--   0        0        0     3826 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/examination.py
+-rw-r--r--   0        0        0      922 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/id_mapper.py
+-rw-r--r--   0        0        0     7516 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/job.py
+-rw-r--r--   0        0        0     2156 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/slide.py
+-rw-r--r--   0        0        0     2661 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/storage.py
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/tests/__init__.py
+-rw-r--r--   0        0        0      448 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/tests/test_job_creator_type.py
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/__init__.py
+-rw-r--r--   0        0        0    13252 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/annotations.py
+-rw-r--r--   0        0        0     3747 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/classes.py
+-rw-r--r--   0        0        0    17090 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/collections.py
+-rw-r--r--   0        0        0      397 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/jobs.py
+-rw-r--r--   0        0        0     6657 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/primitives.py
+-rw-r--r--   0        0        0      423 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/server_settings.py
+-rw-r--r--   0        0        0     6052 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/clinical.py
+-rw-r--r--   0        0        0     3683 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/commons.py
+-rw-r--r--   0        0        0     8591 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/examination.py
+-rw-r--r--   0        0        0      922 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/id_mapper.py
+-rw-r--r--   0        0        0    11686 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/job.py
+-rw-r--r--   0        0        0     2329 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/slide.py
+-rw-r--r--   0        0        0     2661 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/storage.py
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/__init__.py
+-rw-r--r--   0        0        0      373 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/test_examination.py
+-rw-r--r--   0        0        0      500 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/test_job_creator_type.py
+-rw-r--r--   0        0        0     2829 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/test_job_mode.py
+-rw-r--r--   0        0        0     1816 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/test_job_progress.py
+-rw-r--r--   0        0        0     2445 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/test_job_validation_fields.py
+-rw-r--r--   0        0        0       67 2022-11-30 10:14:51.720744 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.git
+-rw-r--r--   0        0        0       31 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.gitignore
+-rw-r--r--   0        0        0      845 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.gitlab/issue_templates/story_qa_level_1.md
+-rw-r--r--   0        0        0      699 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.gitlab/merge_request_templates/merge_request_qa_level_1.md
+-rw-r--r--   0        0        0      791 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.gitlab-ci.yml
+-rw-r--r--   0        0        0      224 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.gitmodules
+-rw-r--r--   0        0        0     1115 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/CHANGELOG.md
+-rw-r--r--   0        0        0     6254 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/README.md
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/__init__.py
+-rw-r--r--   0        0        0     3482 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/docker-compose.yml
+-rw-r--r--   0        0        0    16228 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/poetry.lock
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/__init__.py
+-rw-r--r--   0        0        0     1232 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/__main__.py
+-rw-r--r--   0        0        0      111 2022-11-30 10:14:56.020743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.git
+-rw-r--r--   0        0        0        8 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitignore
+-rw-r--r--   0        0        0      845 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/issue_templates/story_qa_level_1.md
+-rw-r--r--   0        0        0      697 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/merge_request_templates/merge_request_qa_level_1.md
+-rw-r--r--   0        0        0     1505 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/README.md
+-rw-r--r--   0        0        0    12338 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft1.json
+-rw-r--r--   0        0        0    17247 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft3.json
+-rw-r--r--   0        0        0    18941 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v3.json
+-rw-r--r--   0        0        0      283 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead-settings.json
+-rw-r--r--   0        0        0      170 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/namespaces/org.empaia.global.v1.json
+-rw-r--r--   0        0        0     9133 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/tags/tags.csv
+-rw-r--r--   0        0        0     5744 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/ead_validator.py
+-rw-r--r--   0        0        0      457 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/exceptions.py
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/__init__.py
+-rw-r--r--   0        0        0     2230 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/common.py
+-rw-r--r--   0        0        0        0 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/__init__.py
+-rw-r--r--   0        0        0     2674 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/ead.py
+-rw-r--r--   0        0        0        0 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/__init__.py
+-rw-r--r--   0        0        0     4439 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/ead.py
+-rw-r--r--   0        0        0    16713 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/job.py
+-rw-r--r--   0        0        0     2149 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/job_validator.py
+-rw-r--r--   0        0        0      869 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/sample.env
+-rw-r--r--   0        0        0       36 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/setup.cfg
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/__init__.py
+-rw-r--r--   0        0        0     9099 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/test_ead_validator.py
+-rw-r--r--   0        0        0    23309 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead.py
+-rw-r--r--   0        0        0    10278 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead_with_config.py
+-rw-r--r--   0        0        0    35567 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3.py
+-rw-r--r--   0        0        0    10465 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3_with_config.py
+-rw-r--r--   0        0        0        0 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/__init__.py
+-rw-r--r--   0        0        0    43792 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/conftest.py
+-rw-r--r--   0        0        0     2186 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_completeness.py
+-rw-r--r--   0        0        0    34033 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_compliance.py
+-rw-r--r--   0        0        0     2345 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_completeness.py
+-rw-r--r--   0        0        0    42502 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_compliance.py
+-rw-r--r--   0        0        0     3024 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_suitable_job_status.py
+-rw-r--r--   0        0        0      864 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/test_exceptions.py
+-rw-r--r--   0        0        0     2999 2023-04-17 13:48:35.451634 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/docker-compose.yml
+-rw-r--r--   0        0        0       48 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/nginx/Dockerfile
+-rw-r--r--   0        0        0     1134 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/nginx/nginx.conf
+-rw-r--r--   0        0        0     1256 2023-04-17 06:03:21.906959 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/Dockerfile
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:58.080743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/__init__.py
+-rw-r--r--   0        0        0     5688 2022-11-30 10:14:58.080743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/__main__.py
+-rw-r--r--   0        0        0     9355 2023-04-17 06:03:21.906959 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/isyntax_reader.py
+-rw-r--r--   0        0        0      361 2023-04-17 06:03:21.906959 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/pyproject.toml
+-rw-r--r--   0        0        0     1033 2023-04-17 07:10:52.894495 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-mirax/mirax_backend/Dockerfile
+-rw-r--r--   0        0        0       81 2023-04-17 07:10:52.894495 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-mirax/mirax_backend/entrypoint.sh
+-rw-r--r--   0        0        0    18174 2023-04-17 13:48:35.451634 empaia_app_test_suite-3.2.0/empaia_app_test_suite/settings.py
+-rw-r--r--   0        0        0        0 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/__init__.py
+-rw-r--r--   0        0        0      511 2023-03-31 14:14:09.315022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_aaa.py
+-rw-r--r--   0        0        0     2448 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_commons.py
+-rw-r--r--   0        0        0     8016 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_mds.py
+-rw-r--r--   0        0        0     2158 2023-03-23 08:17:05.515364 empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_mps.py
+-rw-r--r--   0        0        0     5671 2023-03-31 14:14:09.315022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_print.py
+-rw-r--r--   0        0        0     3037 2023-04-17 13:48:35.451634 empaia_app_test_suite-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8304 1970-01-01 00:00:00.000000 empaia_app_test_suite-3.2.0/PKG-INFO
```

### Comparing `empaia_app_test_suite-3.1.0/LICENSE` & `empaia_app_test_suite-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/README.md` & `empaia_app_test_suite-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/cli.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/cli_definitions/apps_cli.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/apps_cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/cli_definitions/cases_cli.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/cases_cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/cli_definitions/jobs_cli.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/jobs_cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/cli_definitions/main_cli.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/main_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         pull: bool = typer.Option(False, "--pull", help=const.PULL_HELP),
         docker_config: Path = typer.Option(None, "--docker-config", help=const.DOCKER_CONFIG_FILE_HELP),
         global_config_file: Path = typer.Option(None, "--global-config-file", help=const.GLOBAL_CONFIG_FILE_HELP),
         customer_config_file: Path = typer.Option(None, "--customer-config-file", help=const.CUSTOMER_CONFIG_FILE_HELP),
         nginx_port: int = typer.Option(8888, "--nginx-port", help=const.NGINX_PORT_HELP),
         wbs_url: str = typer.Option(None, "--wbs-url", help=const.WBS_URL_HELP),
         isyntax_sdk: str = typer.Option(None, "--isyntax-sdk", help=const.ISYNTAX_SDK_HELP),
+        mirax_plugin: str = typer.Option(None, "--mirax-plugin", help=const.MIRAX_PLUGIN_HELP),
         volume_prefix: str = typer.Option(None, "--volume-prefix", help=const.VOLUME_PREFIX_HELP),
         gpu_driver: str = typer.Option(None, "--gpu-driver", help=const.GPU_DRIVER_HELP),
         frontend_token_exp: int = typer.Option(60, "--frontend-token-exp", help=const.FRONTEND_TOKEN_EXP),
         scope_token_exp: int = typer.Option(300, "--scope-token-exp", help=const.SCOPE_TOKEN_EXP),
         app_ui_frame_ancestors: str = typer.Option(None, "--app-ui-frame-ancestors", help=const.FRAME_ANCENSTORS_HELP),
         app_ui_connect_src: str = typer.Option(None, "--app-ui-connect-src", help=const.CONNECT_SOURCE_HELP),
         app_ui_disable_csp: bool = typer.Option(False, "--app-ui-disable-csp", help=const.DISABLE_CSP_HELP),
@@ -64,14 +65,15 @@
             wsi_mount_points=wsi_mount_points,
             docker_config=docker_config,
             build=build,
             pull=pull,
             nginx_port=nginx_port,
             wbs_url=wbs_url,
             isyntax_sdk=isyntax_sdk,
+            mirax_plugin=mirax_plugin,
             volume_prefix=volume_prefix,
             gpu_driver=gpu_driver,
             frontend_token_exp=frontend_token_exp,
             scope_token_exp=scope_token_exp,
             app_ui_frame_ancestors=app_ui_frame_ancestors,
             app_ui_connect_src=app_ui_connect_src,
             app_ui_disable_csp=app_ui_disable_csp,
```

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/cli_definitions/services_cli.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/services_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         wsi_mount_points_file: Path = typer.Argument(..., help=const.WSI_MOUNT_POINTS_FILE_HELP),
         build: bool = typer.Option(False, "--build", help=const.BUILD_HELP),
         pull: bool = typer.Option(False, "--pull", help=const.PULL_HELP),
         docker_config: Path = typer.Option(None, "--docker-config", help=const.DOCKER_CONFIG_FILE_HELP),
         nginx_port: int = typer.Option(8888, "--nginx-port", help=const.NGINX_PORT_HELP),
         wbs_url: str = typer.Option(None, "--wbs-url", help=const.WBS_URL_HELP),
         isyntax_sdk: str = typer.Option(None, "--isyntax-sdk", help=const.ISYNTAX_SDK_HELP),
+        mirax_plugin: str = typer.Option(None, "--mirax-plugin", help=const.MIRAX_PLUGIN_HELP),
         volume_prefix: str = typer.Option(None, "--volume-prefix", help=const.VOLUME_PREFIX_HELP),
         gpu_driver: str = typer.Option(None, "--gpu-driver", help=const.GPU_DRIVER_HELP),
         frontend_token_exp: int = typer.Option(60, "--frontend-token-exp", help=const.FRONTEND_TOKEN_EXP),
         scope_token_exp: int = typer.Option(300, "--scope-token-exp", help=const.SCOPE_TOKEN_EXP),
         app_ui_frame_ancestors: str = typer.Option(None, "--app-ui-frame-ancestors", help=const.FRAME_ANCENSTORS_HELP),
         app_ui_connect_src: str = typer.Option(None, "--app-ui-connect-src", help=const.CONNECT_SOURCE_HELP),
         app_ui_disable_csp: bool = typer.Option(False, "--app-ui-disable-csp", help=const.DISABLE_CSP_HELP),
@@ -43,14 +44,15 @@
             wsi_mount_points=wsi_mount_points,
             docker_config=docker_config,
             build=build,
             pull=pull,
             nginx_port=nginx_port,
             wbs_url=wbs_url,
             isyntax_sdk=isyntax_sdk,
+            mirax_plugin=mirax_plugin,
             volume_prefix=volume_prefix,
             gpu_driver=gpu_driver,
             frontend_token_exp=frontend_token_exp,
             scope_token_exp=scope_token_exp,
             app_ui_frame_ancestors=app_ui_frame_ancestors,
             app_ui_connect_src=app_ui_connect_src,
             app_ui_disable_csp=app_ui_disable_csp,
```

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/cli_definitions/slides_cli.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/slides_cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/apps_commands.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/apps_commands.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/cases_commands.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/cases_commands.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/helper/app_helper.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/app_helper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/helper/data_helper.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/data_helper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/helper/job_helper.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/job_helper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/helper/job_validation_helper.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/job_validation_helper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/helper/wsi_helper.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/wsi_helper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/jobs_commands.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/jobs_commands.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/services_commands.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/services_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,19 +80,20 @@
         if service["name"] in SERVICE_API_MAPPING and "service" in service["name"]:
             exposed_services.append(service["name"])
     return exposed_services
 
 
 def services_list(client):
     services = settings.get_services()
-    try:
-        client.containers.get("isyntax-backend")
-        services.append({"name": "isyntax-backend"})
-    except docker.errors.NotFound:
-        pass
+    for plugin in ["isyntax-backend", "mirax-backend"]:
+        try:
+            client.containers.get(plugin)
+            services.append({"name": plugin})
+        except docker.errors.NotFound:
+            pass
     databases = settings.get_databases()
     return [service["name"] for service in services] + [db["name"] for db in databases]
 
 
 def services_volumes(volume_prefix):
     services = settings.get_services()
     databases = settings.get_databases()
@@ -125,14 +126,15 @@
     wsi_mount_points,
     build,
     pull,
     docker_config=None,
     nginx_port=None,
     wbs_url=None,
     isyntax_sdk=None,
+    mirax_plugin=None,
     volume_prefix=None,
     gpu_driver=None,
     frontend_token_exp=None,
     scope_token_exp=None,
     app_ui_frame_ancestors=None,
     app_ui_connect_src=None,
     app_ui_disable_csp=False,
@@ -156,14 +158,15 @@
             assert key_path.is_absolute()
             assert val_path.startswith("/")
 
     services = settings.get_services(
         nginx_port=nginx_port,
         wbs_url=wbs_url,
         isyntax_sdk=isyntax_sdk,
+        mirax_plugin=mirax_plugin,
         gpu_driver=gpu_driver,
         frontend_token_exp=frontend_token_exp,
         scope_token_exp=scope_token_exp,
         app_ui_frame_ancestors=app_ui_frame_ancestors,
         app_ui_connect_src=app_ui_connect_src,
         app_ui_disable_csp=app_ui_disable_csp,
     )
@@ -224,15 +227,15 @@
         with PrintStep(f"Starting: {name}"):
             volumes = {}
 
             if "volume" in service:
                 volume = service["volume"]
                 volumes[_volume_name(volume["name"], volume_prefix)] = {"bind": volume["mount"], "mode": "rw"}
 
-            if name == "wsi-service" or name == "isyntax-backend":
+            if str(name) in ["wsi-service", "isyntax-backend", "mirax-backend"]:
                 for key, val in wsi_mount_points.items():
                     volumes[key] = {"bind": val, "mode": "ro"}
 
             if name == "job-execution-service":
                 if docker_config is not None:
                     # just check valid json:
                     with open(docker_config, encoding="utf-8") as f:
```

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/commands/slides_commands.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/slides_commands.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/constants.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 GPU_DRIVER_HELP = "GPU driver to use for App images, e.g. 'nvidia' (default: no GPU)"
 TRIALS_SERVICES_HELP = "Number of times to try connecting to all services"
 WBS_PORT_HELP = "Listen port of workbench-service container"
 WBS_URL_HELP = "URL used by workbench-client-v3 to access workbench-service (enables custom hosting setups)"
 WBC3_PORT_HELP = "Listen port of workbench-client-v3 container"
 NGINX_PORT_HELP = "Listen port of nginx container"
 ISYNTAX_SDK_HELP = "Full path to philips-pathologysdk-2.0-ubuntu18_04_py36_research.zip for isyntax support"
+MIRAX_PLUGIN_HELP = "Full path to mirax_backend.zip for native mirax support"
 VOLUME_PREFIX_HELP = "Prefix for the names of the container volumes holding service state"
 DOCKER_CONFIG_FILE_HELP = (
     "Docker config file. E.g. to pass proxy configuration to the apps by the job-execution-service."
 )
 FRONTEND_TOKEN_EXP = "Expiration time in seconds of frontend token (needed to retrieve app ui from workbench service)"
 SCOPE_TOKEN_EXP = (
     "Expiration time in seconds of scope token (needed to send or retrieve app data to / from workbench service)"
```

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/custom_models.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/custom_models.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/.gitlab/issue_templates/story_qa_level_1.md` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/.gitlab/issue_templates/story_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/.gitlab/merge_request_templates/merge_request_qa_level_1.md` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/.gitlab/merge_request_templates/merge_request_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/.gitlab-ci.yml` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/CHANGELOG.md` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/LICENSE` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/LICENSE`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/commons.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/commons.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/marketplace/app.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/marketplace/app.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/poetry.lock` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/poetry.lock`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/pyproject.toml` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/pyproject.toml`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/utils/access_token_tools.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/utils/access_token_tools.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/utils/tests/test_access_token_tools.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/utils/tests/test_access_token_tools.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/annotation/annotations.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/annotations.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/annotation/classes.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/classes.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/annotation/collections.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/collections.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/annotation/jobs.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/jobs.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/annotation/primitives.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/primitives.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/clinical.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/clinical.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/commons.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/commons.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/examination.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/examination.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/id_mapper.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/id_mapper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/job.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/job.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/slide.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/slide.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v1/storage.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/storage.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/annotation/annotations.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/annotations.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/annotation/classes.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/classes.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/annotation/collections.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/collections.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/annotation/primitives.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/primitives.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/clinical.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/clinical.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/commons.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/commons.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/examination.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/examination.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/id_mapper.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/id_mapper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/job.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/job.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/slide.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/slide.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/storage.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/storage.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/tests/test_job_mode.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/test_job_mode.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/tests/test_job_progress.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/test_job_progress.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/models/v3/tests/test_job_validation_fields.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/test_job_validation_fields.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/.gitlab/issue_templates/story_qa_level_1.md` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.gitlab/issue_templates/story_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/.gitlab/merge_request_templates/merge_request_qa_level_1.md` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.gitlab/merge_request_templates/merge_request_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/.gitlab-ci.yml` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/CHANGELOG.md` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/README.md` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/README.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/docker-compose.yml` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/poetry.lock` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/poetry.lock`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/__main__.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/__main__.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/issue_templates/story_qa_level_1.md` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/issue_templates/story_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/merge_request_templates/merge_request_qa_level_1.md` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/merge_request_templates/merge_request_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/README.md` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/README.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft1.json` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft1.json`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft3.json` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft3.json`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v3.json` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v3.json`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/tags/tags.csv` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/tags/tags.csv`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/ead_validator.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/ead_validator.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/common.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/common.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/ead.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/ead.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/ead.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/ead.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/job.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/job.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/job_validator.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/job_validator.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/pyproject.toml` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/pyproject.toml`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/test_ead_validator.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/test_ead_validator.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead_with_config.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead_with_config.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3_with_config.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3_with_config.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/conftest.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/conftest.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_completeness.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_completeness.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_compliance.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_compliance.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_completeness.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_completeness.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_compliance.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_compliance.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_suitable_job_status.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_suitable_job_status.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/py_ead_validation/tests/test_exceptions.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/services/docker-compose.yml` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/docker-compose.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 services:
   app-service:
-    image: registry.gitlab.com/empaia/services/app-service:0.7.18@sha256:68fc876459820acac182d5b168f8238083e6a5a9b4351d78d90db20c2b9af494
+    image: registry.gitlab.com/empaia/services/app-service:0.7.19@sha256:f2c1b638e9a1ecd0dc2e4766b66d801e544bd7da22998726b64daf359c13514b
   annotation-service:
-    image: registry.gitlab.com/empaia/services/annotation-service:0.16.4@sha256:228a68ceda2c6dde556a9de9f4bab16e622e5c75c8944cd1c6d3141c3d47ddb7
+    image: registry.gitlab.com/empaia/services/annotation-service:0.16.5@sha256:131da84de1a31cd31c7660583aac149288431e80b88f6a7ffa13ffd92c8f0c85
   job-service:
     image: registry.gitlab.com/empaia/services/job-service:0.7.2@sha256:615c90ce7b353208da06e5deefcebcd74c4705e976123b9b0d2a298505e815e4
   examination-service:
-    image: registry.gitlab.com/empaia/services/examination-service:0.7.22@sha256:d2ad5c3042dcfdff5807b35fb03e1b20057b2364b2c1dd0b5ba3966b8a1a0e50
+    image: registry.gitlab.com/empaia/services/examination-service:0.7.25@sha256:a4ea5e8dfdc4acb91f30e416f21f4669d6d52ebd04ff02bc4f35fc6a9b60bdab
   clinical-data-service:
     image: registry.gitlab.com/empaia/services/clinical-data-service:0.3.2
   storage-mapper-service:
-    image: registry.gitlab.com/empaia/services/storage-mapper-service:0.2.10@sha256:105b6ab0a58a0079961aeb5f65b89fc63b17aacb3f5bdbf8ddcda4abc857320e
+    image: registry.gitlab.com/empaia/services/storage-mapper-service:0.2.13@sha256:1cc1198dbed37050b817afd0ed7ea9044751319abc296420bb6ca6d2c7f11a01
   wsi-service:
-    image: registry.gitlab.com/empaia/services/wsi-service-plugin-integration:0.10.17@sha256:2a339f552389bd46dd97c989b99ded10d11419299b57d85532a36a7c9bcc2712
+    image: registry.gitlab.com/empaia/services/wsi-service-plugin-integration:0.11.2@sha256:5f9aee9740c75dd96bca6ac622517da858198fb1cf0ef4eb8465b0d0358dc937
   medical-data-service:
-    image: registry.gitlab.com/empaia/services/medical-data-service:0.7.10@sha256:386acd0aabbcf23a5643ec4880e60469c2f8adf84f3ab02aab043c7aa8b0a339
+    image: registry.gitlab.com/empaia/services/medical-data-service:0.7.13@sha256:0058b21a96c3f512d73dc6514dc954184400669764e8e96ad21dd4e6ef882714
   marketplace-service-mock:
-    image: registry.gitlab.com/empaia/service-mocks/marketplace-service-mock:0.1.53@sha256:9780c2a0d2ed15868a3c71cac1b28feffea56a72eb1d989d22a13d9bcd0736b3
+    image: registry.gitlab.com/empaia/service-mocks/marketplace-service-mock:0.1.54@sha256:8398a236513e1a116b5914c9c954f0259452a37b0187a85cdb98f7d93a7d5e98
   aaa-service-mock:
     image: registry.gitlab.com/empaia/service-mocks/aaa-service-mock:0.1.41@sha256:98ac5973963f23c5a3f2f6ba333964fa5de4f82ee113b42d728d335de2ca232e
   job-execution-service:
-    image: registry.gitlab.com/empaia/services/job-execution-service:0.5.30@sha256:60b86d5dd353edf0d73be2f444a2802b533541e5fc727ebb3e74e4470f434eb5
+    image: registry.gitlab.com/empaia/services/job-execution-service:0.5.34@sha256:c80551a992011e75626babf42deaa1bf4361de31937f532024988c2008422029
   workbench-daemon:
-    image: registry.gitlab.com/empaia/services/workbench-service:0.9.3@sha256:d34a03c154e168c374f86eca9238be927cd7884d985524955e8929e560316df0
+    image: registry.gitlab.com/empaia/services/workbench-service:0.9.5@sha256:3f7ebe644f003cd2c77023ef3dcf73a2aa82f5dd70d1990da29759ac6de6f138
   workbench-service:
-    image: registry.gitlab.com/empaia/services/workbench-service:0.9.3@sha256:d34a03c154e168c374f86eca9238be927cd7884d985524955e8929e560316df0
+    image: registry.gitlab.com/empaia/services/workbench-service:0.9.5@sha256:3f7ebe644f003cd2c77023ef3dcf73a2aa82f5dd70d1990da29759ac6de6f138
   workbench-client-v3:
-    image: registry.gitlab.com/empaia/integration/frontend-workspace/workbench-client-v3:3.0.0@sha256:f4bc46a897d3e277a551a0eb12595113e80284cfe241f8682d9d562778d84841
+    image: registry.gitlab.com/empaia/integration/frontend-workspace/workbench-client-v3:3.0.6@sha256:bc94d9d1f960b4e6dd43e83473b58009aae0f666f4dcda1da58b692bcbbbff51
   workbench-client-v3-sample-ui:
-    image: registry.gitlab.com/empaia/integration/frontend-workspace/sample-app-v3:3.0.0@sha256:23e2656d65d0d463cfda458051d987582168cf03fa93efa7c731546cde7ee176
+    image: registry.gitlab.com/empaia/integration/frontend-workspace/sample-app-v3:3.0.4@sha256:9ef80b91aa2484bb064e0406290691f2ca92ebc66b4ad9523bb6b3aaa8dec190
   workbench-client-v3-generic-ui:
-    image: registry.gitlab.com/empaia/integration/frontend-workspace/generic-app-ui-v3:3.2.1@sha256:53367d1ff23019df967e8b872c7bc1b4d985afa672d45c0a7494e3e0745d31a0
+    image: registry.gitlab.com/empaia/integration/frontend-workspace/generic-app-ui-v3:3.2.2@sha256:b9704fae8c6f30a996e85ec3f8af1d091b82abd6cc2616bf782cbb5ec205b3e5
   eats-postgres-db:
-    image: registry.gitlab.com/empaia/integration/ci-docker-images/custom-postgres:0.1.62@sha256:ec2dd83bb273dff1a721019a42bce3df7465991a5413848897ecca180e79e6b9
+    image: registry.gitlab.com/empaia/integration/ci-docker-images/custom-postgres:0.1.67@sha256:86ce606ee6e340c8f81fab89016a6005d52169bf20e10910f95b8d53041674ae
   eats-mongo-db:
-    image: mongo:5.0.15@sha256:b5d59773a3b216b58e85f6d6ef8670ca5ccb89b44e3f19f078bec6301a81f0f7
+    image: mongo:5.0.16@sha256:6ea33882c70df83283a6ba0a89fdd304795ba42bcb2c714b49e3ad722dd41b62
```

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/services/nginx/nginx.conf` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/Dockerfile` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/Dockerfile`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM registry.gitlab.com/empaia/integration/ci-docker-images/test-runner:0.1.70@sha256:20758515a51af7e414baf77c0cfc5974d4dd2f0f6fbb789a16a2d4af17ee9503 AS build0
+FROM registry.gitlab.com/empaia/integration/ci-docker-images/test-runner:0.1.72@sha256:a47beb9877f1ed561fbd7b93069902b9d56f70130bc6ec7b42cbfd0a692ad848 AS build0
 
 ENV DEBIAN_FRONTEND=noninteractive
 ENV PYTHONDONTWRITEBYTECODE=1
 ENV PYTHONUNBUFFERED=1
 
 COPY isyntax_backend /isyntax/isyntax_backend
 COPY pyproject.toml /isyntax/pyproject.toml
```

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/__main__.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/__main__.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/isyntax_reader.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/isyntax_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,18 +58,18 @@
                 "rep": "error",
                 "status_code": 422,
                 "detail": f"""The requested pyramid level is not available.
                     The coarsest available level is {len(slide_info["levels"]) - 1}.""",
             }
 
         view_range = [
-            start_x * (2 ** level),
-            (start_x + size_x) * (2 ** level),
-            start_y * (2 ** level),
-            (start_y + size_y) * (2 ** level),
+            start_x * (2**level),
+            (start_x + size_x) * (2**level),
+            start_y * (2**level),
+            (start_y + size_y) * (2**level),
             level,
         ]
 
         try:
             # get data envelopes for requested levels
             data_envelopes = image.source_view.data_envelopes(level)
             regions = image.source_view.request_regions(
@@ -156,15 +156,15 @@
             dim = self.pe_input[image].source_view.dimension_ranges(resolution)
             # we need to calculate level dimensions for x and y manually
             dim_x = (dim[0][2] - dim[0][0]) / dim[0][1]
             dim_y = (dim[1][2] - dim[1][0]) / dim[1][1]
             levels.append(
                 {
                     "extent": {"x": dim_x, "y": dim_y, "z": 1},
-                    "downsample_factor": (2 ** resolution),
+                    "downsample_factor": (2**resolution),
                 }
             )
 
         return levels, derived_levels
 
     def __get_pixel_size(self, image):
         units = self.pe_input[image].source_view.dimension_units
```

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/settings.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     ]
 
 
 def get_services(
     nginx_port=None,
     wbs_url=None,
     isyntax_sdk=None,
+    mirax_plugin=None,
     gpu_driver=None,
     frontend_token_exp=None,
     scope_token_exp=None,
     app_ui_frame_ancestors=None,
     app_ui_connect_src=None,
     app_ui_disable_csp=False,
 ):
@@ -94,304 +95,332 @@
 
     path_to_this_file = pathlib.Path(__file__).parent.absolute()
     path_to_services = os.path.join(path_to_this_file, "services")
     default_version = f"eats-{__version__}"
 
     docker_compose_dict = get_docker_compose_dict()
 
-    services = [
-        {
-            "name": "app-service",
-            "image": docker_compose_dict["services"]["app-service"]["image"],
-            "environment": {
-                "AS_MPS_URL": "http://marketplace-service-mock:8000",
-                "AS_MPS_USE_V1_ROUTES": "True",
-                "AS_CLIENT_ID": "mustnotbeempty",
-                "AS_CLIENT_SECRET": "mustnotbeempty",
-                "AS_MDS_URL": "http://medical-data-service:8000",
-                "AS_ROOT_PATH": "/app-api",
-                "NO_PROXY": "marketplace-service-mock,medical-data-service,mustnotbeempty",
-                "AS_ORGANIZATION_ID": STATIC_ORGANIZATION_ID,
-                "AS_ENABLE_TOKEN_VERIFICATION": True,
-            },
-            "command": ["--port=8000", "--host=0.0.0.0"],
-            "ports": {},
-        },
-        {
-            "name": "annotation-service",
-            "image": docker_compose_dict["services"]["annotation-service"]["image"],
-            "environment": {
-                "ANNOT_DB_HOST": "eats-postgres-db",
-                "ANNOT_DB_PORT": 5432,
-                "ANNOT_DB": "eats",
-                "ANNOT_DB_USERNAME": "empaia",
-                "ANNOT_DB_PASSWORD": "empaia",
-                "ANNOT_API_V1_INTEGRATION": "annotation_service.api.v1.integrations.disable_auth:DisableAuth",
-                "ANNOT_API_V3_INTEGRATION": "annotation_service.api.v3.integrations.disable_auth:DisableAuth",
-                "ANNOT_ALLOW_EXTERNAL_IDS": "True",
-                "ANNOT_V1_ITEM_LIMIT": 10000,
-                "ANNOT_V1_POST_LIMIT": 10000,
-                "ANNOT_V3_ITEM_LIMIT": 10000,
-                "ANNOT_V3_POST_LIMIT": 10000,
-                "ANNOT_ENABLE_PROFILER": False,
-                "ANNOT_ENABLE_FILE_PROFILER": False,
-                "NO_PROXY": "eats-postgres-db",
-            },
-            "command": ["run.sh", "--host=0.0.0.0", "--workers=4", "--port=8000"],
-            "ports": {},
-        },
-        {
-            "name": "job-service",
-            "image": docker_compose_dict["services"]["job-service"]["image"],
-            "environment": {
-                "JS_DB_HOST": "eats-postgres-db",
-                "JS_DB_PORT": 5432,
-                "JS_DB": "eats",
-                "JS_DB_USERNAME": "empaia",
-                "JS_DB_PASSWORD": "empaia",
-                "JS_RSA_KEYS_DIRECTORY": "/app/rsa",
-                "NO_PROXY": "eats-postgres-db",
-            },
-            "command": ["run.sh", "--host=0.0.0.0", "--port=8000"],
-            "ports": {},
-            "volume": {
-                "name": "job-service-vol",
-                "mount": "/app/rsa",
-            },
-        },
-        {
-            "name": "examination-service",
-            "image": docker_compose_dict["services"]["examination-service"]["image"],
-            "environment": {
-                "ES_DB_HOST": "eats-postgres-db",
-                "ES_DB_PORT": 5432,
-                "ES_DB": "eats",
-                "ES_DB_USERNAME": "empaia",
-                "ES_DB_PASSWORD": "empaia",
-                "ES_SCOPE_TOKEN_EXP": scope_token_exp,
-                "ES_API_V1_INTEGRATION": "examination_service.api.v1.integrations.disable_auth:DisableAuth",
-                "NO_PROXY": "eats-postgres-db",
-            },
-            "command": ["run.sh", "--host=0.0.0.0", "--port=8000"],
-            "ports": {},
-        },
-        {
-            "name": "clinical-data-service",
-            "image": docker_compose_dict["services"]["clinical-data-service"]["image"],
-            "environment": {
-                "CDS_DB_HOST": "eats-postgres-db",
-                "CDS_DB_PORT": 5432,
-                "CDS_DB": "eats",
-                "CDS_DB_USERNAME": "empaia",
-                "CDS_DB_PASSWORD": "empaia",
-                "CDS_ALLOW_EXTERNAL_IDS": "True",
-                "NO_PROXY": "eats-postgres-db",
-            },
-            "command": ["run.sh", "--host=0.0.0.0", "--port=8000"],
-            "ports": {},
-        },
-        {
-            "name": "storage-mapper-service",
-            "image": docker_compose_dict["services"]["storage-mapper-service"]["image"],
-            "environment": {
-                "SM_DB_USERNAME": "empaia",
-                "SM_DB_PASSWORD": "empaia",
-                "SM_DB": "eats",
-                "SM_DB_HOST": "eats-postgres-db",
-                "SM_DB_PORT": 5432,
-                "NO_PROXY": "eats-postgres-db",
-            },
-            "command": [],
-            "ports": {},
-        },
-        {
-            "name": "wsi-service",
-            "image": docker_compose_dict["services"]["wsi-service"]["image"],
-            "environment": {
-                "WS_DATA_DIR": "/data",
-                "WS_MAPPER_ADDRESS": "http://storage-mapper-service:8000/v1/slides/{slide_id}",
-                "NO_PROXY": "storage-mapper-service",
-            },
-            "command": [],
-            "ports": {},
-        },
-        {
-            "name": "medical-data-service",
-            "image": docker_compose_dict["services"]["medical-data-service"]["image"],
-            "environment": {
-                "MDS_API_INTEGRATION": "medical_data_service.api.integrations.disable_auth:DisableAuth",
-                "MDS_WS_URL": "http://wsi-service:8080",
-                "MDS_SMS_URL": "http://storage-mapper-service:8000",
-                "MDS_JS_URL": "http://job-service:8000",
-                "MDS_AS_URL": "http://annotation-service:8000",
-                "MDS_CDS_URL": "http://clinical-data-service:8000",
-                "MDS_ES_URL": "http://examination-service:8000",
-                "MDS_ROOT_PATH": "/mds-api",
-                "NO_PROXY": "wsi-service,storage-mapper-service,job-service,annotation-service,"
-                + "clinical-data-service,examination-service",
-            },
-            "command": ["uvicorn", "--host=0.0.0.0", "--port=8000", "--workers=2", "medical_data_service.app:app"],
-            "ports": {},
-        },
-        {
-            "name": "marketplace-service-mock",
-            "image": docker_compose_dict["services"]["marketplace-service-mock"]["image"],
-            "environment": {
-                "MPSM_API_INTEGRATION": "marketplace_service_mock.api.integrations.disable_auth:DisableAuth",
-                "MPSM_ROOT_PATH": "/mps-api",
-                "MPSM_DISABLE_API_V0": "True",
-                "MPSM_ENABLE_API_V1": "True",
-            },
-            "command": ["uvicorn", "--host=0.0.0.0", "--port=8000", "marketplace_service_mock.app:app"],
-            "ports": {},
-            "volume": {
-                "name": "marketplace-service-mock-vol",
-                "mount": "/data",
-            },
-        },
-        {
-            "name": "aaa-service-mock",
-            "image": docker_compose_dict["services"]["aaa-service-mock"]["image"],
-            "environment": {
-                "AAAM_API_INTEGRATION": "aaa_service_mock.api.integrations.disable_auth:DisableAuth",
-                "AAAM_ROOT_PATH": "/aaa-api",
-            },
-            "command": ["uvicorn", "--host=0.0.0.0", "--port=8000", "aaa_service_mock.app:app"],
-            "ports": {},
-            "volume": {
-                "name": "aaa-service-mock-vol",
-                "mount": "/data",
-            },
-        },
-        {
-            "name": "job-execution-service",
-            "image": docker_compose_dict["services"]["job-execution-service"]["image"],
-            "environment": {
-                "JES_DATABASE_URL": "mongodb://eats-mongo-db:27017",
-                "JES_DOCKER_NETWORK": EATS_NET,
-                "JES_DOCKER_GPU_DRIVER": gpu_driver,
-                "JES_JOB_RUNNER": "EVENTED",
-                "JES_MAX_NUMBER_OF_JOBS": 1,
-                "JES_ENABLE_RECEIVER_AUTH": "False",
-                "JES_DOCKER_ALWAYS_PULL": "False",
-                "JES_MPS_URL": "http://marketplace-service-mock:8000",
-                "JES_MPS_USE_V1_ROUTES": "True",
-                "JES_ROOT_PATH": "/jes-api",
-                "NO_PROXY": "eats-mongo-db,marketplace-service-mock",
-            },
-            "command": [],
-            "ports": {},
-            "volume": {
-                "name": "/var/run/docker.sock",
-                "mount": "/var/run/docker.sock",
-            },
-        },
-        {
-            "name": "workbench-daemon",
-            "image": docker_compose_dict["services"]["workbench-daemon"]["image"],
-            "environment": {
-                "WBS_MEDICAL_DATA_SERVICE_URL": "http://medical-data-service:8000",
-                "WBS_JOB_EXECUTION_SERVICE_URL": "http://job-execution-service:8000",
-                "WBS_APP_SERVICE_URL": "http://app-service:8000",
-                "WBS_MARKETPLACE_SERVICE_URL": "http://marketplace-service-mock:8000",
-                "WBS_ORGANIZATION_ID": STATIC_ORGANIZATION_ID,
-                "NO_PROXY": "medical-data-service,job-execution-service,marketplace-service-mock",
-                "WBS_CLIENT_ID": "wbs",
-                "WBS_DEBUG": "True",
-            },
-            "command": ["wbd"],
-            "ports": {},
-        },
-        {
-            "name": "workbench-service",
-            "image": docker_compose_dict["services"]["workbench-service"]["image"],
-            "environment": {
-                "WBS_ENABLE_EATS_MODE": "True",
-                "WBS_AAA_SERVICE_URL": "http://aaa-service-mock:8000",
-                "WBS_MEDICAL_DATA_SERVICE_URL": "http://medical-data-service:8000",
-                "WBS_APP_SERVICE_URL": "http://app-service:8000",
-                "WBS_JOB_EXECUTION_SERVICE_URL": "http://job-execution-service:8000",
-                "WBS_MARKETPLACE_SERVICE_URL": "http://marketplace-service-mock:8000",
-                "WBS_CORS_ALLOW_ORIGINS": '["*"]',
-                "WBS_API_V1_INTEGRATION": "workbench_service.api.v1.integrations.disable_auth:DisableAuth",
-                "WBS_API_V2_INTEGRATION": "workbench_service.api.v2.integrations.disable_auth:DisableAuth",
-                "WBS_API_V3_INTEGRATION": "workbench_service.api.v3.integrations.disable_auth:DisableAuth",
-                "WBS_ORGANIZATION_ID": STATIC_ORGANIZATION_ID,
-                "WBS_CLIENT_ID": "wbs",
-                "WBS_FRONTEND_TOKEN_EXP": frontend_token_exp,
-                "WBS_ROOT_PATH": "/wbs-api",
-                "WBS_APP_UI_FRAME_ANCESTORS": app_ui_frame_ancestors,
-                "WBS_APP_UI_CONNECT_SRC": app_ui_connect_src,
-                "NO_PROXY": (
-                    "aaa-service-mock,medical-data-service,app-service,job-execution-service,"
-                    "marketplace-service-mock,workbench-client-v3-generic-ui"
-                ),
-                "WBS_GENERIC_APP_UI_V3_URL": "http://workbench-client-v3-generic-ui",
-                "WBS_FRONTEND_CSP_URL": f"http://localhost:{nginx_port}",
-                "WBS_DISABLE_CSP_SETTINGS": app_ui_disable_csp,
-            },
-            "command": ["run.sh", "--host=0.0.0.0", "--port=8000"],
-            "ports": {},
-            "extra_hosts": {"host.docker.internal": "host-gateway"},
-        },
-        {
-            "name": "workbench-client-v3",
-            "image": docker_compose_dict["services"]["workbench-client-v3"]["image"],
-            "environment": {
-                "WBC_WBS_SERVER_API_URL": wbs_url,
-                "WBC_WBS_USER_ID": STATIC_USER_ID,
-                "NO_PROXY": "localhost,127.0.0.1",
-            },
-            "ports": {},
-            "command": [],
-        },
-        {
-            "name": "workbench-client-v3-sample-ui",
-            "image": docker_compose_dict["services"]["workbench-client-v3-sample-ui"]["image"],
-            "environment": {
-                "NO_PROXY": "localhost,127.0.0.1",
-            },
-            "command": [],
-        },
-        {
-            "name": "workbench-client-v3-generic-ui",
-            "image": docker_compose_dict["services"]["workbench-client-v3-generic-ui"]["image"],
-            "environment": {
-                "NO_PROXY": "localhost,127.0.0.1",
-            },
-            "command": [],
-        },
-        {
-            "name": "nginx",
-            "environment": {},
-            "path": str(pathlib.Path(path_to_services, "nginx")),
-            "dockerfile_path": "Dockerfile",
-            "ports": {"80": nginx_port},
-            "command": [],
-        },
-    ]
+    services = []
+    enable_isyntax_plugin = -1
+    enable_mirax_plugin = -1
 
     # check for isyntax sdk
     isyntax_sdk_path = os.path.join(
         path_to_services,
         "wsi-service-plugin-isyntax/isyntax_backend",
         "philips-pathologysdk-2.0-ubuntu18_04_py36_research.zip",
     )
     if isyntax_sdk:
+        enable_isyntax_plugin = 1
         shutil.copy(isyntax_sdk, isyntax_sdk_path)
         services.append(
             {
                 "name": "isyntax-backend",
                 "environment": {},
                 "ports": {},
                 "command": [],
                 "path": str(pathlib.Path(path_to_services, "wsi-service-plugin-isyntax/isyntax_backend")),
             }
         )
 
+    mirax_plugin_path = os.path.join(
+        path_to_services,
+        "wsi-service-plugin-mirax/mirax_backend",
+        "mirax_backend.zip",
+    )
+    if mirax_plugin:
+        enable_mirax_plugin = 1
+        shutil.copy(mirax_plugin, mirax_plugin_path)
+        services.append(
+            {
+                "name": "mirax-backend",
+                "environment": {},
+                "ports": {},
+                "command": [],
+                "path": str(pathlib.Path(path_to_services, "wsi-service-plugin-mirax/mirax_backend")),
+            }
+        )
+
+    services.extend(
+        [
+            {
+                "name": "app-service",
+                "image": docker_compose_dict["services"]["app-service"]["image"],
+                "environment": {
+                    "AS_MPS_URL": "http://marketplace-service-mock:8000",
+                    "AS_MPS_USE_V1_ROUTES": "True",
+                    "AS_CLIENT_ID": "mustnotbeempty",
+                    "AS_CLIENT_SECRET": "mustnotbeempty",
+                    "AS_MDS_URL": "http://medical-data-service:8000",
+                    "AS_ROOT_PATH": "/app-api",
+                    "NO_PROXY": "marketplace-service-mock,medical-data-service,mustnotbeempty",
+                    "AS_ORGANIZATION_ID": STATIC_ORGANIZATION_ID,
+                    "AS_ENABLE_TOKEN_VERIFICATION": True,
+                },
+                "command": ["--port=8000", "--host=0.0.0.0"],
+                "ports": {},
+            },
+            {
+                "name": "annotation-service",
+                "image": docker_compose_dict["services"]["annotation-service"]["image"],
+                "environment": {
+                    "ANNOT_DB_HOST": "eats-postgres-db",
+                    "ANNOT_DB_PORT": 5432,
+                    "ANNOT_DB": "eats",
+                    "ANNOT_DB_USERNAME": "empaia",
+                    "ANNOT_DB_PASSWORD": "empaia",
+                    "ANNOT_API_V1_INTEGRATION": "annotation_service.api.v1.integrations.disable_auth:DisableAuth",
+                    "ANNOT_API_V3_INTEGRATION": "annotation_service.api.v3.integrations.disable_auth:DisableAuth",
+                    "ANNOT_ALLOW_EXTERNAL_IDS": "True",
+                    "ANNOT_V1_ITEM_LIMIT": 10000,
+                    "ANNOT_V1_POST_LIMIT": 10000,
+                    "ANNOT_V3_ITEM_LIMIT": 10000,
+                    "ANNOT_V3_POST_LIMIT": 10000,
+                    "ANNOT_ENABLE_PROFILER": False,
+                    "ANNOT_ENABLE_FILE_PROFILER": False,
+                    "NO_PROXY": "eats-postgres-db",
+                },
+                "command": ["run.sh", "--host=0.0.0.0", "--workers=4", "--port=8000"],
+                "ports": {},
+            },
+            {
+                "name": "job-service",
+                "image": docker_compose_dict["services"]["job-service"]["image"],
+                "environment": {
+                    "JS_DB_HOST": "eats-postgres-db",
+                    "JS_DB_PORT": 5432,
+                    "JS_DB": "eats",
+                    "JS_DB_USERNAME": "empaia",
+                    "JS_DB_PASSWORD": "empaia",
+                    "JS_RSA_KEYS_DIRECTORY": "/app/rsa",
+                    "NO_PROXY": "eats-postgres-db",
+                },
+                "command": ["run.sh", "--host=0.0.0.0", "--port=8000"],
+                "ports": {},
+                "volume": {
+                    "name": "job-service-vol",
+                    "mount": "/app/rsa",
+                },
+            },
+            {
+                "name": "examination-service",
+                "image": docker_compose_dict["services"]["examination-service"]["image"],
+                "environment": {
+                    "ES_DB_HOST": "eats-postgres-db",
+                    "ES_DB_PORT": 5432,
+                    "ES_DB": "eats",
+                    "ES_DB_USERNAME": "empaia",
+                    "ES_DB_PASSWORD": "empaia",
+                    "ES_SCOPE_TOKEN_EXP": scope_token_exp,
+                    "ES_API_V1_INTEGRATION": "examination_service.api.v1.integrations.disable_auth:DisableAuth",
+                    "NO_PROXY": "eats-postgres-db",
+                },
+                "command": ["run.sh", "--host=0.0.0.0", "--port=8000"],
+                "ports": {},
+            },
+            {
+                "name": "clinical-data-service",
+                "image": docker_compose_dict["services"]["clinical-data-service"]["image"],
+                "environment": {
+                    "CDS_DB_HOST": "eats-postgres-db",
+                    "CDS_DB_PORT": 5432,
+                    "CDS_DB": "eats",
+                    "CDS_DB_USERNAME": "empaia",
+                    "CDS_DB_PASSWORD": "empaia",
+                    "CDS_ALLOW_EXTERNAL_IDS": "True",
+                    "NO_PROXY": "eats-postgres-db",
+                },
+                "command": ["run.sh", "--host=0.0.0.0", "--port=8000"],
+                "ports": {},
+            },
+            {
+                "name": "storage-mapper-service",
+                "image": docker_compose_dict["services"]["storage-mapper-service"]["image"],
+                "environment": {
+                    "SM_DB_USERNAME": "empaia",
+                    "SM_DB_PASSWORD": "empaia",
+                    "SM_DB": "eats",
+                    "SM_DB_HOST": "eats-postgres-db",
+                    "SM_DB_PORT": 5432,
+                    "NO_PROXY": "eats-postgres-db",
+                },
+                "command": [],
+                "ports": {},
+            },
+            {
+                "name": "wsi-service",
+                "image": docker_compose_dict["services"]["wsi-service"]["image"],
+                "environment": {
+                    "WS_DATA_DIR": "/data",
+                    "WS_MAPPER_ADDRESS": "http://storage-mapper-service:8000/v1/slides/{slide_id}",
+                    "WS_PLUGIN_PRIORITY_ISYNTAX": enable_isyntax_plugin,
+                    "WS_PLUGIN_PRIORITY_MIRAX": enable_mirax_plugin,
+                    "NO_PROXY": "storage-mapper-service",
+                },
+                "command": [],
+                "ports": {},
+            },
+            {
+                "name": "medical-data-service",
+                "image": docker_compose_dict["services"]["medical-data-service"]["image"],
+                "environment": {
+                    "MDS_API_INTEGRATION": "medical_data_service.api.integrations.disable_auth:DisableAuth",
+                    "MDS_WS_URL": "http://wsi-service:8080",
+                    "MDS_SMS_URL": "http://storage-mapper-service:8000",
+                    "MDS_JS_URL": "http://job-service:8000",
+                    "MDS_AS_URL": "http://annotation-service:8000",
+                    "MDS_CDS_URL": "http://clinical-data-service:8000",
+                    "MDS_ES_URL": "http://examination-service:8000",
+                    "MDS_ROOT_PATH": "/mds-api",
+                    "NO_PROXY": "wsi-service,storage-mapper-service,job-service,annotation-service,"
+                    + "clinical-data-service,examination-service",
+                },
+                "command": ["uvicorn", "--host=0.0.0.0", "--port=8000", "--workers=2", "medical_data_service.app:app"],
+                "ports": {},
+            },
+            {
+                "name": "marketplace-service-mock",
+                "image": docker_compose_dict["services"]["marketplace-service-mock"]["image"],
+                "environment": {
+                    "MPSM_API_INTEGRATION": "marketplace_service_mock.api.integrations.disable_auth:DisableAuth",
+                    "MPSM_ROOT_PATH": "/mps-api",
+                    "MPSM_DISABLE_API_V0": "True",
+                    "MPSM_ENABLE_API_V1": "True",
+                },
+                "command": ["uvicorn", "--host=0.0.0.0", "--port=8000", "marketplace_service_mock.app:app"],
+                "ports": {},
+                "volume": {
+                    "name": "marketplace-service-mock-vol",
+                    "mount": "/data",
+                },
+            },
+            {
+                "name": "aaa-service-mock",
+                "image": docker_compose_dict["services"]["aaa-service-mock"]["image"],
+                "environment": {
+                    "AAAM_API_INTEGRATION": "aaa_service_mock.api.integrations.disable_auth:DisableAuth",
+                    "AAAM_ROOT_PATH": "/aaa-api",
+                },
+                "command": ["uvicorn", "--host=0.0.0.0", "--port=8000", "aaa_service_mock.app:app"],
+                "ports": {},
+                "volume": {
+                    "name": "aaa-service-mock-vol",
+                    "mount": "/data",
+                },
+            },
+            {
+                "name": "job-execution-service",
+                "image": docker_compose_dict["services"]["job-execution-service"]["image"],
+                "environment": {
+                    "JES_DATABASE_URL": "mongodb://eats-mongo-db:27017",
+                    "JES_DOCKER_NETWORK": EATS_NET,
+                    "JES_DOCKER_GPU_DRIVER": gpu_driver,
+                    "JES_JOB_RUNNER": "EVENTED",
+                    "JES_MAX_NUMBER_OF_JOBS": 1,
+                    "JES_ENABLE_RECEIVER_AUTH": "False",
+                    "JES_DOCKER_ALWAYS_PULL": "False",
+                    "JES_MPS_URL": "http://marketplace-service-mock:8000",
+                    "JES_MPS_USE_V1_ROUTES": "True",
+                    "JES_ROOT_PATH": "/jes-api",
+                    "NO_PROXY": "eats-mongo-db,marketplace-service-mock",
+                },
+                "command": [],
+                "ports": {},
+                "volume": {
+                    "name": "/var/run/docker.sock",
+                    "mount": "/var/run/docker.sock",
+                },
+            },
+            {
+                "name": "workbench-daemon",
+                "image": docker_compose_dict["services"]["workbench-daemon"]["image"],
+                "environment": {
+                    "WBS_MEDICAL_DATA_SERVICE_URL": "http://medical-data-service:8000",
+                    "WBS_JOB_EXECUTION_SERVICE_URL": "http://job-execution-service:8000",
+                    "WBS_APP_SERVICE_URL": "http://app-service:8000",
+                    "WBS_MARKETPLACE_SERVICE_URL": "http://marketplace-service-mock:8000",
+                    "WBS_ORGANIZATION_ID": STATIC_ORGANIZATION_ID,
+                    "NO_PROXY": "medical-data-service,job-execution-service,marketplace-service-mock",
+                    "WBS_CLIENT_ID": "wbs",
+                    "WBS_DEBUG": "True",
+                    "WBS_ENABLE_EATS_MODE": "True",
+                },
+                "command": ["wbd"],
+                "ports": {},
+            },
+            {
+                "name": "workbench-service",
+                "image": docker_compose_dict["services"]["workbench-service"]["image"],
+                "environment": {
+                    "WBS_ENABLE_EATS_MODE": "True",
+                    "WBS_AAA_SERVICE_URL": "http://aaa-service-mock:8000",
+                    "WBS_MEDICAL_DATA_SERVICE_URL": "http://medical-data-service:8000",
+                    "WBS_APP_SERVICE_URL": "http://app-service:8000",
+                    "WBS_JOB_EXECUTION_SERVICE_URL": "http://job-execution-service:8000",
+                    "WBS_MARKETPLACE_SERVICE_URL": "http://marketplace-service-mock:8000",
+                    "WBS_CORS_ALLOW_ORIGINS": '["*"]',
+                    "WBS_API_V1_INTEGRATION": "workbench_service.api.v1.integrations.disable_auth:DisableAuth",
+                    "WBS_API_V2_INTEGRATION": "workbench_service.api.v2.integrations.disable_auth:DisableAuth",
+                    "WBS_API_V3_INTEGRATION": "workbench_service.api.v3.integrations.disable_auth:DisableAuth",
+                    "WBS_ORGANIZATION_ID": STATIC_ORGANIZATION_ID,
+                    "WBS_CLIENT_ID": "wbs",
+                    "WBS_FRONTEND_TOKEN_EXP": frontend_token_exp,
+                    "WBS_ROOT_PATH": "/wbs-api",
+                    "WBS_APP_UI_FRAME_ANCESTORS": app_ui_frame_ancestors,
+                    "WBS_APP_UI_CONNECT_SRC": app_ui_connect_src,
+                    "NO_PROXY": (
+                        "aaa-service-mock,medical-data-service,app-service,job-execution-service,"
+                        "marketplace-service-mock,workbench-client-v3-generic-ui"
+                    ),
+                    "WBS_GENERIC_APP_UI_V3_URL": "http://workbench-client-v3-generic-ui",
+                    "WBS_FRONTEND_CSP_URL": f"http://localhost:{nginx_port}",
+                    "WBS_DISABLE_CSP_SETTINGS": app_ui_disable_csp,
+                },
+                "command": ["run.sh", "--host=0.0.0.0", "--port=8000"],
+                "ports": {},
+                "extra_hosts": {"host.docker.internal": "host-gateway"},
+            },
+            {
+                "name": "workbench-client-v3",
+                "image": docker_compose_dict["services"]["workbench-client-v3"]["image"],
+                "environment": {
+                    "WBC_WBS_SERVER_API_URL": wbs_url,
+                    "WBC_WBS_USER_ID": STATIC_USER_ID,
+                    "NO_PROXY": "localhost,127.0.0.1",
+                },
+                "ports": {},
+                "command": [],
+            },
+            {
+                "name": "workbench-client-v3-sample-ui",
+                "image": docker_compose_dict["services"]["workbench-client-v3-sample-ui"]["image"],
+                "environment": {
+                    "NO_PROXY": "localhost,127.0.0.1",
+                },
+                "command": [],
+            },
+            {
+                "name": "workbench-client-v3-generic-ui",
+                "image": docker_compose_dict["services"]["workbench-client-v3-generic-ui"]["image"],
+                "environment": {
+                    "NO_PROXY": "localhost,127.0.0.1",
+                },
+                "command": [],
+            },
+            {
+                "name": "nginx",
+                "environment": {},
+                "path": str(pathlib.Path(path_to_services, "nginx")),
+                "dockerfile_path": "Dockerfile",
+                "ports": {"80": nginx_port},
+                "command": [],
+            },
+        ]
+    )
+
     for service in services:
         if "path" not in service:
             service["path"] = str(pathlib.Path(path_to_services, service["name"]))
 
         if "image" not in service:
             pyproject_file = pathlib.Path(service["path"], "pyproject.toml")
             version = default_version
```

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/utils/utils_commons.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_commons.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/utils/utils_mds.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_mds.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/utils/utils_mps.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_mps.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/empaia_app_test_suite/utils/utils_print.py` & `empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_print.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.1.0/pyproject.toml` & `empaia_app_test_suite-3.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "empaia-app-test-suite"
-version = "3.1.0"
+version = "3.2.0"
 description = "The EMPAIA App Test Suite (EATS)"
 license = "MIT"
 
 # Authors / Maintainers
 authors = ["EMPAIA <dev-support@empaia.org>"]
 maintainers = ["EMPAIA <dev-support@empaia.org>"]
 
@@ -31,14 +31,16 @@
     "empaia_app_test_suite/services/",
     "**/__pycache__/"
 ]
 include = [
     "empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/Dockerfile",
     "empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/pyproject.toml",
     "empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/*",
+    "empaia_app_test_suite/services/wsi-service-plugin-mirax/mirax_backend/Dockerfile",
+    "empaia_app_test_suite/services/wsi-service-plugin-mirax/mirax_backend/entrypoint.sh",
     "empaia_app_test_suite/services/nginx/Dockerfile",
     "empaia_app_test_suite/services/nginx/nginx.conf",
     "empaia_app_test_suite/services/docker-compose.yml",
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://gitlab.com/empaia/integration/empaia-app-test-suite/-/issues"
@@ -51,26 +53,25 @@
 python = "^3.8"
 jsonschema = "^4.4.0"
 pydantic = {extras = ["dotenv"], version = "^1.9.0"}
 requests = "^2.27.1"
 toml = "^0.10.2"
 docker = "^6.0.0"
 prettytable = "^3.2.0"
-typer = "^0.6.0"
+typer = "^0.7.0"
 PyYAML = "^6.0"
 
-[tool.poetry.dev-dependencies]
-pydantic = "^1.9.0"
-Pillow = "^9.0.1"
-pytest = "^7.1.1"
-requests = "^2.27.1"
-pycodestyle = "^2.8.0"
-black = "^22.1.0"
-pylint = "^2.12.2"
-packaging = "^21.3"
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+pillow = "^9.5.0"
+pydantic = "^1.10.7"
+pytest = "^7.3.1"
+pycodestyle = "^2.10.0"
+requests = "^2.28.2"
+pylint = "^2.17.2"
 
 [tool.pytest.ini_options]
 norecursedirs = ["empaia_app_test_suite/services"]
 
 [tool.black]
 line-length = 120
 exclude = "(sample_apps)|(empaia_app_test_suite/services)|(empaia_app_test_suite/models)|(empaia_app_test_suite/py_ead_validation)"
```

### Comparing `empaia_app_test_suite-3.1.0/PKG-INFO` & `empaia_app_test_suite-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empaia-app-test-suite
-Version: 3.1.0
+Version: 3.2.0
 Summary: The EMPAIA App Test Suite (EATS)
 Home-page: https://developer.empaia.org/app_developer_docs/#/
 License: MIT
 Author: EMPAIA
 Author-email: dev-support@empaia.org
 Maintainer: EMPAIA
 Maintainer-email: dev-support@empaia.org
@@ -27,15 +27,15 @@
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: docker (>=6.0.0,<7.0.0)
 Requires-Dist: jsonschema (>=4.4.0,<5.0.0)
 Requires-Dist: prettytable (>=3.2.0,<4.0.0)
 Requires-Dist: pydantic[dotenv] (>=1.9.0,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: typer (>=0.6.0,<0.7.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Bug Tracker, https://gitlab.com/empaia/integration/empaia-app-test-suite/-/issues
 Project-URL: Documentation, https://developer.empaia.org/app_developer_docs/#/
 Project-URL: Repository, https://gitlab.com/empaia/integration/empaia-app-test-suite
 Description-Content-Type: text/markdown
 
 # EMPAIA App Test Suite (EATS)
```

