# Comparing `tmp/harborapi-0.8.6.tar.gz` & `tmp/harborapi-0.9.0.tar.gz`

## Comparing `harborapi-0.8.6.tar` & `harborapi-0.9.0.tar`

### file list

```diff
@@ -1,157 +1,157 @@
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 harborapi-0.8.6/.coveragerc
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 harborapi-0.8.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 harborapi-0.8.6/CHANGELOG.md
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 harborapi-0.8.6/README.md
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 harborapi-0.8.6/justfile
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 harborapi-0.8.6/mkdocs.yml
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 harborapi-0.8.6/.github/workflows/build.yml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 harborapi-0.8.6/.github/workflows/docs.yml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 harborapi-0.8.6/.github/workflows/project.yml
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 harborapi-0.8.6/.github/workflows/test.yml
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/index.md
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/artifacts.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/auditlogs.md
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/configure.md
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/cveallowlist.md
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/gc.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/health.md
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/index.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/ldap.md
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/oidc.md
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/ping.md
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/projectmetadata.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/projects.md
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/quota.md
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/registries.md
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/replication.md
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/repositories.md
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/robots.md
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/scan.md
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/scanall.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/scanners.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/search.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/statistics.md
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/systeminfo.md
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/usergroups.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/endpoints/users.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/recipes/index.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/recipes/artifacts/artifact-digest.md
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/recipes/artifacts/artifact-vulns.md
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/recipes/artifacts/artifactowner.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/recipes/artifacts/artifactowner.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/recipes/artifacts/conc-artifact.md
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/recipes/repos/conc-repo.md
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/auth.md
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/client.md
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/client_sync.md
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/exceptions.md
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/index.md
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/types.md
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/utils.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/ext/api.md
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/ext/artifact.md
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/ext/cve.md
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/ext/report.md
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/models/_models.md
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/models/_scanner.md
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/models/base.md
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/models/buildhistory.md
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/models/models.md
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/models/oidc.md
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/reference/models/scanner.md
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/async-sync.md
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/authentication.md
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/creating-system-robot.md
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/exceptions.md
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/index.md
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/rich.md
--rw-r--r--   0        0        0     6307 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/validation.md
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/ext/_example_callback.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/ext/_example_get_artifact.py
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/ext/api.md
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/ext/artifact.md
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/ext/index.md
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/ext/report.md
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/methods/create-update.md
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/methods/delete.md
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/methods/examples.md
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/methods/index.md
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 harborapi-0.8.6/docs/usage/methods/read.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/__about__.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/__init__.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/_types.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/auth.py
--rw-r--r--   0        0        0   123644 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/client.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/client_sync.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/py.typed
--rw-r--r--   0        0        0     7672 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/utils.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/version.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/ext/__init__.py
--rw-r--r--   0        0        0    16239 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/ext/api.py
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/ext/artifact.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/ext/cve.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/ext/regex.py
--rw-r--r--   0        0        0    14735 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/ext/report.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/ext/stats.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/models/__init__.py
--rw-r--r--   0        0        0    88258 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/models/_models.py
--rw-r--r--   0        0        0     6651 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/models/_scanner.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/models/_utils.py
--rw-r--r--   0        0        0    10700 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/models/base.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/models/buildhistory.py
--rw-r--r--   0        0        0    16762 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/models/models.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/models/oidc.py
--rw-r--r--   0        0        0    18546 2020-02-02 00:00:00.000000 harborapi-0.8.6/harborapi/models/scanner.py
--rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 harborapi-0.8.6/scripts/bump_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/__init__.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/conftest.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/test_auth.py
--rw-r--r--   0        0        0    20382 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/test_client.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/test_client_sync.py
--rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/test_utils.py
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/test_version.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/__init__.py
--rw-r--r--   0        0        0    10955 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_artifacts.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_audit.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_configure.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_cveallowlist.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_gc.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_health.py
--rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_ldap.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_oidc.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_ping.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_projectmetadata.py
--rw-r--r--   0        0        0     6489 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_projects.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_quota.py
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_registries.py
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_replication.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_repositories.py
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_robots.py
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_scan.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_scanall.py
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_scanners.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_search.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_statistic.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_systeminfo.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_usergroups.py
--rw-r--r--   0        0        0     8321 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/endpoints/test_users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/ext/__init__.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/ext/test_artifact.py
--rw-r--r--   0        0        0     8504 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/ext/test_report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/models/__init__.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/models/test_base.py
--rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/models/test_models.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/models/test_rich.py
--rw-r--r--   0        0        0     6662 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/models/test_scanner.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/models/utils.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/strategies/__init__.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/strategies/artifact.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/strategies/cveallowlist.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/strategies/errors.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 harborapi-0.8.6/tests/strategies/ext.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 harborapi-0.8.6/.gitignore
--rw-r--r--   0        0        0    35120 2020-02-02 00:00:00.000000 harborapi-0.8.6/LICENSE
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 harborapi-0.8.6/pyproject.toml
--rw-r--r--   0        0        0     8332 2020-02-02 00:00:00.000000 harborapi-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 harborapi-0.9.0/.coveragerc
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 harborapi-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 harborapi-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 harborapi-0.9.0/README.md
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 harborapi-0.9.0/justfile
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 harborapi-0.9.0/mkdocs.yml
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 harborapi-0.9.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 harborapi-0.9.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 harborapi-0.9.0/.github/workflows/project.yml
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 harborapi-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/index.md
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/artifacts.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/auditlogs.md
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/configure.md
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/cveallowlist.md
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/gc.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/health.md
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/index.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/ldap.md
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/oidc.md
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/ping.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/projectmetadata.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/projects.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/quota.md
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/registries.md
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/replication.md
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/repositories.md
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/robots.md
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/scan.md
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/scanall.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/scanners.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/search.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/statistics.md
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/systeminfo.md
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/usergroups.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/endpoints/users.md
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/recipes/index.md
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/recipes/artifacts/artifact-digest.md
+-rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/recipes/artifacts/artifact-vulns.md
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/recipes/artifacts/artifactowner.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/recipes/artifacts/artifactowner.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/recipes/artifacts/conc-artifact.md
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/recipes/repos/conc-repo.md
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/auth.md
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/client.md
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/client_sync.md
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/exceptions.md
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/index.md
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/types.md
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/utils.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/ext/api.md
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/ext/artifact.md
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/ext/cve.md
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/ext/report.md
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/models/_models.md
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/models/_scanner.md
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/models/base.md
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/models/buildhistory.md
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/models/models.md
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/models/oidc.md
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/reference/models/scanner.md
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/async-sync.md
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/authentication.md
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/creating-system-robot.md
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/exceptions.md
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/index.md
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/rich.md
+-rw-r--r--   0        0        0     6307 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/validation.md
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/ext/_example_callback.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/ext/_example_get_artifact.py
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/ext/api.md
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/ext/artifact.md
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/ext/index.md
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/ext/report.md
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/methods/create-update.md
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/methods/delete.md
+-rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/methods/examples.md
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/methods/index.md
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 harborapi-0.9.0/docs/usage/methods/read.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/__about__.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/__init__.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/_types.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/auth.py
+-rw-r--r--   0        0        0   123644 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/client.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/client_sync.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/py.typed
+-rw-r--r--   0        0        0     7672 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/utils.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/version.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/ext/__init__.py
+-rw-r--r--   0        0        0    16239 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/ext/api.py
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/ext/artifact.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/ext/cve.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/ext/regex.py
+-rw-r--r--   0        0        0    14735 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/ext/report.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/ext/stats.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/models/__init__.py
+-rw-r--r--   0        0        0    88955 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/models/_models.py
+-rw-r--r--   0        0        0     6651 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/models/_scanner.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/models/_utils.py
+-rw-r--r--   0        0        0    10700 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/models/base.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/models/buildhistory.py
+-rw-r--r--   0        0        0    17003 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/models/models.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/models/oidc.py
+-rw-r--r--   0        0        0    18546 2020-02-02 00:00:00.000000 harborapi-0.9.0/harborapi/models/scanner.py
+-rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 harborapi-0.9.0/scripts/bump_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/test_auth.py
+-rw-r--r--   0        0        0    20382 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/test_client.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/test_client_sync.py
+-rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/test_utils.py
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/test_version.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/__init__.py
+-rw-r--r--   0        0        0    10955 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_artifacts.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_audit.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_configure.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_cveallowlist.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_gc.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_health.py
+-rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_ldap.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_oidc.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_ping.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_projectmetadata.py
+-rw-r--r--   0        0        0     6489 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_projects.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_quota.py
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_registries.py
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_replication.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_repositories.py
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_robots.py
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_scan.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_scanall.py
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_scanners.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_search.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_statistic.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_systeminfo.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_usergroups.py
+-rw-r--r--   0        0        0     8321 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/endpoints/test_users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/ext/__init__.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/ext/test_artifact.py
+-rw-r--r--   0        0        0     8504 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/ext/test_report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/models/__init__.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/models/test_base.py
+-rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/models/test_models.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/models/test_rich.py
+-rw-r--r--   0        0        0     6662 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/models/test_scanner.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/models/utils.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/strategies/__init__.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/strategies/artifact.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/strategies/cveallowlist.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/strategies/errors.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 harborapi-0.9.0/tests/strategies/ext.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 harborapi-0.9.0/.gitignore
+-rw-r--r--   0        0        0    35120 2020-02-02 00:00:00.000000 harborapi-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 harborapi-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 harborapi-0.9.0/PKG-INFO
```

### Comparing `harborapi-0.8.6/.pre-commit-config.yaml` & `harborapi-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/CHANGELOG.md` & `harborapi-0.9.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 The **second number** is the minor version (new features)
 The **third number** is the patch version (bug fixes)
 
 <!-- changelog follows -->
 
 <!-- ## [Unreleased] -->
 
+## [0.9.0](https://github.com/pederhan/harborapi/tree/harborapi-v0.9.0) - 2023-02-21
+
+### Changed
+
+- Updated `harborapi.models` to match the latest version of the Harbor API spec [goharbor/harbor@d03f0dc](https://github.com/goharbor/harbor/blob/99b37117e15ee25e54c4d67f4a9bd14d6df95d5a/api/v2.0/swagger.yaml).
+
+- `harborapi.models.GeneralInfo.with_chartmuseum` has been removed from the API spec, but remains on the model for backwards compatibility. In the future, this field will be removed, as the API will never return this it in sufficiently new versions of Harbor.
+
 ## [0.8.6](https://github.com/pederhan/harborapi/tree/harborapi-v0.8.6) - 2023-02-20
 
 
 ### Fixed
 
 - Models with `harborapi.models.ScheduleObj` fields are now correctly validated when the Harbor API responds with a value of `"Schedule"` for the field `ScheduleObj.type`, which is not a valid value for the enum according to their own spec.
```

### Comparing `harborapi-0.8.6/README.md` & `harborapi-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/justfile` & `harborapi-0.9.0/justfile`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/mkdocs.yml` & `harborapi-0.9.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/.github/workflows/build.yml` & `harborapi-0.9.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/.github/workflows/docs.yml` & `harborapi-0.9.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/.github/workflows/test.yml` & `harborapi-0.9.0/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,16 @@
   push:
     branches:
       - main
     paths-ignore:
       - "docs/**"
       - "*.md"
       - "mkdocs.yml"
+      - ".github/workflows/docs.yml"
+      - ".github/workflows/project.yml"
   pull_request:
     branches:
       - main
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.sha }}
   cancel-in-progress: true
```

### Comparing `harborapi-0.8.6/docs/recipes/index.md` & `harborapi-0.9.0/docs/recipes/index.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/recipes/artifacts/artifact-vulns.md` & `harborapi-0.9.0/docs/recipes/artifacts/artifact-vulns.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/recipes/artifacts/artifactowner.md` & `harborapi-0.9.0/docs/recipes/artifacts/artifactowner.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/recipes/artifacts/artifactowner.py` & `harborapi-0.9.0/docs/recipes/artifacts/artifactowner.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/recipes/artifacts/conc-artifact.md` & `harborapi-0.9.0/docs/recipes/artifacts/conc-artifact.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/recipes/repos/conc-repo.md` & `harborapi-0.9.0/docs/recipes/repos/conc-repo.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/reference/ext/api.md` & `harborapi-0.9.0/docs/reference/ext/api.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/usage/async-sync.md` & `harborapi-0.9.0/docs/usage/async-sync.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/usage/authentication.md` & `harborapi-0.9.0/docs/usage/authentication.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/usage/creating-system-robot.md` & `harborapi-0.9.0/docs/usage/creating-system-robot.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/usage/exceptions.md` & `harborapi-0.9.0/docs/usage/exceptions.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/usage/index.md` & `harborapi-0.9.0/docs/usage/index.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/usage/rich.md` & `harborapi-0.9.0/docs/usage/rich.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/usage/validation.md` & `harborapi-0.9.0/docs/usage/validation.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/usage/ext/_example_callback.py` & `harborapi-0.9.0/docs/usage/ext/_example_callback.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/usage/ext/_example_get_artifact.py` & `harborapi-0.9.0/docs/usage/ext/_example_get_artifact.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/usage/ext/api.md` & `harborapi-0.9.0/docs/usage/ext/api.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/usage/ext/artifact.md` & `harborapi-0.9.0/docs/usage/ext/artifact.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/usage/ext/index.md` & `harborapi-0.9.0/docs/usage/ext/index.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/usage/ext/report.md` & `harborapi-0.9.0/docs/usage/ext/report.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/usage/methods/create-update.md` & `harborapi-0.9.0/docs/usage/methods/create-update.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/usage/methods/examples.md` & `harborapi-0.9.0/docs/usage/methods/examples.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/docs/usage/methods/read.md` & `harborapi-0.9.0/docs/usage/methods/read.md`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/_types.py` & `harborapi-0.9.0/harborapi/_types.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/auth.py` & `harborapi-0.9.0/harborapi/auth.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/client.py` & `harborapi-0.9.0/harborapi/client.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/client_sync.py` & `harborapi-0.9.0/harborapi/client_sync.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/exceptions.py` & `harborapi-0.9.0/harborapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/utils.py` & `harborapi-0.9.0/harborapi/utils.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/version.py` & `harborapi-0.9.0/harborapi/version.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/ext/__init__.py` & `harborapi-0.9.0/harborapi/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/ext/api.py` & `harborapi-0.9.0/harborapi/ext/api.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/ext/artifact.py` & `harborapi-0.9.0/harborapi/ext/artifact.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/ext/cve.py` & `harborapi-0.9.0/harborapi/ext/cve.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/ext/regex.py` & `harborapi-0.9.0/harborapi/ext/regex.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/ext/report.py` & `harborapi-0.9.0/harborapi/ext/report.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/ext/stats.py` & `harborapi-0.9.0/harborapi/ext/stats.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/models/__init__.py` & `harborapi-0.9.0/harborapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/models/_models.py` & `harborapi-0.9.0/harborapi/models/_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  swagger.yaml
-#   timestamp: 2023-02-06T11:49:46+00:00
+#   timestamp: 2023-02-21T13:53:08+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
@@ -1127,14 +1127,18 @@
 
 
 class Configurations(BaseModel):
     auth_mode: Optional[str] = Field(
         None,
         description='The auth mode of current system, such as "db_auth", "ldap_auth", "oidc_auth"',
     )
+    primary_auth_mode: Optional[bool] = Field(
+        None,
+        description="The flag to indicate whether the current auth mode should consider as a primary one.",
+    )
     ldap_base_dn: Optional[str] = Field(
         None, description="The Base DN for LDAP binding."
     )
     ldap_filter: Optional[str] = Field(None, description="The filter for LDAP search")
     ldap_group_base_dn: Optional[str] = Field(
         None, description="The base DN to search LDAP group."
     )
@@ -1276,14 +1280,17 @@
     )
     skip_audit_log_database: Optional[bool] = Field(
         None, description="Skip audit log database"
     )
     session_timeout: Optional[int] = Field(
         None, description="The session timeout for harbor, in minutes."
     )
+    scanner_skip_update_pulltime: Optional[bool] = Field(
+        None, description="Whether or not to skip update pull time for scanner"
+    )
 
 
 class StringConfigItem(BaseModel):
     value: Optional[str] = Field(
         None, description="The string value of current config item"
     )
     editable: Optional[bool] = Field(
@@ -1744,27 +1751,28 @@
 class GeneralInfo(BaseModel):
     current_time: Optional[datetime] = Field(
         None, description="The current time of the server."
     )
     with_notary: Optional[bool] = Field(
         None, description="If the Harbor instance is deployed with nested notary."
     )
-    with_chartmuseum: Optional[bool] = Field(
-        None, description="If the Harbor instance is deployed with nested chartmuseum."
-    )
     registry_url: Optional[str] = Field(
         None,
         description="The url of registry against which the docker command should be issued.",
     )
     external_url: Optional[str] = Field(
         None, description="The external URL of Harbor, with protocol."
     )
     auth_mode: Optional[str] = Field(
         None, description="The auth mode of current Harbor instance."
     )
+    primary_auth_mode: Optional[bool] = Field(
+        None,
+        description="The flag to indicate whether the current auth mode should consider as a primary one.",
+    )
     project_creation_restriction: Optional[str] = Field(
         None,
         description="Indicate who can create projects, it could be 'adminonly' or 'everyone'.",
     )
     self_registration: Optional[bool] = Field(
         None,
         description="Indicate whether the Harbor instance enable user to register himself.",
@@ -1880,14 +1888,18 @@
 
 
 class ConfigurationsResponse(BaseModel):
     auth_mode: Optional[StringConfigItem] = Field(
         None,
         description='The auth mode of current system, such as "db_auth", "ldap_auth", "oidc_auth"',
     )
+    primary_auth_mode: Optional[BoolConfigItem] = Field(
+        None,
+        description="The flag to indicate whether the current auth mode should consider as a primary one.",
+    )
     ldap_base_dn: Optional[StringConfigItem] = Field(
         None, description="The Base DN for LDAP binding."
     )
     ldap_filter: Optional[StringConfigItem] = Field(
         None, description="The filter for LDAP search"
     )
     ldap_group_base_dn: Optional[StringConfigItem] = Field(
@@ -2032,14 +2044,17 @@
     )
     audit_log_forward_endpoint: Optional[StringConfigItem] = Field(
         None, description="The endpoint of the audit log forwarder"
     )
     skip_audit_log_database: Optional[BoolConfigItem] = Field(
         None, description="Whether skip the audit log in database"
     )
+    scanner_skip_update_pulltime: Optional[BoolConfigItem] = Field(
+        None, description="Whether or not to skip update the pull time for scanner"
+    )
     scan_all_policy: Optional[ScanAllPolicy] = None
     session_timeout: Optional[IntegerConfigItem] = Field(
         None, description="The session timeout in minutes"
     )
 
 
 class ProjectMember(BaseModel):
```

### Comparing `harborapi-0.8.6/harborapi/models/_scanner.py` & `harborapi-0.9.0/harborapi/models/_scanner.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/models/_utils.py` & `harborapi-0.9.0/harborapi/models/_utils.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/models/base.py` & `harborapi-0.9.0/harborapi/models/base.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/harborapi/models/models.py` & `harborapi-0.9.0/harborapi/models/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
     Error,
     Errors,
     EventType,
 )
 from ._models import ExecHistory as _ExecHistory
 from ._models import Execution, ExtraAttrs, FilterStyle
 from ._models import GCHistory as _GCHistory
+from ._models import GeneralInfo as _GeneralInfo
 from ._models import (
-    GeneralInfo,
     Icon,
     ImmutableRule,
     ImmutableSelector,
     Instance,
     IntegerConfigItem,
     InternalConfigurationsResponse,
     InternalConfigurationValue,
@@ -601,7 +601,15 @@
 
 class ExecHistory(_ExecHistory):
     schedule: Optional[ScheduleObj] = optional_field(_ExecHistory, "schedule")  # type: ignore
 
 
 class Schedule(_Schedule):
     schedule: Optional[ScheduleObj] = optional_field(_Schedule, "schedule")  # type: ignore
+
+
+class GeneralInfo(_GeneralInfo):
+    with_chartmuseum: Optional[bool] = Field(
+        None,
+        description="If the Harbor instance is deployed with nested chartmuseum.",
+        deprecated=True,
+    )
```

### Comparing `harborapi-0.8.6/harborapi/models/scanner.py` & `harborapi-0.9.0/harborapi/models/scanner.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/scripts/bump_version.py` & `harborapi-0.9.0/scripts/bump_version.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/conftest.py` & `harborapi-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/test_auth.py` & `harborapi-0.9.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/test_client.py` & `harborapi-0.9.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/test_client_sync.py` & `harborapi-0.9.0/tests/test_client_sync.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/test_utils.py` & `harborapi-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/test_version.py` & `harborapi-0.9.0/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_artifacts.py` & `harborapi-0.9.0/tests/endpoints/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_audit.py` & `harborapi-0.9.0/tests/endpoints/test_audit.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_configure.py` & `harborapi-0.9.0/tests/endpoints/test_configure.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_cveallowlist.py` & `harborapi-0.9.0/tests/endpoints/test_cveallowlist.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_gc.py` & `harborapi-0.9.0/tests/endpoints/test_gc.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_health.py` & `harborapi-0.9.0/tests/endpoints/test_health.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_ldap.py` & `harborapi-0.9.0/tests/endpoints/test_ldap.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_oidc.py` & `harborapi-0.9.0/tests/endpoints/test_oidc.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_projectmetadata.py` & `harborapi-0.9.0/tests/endpoints/test_projectmetadata.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_projects.py` & `harborapi-0.9.0/tests/endpoints/test_projects.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_quota.py` & `harborapi-0.9.0/tests/endpoints/test_quota.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_registries.py` & `harborapi-0.9.0/tests/endpoints/test_registries.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_replication.py` & `harborapi-0.9.0/tests/endpoints/test_replication.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_repositories.py` & `harborapi-0.9.0/tests/endpoints/test_repositories.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_robots.py` & `harborapi-0.9.0/tests/endpoints/test_robots.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_scan.py` & `harborapi-0.9.0/tests/endpoints/test_scan.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_scanall.py` & `harborapi-0.9.0/tests/endpoints/test_scanall.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_scanners.py` & `harborapi-0.9.0/tests/endpoints/test_scanners.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_search.py` & `harborapi-0.9.0/tests/endpoints/test_search.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_statistic.py` & `harborapi-0.9.0/tests/endpoints/test_statistic.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_systeminfo.py` & `harborapi-0.9.0/tests/endpoints/test_systeminfo.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_usergroups.py` & `harborapi-0.9.0/tests/endpoints/test_usergroups.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/endpoints/test_users.py` & `harborapi-0.9.0/tests/endpoints/test_users.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/ext/test_artifact.py` & `harborapi-0.9.0/tests/ext/test_artifact.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/ext/test_report.py` & `harborapi-0.9.0/tests/ext/test_report.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/models/test_base.py` & `harborapi-0.9.0/tests/models/test_base.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/models/test_models.py` & `harborapi-0.9.0/tests/models/test_models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 import pytest
-from hypothesis import given
+from hypothesis import assume, given
 from hypothesis import strategies as st
 from pydantic import ValidationError
 
 from harborapi.models._models import ChartMetadata as ChartMetadataGenerated
 from harborapi.models._models import ChartVersion as ChartVersionGenerated
 from harborapi.models._models import ReplicationFilter as ReplicationFilterGenerated
 from harborapi.models._models import Search as SearchGenerated
 from harborapi.models._models import SearchResult as SearchResultGenerated
 from harborapi.models.models import (
     Artifact,
     ChartMetadata,
     ChartVersion,
+    ExecHistory,
+    GCHistory,
     LdapConf,
     NativeReportSummary,
     ReplicationFilter,
     Repository,
+    Schedule,
+    ScheduleObj,
     Search,
     SearchResult,
+    Type,
     VulnerabilitySummary,
 )
 from harborapi.models.scanner import Severity
 
 from .utils import (
     _no_references_check,
     _override_class_check,
@@ -206,7 +211,50 @@
     st.builds(
         NativeReportSummary, severity=st.sampled_from([s.value for s in Severity])
     )
 )
 def test_nativereportsummary_severity_enum(report: NativeReportSummary) -> None:
     """Test that the severity enum is correctly parsed from the string"""
     assert isinstance(report.severity_enum, Severity) or report.severity is None
+
+
+# Strategy for testing the overriden ScheduleObj model and the models that
+# reference it
+schedule_enum_values = list(
+    set([s.value for s in Type] + ["Schedule"])
+)  # explicitly make sure "Schedule" is included
+
+
+type_strategy = st.sampled_from(schedule_enum_values)
+schedule_strategy = st.builds(ScheduleObj, type=type_strategy)
+
+
+@given(schedule_strategy)
+def test_scheduleobj_override(schedule: ScheduleObj) -> None:
+    """Test the overriding of the ScheduleObj model"""
+    assert isinstance(schedule.type, Type)
+    assume(schedule.type == Type.schedule)
+    assert schedule.type == Type.schedule
+
+
+@given(st.builds(GCHistory, schedule=schedule_strategy))
+def test_gchistory_override(history: GCHistory) -> None:
+    """Test the overriding of the GCHistory model"""
+    assert isinstance(history.schedule.type, Type)
+    assume(history.schedule.type == Type.schedule)
+    assert history.schedule.type == Type.schedule
+
+
+@given(st.builds(ExecHistory, schedule=schedule_strategy))
+def test_exechistory_override(history: ExecHistory) -> None:
+    """Test the overriding of the ExecHistory model"""
+    assert isinstance(history.schedule.type, Type)
+    assume(history.schedule.type == Type.schedule)
+    assert history.schedule.type == Type.schedule
+
+
+@given(st.builds(Schedule, schedule=schedule_strategy))
+def test_schedule_override(history: Schedule) -> None:
+    """Test the overriding of the Schedule model"""
+    assert isinstance(history.schedule.type, Type)
+    assume(history.schedule.type == Type.schedule)
+    assert history.schedule.type == Type.schedule
```

### Comparing `harborapi-0.8.6/tests/models/test_rich.py` & `harborapi-0.9.0/tests/models/test_rich.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/models/test_scanner.py` & `harborapi-0.9.0/tests/models/test_scanner.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/models/utils.py` & `harborapi-0.9.0/tests/models/utils.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/strategies/artifact.py` & `harborapi-0.9.0/tests/strategies/artifact.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/strategies/cveallowlist.py` & `harborapi-0.9.0/tests/strategies/cveallowlist.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/tests/strategies/ext.py` & `harborapi-0.9.0/tests/strategies/ext.py`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/LICENSE` & `harborapi-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/pyproject.toml` & `harborapi-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `harborapi-0.8.6/PKG-INFO` & `harborapi-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harborapi
-Version: 0.8.6
+Version: 0.9.0
 Summary: Async Harbor API v2.0 client
 Project-URL: Source, https://github.com/pederhan/harborapi
 Project-URL: Documentation, https://pederhan.github.io/harborapi/
 Project-URL: Changelog, https://github.com/pederhan/harborapi/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/pederhan/harborapi/issues
 Author-email: pederhan <pederhan@uio.no>
 License-Expression: MIT
@@ -127,14 +127,22 @@
 - [ ] robotv1
 - [x] projectMetadata
 - [x] auditlog
 
 \*\* `/systeminfo/getcert` NYI
 <!-- ## [Unreleased] -->
 
+## [0.9.0](https://github.com/pederhan/harborapi/tree/harborapi-v0.9.0) - 2023-02-21
+
+### Changed
+
+- Updated `harborapi.models` to match the latest version of the Harbor API spec [goharbor/harbor@d03f0dc](https://github.com/goharbor/harbor/blob/99b37117e15ee25e54c4d67f4a9bd14d6df95d5a/api/v2.0/swagger.yaml).
+
+- `harborapi.models.GeneralInfo.with_chartmuseum` has been removed from the API spec, but remains on the model for backwards compatibility. In the future, this field will be removed, as the API will never return this it in sufficiently new versions of Harbor.
+
 ## [0.8.6](https://github.com/pederhan/harborapi/tree/harborapi-v0.8.6) - 2023-02-20
 
 
 ### Fixed
 
 - Models with `harborapi.models.ScheduleObj` fields are now correctly validated when the Harbor API responds with a value of `"Schedule"` for the field `ScheduleObj.type`, which is not a valid value for the enum according to their own spec.
```

