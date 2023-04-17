# Comparing `tmp/iambic_core-0.1.198.tar.gz` & `tmp/iambic_core-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iambic_core-0.1.198.tar", max compression
+gzip compressed data, was "iambic_core-0.2.1.tar", max compression
```

## Comparing `iambic_core-0.1.198.tar` & `iambic_core-0.2.1.tar`

### file list

```diff
@@ -1,150 +1,156 @@
--rw-r--r--   0        0        0    11356 2023-04-10 23:07:45.632792 iambic_core-0.1.198/LICENSE.md
--rw-r--r--   0        0        0     9696 2023-04-10 23:07:45.632792 iambic_core-0.1.198/README.md
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/config/__init__.py
--rw-r--r--   0        0        0    20072 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/config/dynamic_config.py
--rw-r--r--   0        0        0      460 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/config/templates.py
--rw-r--r--   0        0        0     1755 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/config/utils.py
--rw-r--r--   0        0        0    67671 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/config/wizard.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/core/__init__.py
--rw-r--r--   0        0        0     3010 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/core/aio_utils/__init__.py
--rw-r--r--   0        0        0      290 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/core/context.py
--rw-r--r--   0        0        0      451 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/core/exceptions.py
--rw-r--r--   0        0        0    15217 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/core/git.py
--rw-r--r--   0        0        0      758 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/core/iambic_enum.py
--rw-r--r--   0        0        0     4592 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/core/iambic_plugin.py
--rw-r--r--   0        0        0     1685 2023-04-10 23:07:45.652792 iambic_core-0.1.198/iambic/core/logger.py
--rw-r--r--   0        0        0    24753 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/core/models.py
--rw-r--r--   0        0        0     1782 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/core/noq_json.py
--rw-r--r--   0        0        0     4744 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/core/parser.py
--rw-r--r--   0        0        0    42095 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/core/template_generation.py
--rw-r--r--   0        0        0    24381 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/core/utils.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/github/__init__.py
--rw-r--r--   0        0        0      607 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/github/templates/iambic-detect.yml
--rw-r--r--   0        0        0      654 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/github/templates/iambic-enforce.yml
--rw-r--r--   0        0        0      658 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/github/templates/iambic-expire.yml
--rw-r--r--   0        0        0      656 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/github/templates/iambic-import.yml
--rw-r--r--   0        0        0     1042 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/github/utils.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/lambda/__init__.py
--rw-r--r--   0        0        0     4307 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/lambda/app.py
--rw-r--r--   0        0        0    13644 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/main.py
--rw-r--r--   0        0        0      628 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/output/__init__.py
--rw-r--r--   0        0        0     2763 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/output/filters.py
--rw-r--r--   0        0        0      480 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/output/markdown.py
--rw-r--r--   0        0        0    12556 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/output/models.py
--rw-r--r--   0        0        0     4736 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/output/templates/github_summary.jinja2
--rw-r--r--   0        0        0     1086 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/output/templates/text_file_summary.jinja2
--rw-r--r--   0        0        0     1082 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/output/templates/text_screen_summary.jinja2
--rw-r--r--   0        0        0     1040 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/output/text.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/__init__.py
--rw-r--r--   0        0        0       62 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
--rw-r--r--   0        0        0     1670 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
--rw-r--r--   0        0        0     1715 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
--rw-r--r--   0        0        0     1888 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
--rw-r--r--   0        0        0     1902 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
--rw-r--r--   0        0        0    12863 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
--rw-r--r--   0        0        0      660 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/event_bridge/models.py
--rw-r--r--   0        0        0    29881 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/handlers.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
--rw-r--r--   0        0        0    10478 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/group/models.py
--rw-r--r--   0        0        0    17642 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
--rw-r--r--   0        0        0    13596 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/group/utils.py
--rw-r--r--   0        0        0     1254 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/models.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
--rw-r--r--   0        0        0    15802 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/policy/models.py
--rw-r--r--   0        0        0    17502 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
--rw-r--r--   0        0        0    10795 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
--rw-r--r--   0        0        0       35 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
--rw-r--r--   0        0        0    16584 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/role/models.py
--rw-r--r--   0        0        0    21322 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
--rw-r--r--   0        0        0    22598 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/role/utils.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
--rw-r--r--   0        0        0    15144 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/user/models.py
--rw-r--r--   0        0        0    20581 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
--rw-r--r--   0        0        0    21982 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/user/utils.py
--rw-r--r--   0        0        0     4307 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iambic_plugin.py
--rw-r--r--   0        0        0     4968 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
--rw-r--r--   0        0        0    29547 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
--rw-r--r--   0        0        0    20166 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
--rw-r--r--   0        0        0    35114 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
--rw-r--r--   0        0        0    26441 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/models.py
--rw-r--r--   0        0        0     1086 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/sqs/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.656792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/sqs/util.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/tests/__init__.py
--rw-r--r--   0        0        0    11950 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
--rw-r--r--   0        0        0     3550 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/tests/test_models.py
--rw-r--r--   0        0        0    12155 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/utils.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
--rw-r--r--   0        0        0    13737 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/group/models.py
--rw-r--r--   0        0        0     3746 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
--rw-r--r--   0        0        0    14891 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/group/utils.py
--rw-r--r--   0        0        0     2267 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/handlers.py
--rw-r--r--   0        0        0     1795 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
--rw-r--r--   0        0        0     8455 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/models.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
--rw-r--r--   0        0        0     8619 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/user/models.py
--rw-r--r--   0        0        0     3709 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
--rw-r--r--   0        0        0     7179 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/user/utils.py
--rw-r--r--   0        0        0      258 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/utils.py
--rw-r--r--   0        0        0       82 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/example/README.md
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/example/__init__.py
--rw-r--r--   0        0        0      413 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/example/handlers.py
--rw-r--r--   0        0        0      788 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/example/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/example/local_database/__init__.py
--rw-r--r--   0        0        0     1514 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/example/local_database/models.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/example/local_file/__init__.py
--rw-r--r--   0        0        0     1690 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/example/local_file/models.py
--rw-r--r--   0        0        0      195 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/github/README.md
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/github/__init__.py
--rw-r--r--   0        0        0    31334 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/github/github.py
--rw-r--r--   0        0        0    11851 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/github/github_app.py
--rw-r--r--   0        0        0     1349 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/github/handlers.py
--rw-r--r--   0        0        0     1553 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/github/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
--rw-r--r--   0        0        0     9806 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/group/models.py
--rw-r--r--   0        0        0     5345 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
--rw-r--r--   0        0        0    14549 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/group/utils.py
--rw-r--r--   0        0        0     2030 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/handlers.py
--rw-r--r--   0        0        0     5066 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
--rw-r--r--   0        0        0     4409 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/models.py
--rw-r--r--   0        0        0     1154 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
--rw-r--r--   0        0        0     7852 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
--rw-r--r--   0        0        0    14373 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
--rw-r--r--   0        0        0    11307 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
--rw-r--r--   0        0        0     3020 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
--rw-r--r--   0        0        0     3167 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/app/__init__.py
--rw-r--r--   0        0        0     9404 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/app/models.py
--rw-r--r--   0        0        0     3105 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/app/template_generation.py
--rw-r--r--   0        0        0    17906 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/app/utils.py
--rw-r--r--   0        0        0       91 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/group/__init__.py
--rw-r--r--   0        0        0    11354 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/group/models.py
--rw-r--r--   0        0        0     3535 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/group/template_generation.py
--rw-r--r--   0        0        0    19759 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/group/utils.py
--rw-r--r--   0        0        0     2478 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/handlers.py
--rw-r--r--   0        0        0     2687 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/iambic_plugin.py
--rw-r--r--   0        0        0     6720 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/models.py
--rw-r--r--   0        0        0     1085 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/user/__init__.py
--rw-r--r--   0        0        0     9307 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/user/models.py
--rw-r--r--   0        0        0     3424 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/user/template_generation.py
--rw-r--r--   0        0        0    13806 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/user/utils.py
--rw-r--r--   0        0        0     1536 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/utils.py
--rw-r--r--   0        0        0        0 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/request_handler/__init__.py
--rw-r--r--   0        0        0      878 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/request_handler/expire_resources.py
--rw-r--r--   0        0        0     4110 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/request_handler/git_apply.py
--rw-r--r--   0        0        0      977 2023-04-10 23:07:45.660792 iambic_core-0.1.198/iambic/request_handler/git_plan.py
--rw-r--r--   0        0        0     1924 2023-04-10 23:07:45.664792 iambic_core-0.1.198/pyproject.toml
--rw-r--r--   0        0        0    12021 1970-01-01 00:00:00.000000 iambic_core-0.1.198/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-04-17 21:53:10.610612 iambic_core-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0     9929 2023-04-17 21:53:10.610612 iambic_core-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/config/__init__.py
+-rw-r--r--   0        0        0    20099 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/config/dynamic_config.py
+-rw-r--r--   0        0        0      460 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/config/templates.py
+-rw-r--r--   0        0        0     1773 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/config/utils.py
+-rw-r--r--   0        0        0    67805 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/config/wizard.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/__init__.py
+-rw-r--r--   0        0        0     3010 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/aio_utils/__init__.py
+-rw-r--r--   0        0        0      290 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/context.py
+-rw-r--r--   0        0        0      610 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/exceptions.py
+-rw-r--r--   0        0        0    15217 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/git.py
+-rw-r--r--   0        0        0      758 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/iambic_enum.py
+-rw-r--r--   0        0        0     4592 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/iambic_plugin.py
+-rw-r--r--   0        0        0     1685 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/logger.py
+-rw-r--r--   0        0        0    24817 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/models.py
+-rw-r--r--   0        0        0     1782 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/noq_json.py
+-rw-r--r--   0        0        0     4991 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/parser.py
+-rw-r--r--   0        0        0    42395 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/template_generation.py
+-rw-r--r--   0        0        0    24381 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/core/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.634612 iambic_core-0.2.1/iambic/github/__init__.py
+-rw-r--r--   0        0        0      607 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/github/templates/iambic-detect.yml
+-rw-r--r--   0        0        0      654 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/github/templates/iambic-enforce.yml
+-rw-r--r--   0        0        0      658 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/github/templates/iambic-expire.yml
+-rw-r--r--   0        0        0      656 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/github/templates/iambic-import.yml
+-rw-r--r--   0        0        0     1042 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/github/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/lambda/__init__.py
+-rw-r--r--   0        0        0     4307 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/lambda/app.py
+-rw-r--r--   0        0        0    13644 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/main.py
+-rw-r--r--   0        0        0      628 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/output/__init__.py
+-rw-r--r--   0        0        0     2763 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/output/filters.py
+-rw-r--r--   0        0        0      480 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/output/markdown.py
+-rw-r--r--   0        0        0    12556 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/output/models.py
+-rw-r--r--   0        0        0     4736 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/output/templates/github_summary.jinja2
+-rw-r--r--   0        0        0     1086 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/output/templates/text_file_summary.jinja2
+-rw-r--r--   0        0        0     1082 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/output/templates/text_screen_summary.jinja2
+-rw-r--r--   0        0        0     1040 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/output/text.py
+-rw-r--r--   0        0        0     1240 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/__init__.py
+-rw-r--r--   0        0        0       62 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
+-rw-r--r--   0        0        0     1670 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
+-rw-r--r--   0        0        0     1715 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
+-rw-r--r--   0        0        0     1888 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
+-rw-r--r--   0        0        0     1902 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
+-rw-r--r--   0        0        0    12863 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
+-rw-r--r--   0        0        0      660 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py
+-rw-r--r--   0        0        0    31927 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/handlers.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
+-rw-r--r--   0        0        0    10619 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/group/models.py
+-rw-r--r--   0        0        0    17564 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
+-rw-r--r--   0        0        0    13616 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py
+-rw-r--r--   0        0        0     1254 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/models.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
+-rw-r--r--   0        0        0    15802 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py
+-rw-r--r--   0        0        0    17425 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
+-rw-r--r--   0        0        0    10795 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
+-rw-r--r--   0        0        0       35 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
+-rw-r--r--   0        0        0    16726 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/role/models.py
+-rw-r--r--   0        0        0    21185 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
+-rw-r--r--   0        0        0    23407 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
+-rw-r--r--   0        0        0    15144 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/user/models.py
+-rw-r--r--   0        0        0    20504 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
+-rw-r--r--   0        0        0    22515 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py
+-rw-r--r--   0        0        0     4307 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py
+-rw-r--r--   0        0        0     4968 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
+-rw-r--r--   0        0        0    29870 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
+-rw-r--r--   0        0        0    20177 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
+-rw-r--r--   0        0        0    34945 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
+-rw-r--r--   0        0        0    26764 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/models.py
+-rw-r--r--   0        0        0     1086 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/sqs/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/sqs/util.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/tests/__init__.py
+-rw-r--r--   0        0        0    11950 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
+-rw-r--r--   0        0        0     3550 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/tests/test_models.py
+-rw-r--r--   0        0        0    12458 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
+-rw-r--r--   0        0        0    13766 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/group/models.py
+-rw-r--r--   0        0        0     3746 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
+-rw-r--r--   0        0        0    14891 2023-04-17 21:53:10.638612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py
+-rw-r--r--   0        0        0     2267 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/handlers.py
+-rw-r--r--   0        0        0     1795 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
+-rw-r--r--   0        0        0     8455 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/models.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
+-rw-r--r--   0        0        0     8648 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/user/models.py
+-rw-r--r--   0        0        0     3709 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
+-rw-r--r--   0        0        0     7179 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py
+-rw-r--r--   0        0        0      258 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/utils.py
+-rw-r--r--   0        0        0       82 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/example/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/example/__init__.py
+-rw-r--r--   0        0        0      413 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/example/handlers.py
+-rw-r--r--   0        0        0      788 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/example/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/example/local_database/__init__.py
+-rw-r--r--   0        0        0     1514 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/example/local_database/models.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/example/local_file/__init__.py
+-rw-r--r--   0        0        0     1690 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/example/local_file/models.py
+-rw-r--r--   0        0        0      195 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/github/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/github/__init__.py
+-rw-r--r--   0        0        0    31334 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/github/github.py
+-rw-r--r--   0        0        0    11851 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/github/github_app.py
+-rw-r--r--   0        0        0     1349 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/github/handlers.py
+-rw-r--r--   0        0        0     1553 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/github/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
+-rw-r--r--   0        0        0     9806 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/group/models.py
+-rw-r--r--   0        0        0     5345 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
+-rw-r--r--   0        0        0    14549 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py
+-rw-r--r--   0        0        0     2030 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/handlers.py
+-rw-r--r--   0        0        0     5066 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
+-rw-r--r--   0        0        0     4409 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/models.py
+-rw-r--r--   0        0        0     1154 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
+-rw-r--r--   0        0        0     7852 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
+-rw-r--r--   0        0        0    14373 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
+-rw-r--r--   0        0        0    11307 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
+-rw-r--r--   0        0        0     3020 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
+-rw-r--r--   0        0        0     3167 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/app/__init__.py
+-rw-r--r--   0        0        0     9468 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/app/models.py
+-rw-r--r--   0        0        0     3105 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/app/template_generation.py
+-rw-r--r--   0        0        0    17906 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/app/utils.py
+-rw-r--r--   0        0        0       91 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/group/__init__.py
+-rw-r--r--   0        0        0    11393 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/group/models.py
+-rw-r--r--   0        0        0     3535 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/group/template_generation.py
+-rw-r--r--   0        0        0    19759 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/group/utils.py
+-rw-r--r--   0        0        0     2478 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/handlers.py
+-rw-r--r--   0        0        0     2687 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py
+-rw-r--r--   0        0        0     6720 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/models.py
+-rw-r--r--   0        0        0     1085 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/user/__init__.py
+-rw-r--r--   0        0        0     9307 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/user/models.py
+-rw-r--r--   0        0        0     3424 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/user/template_generation.py
+-rw-r--r--   0        0        0    13806 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/user/utils.py
+-rw-r--r--   0        0        0     1536 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/utils.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/request_handler/__init__.py
+-rw-r--r--   0        0        0      878 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/request_handler/expire_resources.py
+-rw-r--r--   0        0        0     4110 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/request_handler/git_apply.py
+-rw-r--r--   0        0        0      977 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/request_handler/git_plan.py
+-rw-r--r--   0        0        0        0 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/vendor/__init__.py
+-rw-r--r--   0        0        0      168 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
+-rw-r--r--   0        0        0     1069 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/vendor/lambda_multiprocessing/LICENSE
+-rw-r--r--   0        0        0      137 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/vendor/lambda_multiprocessing/__init__.py
+-rw-r--r--   0        0        0    12600 2023-04-17 21:53:10.642612 iambic_core-0.2.1/iambic/vendor/lambda_multiprocessing/main.py
+-rw-r--r--   0        0        0     1922 2023-04-17 21:53:10.646612 iambic_core-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    12252 1970-01-01 00:00:00.000000 iambic_core-0.2.1/PKG-INFO
```

### Comparing `iambic_core-0.1.198/LICENSE.md` & `iambic_core-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/README.md` & `iambic_core-0.2.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [![Supported Versions](https://img.shields.io/pypi/pyversions/iambic-core.svg)](https://pypi.org/project/iambic-core)
 [![codecov.io](https://codecov.io/github/noqdev/iambic/coverage.svg?branch=main)](https://codecov.io/github/noqdev/iambic?branch=main)
 
 # IAMbic: Cloud IAM as Code
 
 "IAMbic: the Terraform of Cloud IAM"
 
-Easily manage and streamline cloud Identity and Access Management (IAM) with IAMbic, a multi-cloud IAM control plane. Discover more at [https://www.iambic.org](https://www.iambic.org).
+Easily manage and streamline cloud Identity and Access Management (IAM) with IAMbic, a multi-cloud IAM control plane. Discover more at [https://docs.iambic.org](https://docs.iambic.org).
 
 ## Key Features
 
-- **GitOps-driven Cloud IAM (IAMOps)**: Leverage GitOps-driven Cloud IAM with human-readable formats and your favorite tools.
-- **[Multi-Cloud](https://iambic.org/getting_started/)**: Unify cloud identity management for AWS, Okta, Azure Active Directory, Google Workspace, and more.
-- **[Dynamic AWS Permissions](https://iambic.org/getting_started/aws#31---create-dynamic-iam-role-policies-that-vary-per-account)**: Simplify multi-account AWS management with flexible templates, allowing multi-account roles to have different permissions and access rules on different accounts.
-- **[Temporary Access, Permissions, and Identities](https://iambic.org/getting_started/aws#32---create-temporary-expiring-iam-permissions)**: Declaratively define and automate expiration dates for resources, permissions, and access rules.
-- **Drift Prevention**: IAMbic can prevent drift on IAM resources that you specify, ensuring that the state of your cloud environment matches the state defined in Git.
+<!-- Keep this in sync with the list of features in the IAMbic Docs Overview Page -->
+
+- **[Universal Cloud Identity](https://docs.iambic.org/getting_started/)**: Unify cloud identity management for AWS, Okta, Azure Active Directory, Google Workspace with more to come.
+- **[Temporary Access](https://docs.iambic.org/getting_started/aws#32---create-temporary-expiring-iam-permissions)**: Declaratively define and automate expiration dates for resources, permissions, and access rules.
+- **[Dynamic AWS Permissions](https://docs.iambic.org/getting_started/aws#31---create-dynamic-iam-role-policies-that-vary-per-account)**: Simplify multi-account AWS management with flexible templates, allowing multi-account roles to have different permissions and access rules on different accounts.
+- **[Drift Prevention](https://docs.iambic.org/how_to_guides/prevent-drift)**: Protect the IAM resources you want to be exclusively managed via IAMbic. What is in Git becomes the absolute source of truth.
+- **[GitOps-driven Cloud IAM (IAMOps)](https://docs.iambic.org/reference/iamops_philosophy)**: Leverage GitOps-driven Cloud IAM with human-readable formats and your favorite tools.
 - **Centralized Management**: IAMbic keeps Git updated with the latest, complete state of your cloud environment, maintaining a single source of truth for auditing and compliance across multiple cloud providers in Git.
 - **Extendable**: Integrate with various clouds and applications through a powerful plugin architecture.
 - **Auditable**: Track changes to IAM policies, permissions, and rules with Git history. For AWS, IAmbic annotates out-of-band commits with details from CloudTrail.
 
 ## Getting Started
 
-Dive into IAMbic with our [quick-start guide](http://iambic.org/getting_started/) and explore powerful template examples for AWS Multi-Account Roles, Dynamic Permissions, Okta Applications and Group Assignments, Azure Active Directory Users and Groups, and Google Workspace Group Assignments. We are rapidly expanding support for existing resources and cloud providers, so check back often!
+Dive into IAMbic with our [quick-start guide](http://docs.iambic.org/getting_started/) and explore powerful template examples for AWS Multi-Account Roles, Dynamic Permissions, Okta Applications and Group Assignments, Azure Active Directory Users and Groups, and Google Workspace Group Assignments. We are rapidly expanding support for existing resources and cloud providers, so check back often!
 
 ## Installing IAMbic and Supported Versions
 
 IAMbic is available on PyPI:
 
 ```console
 python -m pip install iambic-core
@@ -36,15 +38,15 @@
 
 Here are some examples showcasing IAMbic's capabilities:
 
 #### AWS Multi-Account Cloudwatch Role
 
 Create a Cloudwatch role with static permissions across three accounts, dynamically generating role names based on the account the role is deployed to. This template would
 result in the creation of three roles: "dev_cloudwatch",
-"staging_cloudwatch", and "prod_cloudwatch" on the respective AWS accounts. See the [Getting Started guide for AWS](https://iambic.org/getting_started/aws) for more information.
+"staging_cloudwatch", and "prod_cloudwatch" on the respective AWS accounts. See the [Getting Started guide for AWS](https://docs.iambic.org/getting_started/aws) for more information.
 
 ```yaml
 template_type: NOQ::AWS::IAM::Role
 identifier: '{{account_name}}_cloudwatch'
 included_accounts:
     - dev
     - staging
@@ -82,15 +84,15 @@
   tags:
     - key: owner
       value: devops
 ```
 
 ### AWS Dynamic Permissions
 
-Create a BackendDeveloperRole with varying permissions based on the AWS account. See the [Getting Started guide for AWS](https://iambic.org/getting_started/aws) for more information.
+Create a BackendDeveloperRole with varying permissions based on the AWS account. See the [Getting Started guide for AWS](https://docs.iambic.org/getting_started/aws) for more information.
 
 ```yaml
 template_type: NOQ::AWS::IAM::Role
 identifier: '{{account_name}}_backend_developer'
 included_accounts:
   - '*'
 excluded_accounts:
@@ -137,15 +139,15 @@
   tags:
     - key: owner
       value: devops
 ```
 
 ### Okta Application Assignments
 
-Manage Okta application assignments, including expiration dates for specific users. See the [Getting Started guide for Okta](https://iambic.org/getting_started/okta) for more information.
+Manage Okta application assignments, including expiration dates for specific users. See the [Getting Started guide for Okta](https://docs.iambic.org/getting_started/okta) for more information.
 
 ```yaml
 template_type: NOQ::Okta::App
 idp_name: development
 properties:
   name: Salesforce.com
   assignments:
@@ -154,15 +156,15 @@
     - user: username3@example.com
       expires_at: 2023-09-01T00:00 UTC
   status: ACTIVE
 ```
 
 ### Okta Group Assignments
 
-Easily manage Okta group assignments with expiration dates for members. See the [Getting Started guide for Okta](https://iambic.org/getting_started/okta) for more information.
+Easily manage Okta group assignments with expiration dates for members. See the [Getting Started guide for Okta](https://docs.iambic.org/getting_started/okta) for more information.
 
 ```yaml
 template_type: NOQ::Okta::Group
 idp_name: main
 properties:
   name: engineering_interns
   description: Engineering Interns
@@ -173,15 +175,15 @@
       expires_at: 2023-09-01
 
 ```
 
 ### Google Group Assignments
 
 Manage Google Workspace group assignments, including temporary access for external users. See the [Getting Started guide for Google
-Workspace](https://iambic.org/getting_started/google) for more information.
+Workspace](https://docs.iambic.org/getting_started/google) for more information.
 
 ```yaml
 template_type: NOQ::GoogleWorkspace::Group
 properties:
   name: DockerHub
   description: Dockerhub Access
   domain: example.com
@@ -192,29 +194,29 @@
     - email: external_user@gmail.com
     - email: some_engineer@example.com
       expires_at: 2023-03-05
 ```
 
 ## Azure Active Directory Users
 
-Manage Azure Active Directory users and their attributes. See the [Getting Started guide for Azure AD](https://iambic.org/getting_started/azure_ad) for more information.
+Manage Azure Active Directory users and their attributes. See the [Getting Started guide for Azure AD](https://docs.iambic.org/getting_started/azure_ad) for more information.
 
 ```yaml
 expires_at: 2025-01-01
 template_type: NOQ::AzureAD::User
 idp_name: development
 properties:
   display_name: Example User
   given_name: Example
   username: user@example.com
 ```
 
 ### Azure Active Directory Groups and Group Assignments
 
-Manage Azure Active Directory groups and group assignments, including temporary access for external users. See the [Getting Started guide for Azure AD](https://iambic.org/getting_started/azure_ad) for more information.
+Manage Azure Active Directory groups and group assignments, including temporary access for external users. See the [Getting Started guide for Azure AD](https://docs.iambic.org/getting_started/azure_ad) for more information.
 
 ```yaml
 template_type: NOQ::AzureAD::Group
 idp_name: development
 properties:
   name: iambic_test_group
   description: A test group to use with IAMbic
@@ -246,8 +248,8 @@
 
 IAMbic is licensed under the Apache-2.0 license. Commercial licenses and support are also available from Noq Software, Inc.
 
 ### Provider Plugins
 
 Provider Plugins (Such as the AWS, Okta, Azure Active Directory, and Google Workspace plugins) are licensed under Apache 2. You are free to write your own provider plugins for internal services without releasing its source code.
 
-For more information, please visit [iambic.org](https://iambic.org/license).
+For more information, please visit [iambic.org](https://docs.iambic.org/license).
```

### Comparing `iambic_core-0.1.198/iambic/config/dynamic_config.py` & `iambic_core-0.2.1/iambic/config/dynamic_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from pathlib import Path
 from typing import List, Optional, Union
 from uuid import uuid4
 
 import ujson as json
 from pydantic import BaseModel, Field
 from pydantic import create_model as create_pydantic_model
+from iambic.core.exceptions import MultipleSecretsNotAcceptedException
 
 import iambic.plugins.v0_1_0.github
 from iambic.core.context import ctx
 from iambic.core.iambic_plugin import ProviderPlugin
 from iambic.core.logger import log
 from iambic.core.models import BaseTemplate, ExecutionMessage, TemplateChangeDetails
 from iambic.core.utils import sort_dict, yaml
@@ -156,51 +157,54 @@
     def configured_plugins(self):
         return [
             plugin for plugin in self.plugin_instances if self.get_config_plugin(plugin)
         ]
 
     async def set_config_secrets(self):
         if self.extends:
-            for extend in self.extends:
-                if extend.key == ExtendsConfigKey.LOCAL_FILE:
-                    dir_path = os.path.dirname(self.file_path)
-                    extend_path = os.path.join(dir_path, extend.value)
-                    with open(extend_path, "r") as ymlfile:
-                        extend_config = yaml.load(ymlfile)
-                    for k, v in extend_config.items():
-                        if not getattr(self, k, None):
-                            setattr(self, k, v)
-                else:
-                    decoded_secret_responses: list[dict] = await asyncio.gather(
-                        *[
-                            plugin.async_decode_secret_callable(
-                                self.get_config_plugin(plugin), extend
-                            )
-                            for plugin in self.plugin_instances
-                            if plugin.async_decode_secret_callable
-                        ]
-                    )
-                    for decoded_secret in decoded_secret_responses:
-                        if decoded_secret:
-                            if "secrets" not in decoded_secret:
-                                decoded_secret = dict(secrets=decoded_secret)
-                            else:
-                                for k, v in decoded_secret.items():
-                                    if k != "secrets":
-                                        decoded_secret["secrets"][k] = v
-
-                            for k, v in decoded_secret.get("secrets", {}).items():
-                                if k in decoded_secret:
-                                    log.warning(
-                                        "Secret key already exists. "
-                                        "This means it was defined in multiple secrets"
-                                        " or multiple times in the same secret.",
-                                        key=k,
-                                    )
-                                self.secrets.setdefault(k, v)
+            if len(self.extends) > 1:
+                raise MultipleSecretsNotAcceptedException()
+
+            extend = self.extends[0]
+            if extend.key == ExtendsConfigKey.LOCAL_FILE:
+                dir_path = os.path.dirname(self.file_path)
+                extend_path = os.path.join(dir_path, extend.value)
+                with open(extend_path, "r") as ymlfile:
+                    extend_config = yaml.load(ymlfile)
+                for k, v in extend_config.items():
+                    if not getattr(self, k, None):
+                        setattr(self, k, v)
+            else:
+                decoded_secret_responses: list[dict] = await asyncio.gather(
+                    *[
+                        plugin.async_decode_secret_callable(
+                            self.get_config_plugin(plugin), extend
+                        )
+                        for plugin in self.plugin_instances
+                        if plugin.async_decode_secret_callable
+                    ]
+                )
+                for decoded_secret in decoded_secret_responses:
+                    if decoded_secret:
+                        if "secrets" not in decoded_secret:
+                            decoded_secret = dict(secrets=decoded_secret)
+                        else:
+                            for k, v in decoded_secret.items():
+                                if k != "secrets":
+                                    decoded_secret["secrets"][k] = v
+
+                        for k, v in decoded_secret.get("secrets", {}).items():
+                            if k in decoded_secret:
+                                log.warning(
+                                    "Secret key already exists. "
+                                    "This means it was defined in multiple secrets"
+                                    " or multiple times in the same secret.",
+                                    key=k,
+                                )
+                            self.secrets.setdefault(k, v)
 
     async def run_import(
         self,
         exe_message: ExecutionMessage,
         output_dir: str,
     ):
         ctx.command = exe_message.parent_command
```

### Comparing `iambic_core-0.1.198/iambic/config/utils.py` & `iambic_core-0.2.1/iambic/config/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             "Create a configuration with the `NOQ::Core::Config` template type. "
             "You can run `iambic setup` to generate a configuration."
         )
     if len(config_template_file_path) > 1:
         # IAMbic supports 1 configuration per repo
         raise RuntimeError(
             f"Too many NOQ::Core::Config templates discovered. Found ({len(config_template_file_path)}). "
-            f"Expected 1. Files: {','.join(config_template_file_path)}"
+            f"Expected 1. Files: {','.join([str(x) for x in config_template_file_path])}"
         )
 
     return pathlib.Path(config_template_file_path[0])
 
 
 def check_and_update_resource_limit(config: Config):
     soft_limit, hard_limit = resource.getrlimit(resource.RLIMIT_NOFILE)
```

### Comparing `iambic_core-0.1.198/iambic/config/wizard.py` & `iambic_core-0.2.1/iambic/config/wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,14 +351,15 @@
 
         if not self.hub_account_id:
             while True:
                 self.hub_account_id = set_required_text_value(
                     "To get started with the IAMbic setup wizard, you'll need an AWS account.\n"
                     "This is where IAMbic will deploy its main role. If you have an AWS Organization, "
                     "that account will be your hub account.\n"
+                    "Review to-be-created IAMbic roles at https://docs.iambic.org/reference/aws_hub_and_spoke_roles\n"
                     "Which Account ID should we use to deploy the IAMbic hub role?",
                     default_val=default_hub_account_id,
                 )
                 if is_valid_account_id(self.hub_account_id):
                     break
 
         if self.hub_account_id == default_hub_account_id:
@@ -1315,15 +1316,15 @@
             asyncio.run(self.run_import_google_workspace_resources())
             self.update_secret()
             self.config.write()
 
     def configuration_wizard_google_workspace(self):
         log.info(
             "For details on how to retrieve the information required to add a Google Workspace "
-            "to IAMbic check out our docs: https://iambic.org/getting_started/google/"
+            "to IAMbic check out our docs: https://docs.iambic.org/getting_started/google/"
         )
 
         if self.config.google_workspace:
             action = questionary.select(
                 "What would you like to do?",
                 choices=["Go back", "Add", "Edit"],
             ).unsafe_ask()
@@ -1426,15 +1427,15 @@
             asyncio.run(self.run_import_okta_resources())
             self.update_secret()
             self.config.write()
 
     def configuration_wizard_okta(self):
         log.info(
             "For details on how to retrieve the information required to add an Okta Organization "
-            "to IAMbic check out our docs: https://iambic.org/getting_started/okta/"
+            "to IAMbic check out our docs: https://docs.iambic.org/getting_started/okta/"
         )
         if self.config.okta:
             action = questionary.select(
                 "What would you like to do?",
                 choices=["Go back", "Add", "Edit"],
             ).unsafe_ask()
             if action == "Go back":
@@ -1549,15 +1550,15 @@
 
             self.update_secret()
             self.config.write()
 
     def configuration_wizard_azure_ad(self):
         log.info(
             "For details on how to retrieve the information required to add an Azure AD Organization "
-            "to IAMbic check out our docs: https://iambic.org/getting_started/azure_ad/"
+            "to IAMbic check out our docs: https://docs.iambic.org/getting_started/azure_ad/"
         )
         if self.config.azure_ad:
             action = questionary.select(
                 "What would you like to do?",
                 choices=["Go back", "Add", "Edit"],
             ).unsafe_ask()
             if action == "Go back":
```

### Comparing `iambic_core-0.1.198/iambic/core/aio_utils/__init__.py` & `iambic_core-0.2.1/iambic/core/aio_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/core/git.py` & `iambic_core-0.2.1/iambic/core/git.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/core/iambic_enum.py` & `iambic_core-0.2.1/iambic/core/iambic_enum.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/core/iambic_plugin.py` & `iambic_core-0.2.1/iambic/core/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/core/logger.py` & `iambic_core-0.2.1/iambic/core/logger.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/core/models.py` & `iambic_core-0.2.1/iambic/core/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,19 @@
 
 original_field_schema = schema.field_schema
 schema.field_schema = field_schema
 
 
 class IambicPydanticBaseModel(PydanticBaseModel):
     metadata_iambic_fields = Field(
-        set(), description="metadata for iambic", exclude=True
+        set(), description="metadata for iambic", exclude=True, hidden_from_schema=True
+    )
+    metadata_commented_dict: dict = Field(
+        {}, description="yaml inline comments", hidden_from_schema=True
     )
-    metadata_commented_dict: dict = Field({}, description="yaml inline comments")
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         ancestors = inspect.getmro(type(self))
         for ancestor in ancestors:
             if getattr(ancestor, "iambic_specific_knowledge", None):
```

### Comparing `iambic_core-0.1.198/iambic/core/noq_json.py` & `iambic_core-0.2.1/iambic/core/noq_json.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/core/parser.py` & `iambic_core-0.2.1/iambic/core/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 from __future__ import annotations
 
 import json
+import os
 import traceback
 from functools import partial
-from multiprocessing import Pool, cpu_count
 from typing import Union
 
 from pydantic import ValidationError
 from ruamel.yaml.scanner import ScannerError
 
 from iambic.config.templates import TEMPLATES
 from iambic.core.logger import log
 from iambic.core.models import BaseTemplate
 from iambic.core.utils import transform_comments, yaml
 
+# we must avoid import multiprocessing pool in the module loading time
+if os.environ.get("AWS_LAMBDA_FUNCTION_NAME", False):
+    from multiprocessing import cpu_count
+
+    from iambic.vendor.lambda_multiprocessing import Pool
+else:
+    from multiprocessing import Pool, cpu_count
+
 
 # line number is zero-th based
 def resolve_location(loc_list: list[str], ruamel_dict) -> Union[None, int]:
     local_loc_list = loc_list
     local_ruamel_dict = ruamel_dict
     last_known_location = None
     if len(local_loc_list) == 0:
```

### Comparing `iambic_core-0.1.198/iambic/core/template_generation.py` & `iambic_core-0.2.1/iambic/core/template_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,25 +16,34 @@
     get_provider_value,
     is_regex_match,
     sanitize_string,
 )
 from iambic.plugins.v0_1_0.aws.models import AWSAccount
 
 
-async def get_existing_template_map(repo_dir: str, template_type: str) -> dict:
+async def get_existing_template_map(
+    repo_dir: str, template_type: str, nested: bool = False
+) -> dict:
     """Used to keep track of existing templates on import
 
      Write to the existing file before creating a new one.
 
     :param repo_dir:
     :param template_type:
+    :param nested: If true, will return a map of {template_type: {resource_id: template}}
     :return: {resource_id: template}
     """
     templates = load_templates(await gather_templates(repo_dir, template_type))
-    return {template.resource_id: template for template in templates}
+    if not nested:
+        return {template.resource_id: template for template in templates}
+
+    response = defaultdict(dict)
+    for template in templates:
+        response[template.template_type][template.resource_id] = template
+    return response
 
 
 def templatize_resource(aws_account: AWSAccount, resource):
     # TODO: Move away from AWSAccount to a provider agnostic implementation
     resource_type = type(resource)
 
     if isinstance(resource, dict) or isinstance(resource, list):
```

### Comparing `iambic_core-0.1.198/iambic/core/utils.py` & `iambic_core-0.2.1/iambic/core/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/github/templates/iambic-detect.yml` & `iambic_core-0.2.1/iambic/github/templates/iambic-detect.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/github/templates/iambic-enforce.yml` & `iambic_core-0.2.1/iambic/github/templates/iambic-enforce.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/github/templates/iambic-expire.yml` & `iambic_core-0.2.1/iambic/github/templates/iambic-expire.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/github/templates/iambic-import.yml` & `iambic_core-0.2.1/iambic/github/templates/iambic-import.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/github/utils.py` & `iambic_core-0.2.1/iambic/github/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/lambda/app.py` & `iambic_core-0.2.1/iambic/lambda/app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/main.py` & `iambic_core-0.2.1/iambic/main.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/output/__init__.py` & `iambic_core-0.2.1/iambic/output/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/output/filters.py` & `iambic_core-0.2.1/iambic/output/filters.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/output/models.py` & `iambic_core-0.2.1/iambic/output/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/output/templates/github_summary.jinja2` & `iambic_core-0.2.1/iambic/output/templates/github_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/output/templates/text_file_summary.jinja2` & `iambic_core-0.2.1/iambic/output/templates/text_file_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/output/templates/text_screen_summary.jinja2` & `iambic_core-0.2.1/iambic/output/templates/text_screen_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/output/text.py` & `iambic_core-0.2.1/iambic/output/text.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/event_bridge/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/handlers.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from iambic.config.dynamic_config import ExtendsConfig, ExtendsConfigKey
 from iambic.core.context import ctx
 from iambic.core.iambic_enum import Command, IambicManaged
 from iambic.core.logger import log
 from iambic.core.models import BaseTemplate, ExecutionMessage, TemplateChangeDetails
 from iambic.core.parser import load_templates
+from iambic.core.template_generation import get_existing_template_map
 from iambic.core.utils import async_batch_processor, gather_templates, yaml
 from iambic.plugins.v0_1_0.aws.event_bridge.models import (
     GroupMessageDetails,
     ManagedPolicyMessageDetails,
     PermissionSetMessageDetails,
     RoleMessageDetails,
     UserMessageDetails,
@@ -122,14 +123,15 @@
     The async_apply_callable for IdentityCenter (SSO) resources.
 
     :param exe_message: Execution context
     :param config: The config object.
     :param templates: The list of templates to apply.
     :param remote_worker: The remote worker to use for applying templates.
     """
+    await config.set_identity_center_details(exe_message.provider_id)
     return await async_batch_processor(
         [template.apply(config) for template in templates],
         5,
         0.5,
     )
 
 
@@ -228,14 +230,15 @@
     config: AWSConfig,
     base_output_dir: str,
     service_name: str,
     async_collector_callables: list,
     async_generator_callables: list,
     messages: list = None,
     remote_worker=None,
+    existing_template_map: dict = None,
 ):
     base_runner = bool(not exe_message.metadata)
     if not exe_message.metadata:
         exe_message = exe_message.copy()
         exe_message.metadata = dict(service=service_name)
 
     for async_collector_callable in async_collector_callables:
@@ -252,15 +255,15 @@
             elif account.iambic_managed == IambicManaged.DISABLED:
                 continue
             elif not task_message.provider_id:
                 task_message.provider_id = account.account_id
 
             tasks.append(
                 async_collector_callable(
-                    task_message, config, base_output_dir, messages
+                    task_message, config, existing_template_map, messages
                 )
             )
 
         if tasks:
             if base_runner and ctx.use_remote and remote_worker and not messages:
                 # TODO: Update to use the remote_worker
                 await asyncio.gather(*tasks)
@@ -271,26 +274,33 @@
                         "The remote worker definition must be defined in the config to run remote execution."
                     )
                 await asyncio.gather(*tasks)
 
     if base_runner:
         await asyncio.gather(
             *[
-                async_generator_callable(exe_message, config, base_output_dir, messages)
+                async_generator_callable(
+                    exe_message,
+                    config,
+                    base_output_dir,
+                    existing_template_map,
+                    messages,
+                )
                 for async_generator_callable in async_generator_callables
             ]
         )
 
 
 async def import_identity_center_resources(
     exe_message: ExecutionMessage,
     config: AWSConfig,
     base_output_dir: str,
     messages: list = None,
     remote_worker=None,
+    existing_template_map: dict = None,
 ):
     identity_center_config = config.copy()
     identity_center_config.accounts = [
         account
         for account in config.accounts
         if account.identity_center_details
         and account.iambic_managed != IambicManaged.DISABLED
@@ -312,34 +322,57 @@
         identity_center_config,
         base_output_dir,
         "identity_center",
         [collect_aws_permission_sets],
         [generate_aws_permission_set_templates],
         messages,
         remote_worker,
+        existing_template_map,
     )
 
 
 async def import_aws_resources(
     exe_message: ExecutionMessage,
     config: AWSConfig,
     base_output_dir: str,
     messages: list = None,
     remote_worker=None,
 ):
     tasks = []
 
     if not exe_message.metadata or exe_message.metadata["service"] == "identity_center":
+        identity_center_template_map = None
+        if not remote_worker or exe_message.metadata:
+            identity_center_template_map = await get_existing_template_map(
+                repo_dir=base_output_dir,
+                template_type="AWS::IdentityCenter.*",
+                nested=True,
+            )
+
         tasks.append(
             import_identity_center_resources(
-                exe_message, config, base_output_dir, messages, remote_worker
+                exe_message,
+                config,
+                base_output_dir,
+                messages,
+                remote_worker,
+                identity_center_template_map,
             )
         )
 
     if not exe_message.metadata or exe_message.metadata["service"] == "iam":
+        iam_template_map = None
+
+        if not remote_worker or exe_message.metadata:
+            iam_template_map = await get_existing_template_map(
+                repo_dir=base_output_dir,
+                template_type="AWS::IAM.*",
+                nested=True,
+            )
+
         tasks.append(
             import_service_resources(
                 exe_message,
                 config,
                 base_output_dir,
                 "iam",
                 [
@@ -352,14 +385,15 @@
                     generate_aws_role_templates,
                     generate_aws_user_templates,
                     generate_aws_group_templates,
                     generate_aws_managed_policy_templates,
                 ],
                 messages,
                 remote_worker,
+                iam_template_map,
             )
         )
 
     await asyncio.gather(*tasks)
 
 
 async def detect_changes(  # noqa: C901
@@ -521,72 +555,99 @@
                 QueueUrl=queue_url, MaxNumberOfMessages=10
             ).get("Messages", [])
 
     exe_message = ExecutionMessage(
         execution_id=str(uuid.uuid4()), command=Command.IMPORT, provider_type="aws"
     )
     collect_tasks = []
+    iam_template_map = None
+    identity_center_template_map = None
+
+    if role_messages or user_messages or group_messages or managed_policy_messages:
+        iam_template_map = await get_existing_template_map(
+            repo_dir=repo_dir,
+            template_type="AWS::IAM.*",
+            nested=True,
+        )
+
+    if permission_set_messages:
+        identity_center_template_map = await get_existing_template_map(
+            repo_dir=repo_dir,
+            template_type="AWS::IdentityCenter.*",
+            nested=True,
+        )
 
     if role_messages:
         collect_tasks.append(
-            collect_aws_roles(exe_message, config, repo_dir, role_messages)
+            collect_aws_roles(exe_message, config, iam_template_map, role_messages)
         )
     if user_messages:
         collect_tasks.append(
-            collect_aws_users(exe_message, config, repo_dir, user_messages)
+            collect_aws_users(exe_message, config, iam_template_map, user_messages)
         )
     if group_messages:
         collect_tasks.append(
-            collect_aws_groups(exe_message, config, repo_dir, group_messages)
+            collect_aws_groups(exe_message, config, iam_template_map, group_messages)
         )
     if managed_policy_messages:
         collect_tasks.append(
             collect_aws_managed_policies(
-                exe_message, config, repo_dir, managed_policy_messages
+                exe_message, config, iam_template_map, managed_policy_messages
             )
         )
     if permission_set_messages:
         collect_tasks.append(
             collect_aws_permission_sets(
-                exe_message, config, repo_dir, permission_set_messages
+                exe_message,
+                config,
+                identity_center_template_map,
+                permission_set_messages,
             )
         )
 
     if collect_tasks:
         await asyncio.gather(*collect_tasks)
 
         tasks = []
         if role_messages:
             tasks.append(
                 generate_aws_role_templates(
-                    exe_message, config, repo_dir, role_messages
+                    exe_message, config, repo_dir, iam_template_map, role_messages
                 )
             )
         if user_messages:
             tasks.append(
                 generate_aws_user_templates(
-                    exe_message, config, repo_dir, user_messages
+                    exe_message, config, repo_dir, iam_template_map, user_messages
                 )
             )
         if group_messages:
             tasks.append(
                 generate_aws_group_templates(
-                    exe_message, config, repo_dir, group_messages
+                    exe_message, config, repo_dir, iam_template_map, group_messages
                 )
             )
         if managed_policy_messages:
             tasks.append(
                 generate_aws_managed_policy_templates(
-                    exe_message, config, repo_dir, managed_policy_messages
+                    exe_message,
+                    config,
+                    repo_dir,
+                    iam_template_map,
+                    managed_policy_messages,
                 )
             )
         if permission_set_messages:
             tasks.append(
                 generate_aws_permission_set_templates(
-                    exe_message, config, repo_dir, permission_set_messages
+                    exe_message,
+                    config,
+                    repo_dir,
+                    identity_center_template_map,
+                    permission_set_messages,
                 )
             )
         await asyncio.gather(*tasks)
 
         return commit_message
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/group/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/group/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,18 @@
         )
         log_params = dict(
             resource_type=self.resource_type,
             resource_id=group_name,
             account=str(aws_account),
         )
         iambic_import_only = self._is_iambic_import_only(aws_account)
-
-        current_group = await get_group(group_name, client)
+        deleted = self.get_attribute_val_for_account(aws_account, "deleted", False)
+        current_group = await get_group(
+            group_name, client, include_policies=bool(not deleted)
+        )
         if current_group:
             account_change_details.current_value = {
                 **current_group
             }  # Create a new dict
 
             if ctx.command == Command.CONFIG_DISCOVERY:
                 # Don't overwrite a resource during config discovery
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from iambic.core import noq_json as json
 from iambic.core.logger import log
 from iambic.core.models import ExecutionMessage
 from iambic.core.template_generation import (
     base_group_str_attribute,
     create_or_update_template,
     delete_orphaned_templates,
-    get_existing_template_map,
     group_dict_attribute,
     group_int_or_str_attribute,
 )
 from iambic.core.utils import NoqSemaphore, normalize_dict_keys, resource_file_upsert
 from iambic.plugins.v0_1_0.aws.event_bridge.models import GroupMessageDetails
 from iambic.plugins.v0_1_0.aws.iam.group.models import (
     AWS_IAM_GROUP_TEMPLATE_TYPE,
@@ -311,15 +310,15 @@
         list(aws_account_map.values()),
     )
 
 
 async def collect_aws_groups(
     exe_message: ExecutionMessage,
     config: AWSConfig,
-    base_output_dir: str,
+    iam_template_map: dict,
     detect_messages: list[GroupMessageDetails] = None,
 ):
     aws_account_map = await get_aws_account_map(config)
     if exe_message.provider_id:
         aws_account_map = {
             exe_message.provider_id: aws_account_map[exe_message.provider_id]
         }
@@ -327,17 +326,15 @@
     if detect_messages:
         detect_messages = [
             msg for msg in detect_messages if isinstance(msg, GroupMessageDetails)
         ]
         if not detect_messages:
             return
 
-    existing_template_map = await get_existing_template_map(
-        base_output_dir, AWS_IAM_GROUP_TEMPLATE_TYPE
-    )
+    existing_template_map = iam_template_map.get(AWS_IAM_GROUP_TEMPLATE_TYPE, {})
     set_group_resource_inline_policies_semaphore = NoqSemaphore(
         set_group_resource_inline_policies, 20
     )
     set_group_resource_managed_policies_semaphore = NoqSemaphore(
         set_group_resource_managed_policies, 30
     )
 
@@ -447,26 +444,25 @@
         f.write(account_group_output)
 
 
 async def generate_aws_group_templates(
     exe_message: ExecutionMessage,
     config: AWSConfig,
     base_output_dir: str,
+    iam_template_map: dict,
     detect_messages: list[GroupMessageDetails] = None,
 ):
     aws_account_map = await get_aws_account_map(config)
-    existing_template_map = await get_existing_template_map(
-        base_output_dir, AWS_IAM_GROUP_TEMPLATE_TYPE
-    )
+    existing_template_map = iam_template_map.get(AWS_IAM_GROUP_TEMPLATE_TYPE, {})
     group_dir = get_template_dir(base_output_dir)
     account_groups = await exe_message.get_sub_exe_files(
         *RESOURCE_DIR, file_name_and_extension="output.json", flatten_results=True
     )
 
-    log.debug("Grouping groups")
+    log.info("Grouping groups")
     # Move everything to required structure
     for account_group_elem in range(len(account_groups)):
         for group_elem in range(len(account_groups[account_group_elem]["groups"])):
             group_name = account_groups[account_group_elem]["groups"][group_elem].pop(
                 "name"
             )
             account_groups[account_group_elem]["groups"][group_elem][
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/group/utils.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,15 +199,15 @@
     iam_client,
     template_policies: list[dict],
     existing_policies: list[dict],
     log_params: dict,
 ) -> list[ProposedChange]:
     apply_tasks = []
     delete_tasks = []
-    response = []
+    plan_response = []
     template_policy_map = {
         policy["PolicyName"]: {k: v for k, v in policy.items() if k != "PolicyName"}
         for policy in template_policies
     }
     existing_policy_map = {
         policy["PolicyName"]: {k: v for k, v in policy.items() if k != "PolicyName"}
         for policy in existing_policies
@@ -220,15 +220,15 @@
                 ProposedChange(
                     change_type=ProposedChangeType.DELETE,
                     resource_type="aws:policy_document",
                     resource_id=policy_name,
                     attribute="inline_policies",
                 )
             ]
-            response.extend(proposed_changes)
+            plan_response.extend(proposed_changes)
 
             if ctx.execute:
                 log_str = f"{log_str} Removing inline policy..."
 
                 apply_awaitable = boto_crud_call(
                     iam_client.delete_group_policy,
                     GroupName=group_name,
@@ -280,15 +280,15 @@
                         change_type=ProposedChangeType.CREATE,
                         resource_type="aws:policy_document",
                         resource_id=policy_name,
                         attribute="inline_policies",
                         new_value=policy_document,
                     )
                 ]
-            response.extend(proposed_changes)
+            plan_response.extend(proposed_changes)
 
             log_str = f"{resource_existence} inline policies discovered."
             if ctx.execute and policy_document:
                 log_str = f"{log_str} {boto_action} inline policy..."
                 apply_awaitable = boto_crud_call(
                     iam_client.put_group_policy,
                     GroupName=group_name,
@@ -311,15 +311,15 @@
                 await asyncio.sleep(3)
 
         if apply_tasks:
             results.extend(await asyncio.gather(*apply_tasks))
 
         return list(chain.from_iterable(results))
     else:
-        return response
+        return plan_response
 
 
 async def delete_iam_group(group_name: str, iam_client, log_params: dict):
     tasks = []
     # Remove users from group
     attached_users = await list_users_in_group(group_name, iam_client)
     if attached_users:
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/policy/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from iambic.core import noq_json as json
 from iambic.core.logger import log
 from iambic.core.models import ExecutionMessage
 from iambic.core.template_generation import (
     base_group_str_attribute,
     create_or_update_template,
     delete_orphaned_templates,
-    get_existing_template_map,
     group_dict_attribute,
     group_int_or_str_attribute,
 )
 from iambic.core.utils import NoqSemaphore, normalize_dict_keys, resource_file_upsert
 from iambic.plugins.v0_1_0.aws.event_bridge.models import ManagedPolicyMessageDetails
 from iambic.plugins.v0_1_0.aws.iam.policy.models import (
     AWS_MANAGED_POLICY_TEMPLATE_TYPE,
@@ -298,15 +297,15 @@
         list(aws_account_map.values()),
     )
 
 
 async def collect_aws_managed_policies(
     exe_message: ExecutionMessage,
     config: AWSConfig,
-    base_output_dir: str,
+    iam_template_map: dict,
     detect_messages: list[ManagedPolicyMessageDetails] = None,
 ):
     aws_account_map = await get_aws_account_map(config)
     if exe_message.provider_id:
         aws_account_map = {
             exe_message.provider_id: aws_account_map[exe_message.provider_id]
         }
@@ -316,17 +315,15 @@
             msg
             for msg in detect_messages
             if isinstance(msg, ManagedPolicyMessageDetails)
         ]
         if not detect_messages:
             return
 
-    existing_template_map = await get_existing_template_map(
-        base_output_dir, AWS_MANAGED_POLICY_TEMPLATE_TYPE
-    )
+    existing_template_map = iam_template_map.get(AWS_MANAGED_POLICY_TEMPLATE_TYPE, {})
 
     log.info(
         "Generating AWS managed policy templates. Beginning to retrieve AWS IAM Managed Policies.",
         accounts=list(aws_account_map.keys()),
     )
 
     if detect_messages:
@@ -436,20 +433,19 @@
         f.write(account_managed_policy_output)
 
 
 async def generate_aws_managed_policy_templates(
     exe_message: ExecutionMessage,
     config: AWSConfig,
     base_output_dir: str,
+    iam_template_map: dict,
     detect_messages: list[ManagedPolicyMessageDetails] = None,
 ):
     aws_account_map = await get_aws_account_map(config)
-    existing_template_map = await get_existing_template_map(
-        base_output_dir, AWS_MANAGED_POLICY_TEMPLATE_TYPE
-    )
+    existing_template_map = iam_template_map.get(AWS_MANAGED_POLICY_TEMPLATE_TYPE, {})
     resource_dir = get_template_dir(base_output_dir)
     account_managed_policies = await exe_message.get_sub_exe_files(
         *RESOURCE_DIR, file_name_and_extension="output.json", flatten_results=True
     )
 
     log.info("Grouping managed policies")
     # Move everything to required structure
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/policy/utils.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/role/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/role/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,18 @@
         log_params = dict(
             resource_type=self.resource_type,
             resource_id=role_name,
             account=str(aws_account),
         )
         iambic_import_only = self._is_iambic_import_only(aws_account)
 
-        current_role = await get_role(role_name, client)
+        deleted = self.get_attribute_val_for_account(aws_account, "deleted", False)
+        current_role = await get_role(
+            role_name, client, include_policies=bool(not deleted)
+        )
         if current_role:
             account_change_details.current_value = {**current_role}  # Create a new dict
 
             if ctx.command == Command.CONFIG_DISCOVERY:
                 # Don't overwrite a resource during config discovery
                 account_change_details.new_value = {}
                 return account_change_details
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from iambic.core import noq_json as json
 from iambic.core.logger import log
 from iambic.core.models import ExecutionMessage
 from iambic.core.template_generation import (
     base_group_str_attribute,
     create_or_update_template,
     delete_orphaned_templates,
-    get_existing_template_map,
     group_dict_attribute,
     group_int_or_str_attribute,
 )
 from iambic.core.utils import NoqSemaphore, normalize_dict_keys, resource_file_upsert
 from iambic.plugins.v0_1_0.aws.event_bridge.models import RoleMessageDetails
 from iambic.plugins.v0_1_0.aws.iam.policy.models import AssumeRolePolicyDocument
 from iambic.plugins.v0_1_0.aws.iam.role.models import (
@@ -417,26 +416,24 @@
         list(aws_account_map.values()),
     )
 
 
 async def collect_aws_roles(
     exe_message: ExecutionMessage,
     config: AWSConfig,
-    base_output_dir: str,
+    iam_template_map: dict,
     detect_messages: list[RoleMessageDetails] = None,
 ):
     aws_account_map = await get_aws_account_map(config)
     if exe_message.provider_id:
         aws_account_map = {
             exe_message.provider_id: aws_account_map[exe_message.provider_id]
         }
 
-    existing_template_map = await get_existing_template_map(
-        base_output_dir, AWS_IAM_ROLE_TEMPLATE_TYPE
-    )
+    existing_template_map = iam_template_map.get(AWS_IAM_ROLE_TEMPLATE_TYPE, {})
     set_role_resource_inline_policies_semaphore = NoqSemaphore(
         set_role_resource_inline_policies, 20
     )
     set_role_resource_managed_policies_semaphore = NoqSemaphore(
         set_role_resource_managed_policies, 30
     )
     set_role_resource_tags_semaphore = NoqSemaphore(set_role_resource_tags, 45)
@@ -478,15 +475,14 @@
                     else:
                         # There are other accounts for the template so re-eval the template
                         tasks.append(
                             {
                                 "exe_message": exe_message,
                                 "aws_accounts": aws_accounts,
                                 "role_name": existing_template.properties.role_name,
-                                "exe_message": exe_message,
                             }
                         )
 
         account_role_list = (
             await generate_role_resource_file_for_all_accounts_semaphore.process(tasks)
         )
         account_role_list = list(itertools.chain.from_iterable(account_role_list))
@@ -547,21 +543,20 @@
         f.write(account_role_output)
 
 
 async def generate_aws_role_templates(
     exe_message: ExecutionMessage,
     config: AWSConfig,
     base_output_dir: str,
+    iam_template_map: dict,
     detect_messages: list[RoleMessageDetails] = None,
 ):
     role_dir = get_template_dir(base_output_dir)
     aws_account_map = await get_aws_account_map(config)
-    existing_template_map = await get_existing_template_map(
-        base_output_dir, AWS_IAM_ROLE_TEMPLATE_TYPE
-    )
+    existing_template_map = iam_template_map.get(AWS_IAM_ROLE_TEMPLATE_TYPE, {})
     account_roles = await exe_message.get_sub_exe_files(
         *RESOURCE_DIR, file_name_and_extension="output.json", flatten_results=True
     )
 
     if detect_messages:
         detect_messages = [
             msg for msg in detect_messages if isinstance(msg, RoleMessageDetails)
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/role/utils.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -492,44 +492,49 @@
 async def apply_role_inline_policies(
     role_name,
     iam_client,
     template_policies: list[dict],
     existing_policies: list[dict],
     log_params: dict,
 ) -> list[ProposedChange]:
-    tasks = []
-    response = []
+    apply_tasks = []
+    delete_tasks = []
+    plan_response = []
     template_policy_map = {
         policy["PolicyName"]: {k: v for k, v in policy.items() if k != "PolicyName"}
         for policy in template_policies
     }
     existing_policy_map = {
         policy["PolicyName"]: {k: v for k, v in policy.items() if k != "PolicyName"}
         for policy in existing_policies
     }
 
     for policy_name in existing_policy_map.keys():
         if not template_policy_map.get(policy_name):
             log_str = "Stale inline policies discovered."
-            response.append(
+            proposed_changes = [
                 ProposedChange(
                     change_type=ProposedChangeType.DELETE,
                     resource_type="aws:policy_document",
                     resource_id=policy_name,
                     attribute="inline_policies",
                 )
-            )
+            ]
+            plan_response.extend(proposed_changes)
+
             if ctx.execute:
                 log_str = f"{log_str} Removing inline policy..."
-                tasks.append(
-                    boto_crud_call(
-                        iam_client.delete_role_policy,
-                        RoleName=role_name,
-                        PolicyName=policy_name,
-                    )
+
+                apply_awaitable = boto_crud_call(
+                    iam_client.delete_role_policy,
+                    RoleName=role_name,
+                    PolicyName=policy_name,
+                )
+                delete_tasks.append(
+                    plugin_apply_wrapper(apply_awaitable, proposed_changes)
                 )
             log.debug(log_str, policy_name=policy_name, **log_params)
 
     for policy_name, policy_document in template_policy_map.items():
         existing_policy_doc = existing_policy_map.get(policy_name)
         policy_drift = None
         if existing_policy_doc:
@@ -547,56 +552,69 @@
             policy_drift = json.loads(policy_drift.to_json())
 
         if not existing_policy_doc or policy_drift:
             if policy_drift:
                 log_params["policy_drift"] = policy_drift
                 boto_action = "Updating"
                 resource_existence = "Stale"
-                response.append(
+                proposed_changes = [
                     ProposedChange(
                         change_type=ProposedChangeType.UPDATE,
                         resource_type="aws:policy_document",
                         resource_id=policy_name,
                         attribute="inline_policies",
                         change_summary=policy_drift,
                         current_value=existing_policy_doc,
                         new_value=policy_document,
                     )
-                )
+                ]
             else:
                 boto_action = "Creating"
                 resource_existence = "New"
-                response.append(
+                proposed_changes = [
                     ProposedChange(
                         change_type=ProposedChangeType.CREATE,
                         resource_type="aws:policy_document",
                         resource_id=policy_name,
                         attribute="inline_policies",
                         new_value=policy_document,
                     )
-                )
+                ]
+            plan_response.extend(proposed_changes)
 
             log_str = f"{resource_existence} inline policies discovered."
             if ctx.execute and policy_document:
                 log_str = f"{log_str} {boto_action} inline policy..."
-                tasks.append(
-                    boto_crud_call(
-                        iam_client.put_role_policy,
-                        RoleName=role_name,
-                        PolicyName=policy_name,
-                        PolicyDocument=json.dumps(policy_document),
-                    )
+                apply_awaitable = boto_crud_call(
+                    iam_client.put_role_policy,
+                    RoleName=role_name,
+                    PolicyName=policy_name,
+                    PolicyDocument=json.dumps(policy_document),
+                )
+                apply_tasks.append(
+                    plugin_apply_wrapper(apply_awaitable, proposed_changes)
                 )
 
             log.debug(log_str, policy_name=policy_name, **log_params)
 
-    if tasks:
-        await asyncio.gather(*tasks)
-
-    return response
+    if apply_tasks or delete_tasks:
+        results: list[list[ProposedChange]] = []
+        if delete_tasks:
+            results.extend(await asyncio.gather(*delete_tasks))
+            if apply_tasks:
+                # Wait for the policy deletion to propagate before applying new policies
+                # Otherwise a max policy limit error may be thrown
+                await asyncio.sleep(3)
+
+        if apply_tasks:
+            results.extend(await asyncio.gather(*apply_tasks))
+
+        return list(chain.from_iterable(results))
+    else:
+        return plan_response
 
 
 async def delete_iam_role(role_name: str, iam_client, log_params: dict):
     instance_profiles = await get_role_instance_profiles(role_name, iam_client)
 
     tasks = []
     for instance_profile in instance_profiles:
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/user/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from iambic.core import noq_json as json
 from iambic.core.logger import log
 from iambic.core.models import ExecutionMessage
 from iambic.core.template_generation import (
     base_group_str_attribute,
     create_or_update_template,
     delete_orphaned_templates,
-    get_existing_template_map,
     group_dict_attribute,
     group_int_or_str_attribute,
 )
 from iambic.core.utils import NoqSemaphore, normalize_dict_keys, resource_file_upsert
 from iambic.plugins.v0_1_0.aws.event_bridge.models import UserMessageDetails
 from iambic.plugins.v0_1_0.aws.iam.user.models import (
     AWS_IAM_USER_TEMPLATE_TYPE,
@@ -395,35 +394,33 @@
         list(aws_account_map.values()),
     )
 
 
 async def collect_aws_users(
     exe_message: ExecutionMessage,
     config: AWSConfig,
-    base_output_dir: str,
+    iam_template_map: dict,
     detect_messages: list[UserMessageDetails] = None,
 ):
     aws_account_map = await get_aws_account_map(config)
     if exe_message.provider_id:
         aws_account_map = {
             exe_message.provider_id: aws_account_map[exe_message.provider_id]
         }
 
-    existing_template_map = await get_existing_template_map(
-        base_output_dir, AWS_IAM_USER_TEMPLATE_TYPE
-    )
+    existing_template_map = iam_template_map.get(AWS_IAM_USER_TEMPLATE_TYPE, {})
     set_user_resource_inline_policies_semaphore = NoqSemaphore(
         set_user_resource_inline_policies, 20
     )
     set_user_resource_managed_policies_semaphore = NoqSemaphore(
         set_user_resource_managed_policies, 30
     )
 
-    set_user_resource_groups_semaphore = NoqSemaphore(set_user_resource_groups, 30)
-    set_user_resource_tags_semaphore = NoqSemaphore(set_user_resource_tags, 50)
+    set_user_resource_groups_semaphore = NoqSemaphore(set_user_resource_groups, 25)
+    set_user_resource_tags_semaphore = NoqSemaphore(set_user_resource_tags, 30)
 
     log.info(
         "Generating AWS user templates. Beginning to retrieve AWS IAM Users.",
         accounts=list(aws_account_map.keys()),
     )
 
     if detect_messages:
@@ -528,28 +525,27 @@
         f.write(account_user_output)
 
 
 async def generate_aws_user_templates(
     exe_message: ExecutionMessage,
     config: AWSConfig,
     base_output_dir: str,
+    iam_template_map: dict,
     detect_messages: list[UserMessageDetails] = None,
 ):
     aws_account_map = await get_aws_account_map(config)
 
     if detect_messages:
         detect_messages = [
             msg for msg in detect_messages if isinstance(msg, UserMessageDetails)
         ]
         if not detect_messages:
             return
 
-    existing_template_map = await get_existing_template_map(
-        base_output_dir, AWS_IAM_USER_TEMPLATE_TYPE
-    )
+    existing_template_map = iam_template_map.get(AWS_IAM_USER_TEMPLATE_TYPE, {})
     user_dir = get_template_dir(base_output_dir)
     account_users = await exe_message.get_sub_exe_files(
         *RESOURCE_DIR, file_name_and_extension="output.json", flatten_results=True
     )
 
     log.info("Grouping users")
     # Move everything to required structure
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iam/user/utils.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,48 +409,50 @@
 async def apply_user_inline_policies(
     user_name,
     iam_client,
     template_policies: list[dict],
     existing_policies: list[dict],
     log_params: dict,
 ) -> list[ProposedChange]:
-    tasks = []
-    response = []
+    apply_tasks = []
+    delete_tasks = []
+    plan_response = []
     template_policy_map = {
         policy["PolicyName"]: {k: v for k, v in policy.items() if k != "PolicyName"}
         for policy in template_policies
     }
     existing_policy_map = {
         policy["PolicyName"]: {k: v for k, v in policy.items() if k != "PolicyName"}
         for policy in existing_policies
     }
 
     for policy_name in existing_policy_map.keys():
         if not template_policy_map.get(policy_name):
             log_str = "Stale inline policies discovered."
-
             proposed_changes = [
                 ProposedChange(
                     change_type=ProposedChangeType.DELETE,
                     resource_type="aws:policy_document",
                     resource_id=policy_name,
                     attribute="inline_policies",
                 )
             ]
-            response.extend(proposed_changes)
+            plan_response.extend(proposed_changes)
 
             if ctx.execute:
                 log_str = f"{log_str} Removing inline policy..."
 
                 apply_awaitable = boto_crud_call(
                     iam_client.delete_user_policy,
                     UserName=user_name,
                     PolicyName=policy_name,
                 )
-                tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
+                delete_tasks.append(
+                    plugin_apply_wrapper(apply_awaitable, proposed_changes)
+                )
 
             log.debug(log_str, policy_name=policy_name, **log_params)
 
     for policy_name, policy_document in template_policy_map.items():
         existing_policy_doc = existing_policy_map.get(policy_name)
         policy_drift = None
         if existing_policy_doc:
@@ -491,35 +493,47 @@
                         change_type=ProposedChangeType.CREATE,
                         resource_type="aws:policy_document",
                         resource_id=policy_name,
                         attribute="inline_policies",
                         new_value=policy_document,
                     )
                 ]
-            response.extend(proposed_changes)
+            plan_response.extend(proposed_changes)
 
             log_str = f"{resource_existence} inline policies discovered."
             if ctx.execute and policy_document:
                 log_str = f"{log_str} {boto_action} inline policy..."
 
                 apply_awaitable = boto_crud_call(
                     iam_client.put_user_policy,
                     UserName=user_name,
                     PolicyName=policy_name,
                     PolicyDocument=json.dumps(policy_document),
                 )
-                tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
+                apply_tasks.append(
+                    plugin_apply_wrapper(apply_awaitable, proposed_changes)
+                )
 
             log.debug(log_str, policy_name=policy_name, **log_params)
 
-    if tasks:
-        results: list[list[ProposedChange]] = await asyncio.gather(*tasks)
+    if apply_tasks or delete_tasks:
+        results: list[list[ProposedChange]] = []
+        if delete_tasks:
+            results.extend(await asyncio.gather(*delete_tasks))
+            if apply_tasks:
+                # Wait for the policy deletion to propagate before applying new policies
+                # Otherwise a max policy limit error may be thrown
+                await asyncio.sleep(3)
+
+        if apply_tasks:
+            results.extend(await asyncio.gather(*apply_tasks))
+
         return list(chain.from_iterable(results))
     else:
-        return response
+        return plan_response
 
 
 async def apply_user_groups(
     user_name,
     iam_client,
     template_groups: list[dict],
     existing_groups: list[dict],
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/iambic_plugin.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -742,14 +742,22 @@
                 continue
 
             if evaluate_on_provider(self, account):
                 relevant_accounts.append(str(account))
                 tasks.append(self._apply_to_account(account))
 
         if not relevant_accounts:
+            if ctx.execute:
+                if self.deleted:
+                    log_str = "Successfully removed resource."
+                    self.delete()
+                else:
+                    log_str = "No changes detected for resource."
+                log.info(log_str, accounts=relevant_accounts, **log_params)
+
             return template_changes
 
         if ctx.execute:
             log_str = "Applying changes to resource."
         else:
             log_str = "Detecting changes for resource."
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from iambic.core import noq_json as json
 from iambic.core.logger import log
 from iambic.core.models import ExecutionMessage
 from iambic.core.template_generation import (
     base_group_str_attribute,
     create_or_update_template,
     delete_orphaned_templates,
-    get_existing_template_map,
     group_dict_attribute,
     group_int_or_str_attribute,
 )
 from iambic.core.utils import NoqSemaphore, normalize_dict_keys, resource_file_upsert
 from iambic.plugins.v0_1_0.aws.event_bridge.models import PermissionSetMessageDetails
 from iambic.plugins.v0_1_0.aws.identity_center.permission_set.models import (
     AWS_IDENTITY_CENTER_PERMISSION_SET_TEMPLATE_TYPE,
@@ -370,15 +369,15 @@
         list(aws_account_map.values()),
     )
 
 
 async def collect_aws_permission_sets(
     exe_message: ExecutionMessage,
     config: AWSConfig,
-    base_output_dir: str,
+    identity_center_template_map: dict,
     detect_messages: list[PermissionSetMessageDetails] = None,
 ):
     resource_dir = exe_message.get_directory(*RESOURCE_DIR)
     aws_account_map = await get_aws_account_map(config)
     if exe_message.provider_id:
         aws_account_map = {
             exe_message.provider_id: aws_account_map[exe_message.provider_id]
@@ -502,20 +501,21 @@
         f.write(all_permission_sets_output)
 
 
 async def generate_aws_permission_set_templates(
     exe_message: ExecutionMessage,
     config: AWSConfig,
     base_output_dir: str,
+    identity_center_template_map: dict,
     detect_messages: list[PermissionSetMessageDetails] = None,
 ):
     resource_dir = get_template_dir(base_output_dir)
     aws_account_map = await get_aws_account_map(config)
-    existing_template_map = await get_existing_template_map(
-        base_output_dir, AWS_IDENTITY_CENTER_PERMISSION_SET_TEMPLATE_TYPE
+    existing_template_map = identity_center_template_map.get(
+        AWS_IDENTITY_CENTER_PERMISSION_SET_TEMPLATE_TYPE, {}
     )
 
     all_permission_sets = await exe_message.get_sub_exe_files(
         *RESOURCE_DIR, file_name_and_extension="output.json", flatten_results=True
     )
 
     permission_sets_grouped_by_account = defaultdict(list)
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,97 +211,87 @@
     new_managed_policies = [
         policy_arn
         for policy_arn in template_policy_arns
         if policy_arn not in existing_policy_arns
     ]
     if new_managed_policies:
         log_str = "New AWS managed policies discovered."
+        if ctx.execute:
+            log_str = f"{log_str} Attaching AWS managed policies..."
+
         for policy_arn in new_managed_policies:
             proposed_changes = [
                 ProposedChange(
                     change_type=ProposedChangeType.ATTACH,
                     resource_type="aws:policy_document",
                     resource_id=policy_arn,
                     attribute="managed_policies",
                 )
             ]
             response.extend(proposed_changes)
             if ctx.execute:
-                log_str = f"{log_str} Attaching AWS managed policies..."
                 apply_awaitable = boto_crud_call(
                     identity_center_client.attach_managed_policy_to_permission_set,
                     InstanceArn=instance_arn,
                     PermissionSetArn=permission_set_arn,
                     ManagedPolicyArn=policy_arn,
                 )
                 tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
-        log.info(log_str, managed_policies=new_managed_policies, **log_params)
+        log.debug(log_str, managed_policies=new_managed_policies, **log_params)
 
     # Delete existing managed policies not in template
     existing_managed_policies = [
         policy_arn
         for policy_arn in existing_policy_arns
         if policy_arn not in template_policy_arns
     ]
     if existing_managed_policies:
         log_str = "Stale AWS managed policies discovered."
+        if ctx.execute:
+            log_str = f"{log_str} Detaching AWS managed policies..."
+
         for policy_arn in existing_managed_policies:
             proposed_changes = [
                 ProposedChange(
                     change_type=ProposedChangeType.DETACH,
                     resource_type="aws:policy_document",
                     resource_id=policy_arn,
                     attribute="managed_policies",
                 )
             ]
             response.extend(proposed_changes)
             if ctx.execute:
-                log_str = f"{log_str} Detaching AWS managed policies..."
                 apply_awaitable = boto_crud_call(
                     identity_center_client.detach_managed_policy_from_permission_set,
                     InstanceArn=instance_arn,
                     PermissionSetArn=permission_set_arn,
                     ManagedPolicyArn=policy_arn,
                 )
                 tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
-        log.info(log_str, managed_policies=existing_managed_policies, **log_params)
+        log.debug(log_str, managed_policies=existing_managed_policies, **log_params)
 
     if tasks:
         results: list[list[ProposedChange]] = await asyncio.gather(*tasks)
         return list(chain.from_iterable(results))
     else:
         return response
 
 
-async def detach_customer_managed_policy_ref(
-    identity_center_client, instance_arn: str, permission_set_arn: str, policy: dict
-):
-    try:
-        await boto_crud_call(
-            identity_center_client.detach_customer_managed_policy_reference_from_permission_set,
-            InstanceArn=instance_arn,
-            PermissionSetArn=permission_set_arn,
-            CustomerManagedPolicyReference=policy,
-        )
-    except identity_center_client.exceptions.ConflictException:
-        return
-
-
 async def apply_permission_set_customer_managed_policies(
     identity_center_client,
     instance_arn: str,
     permission_set_arn: str,
     template_policies: list[dict],
     existing_policies: list[dict],
     log_params: dict,
 ) -> list[ProposedChange]:
     tasks = []
     response = []
 
-    log.warning(
+    log.debug(
         "Customer Managed Policies",
         template_policies=template_policies,
         existing_policies=existing_policies,
     )
 
     template_policy_map = {
         f"{policy['Path']}{policy['Name']}": policy for policy in template_policies
@@ -314,67 +304,72 @@
     new_customer_managed_policy_references = [
         policy
         for policy_path, policy in template_policy_map.items()
         if not existing_policy_map.get(policy_path)
     ]
     if new_customer_managed_policy_references:
         log_str = "New customer managed policies discovered."
+        if ctx.execute:
+            log_str = f"{log_str} Attaching customer managed policies..."
+
         for policy in new_customer_managed_policy_references:
             proposed_changes = [
                 ProposedChange(
                     change_type=ProposedChangeType.ATTACH,
                     resource_type="aws:policy_document",
                     resource_id=f"{policy['Path']}{policy['Name']}",
                     attribute="customer_managed_policies",
                 )
             ]
             response.extend(proposed_changes)
             if ctx.execute:
-                log_str = f"{log_str} Attaching customer managed policies..."
                 apply_awaitable = boto_crud_call(
                     identity_center_client.attach_customer_managed_policy_reference_to_permission_set,
                     InstanceArn=instance_arn,
                     PermissionSetArn=permission_set_arn,
                     CustomerManagedPolicyReference=policy,
                 )
                 tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
-        log.info(
+        log.debug(
             log_str,
             customer_managed_policy_refs=new_customer_managed_policy_references,
             **log_params,
         )
 
     # Delete existing managed policies not in template
     existing_customer_managed_policy_references = [
         policy
         for policy_path, policy in existing_policy_map.items()
         if not template_policy_map.get(policy_path)
     ]
     if existing_customer_managed_policy_references:
         log_str = "Stale customer managed policies discovered."
+        if ctx.execute:
+            log_str = f"{log_str} Detaching customer managed policies..."
+
         for policy in existing_customer_managed_policy_references:
             proposed_changes = [
                 ProposedChange(
                     change_type=ProposedChangeType.DETACH,
                     resource_type="aws:policy_document",
                     resource_id=f"{policy['Path']}{policy['Name']}",
                     attribute="customer_managed_policies",
                 )
             ]
             response.extend(proposed_changes)
             if ctx.execute:
-                log_str = f"{log_str} Detaching customer managed policies..."
-                apply_awaitable = detach_customer_managed_policy_ref(
-                    identity_center_client,
-                    instance_arn=instance_arn,
-                    permission_set_arn=permission_set_arn,
-                    policy=policy,
+                apply_awaitable = boto_crud_call(
+                    identity_center_client.detach_customer_managed_policy_reference_from_permission_set,
+                    retryable_errors=["ConflictException"],
+                    InstanceArn=instance_arn,
+                    PermissionSetArn=permission_set_arn,
+                    CustomerManagedPolicyReference=policy,
                 )
                 tasks.append(plugin_apply_wrapper(apply_awaitable, proposed_changes))
-        log.info(
+        log.debug(
             log_str,
             customer_managed_policy_refs=existing_customer_managed_policy_references,
             **log_params,
         )
 
     if tasks:
         results: list[list[ProposedChange]] = await asyncio.gather(*tasks)
@@ -416,15 +411,15 @@
 
         if creation_status.get("Status") == "FAILED":
             log_params = {
                 **log_params,
                 "resource_type": f"aws:identity_center:account_assignment:{resource_type.lower()}",
             }
             log.error(
-                "Unable to delete account assignment.",
+                "Unable to create account assignment.",
                 reason=creation_status.get("FailureReason"),
                 assigned_account_id=account_id,
                 resource_name=resource_name,
                 **log_params,
             )
             return
 
@@ -874,19 +869,20 @@
         )
     if customer_managed_policy_references:
         log_params[
             "customer_managed_policy_references"
         ] = customer_managed_policy_references
         tasks.extend(
             [
-                detach_customer_managed_policy_ref(
-                    identity_center_client,
-                    instance_arn=instance_arn,
-                    permission_set_arn=permission_set_arn,
-                    policy=policy,
+                boto_crud_call(
+                    identity_center_client.detach_customer_managed_policy_reference_from_permission_set,
+                    retryable_errors=["ConflictException"],
+                    InstanceArn=instance_arn,
+                    PermissionSetArn=permission_set_arn,
+                    CustomerManagedPolicyReference=policy,
                 )
                 for policy in customer_managed_policy_references
             ]
         )
     if permissions_boundary:
         log_params["permissions_boundary"] = permissions_boundary
         tasks.append(
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -726,14 +726,22 @@
 
         for account in config.accounts:
             if evaluate_on_provider(self, account):
                 relevant_accounts.append(str(account))
                 tasks.append(self._apply_to_account(account))
 
         if not relevant_accounts:
+            if ctx.execute:
+                if self.deleted:
+                    log_str = "Successfully removed resource."
+                    self.delete()
+                else:
+                    log_str = "No changes detected for resource."
+                log.info(log_str, accounts=relevant_accounts, **log_params)
+
             return template_changes
 
         if ctx.execute:
             log_str = "Applying changes to resource."
         else:
             log_str = "Detecting changes for resource."
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/pyproject.toml` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/tests/test_models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/aws/utils.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/aws/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,27 +29,37 @@
         # We are willing to tolerate exception because
         # we are calculating preference from possibly bad templates on disk
         log_params = {"exc_info": str(exc_info)}
         log.error("cannot calculate preference from existing template", **log_params)
     return prefer_templatized
 
 
-async def boto_crud_call(boto_fnc, **kwargs) -> Union[list, dict]:
+async def boto_crud_call(
+    boto_fnc, retryable_errors: list = None, **kwargs
+) -> Union[list, dict]:
     """Responsible for calls to boto. Adds async support and error handling
     :param boto_fnc:
+    :param retryable_errors: A list of error codes that should be retried
     :param kwargs: The params to pass to the boto fnc
     :return:
     """
     retry_count = 0
+    if not retryable_errors:
+        retryable_errors = []
+
+    retryable_errors.append("Throttling")
 
     while True:
         try:
             return await aio_wrapper(boto_fnc, **kwargs)
         except ClientError as err:
-            if "Throttling" in err.response["Error"]["Code"]:
+            if any(
+                retryable_err in err.response["Error"]["Code"]
+                for retryable_err in retryable_errors
+            ):
                 if retry_count >= 10:
                     raise
                 retry_count += 1
                 log.warning(f"Throttling error on {str(boto_fnc)}")
                 await asyncio.sleep(retry_count / 4)
                 continue
             elif "AccessDenied" in err.response["Error"]["Code"]:
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/group/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/group/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,14 +332,15 @@
                     description=self.properties.description,
                     mail_enabled=self.properties.mail_enabled,
                     mail_nickname=self.properties.mail_nickname,
                     security_enabled=self.properties.security_enabled,
                     group_types=self.properties.group_types,
                 )
                 self.properties.group_id = cloud_group.group_id
+                self.write()
             except ClientResponseError as err:
                 log.exception(
                     "Failed to create user in Azure AD",
                     **log_params,
                 )
                 proposed_change = change_details.proposed_changes.pop(-1)
                 proposed_change.exceptions_seen.append(str(err))
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/group/utils.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/handlers.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/user/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/user/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,14 +195,15 @@
                     azure_ad_organization=azure_ad_organization,
                     username=self.properties.username,
                     display_name=self.properties.display_name,
                     mail_nickname=self.properties.mail_nickname
                     or self.properties.username.split("@")[0],
                 )
                 self.properties.user_id = cloud_user.user_id
+                self.write()
             except ClientResponseError as err:
                 log.exception(
                     "Failed to create user in Azure AD",
                     **log_params,
                 )
                 proposed_change = change_details.proposed_changes.pop(-1)
                 proposed_change.exceptions_seen.append(str(err))
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/azure_ad/user/utils.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/example/iambic_plugin.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/example/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/example/local_database/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/example/local_database/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/example/local_file/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/example/local_file/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/github/github.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/github/github.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/github/github_app.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/github/github_app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/github/handlers.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/github/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/github/iambic_plugin.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/github/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/group/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/group/utils.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/handlers.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/pyproject.toml` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/app/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/app/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,20 @@
 
 class AppProperties(ExpiryModel, BaseModel):
     name: str = Field(..., description="Name of the app")
     status: Optional[Status] = Field(None, description="Status of the app")
     id: Optional[str] = Field(
         None, description="Unique App ID for the app. Usually it's {idp-name}-{name}"
     )
-    file_path: str = Field("", description="Path to the template file", exclude=True)
+    file_path: str = Field(
+        "",
+        description="Path to the template file",
+        exclude=True,
+        hidden_from_schema=True,
+    )
     description: Optional[str] = Field("", description="Description of the app")
     extra: Any = Field(None, description=("Extra attributes to store"))
     created: Optional[str] = Field("", description="Date the app was created")
     assignments: List[Assignment] = Field([], description="List of assignments")
 
     @property
     def resource_type(self) -> str:
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/app/template_generation.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/app/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/app/utils.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/app/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/group/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/group/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,17 @@
 
 
 class GroupProperties(ExpiryModel, BaseModel):
     name: str = Field(..., description="Name of the group")
     group_id: str = Field(
         "", description="Unique Group ID for the group. Usually it's {idp-name}-{name}"
     )
-    file_path: str = Field("", description="File path of the group", exclude=True)
+    file_path: str = Field(
+        "", description="File path of the group", exclude=True, hidden_from_schema=True
+    )
     description: Optional[str] = Field("", description="Description of the group")
     extra: Any = Field(None, description=("Extra attributes to store"))
     members: List[UserSimple] = Field([], description="Users in the group")
     identifier: Optional[str] = Field(
         None,
         description="Identifier for the group. Usually it's the group name",
         exclude=True,
```

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/group/template_generation.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/group/utils.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/handlers.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/iambic_plugin.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/pyproject.toml` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/user/models.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/user/template_generation.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/user/utils.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/plugins/v0_1_0/okta/utils.py` & `iambic_core-0.2.1/iambic/plugins/v0_1_0/okta/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/request_handler/expire_resources.py` & `iambic_core-0.2.1/iambic/request_handler/expire_resources.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/request_handler/git_apply.py` & `iambic_core-0.2.1/iambic/request_handler/git_apply.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/iambic/request_handler/git_plan.py` & `iambic_core-0.2.1/iambic/request_handler/git_plan.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.1.198/pyproject.toml` & `iambic_core-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "iambic-core"
 packages = [
     { include="iambic", from="." },
 ]
-version = "0.1.198"
+version = "0.2.1"
 license = "Apache-2.0"
 description = "The python package used to generate, parse, and execute noqform yaml templates."
 authors = ["Noq Software <hello@noq.dev>"]
 readme = "README.md"
 exclude = ["build_util/*"]
 include = ["iambic/output/templates/*"]
```

### Comparing `iambic_core-0.1.198/PKG-INFO` & `iambic_core-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iambic-core
-Version: 0.1.198
+Version: 0.2.1
 Summary: The python package used to generate, parse, and execute noqform yaml templates.
 License: Apache-2.0
 Author: Noq Software
 Author-email: hello@noq.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -57,30 +57,32 @@
 [![Supported Versions](https://img.shields.io/pypi/pyversions/iambic-core.svg)](https://pypi.org/project/iambic-core)
 [![codecov.io](https://codecov.io/github/noqdev/iambic/coverage.svg?branch=main)](https://codecov.io/github/noqdev/iambic?branch=main)
 
 # IAMbic: Cloud IAM as Code
 
 "IAMbic: the Terraform of Cloud IAM"
 
-Easily manage and streamline cloud Identity and Access Management (IAM) with IAMbic, a multi-cloud IAM control plane. Discover more at [https://www.iambic.org](https://www.iambic.org).
+Easily manage and streamline cloud Identity and Access Management (IAM) with IAMbic, a multi-cloud IAM control plane. Discover more at [https://docs.iambic.org](https://docs.iambic.org).
 
 ## Key Features
 
-- **GitOps-driven Cloud IAM (IAMOps)**: Leverage GitOps-driven Cloud IAM with human-readable formats and your favorite tools.
-- **[Multi-Cloud](https://iambic.org/getting_started/)**: Unify cloud identity management for AWS, Okta, Azure Active Directory, Google Workspace, and more.
-- **[Dynamic AWS Permissions](https://iambic.org/getting_started/aws#31---create-dynamic-iam-role-policies-that-vary-per-account)**: Simplify multi-account AWS management with flexible templates, allowing multi-account roles to have different permissions and access rules on different accounts.
-- **[Temporary Access, Permissions, and Identities](https://iambic.org/getting_started/aws#32---create-temporary-expiring-iam-permissions)**: Declaratively define and automate expiration dates for resources, permissions, and access rules.
-- **Drift Prevention**: IAMbic can prevent drift on IAM resources that you specify, ensuring that the state of your cloud environment matches the state defined in Git.
+<!-- Keep this in sync with the list of features in the IAMbic Docs Overview Page -->
+
+- **[Universal Cloud Identity](https://docs.iambic.org/getting_started/)**: Unify cloud identity management for AWS, Okta, Azure Active Directory, Google Workspace with more to come.
+- **[Temporary Access](https://docs.iambic.org/getting_started/aws#32---create-temporary-expiring-iam-permissions)**: Declaratively define and automate expiration dates for resources, permissions, and access rules.
+- **[Dynamic AWS Permissions](https://docs.iambic.org/getting_started/aws#31---create-dynamic-iam-role-policies-that-vary-per-account)**: Simplify multi-account AWS management with flexible templates, allowing multi-account roles to have different permissions and access rules on different accounts.
+- **[Drift Prevention](https://docs.iambic.org/how_to_guides/prevent-drift)**: Protect the IAM resources you want to be exclusively managed via IAMbic. What is in Git becomes the absolute source of truth.
+- **[GitOps-driven Cloud IAM (IAMOps)](https://docs.iambic.org/reference/iamops_philosophy)**: Leverage GitOps-driven Cloud IAM with human-readable formats and your favorite tools.
 - **Centralized Management**: IAMbic keeps Git updated with the latest, complete state of your cloud environment, maintaining a single source of truth for auditing and compliance across multiple cloud providers in Git.
 - **Extendable**: Integrate with various clouds and applications through a powerful plugin architecture.
 - **Auditable**: Track changes to IAM policies, permissions, and rules with Git history. For AWS, IAmbic annotates out-of-band commits with details from CloudTrail.
 
 ## Getting Started
 
-Dive into IAMbic with our [quick-start guide](http://iambic.org/getting_started/) and explore powerful template examples for AWS Multi-Account Roles, Dynamic Permissions, Okta Applications and Group Assignments, Azure Active Directory Users and Groups, and Google Workspace Group Assignments. We are rapidly expanding support for existing resources and cloud providers, so check back often!
+Dive into IAMbic with our [quick-start guide](http://docs.iambic.org/getting_started/) and explore powerful template examples for AWS Multi-Account Roles, Dynamic Permissions, Okta Applications and Group Assignments, Azure Active Directory Users and Groups, and Google Workspace Group Assignments. We are rapidly expanding support for existing resources and cloud providers, so check back often!
 
 ## Installing IAMbic and Supported Versions
 
 IAMbic is available on PyPI:
 
 ```console
 python -m pip install iambic-core
@@ -92,15 +94,15 @@
 
 Here are some examples showcasing IAMbic's capabilities:
 
 #### AWS Multi-Account Cloudwatch Role
 
 Create a Cloudwatch role with static permissions across three accounts, dynamically generating role names based on the account the role is deployed to. This template would
 result in the creation of three roles: "dev_cloudwatch",
-"staging_cloudwatch", and "prod_cloudwatch" on the respective AWS accounts. See the [Getting Started guide for AWS](https://iambic.org/getting_started/aws) for more information.
+"staging_cloudwatch", and "prod_cloudwatch" on the respective AWS accounts. See the [Getting Started guide for AWS](https://docs.iambic.org/getting_started/aws) for more information.
 
 ```yaml
 template_type: NOQ::AWS::IAM::Role
 identifier: '{{account_name}}_cloudwatch'
 included_accounts:
     - dev
     - staging
@@ -138,15 +140,15 @@
   tags:
     - key: owner
       value: devops
 ```
 
 ### AWS Dynamic Permissions
 
-Create a BackendDeveloperRole with varying permissions based on the AWS account. See the [Getting Started guide for AWS](https://iambic.org/getting_started/aws) for more information.
+Create a BackendDeveloperRole with varying permissions based on the AWS account. See the [Getting Started guide for AWS](https://docs.iambic.org/getting_started/aws) for more information.
 
 ```yaml
 template_type: NOQ::AWS::IAM::Role
 identifier: '{{account_name}}_backend_developer'
 included_accounts:
   - '*'
 excluded_accounts:
@@ -193,15 +195,15 @@
   tags:
     - key: owner
       value: devops
 ```
 
 ### Okta Application Assignments
 
-Manage Okta application assignments, including expiration dates for specific users. See the [Getting Started guide for Okta](https://iambic.org/getting_started/okta) for more information.
+Manage Okta application assignments, including expiration dates for specific users. See the [Getting Started guide for Okta](https://docs.iambic.org/getting_started/okta) for more information.
 
 ```yaml
 template_type: NOQ::Okta::App
 idp_name: development
 properties:
   name: Salesforce.com
   assignments:
@@ -210,15 +212,15 @@
     - user: username3@example.com
       expires_at: 2023-09-01T00:00 UTC
   status: ACTIVE
 ```
 
 ### Okta Group Assignments
 
-Easily manage Okta group assignments with expiration dates for members. See the [Getting Started guide for Okta](https://iambic.org/getting_started/okta) for more information.
+Easily manage Okta group assignments with expiration dates for members. See the [Getting Started guide for Okta](https://docs.iambic.org/getting_started/okta) for more information.
 
 ```yaml
 template_type: NOQ::Okta::Group
 idp_name: main
 properties:
   name: engineering_interns
   description: Engineering Interns
@@ -229,15 +231,15 @@
       expires_at: 2023-09-01
 
 ```
 
 ### Google Group Assignments
 
 Manage Google Workspace group assignments, including temporary access for external users. See the [Getting Started guide for Google
-Workspace](https://iambic.org/getting_started/google) for more information.
+Workspace](https://docs.iambic.org/getting_started/google) for more information.
 
 ```yaml
 template_type: NOQ::GoogleWorkspace::Group
 properties:
   name: DockerHub
   description: Dockerhub Access
   domain: example.com
@@ -248,29 +250,29 @@
     - email: external_user@gmail.com
     - email: some_engineer@example.com
       expires_at: 2023-03-05
 ```
 
 ## Azure Active Directory Users
 
-Manage Azure Active Directory users and their attributes. See the [Getting Started guide for Azure AD](https://iambic.org/getting_started/azure_ad) for more information.
+Manage Azure Active Directory users and their attributes. See the [Getting Started guide for Azure AD](https://docs.iambic.org/getting_started/azure_ad) for more information.
 
 ```yaml
 expires_at: 2025-01-01
 template_type: NOQ::AzureAD::User
 idp_name: development
 properties:
   display_name: Example User
   given_name: Example
   username: user@example.com
 ```
 
 ### Azure Active Directory Groups and Group Assignments
 
-Manage Azure Active Directory groups and group assignments, including temporary access for external users. See the [Getting Started guide for Azure AD](https://iambic.org/getting_started/azure_ad) for more information.
+Manage Azure Active Directory groups and group assignments, including temporary access for external users. See the [Getting Started guide for Azure AD](https://docs.iambic.org/getting_started/azure_ad) for more information.
 
 ```yaml
 template_type: NOQ::AzureAD::Group
 idp_name: development
 properties:
   name: iambic_test_group
   description: A test group to use with IAMbic
@@ -302,9 +304,9 @@
 
 IAMbic is licensed under the Apache-2.0 license. Commercial licenses and support are also available from Noq Software, Inc.
 
 ### Provider Plugins
 
 Provider Plugins (Such as the AWS, Okta, Azure Active Directory, and Google Workspace plugins) are licensed under Apache 2. You are free to write your own provider plugins for internal services without releasing its source code.
 
-For more information, please visit [iambic.org](https://iambic.org/license).
+For more information, please visit [iambic.org](https://docs.iambic.org/license).
```

