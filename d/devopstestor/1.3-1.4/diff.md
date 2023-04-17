# Comparing `tmp/devopstestor-1.3.tar.gz` & `tmp/devopstestor-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopstestor-1.3.tar", last modified: Wed Mar  8 10:06:49 2023, max compression
+gzip compressed data, was "devopstestor-1.4.tar", last modified: Mon Apr 17 12:51:36 2023, max compression
```

## Comparing `devopstestor-1.3.tar` & `devopstestor-1.4.tar`

### file list

```diff
@@ -1,124 +1,125 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.030800 devopstestor-1.3/
--rw-rw-rw-   0 root         (0) root         (0)    22958 2023-03-08 10:06:36.000000 devopstestor-1.3/LICENCE
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-03-08 10:06:36.000000 devopstestor-1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      706 2023-03-08 10:06:49.030800 devopstestor-1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-03-08 10:06:36.000000 devopstestor-1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:48.995797 devopstestor-1.3/devopstestor/
--rw-rw-rw-   0 root         (0) root         (0)      430 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.001797 devopstestor-1.3/devopstestor/config/
--rw-rw-rw-   0 root         (0) root         (0)     2837 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/config/arguments.yml
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/config/core.yml
--rw-rw-rw-   0 root         (0) root         (0)      778 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/config/machine.yml
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/config/provisionner.yml
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/config/report.yml
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/config/source_manager.yml
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/config/testcase.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.002797 devopstestor-1.3/devopstestor/src/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.003797 devopstestor-1.3/devopstestor/src/abstract/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/abstract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5114 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/abstract/abstract_machine_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/abstract/abstract_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     3353 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/abstract/abstract_report.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/abstract/abstract_source_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.007798 devopstestor-1.3/devopstestor/src/core/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5804 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/core/devopstestor.py
--rw-rw-rw-   0 root         (0) root         (0)     1469 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/core/devopstestor_client.py
--rw-rw-rw-   0 root         (0) root         (0)     2228 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/core/devopstestor_server.py
--rw-rw-rw-   0 root         (0) root         (0)     7926 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/core/global_config_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8219 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/core/machines_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     4851 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/core/ordonnanceur.py
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/core/report_render_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2083 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/core/source_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/core/testcase_executor_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.009798 devopstestor-1.3/devopstestor/src/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2808 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/lib/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/lib/core_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/lib/json_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2719 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/lib/log_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    11155 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/lib/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.011798 devopstestor-1.3/devopstestor/src/machine/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/machine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2093 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/machine/debug_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     7533 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/machine/docker_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     3534 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/machine/local_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.012798 devopstestor-1.3/devopstestor/src/provisionner/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/provisionner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/provisionner/empty_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     4850 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/provisionner/logstash_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     8768 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/provisionner/minion_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/provisionner/systemd_provisionner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.015798 devopstestor-1.3/devopstestor/src/reporting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/reporting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/reporting/campaign_report.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/reporting/deployment_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5666 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/reporting/report_elk_renderer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.016799 devopstestor-1.3/devopstestor/src/reporting/report_html_renderer/
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/reporting/report_html_renderer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9223 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja
--rw-rw-rw-   0 root         (0) root         (0)     7258 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/reporting/report_text_renderer.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/reporting/scenario_report.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/reporting/testcase_report.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/reporting/verifier_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.018799 devopstestor-1.3/devopstestor/src/scenarios/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/scenarios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/scenarios/devopstestor.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/scenarios/logstash.py
--rw-rw-rw-   0 root         (0) root         (0)     6385 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/scenarios/mock_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/scenarios/systemd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.020799 devopstestor-1.3/devopstestor/src/sources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2604 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/sources/copytemplate_source_accessor.py
--rw-rw-rw-   0 root         (0) root         (0)     2334 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/sources/dirlink_source_accessor.py
--rw-rw-rw-   0 root         (0) root         (0)     2587 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/sources/git_source_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.022799 devopstestor-1.3/devopstestor/src/testcase/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/testcase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8757 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/testcase/scenario_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     6314 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/testcase/test_case.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/testcase/testcase_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     3114 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/src/testcase/tests_cases_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:48.989796 devopstestor-1.3/devopstestor/testconf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:48.993796 devopstestor-1.3/devopstestor/testconf/verifiers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.024799 devopstestor-1.3/devopstestor/testconf/verifiers/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/fixtures/context_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/fixtures/logstash_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.024799 devopstestor-1.3/devopstestor/testconf/verifiers/service/
--rw-rw-rw-   0 root         (0) root         (0)     4529 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/service/http_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.024799 devopstestor-1.3/devopstestor/testconf/verifiers/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.025800 devopstestor-1.3/devopstestor/testconf/verifiers/tests/http_logger/
--rw-rw-rw-   0 root         (0) root         (0)     1317 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.025800 devopstestor-1.3/devopstestor/testconf/verifiers/tests/logstash/
--rw-rw-rw-   0 root         (0) root         (0)     5411 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/tests/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.026800 devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.027800 devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/filesystem/
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.027800 devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/packages/
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.028800 devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/systemd/
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py
--rw-rw-rw-   0 root         (0) root         (0)     2256 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py
--rw-rw-rw-   0 root         (0) root         (0)     3336 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.028800 devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/users/
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.029800 devopstestor-1.3/devopstestor/testconf/verifiers/utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:49.030800 devopstestor-1.3/devopstestor/testconf/verifiers/utils/logstash/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/utils/logstash/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6214 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py
--rw-rw-rw-   0 root         (0) root         (0)     4964 2023-03-08 10:06:36.000000 devopstestor-1.3/devopstestor/testconf/verifiers/utils/verififier_luncher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 10:06:48.997797 devopstestor-1.3/devopstestor.egg-info/
--rw-r--r--   0 root         (0) root         (0)      706 2023-03-08 10:06:48.000000 devopstestor-1.3/devopstestor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4325 2023-03-08 10:06:48.000000 devopstestor-1.3/devopstestor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-08 10:06:48.000000 devopstestor-1.3/devopstestor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-03-08 10:06:48.000000 devopstestor-1.3/devopstestor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-08 10:06:48.000000 devopstestor-1.3/devopstestor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-08 10:06:49.030800 devopstestor-1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-03-08 10:06:36.000000 devopstestor-1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.171841 devopstestor-1.4/
+-rw-rw-rw-   0 root         (0) root         (0)    22958 2023-04-17 12:51:22.000000 devopstestor-1.4/LICENCE
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-04-17 12:51:22.000000 devopstestor-1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      706 2023-04-17 12:51:36.170841 devopstestor-1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-04-17 12:51:22.000000 devopstestor-1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.138838 devopstestor-1.4/devopstestor/
+-rw-rw-rw-   0 root         (0) root         (0)      430 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.143839 devopstestor-1.4/devopstestor/config/
+-rw-rw-rw-   0 root         (0) root         (0)     2837 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/config/arguments.yml
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/config/core.yml
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/config/machine.yml
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/config/provisionner.yml
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/config/report.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/config/source_manager.yml
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/config/testcase.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.143839 devopstestor-1.4/devopstestor/src/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.145839 devopstestor-1.4/devopstestor/src/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/abstract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5424 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/abstract/abstract_machine_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/abstract/abstract_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3498 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/abstract/abstract_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/abstract/abstract_source_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.148839 devopstestor-1.4/devopstestor/src/core/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5805 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/devopstestor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/devopstestor_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2228 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/devopstestor_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     7926 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/global_config_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8219 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/machines_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4851 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/ordonnanceur.py
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/report_render_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2083 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/source_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/core/testcase_executor_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.150839 devopstestor-1.4/devopstestor/src/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2808 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/lib/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/lib/core_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/lib/json_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/lib/log_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    11155 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/lib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.152839 devopstestor-1.4/devopstestor/src/machine/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/machine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/machine/debug_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     7573 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/machine/docker_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     3754 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/machine/local_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     7547 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/machine/vagrant_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.154839 devopstestor-1.4/devopstestor/src/provisionner/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/provisionner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/provisionner/empty_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/provisionner/logstash_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     8768 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/provisionner/minion_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/provisionner/systemd_provisionner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.157840 devopstestor-1.4/devopstestor/src/reporting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/campaign_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/deployment_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5666 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/report_elk_renderer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.158840 devopstestor-1.4/devopstestor/src/reporting/report_html_renderer/
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/report_html_renderer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9223 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja
+-rw-rw-rw-   0 root         (0) root         (0)     7258 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/report_text_renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/scenario_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/testcase_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/reporting/verifier_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.160840 devopstestor-1.4/devopstestor/src/scenarios/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/scenarios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/scenarios/devopstestor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/scenarios/logstash.py
+-rw-rw-rw-   0 root         (0) root         (0)     6385 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/scenarios/mock_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/scenarios/systemd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.161840 devopstestor-1.4/devopstestor/src/sources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2604 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/sources/copytemplate_source_accessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/sources/dirlink_source_accessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2587 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/sources/git_source_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.163840 devopstestor-1.4/devopstestor/src/testcase/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/testcase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8757 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/testcase/scenario_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6314 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/testcase/test_case.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/testcase/testcase_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3114 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/src/testcase/tests_cases_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.133838 devopstestor-1.4/devopstestor/testconf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.136838 devopstestor-1.4/devopstestor/testconf/verifiers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.164840 devopstestor-1.4/devopstestor/testconf/verifiers/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/fixtures/context_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/fixtures/logstash_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.165840 devopstestor-1.4/devopstestor/testconf/verifiers/service/
+-rw-rw-rw-   0 root         (0) root         (0)     4529 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/service/http_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.165840 devopstestor-1.4/devopstestor/testconf/verifiers/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.165840 devopstestor-1.4/devopstestor/testconf/verifiers/tests/http_logger/
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.166840 devopstestor-1.4/devopstestor/testconf/verifiers/tests/logstash/
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.167840 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.168841 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/filesystem/
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.168841 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/packages/
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.169840 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/systemd/
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py
+-rw-rw-rw-   0 root         (0) root         (0)     3336 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.169840 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/users/
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.169840 devopstestor-1.4/devopstestor/testconf/verifiers/utils/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.170841 devopstestor-1.4/devopstestor/testconf/verifiers/utils/logstash/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/utils/logstash/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6214 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4964 2023-04-17 12:51:22.000000 devopstestor-1.4/devopstestor/testconf/verifiers/utils/verififier_luncher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:51:36.140838 devopstestor-1.4/devopstestor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      706 2023-04-17 12:51:36.000000 devopstestor-1.4/devopstestor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-04-17 12:51:36.000000 devopstestor-1.4/devopstestor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 12:51:36.000000 devopstestor-1.4/devopstestor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-04-17 12:51:36.000000 devopstestor-1.4/devopstestor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 12:51:36.000000 devopstestor-1.4/devopstestor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 12:51:36.171841 devopstestor-1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2023-04-17 12:51:22.000000 devopstestor-1.4/setup.py
```

### Comparing `devopstestor-1.3/LICENCE` & `devopstestor-1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/PKG-INFO` & `devopstestor-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopstestor
-Version: 1.3
+Version: 1.4
 Summary: Framwork to auto test machine provisioning
 Home-page: https://gitlab.com/alexis.porzier.pro/devopstestor
 Author: Alexis PORZIER
 Author-email: alexis.porzier.pro@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `devopstestor-1.3/devopstestor/config/arguments.yml` & `devopstestor-1.4/devopstestor/config/arguments.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/config/machine.yml` & `devopstestor-1.4/devopstestor/config/machine.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/config/report.yml` & `devopstestor-1.4/devopstestor/config/report.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/config/source_manager.yml` & `devopstestor-1.4/devopstestor/config/source_manager.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 
   # Montage des verifiers du noyeau sur les machines (obligatoire)
   devopstestor_verifiers:
     accessor_type: DirlinkSourceAccessor
     readonly: True
     path:
       local: "$(this::lib_path)/testconf/verifiers"
-      machine: /srv/verifiers/generic
+      machine: /srv/verifiers/generic/
   # Montage des verifiers utilisateur sur les machines
   client_verifiers:
     accessor_type: DirlinkSourceAccessor
     readonly: True
     path:
       local: "$(this::client_path)/testconf/verifiers"
-      machine: /srv/verifiers/custom
+      machine: /srv/verifiers/custom/
   # Montage de la lib devopstestor vers la machine
   devopstestor_lib:
     accessor_type: DirlinkSourceAccessor
     readonly: True
     path:
-      local: "$(this::lib_path)"
+      local: "$(this::lib_path)/"
       machine: /usr/local/lib/python3.9/dist-packages/devopstestor
```

### Comparing `devopstestor-1.3/devopstestor/config/testcase.yml` & `devopstestor-1.4/devopstestor/config/testcase.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/abstract/abstract_machine_controller.py` & `devopstestor-1.4/devopstestor/src/abstract/abstract_machine_controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,64 @@
+from source_manager import SourceManager
+from config import Config
 class AbstractMachineController(object):
     """
         Classe abstraite d'un controlleur de machine
         Chaque implementation doit heriter de cette class
     """
 
     @staticmethod
-    def pre_initialize(global_config, machine_configuration, source_manager):
+    def pre_initialize(global_config:Config, machine_configuration:Config, source_manager:SourceManager):
         """
         Lorsque c'est necessaire
         permet d'initialise les pre-requis a la construction d'une machine
         """
         pass
 
-    def is_aldready_exists(self, machine_configuration, machine_name):
+    def is_aldready_exists(self, machine_configuration:Config, machine_name:str) -> bool:
         """
         Retoure True si la machine est deja existante
         """
         return False
 
-    def create_machine(self, global_config, machine_configuration, machine_name, source_manager):
+    def create_machine(self, global_config:Config, machine_configuration:Config, machine_name:str, source_manager:SourceManager):
         """
         Initialise la machine
         A surcharger si necessaire
         """
         pass
 
-    def resume_machine(self, global_config, machine_configuration, machine_name, source_manager):
+    def resume_machine(self, global_config:Config, machine_configuration:Config, machine_name:str, source_manager:SourceManager):
         """
         Se connecte a une machine existante
         A surcharger si necessaire
         """
         pass
 
 
-    def run_cmd(self, command):
+    def run_cmd(self, command:str) -> int:
         """
         Permet de lancer une commande sur la machine
         A surcharger
         """
         pass
 
-    def run_python(self, script):
+    def run_python(self, script:str) -> int:
         """
         Permet de lancer une commande python sur la machine
         en fonction de l'environement
         """
         return self.run_cmd(
             command="{} {}".format(
                 self.global_config.get('machine::env::pythonpath'),
                 script
             )
         )
 
-    def append_in_file(self, content, file_path):
+    def append_in_file(self, content:str, file_path:str) -> int:
         """
         Permet d'ajouter du contenu dans un fichier sur la machine
         :param content: Contenu a copier
         :param file_path: nom du fichier
         :return: code retour
         A surcharger
         """
@@ -64,42 +66,42 @@
         res, oldcontent = self.get_file_content(file_path=file_path)
         if res == 0:
             newcontent = "{}\n{}".format(oldcontent, content) if res is not False else content
         else:
             newcontent = content
         return self.put_in_file(newcontent, file_path)
 
-    def put_in_file(self, content, file_path):
+    def put_in_file(self, content:str, file_path:str) -> int:
         """
         Permet de copier du contenu dans un fichier sur la machine
         :param content: Contenu a copier
         :param file_path: nom du fichier
         :return: code retour
         A surcharger
         """
         pass
 
-    def get_file_content(self, file_path):
+    def get_file_content(self, file_path:str) -> str:
         """
         Permet de recuperer le contenu d'un fichier sur la machine
         :param file_path: Chemin vers le fichier
         :return: contenu du fichier (string)
         A surcharger
         """
         pass
 
-    def destroy_machine(self, global_config, machine_configuration, machine_name, source_manager):
+    def destroy_machine(self, global_config:Config, machine_configuration:Config, machine_name:str, source_manager:SourceManager):
         """
         Liberation de la machine
         A surcharger
         """
         pass
 
 
-    def __init__(self, global_config, machine_configuration, machine_name, source_manager, machine_preset_name):
+    def __init__(self, global_config:Config, machine_configuration:Config, machine_name:str, source_manager:SourceManager, machine_preset_name:str):
         """
         A ne pas surcharger
         Ordonnance la construction de la machine
         """
         self.global_config = global_config
         self.machine_name = machine_name
         self.source_manager = source_manager
@@ -120,15 +122,15 @@
             self.create_machine(
                 global_config=self.global_config,
                 machine_configuration=self.machine_configuration,
                 machine_name=self.machine_name,
                 source_manager=self.source_manager
             )
 
-        # Recuperation des variables d'environement si existantes
+        # Recuperation des variables d'environnement si existantes
         # Ces variables permettent de configurer les testauto en fonction de la machine
         ret, env_values = self.run_cmd("env")
         if ret == 0 and env_values != "":
             env_config = global_config.get_node('machine').get_node('env').config
             for v in env_values.split('\n'):
                 if 'devopstestor_' in v:
                     tmp = v.split('=')
```

### Comparing `devopstestor-1.3/devopstestor/src/abstract/abstract_provisionner.py` & `devopstestor-1.4/devopstestor/src/abstract/abstract_provisionner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,45 @@
+from abstract_machine_controller import AbstractMachineController
+from config import Config
+
 class AbstractProvisionner(object):
     """
     Classe abstraite des provisionners
     Un provisonner permet de controller une machine a travers un outils de deploiement (ex saltstack, ansible)
     """
-    def initialise(self, machine_controller, machine_name):
+    def initialise(self, machine_controller:AbstractMachineController, machine_name:str):
         """
         Initialise le provisioner
         A surcharger si necessaire
         """
         pass
 
 
-    def get_machine_controller(self):
+    def get_machine_controller(self) -> AbstractMachineController:
         """
         A ne pas surcharger
         Retourne le chemin conduisant aux fichiers sur la machine
         """
         return self.machine_controller
 
-    def __init__(self, global_config, machine_controller, machine_name):
+    def __init__(self, global_config:Config, machine_controller:AbstractMachineController, machine_name:str):
         """
         A ne pas surcharger
         Ordonnance l'Initialisation du provisionner
         """
         self.machine_controller = machine_controller
         self.global_config = global_config
 
         # Initialisation du provisioner
         self.initialise(
             machine_controller=machine_controller,
             machine_name=machine_name
         )
 
     ## Parametrage utils ###
-    def set_max_map_count(self, max_map_count, name="testauto"):
+    def set_max_map_count(self, max_map_count:int, name:str="testauto") -> tuple:
         # Set vm_max_map_count
         ret, out = self.machine_controller.run_cmd("sysctl -w vm.max_map_count={}".format(max_map_count))
         if ret != 0:
             return False, out
         ret, out = self.machine_controller.append_in_file(content="vm.max_map_count={}".format(max_map_count), file_path="/etc/sysctl.d/{}.conf".format(name))
         return True, out
```

### Comparing `devopstestor-1.3/devopstestor/src/abstract/abstract_report.py` & `devopstestor-1.4/devopstestor/src/abstract/abstract_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import datetime
+class AbstractReport(object): # Premiere definition pour initialiser le type
+    pass
 class AbstractReport(object):
     """
     Rapport de la campagne de test
     """
     # 1 - Initialisation du rapport
 
-    def __init__(self, elem_name):
+    def __init__(self, elem_name:str):
         """
         Initialise le rapport
 
         :param elem_name: Nom de l'element
         """
         self.elem_name = elem_name
         self.is_running = True
@@ -18,37 +20,37 @@
         self.nb_children_ok = -1
         self.nb_children_ko = -1
         self.result = None
         self.result = None
         self.datetime = datetime.datetime.now()
         self.stdout = ""
 
-    def add_child_to_list(self, name, child):
+    def add_child_to_list(self, name:str, child:AbstractReport):
         """
         Ajoute un sous element
 
         :param name: Nom de la list d'elements
         :param child: Rapport fils a ajouter
         """
         self.__check_is_running()
         if not name in self.children_list:
             self.children_list[name] = []
         self.children_list[name].append(child)
 
-    def get_child_list(self, name):
+    def get_child_list(self, name:str) -> dict:
         """
         Recupere un sous element
         :param name: Nom de la list d'elements
         :return: La list d'element
         """
         return self.children_list.get(name, [])
 
     # 2 - Calcul du resultat
 
-    def set_node_result(self, result, stdout):
+    def set_node_result(self, result:bool, stdout:str):
         """
         Methode 1 : Definit les resultats du noeud (cas feuille)
         """
         self.__compute_duree()
         self.__check_is_running()
         self.is_running = False
         self.result = result
@@ -74,22 +76,22 @@
                 self.nb_children += 1
                 result = child_res and result
         self.result = result
         self.is_running = False
 
     # 3 - Recuperation du resultat
 
-    def get_result(self):
+    def get_result(self) -> bool:
         """
         Recupere le resultat du noeud
         """
         self.__check_is_teminated()
         return self.result
 
-    def get_node_stdout(self):
+    def get_node_stdout(self) -> str:
         """
         Retourne le resultat de la sortie standard
         """
         self.__check_is_teminated()
         return self.stdout
 
     ##### Private methodes #####
```

### Comparing `devopstestor-1.3/devopstestor/src/abstract/abstract_source_accessor.py` & `devopstestor-1.4/devopstestor/src/abstract/abstract_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/core/devopstestor.py` & `devopstestor-1.4/devopstestor/src/core/devopstestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
        # Add lib to machine
        self.source_manager.add_source_accessor(
            name="devopstestor",
            source_config={
                "accessor_type": "DirlinkSourceAccessor",
                "path":{
                  "local": self.lib_path + "/src/",
-                 "machine": '/usr/lib/python3.6/site-packages/devopstestor'
+                 "machine": '/usr/lib/python3.6/site-packages/devopstestor/'
                }
            }
        )
 
    def __load_test_cases(self):
        """
        Recherche et met en memoire les configurations relatives aux testcase
```

### Comparing `devopstestor-1.3/devopstestor/src/core/devopstestor_client.py` & `devopstestor-1.4/devopstestor/src/core/devopstestor_client.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/core/devopstestor_server.py` & `devopstestor-1.4/devopstestor/src/core/devopstestor_server.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/core/global_config_factory.py` & `devopstestor-1.4/devopstestor/src/core/global_config_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/core/machines_factory.py` & `devopstestor-1.4/devopstestor/src/core/machines_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/core/ordonnanceur.py` & `devopstestor-1.4/devopstestor/src/core/ordonnanceur.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/core/report_render_manager.py` & `devopstestor-1.4/devopstestor/src/core/report_render_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/core/source_manager.py` & `devopstestor-1.4/devopstestor/src/core/source_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/core/testcase_executor_factory.py` & `devopstestor-1.4/devopstestor/src/core/testcase_executor_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/lib/config.py` & `devopstestor-1.4/devopstestor/src/lib/config.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/lib/core_utils.py` & `devopstestor-1.4/devopstestor/src/lib/core_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/lib/json_utils.py` & `devopstestor-1.4/devopstestor/src/lib/json_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/lib/log_manager.py` & `devopstestor-1.4/devopstestor/src/lib/log_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/lib/utils.py` & `devopstestor-1.4/devopstestor/src/lib/utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/machine/debug_controller.py` & `devopstestor-1.4/devopstestor/src/machine/debug_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/machine/docker_controller.py` & `devopstestor-1.4/devopstestor/src/machine/docker_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+from source_manager import SourceManager
 import docker
 import os
 import shutil
 import random
 from core_utils import get_global_path
 from abstract_machine_controller import AbstractMachineController
 from log_manager import logging
```

### Comparing `devopstestor-1.3/devopstestor/src/machine/local_controller.py` & `devopstestor-1.4/devopstestor/src/machine/local_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,43 @@
+from config import Config
+from source_manager import SourceManager
 import sys
 import os
 import subprocess
 from abstract_machine_controller import AbstractMachineController
 from log_manager import logging
 logger = logging.getLogger('machine.LocalController')
 
 class LocalController(AbstractMachineController):
     @staticmethod
-    def pre_initialize(global_config, machine_configuration, source_manager):
+    def pre_initialize(global_config:Config, machine_configuration:Config, source_manager:SourceManager):
         global_config.set('machine::parallelize', False) # parallelize forbiden in Local mode
 
-    def create_machine(self, global_config, machine_configuration, machine_name, source_manager):
+    def create_machine(self, global_config:Config, machine_configuration:Config, machine_name:str, source_manager:SourceManager):
         """
-        Initialisation des properiete d'instance
+        Initialisation des proprietes d'instance
         """
         self.file_to_clean = []
 
         # Creation des liens symbomliques pour acceder aux sources
         for name, accessor in list(source_manager.get_accessors().items()):
             if not os.path.exists(accessor.machine_path):
                 self.run_cmd('mkdir -p {}'.format(os.path.abspath(accessor.machine_path+"/..")))
                 self.run_cmd('ln -s {} {}'.format(accessor.local_path, accessor.machine_path))
 
-    def destroy_machine(self, global_config, machine_configuration, machine_name, source_manager):
+    def destroy_machine(self, global_config:Config, machine_configuration:Config, machine_name:str, source_manager:SourceManager):
         """
         Nettoyage
-        Chaques modifications identifies apporte la la machine en local sojt nettoyees
+        Chaque modifications identifiees apporte sur la machine en local doit etre nettoyee
         """
         for path in self.file_to_clean:
             logger.info('Nettoyage du chemin temporaire', path=path)
             os.remove(path)
 
-    def put_in_file(self, content, file_path):
+    def put_in_file(self, content:str, file_path:str) -> tuple:
         """
         Permet de copier du contenu dans un fichier sur la machine
         :param content: Contenu a copier
         :param file_path: nom du fichier
         :return: code retour
         """
         logger.info('put_in_file', filepath=file_path, content=content,  machine_name=self.machine_name)
@@ -44,38 +46,38 @@
             self.file_to_clean.append(file_path)
 
         with open(file_path, "w+") as f:
             f.write(content)
 
         return 0, ""
 
-    def get_file_content(self, file_path):
+    def get_file_content(self, file_path:str) -> tuple:
         """
         Permet de recuperer le contenu d'un fichier sur la machine
         :param file_path: Chemin vers le fichier
         :return: contenu du fichier (string)
         """
         logger.debug('get_filecontent', file_path=file_path, machine_name=self.machine_name)
 
         return self.run_cmd('cat ' + file_path)
 
-    def run_python(self, script):
+    def run_python(self, script:str) -> tuple:
         """
         Permet de lancer une commande python sur la machine
         en fonction de l'environement
         Surcharge AbstractMachineController car specificites
         """
         return self.run_cmd(
             command="{} {}".format(
                 sys.executable, # on reprend le meme binaire python que celui du moteur
                 script
             )
         )
 
-    def run_cmd(self, command):
+    def run_cmd(self, command:str) -> tuple:
         '''
         Lance une commande sur le conteneur.
         '''
         logger.debut('commande', "Lancement d'une commande sur le conteneur", machine_name=self.machine_name, command=command)
         ret = 0
         output = ""
         try:
```

### Comparing `devopstestor-1.3/devopstestor/src/provisionner/empty_provisionner.py` & `devopstestor-1.4/devopstestor/src/provisionner/empty_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/provisionner/logstash_provisionner.py` & `devopstestor-1.4/devopstestor/src/provisionner/logstash_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/provisionner/minion_provisionner.py` & `devopstestor-1.4/devopstestor/src/provisionner/minion_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/provisionner/systemd_provisionner.py` & `devopstestor-1.4/devopstestor/src/provisionner/systemd_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/reporting/report_elk_renderer.py` & `devopstestor-1.4/devopstestor/src/reporting/report_elk_renderer.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/reporting/report_html_renderer/__init__.py` & `devopstestor-1.4/devopstestor/src/reporting/report_html_renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja` & `devopstestor-1.4/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/reporting/report_text_renderer.py` & `devopstestor-1.4/devopstestor/src/reporting/report_text_renderer.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/reporting/scenario_report.py` & `devopstestor-1.4/devopstestor/src/reporting/scenario_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/reporting/testcase_report.py` & `devopstestor-1.4/devopstestor/src/reporting/testcase_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/reporting/verifier_report.py` & `devopstestor-1.4/devopstestor/src/reporting/verifier_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/scenarios/devopstestor.py` & `devopstestor-1.4/devopstestor/src/scenarios/devopstestor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/scenarios/logstash.py` & `devopstestor-1.4/devopstestor/src/scenarios/logstash.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/scenarios/mock_utils.py` & `devopstestor-1.4/devopstestor/src/scenarios/mock_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/scenarios/systemd.py` & `devopstestor-1.4/devopstestor/src/scenarios/systemd.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/sources/copytemplate_source_accessor.py` & `devopstestor-1.4/devopstestor/src/sources/copytemplate_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/sources/dirlink_source_accessor.py` & `devopstestor-1.4/devopstestor/src/sources/dirlink_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/sources/git_source_accessor.py` & `devopstestor-1.4/devopstestor/src/sources/git_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/testcase/scenario_executor.py` & `devopstestor-1.4/devopstestor/src/testcase/scenario_executor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/testcase/test_case.py` & `devopstestor-1.4/devopstestor/src/testcase/test_case.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/testcase/testcase_executor.py` & `devopstestor-1.4/devopstestor/src/testcase/testcase_executor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/src/testcase/tests_cases_loader.py` & `devopstestor-1.4/devopstestor/src/testcase/tests_cases_loader.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/testconf/verifiers/fixtures/context_fixtures.py` & `devopstestor-1.4/devopstestor/testconf/verifiers/fixtures/context_fixtures.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py` & `devopstestor-1.4/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/testconf/verifiers/service/http_logger.py` & `devopstestor-1.4/devopstestor/testconf/verifiers/service/http_logger.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py` & `devopstestor-1.4/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py` & `devopstestor-1.4/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py` & `devopstestor-1.4/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py` & `devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py` & `devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py` & `devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py` & `devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py` & `devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py` & `devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py` & `devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py` & `devopstestor-1.4/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py` & `devopstestor-1.4/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor/testconf/verifiers/utils/verififier_luncher.py` & `devopstestor-1.4/devopstestor/testconf/verifiers/utils/verififier_luncher.py`

 * *Files identical despite different names*

### Comparing `devopstestor-1.3/devopstestor.egg-info/PKG-INFO` & `devopstestor-1.4/devopstestor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopstestor
-Version: 1.3
+Version: 1.4
 Summary: Framwork to auto test machine provisioning
 Home-page: https://gitlab.com/alexis.porzier.pro/devopstestor
 Author: Alexis PORZIER
 Author-email: alexis.porzier.pro@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `devopstestor-1.3/devopstestor.egg-info/SOURCES.txt` & `devopstestor-1.4/devopstestor.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 devopstestor/src/lib/json_utils.py
 devopstestor/src/lib/log_manager.py
 devopstestor/src/lib/utils.py
 devopstestor/src/machine/__init__.py
 devopstestor/src/machine/debug_controller.py
 devopstestor/src/machine/docker_controller.py
 devopstestor/src/machine/local_controller.py
+devopstestor/src/machine/vagrant_controller.py
 devopstestor/src/provisionner/__init__.py
 devopstestor/src/provisionner/empty_provisionner.py
 devopstestor/src/provisionner/logstash_provisionner.py
 devopstestor/src/provisionner/minion_provisionner.py
 devopstestor/src/provisionner/systemd_provisionner.py
 devopstestor/src/reporting/__init__.py
 devopstestor/src/reporting/campaign_report.py
```

### Comparing `devopstestor-1.3/setup.py` & `devopstestor-1.4/setup.py`

 * *Files identical despite different names*

