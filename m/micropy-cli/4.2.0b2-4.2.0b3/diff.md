# Comparing `tmp/micropy_cli-4.2.0b2.tar.gz` & `tmp/micropy_cli-4.2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropy_cli-4.2.0b2.tar", max compression
+gzip compressed data, was "micropy_cli-4.2.0b3.tar", max compression
```

## Comparing `micropy_cli-4.2.0b2.tar` & `micropy_cli-4.2.0b3.tar`

### file list

```diff
@@ -1,124 +1,124 @@
--rw-r--r--   0        0        0    42962 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/CHANGELOG.md
--rw-r--r--   0        0        0     1068 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/LICENSE
--rw-r--r--   0        0        0     9356 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/README.md
--rw-r--r--   0        0        0      503 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/__init__.py
--rw-r--r--   0        0        0      128 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/__main__.py
--rw-r--r--   0        0        0       41 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/app/__init__.py
--rw-r--r--   0        0        0     9530 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/app/main.py
--rw-r--r--   0        0        0     7655 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/app/stubs.py
--rw-r--r--   0        0        0      225 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/config/__init__.py
--rw-r--r--   0        0        0     5626 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/config/config.py
--rw-r--r--   0        0        0      623 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/config/config_dict.py
--rw-r--r--   0        0        0     1804 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/config/config_json.py
--rw-r--r--   0        0        0     1595 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/config/config_source.py
--rw-r--r--   0        0        0      622 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/data/__init__.py
--rw-r--r--   0        0        0     1849 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/data/schemas/firmware.json
--rw-r--r--   0        0        0     1812 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/data/schemas/stubs.json
--rw-r--r--   0        0        0      409 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/data/sources.json
--rw-r--r--   0        0        0     1741 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/exceptions.py
--rw-r--r--   0        0        0     8894 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/logger.py
--rw-r--r--   0        0        0     2902 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/main.py
--rw-r--r--   0        0        0     1418 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/packages/__init__.py
--rw-r--r--   0        0        0     2987 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/packages/package.py
--rw-r--r--   0        0        0     2045 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/packages/source.py
--rw-r--r--   0        0        0     4752 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/packages/source_package.py
--rw-r--r--   0        0        0      789 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/packages/source_path.py
--rw-r--r--   0        0        0      133 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/project/__init__.py
--rw-r--r--   0        0        0     2080 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/project/checks.py
--rw-r--r--   0        0        0      339 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/project/modules/__init__.py
--rw-r--r--   0        0        0     8354 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/project/modules/modules.py
--rw-r--r--   0        0        0     7912 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/project/modules/packages.py
--rw-r--r--   0        0        0     4529 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/project/modules/stubs.py
--rw-r--r--   0        0        0     2454 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/project/modules/templates.py
--rw-r--r--   0        0        0     4659 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/project/project.py
--rw-r--r--   0        0        0     2185 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/project/template/.gitignore
--rw-r--r--   0        0        0     1323 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/project/template/.pylintrc
--rw-r--r--   0        0        0      488 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/project/template/.vscode/extensions.json
--rw-r--r--   0        0        0      538 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/project/template/.vscode/settings.json
--rw-r--r--   0        0        0      431 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/project/template/pymakr.conf
--rw-r--r--   0        0        0       30 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/project/template/src/boot.py
--rw-r--r--   0        0        0       10 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/project/template/src/main.py
--rw-r--r--   0        0        0    10788 2023-03-27 11:07:26.397973 micropy_cli-4.2.0b2/micropy/project/template.py
--rw-r--r--   0        0        0        0 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/py.typed
--rw-r--r--   0        0        0      612 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/pyd/__init__.py
--rw-r--r--   0        0        0     3384 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/pyd/abc.py
--rw-r--r--   0        0        0     6713 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/pyd/backend_rshell.py
--rw-r--r--   0        0        0     8632 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/pyd/backend_upydevice.py
--rw-r--r--   0        0        0     2231 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/pyd/consumers.py
--rw-r--r--   0        0        0     2124 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/pyd/pydevice.py
--rw-r--r--   0        0        0      776 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/stubs/__init__.py
--rw-r--r--   0        0        0     1227 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/stubs/manifest.py
--rw-r--r--   0        0        0      384 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/stubs/package.py
--rw-r--r--   0        0        0     4916 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/stubs/repo.py
--rw-r--r--   0        0        0     1410 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/stubs/repo_package.py
--rw-r--r--   0        0        0      269 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/stubs/repositories/__init__.py
--rw-r--r--   0        0        0     1049 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/stubs/repositories/micropy.py
--rw-r--r--   0        0        0     1354 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/stubs/repositories/micropython.py
--rw-r--r--   0        0        0      462 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/stubs/repository_info.py
--rw-r--r--   0        0        0     4965 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/stubs/source.py
--rw-r--r--   0        0        0    18379 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/stubs/stubs.py
--rw-r--r--   0        0        0      584 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/utils/__init__.py
--rw-r--r--   0        0        0      302 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/utils/_compat.py
--rw-r--r--   0        0        0      382 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/utils/decorators.py
--rw-r--r--   0        0        0    10917 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/utils/helpers.py
--rw-r--r--   0        0        0     3546 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/utils/stub.py
--rw-r--r--   0        0        0      389 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/utils/types.py
--rw-r--r--   0        0        0     1054 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/micropy/utils/validate.py
--rw-r--r--   0        0        0     5847 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/__init__.py
--rw-r--r--   0        0        0     1840 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/app/conftest.py
--rw-r--r--   0        0        0     8443 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/app/test_main.py
--rw-r--r--   0        0        0     6151 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/app/test_stubs.py
--rw-r--r--   0        0        0    10049 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/conftest.py
--rw-r--r--   0        0        0    45229 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/archive_test_stub.tar.gz
--rw-r--r--   0        0        0      882 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/esp32_test_stub/frozen/ntptime.py
--rw-r--r--   0        0        0      231 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/esp32_test_stub/frozen/ntptime.pyi
--rw-r--r--   0        0        0      553 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/esp32_test_stub/info.json
--rw-r--r--   0        0        0      347 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/esp32_test_stub/stubs/machine.py
--rw-r--r--   0        0        0     3346 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/esp32_test_stub/stubs/modules.json
--rw-r--r--   0        0        0      157 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/esp8266_invalid_stub/info.json
--rw-r--r--   0        0        0      882 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/esp8266_test_stub/frozen/ntptime.py
--rw-r--r--   0        0        0      231 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/esp8266_test_stub/frozen/ntptime.pyi
--rw-r--r--   0        0        0      570 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/esp8266_test_stub/info.json
--rw-r--r--   0        0        0      347 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/esp8266_test_stub/stubs/machine.py
--rw-r--r--   0        0        0     3346 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/esp8266_test_stub/stubs/modules.json
--rw-r--r--   0        0        0     2219 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/fware_test_stub/frozen/utarfile.py
--rw-r--r--   0        0        0     1276 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/fware_test_stub/frozen/utarfile.pyi
--rw-r--r--   0        0        0     1868 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/fware_test_stub/frozen/utokenize.py
--rw-r--r--   0        0        0      313 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/fware_test_stub/frozen/utokenize.pyi
--rw-r--r--   0        0        0     1331 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/fware_test_stub/info.json
--rw-r--r--   0        0        0      483 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/project_test/.pylintrc
--rw-r--r--   0        0        0     1900 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/project_test/.vscode/settings.json
--rw-r--r--   0        0        0      334 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/project_test/micropy.json
--rw-r--r--   0        0        0      500 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/stubber_test_stub/micropython.py
--rw-r--r--   0        0        0      401 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/stubber_test_stub/modules.json
--rw-r--r--   0        0        0      560 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/test_repo.json
--rw-r--r--   0        0        0      846 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/test_source.xml
--rw-r--r--   0        0        0       94 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/data/test_sources.json
--rw-r--r--   0        0        0      474 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/test_checks.py
--rw-r--r--   0        0        0     3457 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/test_config.py
--rw-r--r--   0        0        0     5119 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/test_highlevel.py
--rw-r--r--   0        0        0     1399 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/test_main.py
--rw-r--r--   0        0        0     4760 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/test_packages.py
--rw-r--r--   0        0        0    10080 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/test_project.py
--rw-r--r--   0        0        0    12693 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/test_pyd.py
--rw-r--r--   0        0        0     1574 2023-03-27 11:07:26.401973 micropy_cli-4.2.0b2/tests/test_stub_source.py
--rw-r--r--   0        0        0      157 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_stubs/bad_test_stub/modules.json
--rw-r--r--   0        0        0      882 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_stubs/esp32_test_stub/frozen/ntptime.py
--rw-r--r--   0        0        0      231 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_stubs/esp32_test_stub/frozen/ntptime.pyi
--rw-r--r--   0        0        0      553 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_stubs/esp32_test_stub/info.json
--rw-r--r--   0        0        0      347 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_stubs/esp32_test_stub/stubs/machine.py
--rw-r--r--   0        0        0     3346 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_stubs/esp32_test_stub/stubs/modules.json
--rw-r--r--   0        0        0      882 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_stubs/esp8266_test_stub/frozen/ntptime.py
--rw-r--r--   0        0        0      231 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_stubs/esp8266_test_stub/frozen/ntptime.pyi
--rw-r--r--   0        0        0      570 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_stubs/esp8266_test_stub/info.json
--rw-r--r--   0        0        0      347 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_stubs/esp8266_test_stub/stubs/machine.py
--rw-r--r--   0        0        0     3346 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_stubs/esp8266_test_stub/stubs/modules.json
--rw-r--r--   0        0        0     8511 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_stubs.py
--rw-r--r--   0        0        0     2447 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_stubs_repo.py
--rw-r--r--   0        0        0     4534 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_template.py
--rw-r--r--   0        0        0      157 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_utils/fail.json
--rw-r--r--   0        0        0      395 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_utils/pass.json
--rw-r--r--   0        0        0     1088 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_utils/schema.json
--rw-r--r--   0        0        0    10261 2023-03-27 11:07:26.405973 micropy_cli-4.2.0b2/tests/test_utils.py
--rw-r--r--   0        0        0    11807 1970-01-01 00:00:00.000000 micropy_cli-4.2.0b2/PKG-INFO
+-rw-r--r--   0        0        0    45021 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/CHANGELOG.md
+-rw-r--r--   0        0        0     1068 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/LICENSE
+-rw-r--r--   0        0        0     9356 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/README.md
+-rw-r--r--   0        0        0      503 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/__init__.py
+-rw-r--r--   0        0        0      128 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/__main__.py
+-rw-r--r--   0        0        0       41 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/app/__init__.py
+-rw-r--r--   0        0        0     9530 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/app/main.py
+-rw-r--r--   0        0        0     8531 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/app/stubs.py
+-rw-r--r--   0        0        0      225 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/config/__init__.py
+-rw-r--r--   0        0        0     5626 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/config/config.py
+-rw-r--r--   0        0        0      623 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/config/config_dict.py
+-rw-r--r--   0        0        0     1804 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/config/config_json.py
+-rw-r--r--   0        0        0     1595 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/config/config_source.py
+-rw-r--r--   0        0        0      622 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/data/__init__.py
+-rw-r--r--   0        0        0     1849 2023-04-17 20:07:39.160921 micropy_cli-4.2.0b3/micropy/data/schemas/firmware.json
+-rw-r--r--   0        0        0     1812 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/data/schemas/stubs.json
+-rw-r--r--   0        0        0      409 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/data/sources.json
+-rw-r--r--   0        0        0     2190 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/exceptions.py
+-rw-r--r--   0        0        0     8894 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/logger.py
+-rw-r--r--   0        0        0     2902 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/main.py
+-rw-r--r--   0        0        0     1418 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/packages/__init__.py
+-rw-r--r--   0        0        0     2987 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/packages/package.py
+-rw-r--r--   0        0        0     2045 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/packages/source.py
+-rw-r--r--   0        0        0     4752 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/packages/source_package.py
+-rw-r--r--   0        0        0      789 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/packages/source_path.py
+-rw-r--r--   0        0        0      133 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/__init__.py
+-rw-r--r--   0        0        0     2080 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/checks.py
+-rw-r--r--   0        0        0      339 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/modules/__init__.py
+-rw-r--r--   0        0        0     8354 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/modules/modules.py
+-rw-r--r--   0        0        0     7912 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/modules/packages.py
+-rw-r--r--   0        0        0     4529 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/modules/stubs.py
+-rw-r--r--   0        0        0     2454 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/modules/templates.py
+-rw-r--r--   0        0        0     4659 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/project.py
+-rw-r--r--   0        0        0     2185 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/template/.gitignore
+-rw-r--r--   0        0        0     1323 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/template/.pylintrc
+-rw-r--r--   0        0        0      488 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/template/.vscode/extensions.json
+-rw-r--r--   0        0        0      538 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/template/.vscode/settings.json
+-rw-r--r--   0        0        0      431 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/template/pymakr.conf
+-rw-r--r--   0        0        0       30 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/template/src/boot.py
+-rw-r--r--   0        0        0       10 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/template/src/main.py
+-rw-r--r--   0        0        0    10788 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/project/template.py
+-rw-r--r--   0        0        0        0 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/py.typed
+-rw-r--r--   0        0        0      612 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/pyd/__init__.py
+-rw-r--r--   0        0        0     3771 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/pyd/abc.py
+-rw-r--r--   0        0        0     6794 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/pyd/backend_rshell.py
+-rw-r--r--   0        0        0    12055 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/pyd/backend_upydevice.py
+-rw-r--r--   0        0        0     2497 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/pyd/consumers.py
+-rw-r--r--   0        0        0     3096 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/pyd/pydevice.py
+-rw-r--r--   0        0        0      776 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/__init__.py
+-rw-r--r--   0        0        0     1227 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/manifest.py
+-rw-r--r--   0        0        0      384 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/package.py
+-rw-r--r--   0        0        0     4916 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/repo.py
+-rw-r--r--   0        0        0     1410 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/repo_package.py
+-rw-r--r--   0        0        0      269 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/repositories/__init__.py
+-rw-r--r--   0        0        0     1049 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/repositories/micropy.py
+-rw-r--r--   0        0        0     1354 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/repositories/micropython.py
+-rw-r--r--   0        0        0      462 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/repository_info.py
+-rw-r--r--   0        0        0     4965 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/source.py
+-rw-r--r--   0        0        0    18379 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/stubs/stubs.py
+-rw-r--r--   0        0        0      584 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/utils/__init__.py
+-rw-r--r--   0        0        0      302 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/utils/_compat.py
+-rw-r--r--   0        0        0      382 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/utils/decorators.py
+-rw-r--r--   0        0        0    10917 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/utils/helpers.py
+-rw-r--r--   0        0        0     3635 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/utils/stub.py
+-rw-r--r--   0        0        0      389 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/utils/types.py
+-rw-r--r--   0        0        0     1054 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/micropy/utils/validate.py
+-rw-r--r--   0        0        0     5846 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/__init__.py
+-rw-r--r--   0        0        0     1840 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/app/conftest.py
+-rw-r--r--   0        0        0     8443 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/app/test_main.py
+-rw-r--r--   0        0        0     6161 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/app/test_stubs.py
+-rw-r--r--   0        0        0    10049 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/conftest.py
+-rw-r--r--   0        0        0    45229 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/data/archive_test_stub.tar.gz
+-rw-r--r--   0        0        0      882 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/data/esp32_test_stub/frozen/ntptime.py
+-rw-r--r--   0        0        0      231 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/data/esp32_test_stub/frozen/ntptime.pyi
+-rw-r--r--   0        0        0      553 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/data/esp32_test_stub/info.json
+-rw-r--r--   0        0        0      347 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/data/esp32_test_stub/stubs/machine.py
+-rw-r--r--   0        0        0     3346 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/data/esp32_test_stub/stubs/modules.json
+-rw-r--r--   0        0        0      157 2023-04-17 20:07:39.164921 micropy_cli-4.2.0b3/tests/data/esp8266_invalid_stub/info.json
+-rw-r--r--   0        0        0      882 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/esp8266_test_stub/frozen/ntptime.py
+-rw-r--r--   0        0        0      231 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/esp8266_test_stub/frozen/ntptime.pyi
+-rw-r--r--   0        0        0      570 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/esp8266_test_stub/info.json
+-rw-r--r--   0        0        0      347 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/esp8266_test_stub/stubs/machine.py
+-rw-r--r--   0        0        0     3346 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/esp8266_test_stub/stubs/modules.json
+-rw-r--r--   0        0        0     2219 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/fware_test_stub/frozen/utarfile.py
+-rw-r--r--   0        0        0     1276 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/fware_test_stub/frozen/utarfile.pyi
+-rw-r--r--   0        0        0     1868 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/fware_test_stub/frozen/utokenize.py
+-rw-r--r--   0        0        0      313 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/fware_test_stub/frozen/utokenize.pyi
+-rw-r--r--   0        0        0     1331 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/fware_test_stub/info.json
+-rw-r--r--   0        0        0      483 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/project_test/.pylintrc
+-rw-r--r--   0        0        0     1900 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/project_test/.vscode/settings.json
+-rw-r--r--   0        0        0      334 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/project_test/micropy.json
+-rw-r--r--   0        0        0      500 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/stubber_test_stub/micropython.py
+-rw-r--r--   0        0        0      401 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/stubber_test_stub/modules.json
+-rw-r--r--   0        0        0      560 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/test_repo.json
+-rw-r--r--   0        0        0      846 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/test_source.xml
+-rw-r--r--   0        0        0       94 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/data/test_sources.json
+-rw-r--r--   0        0        0      474 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_checks.py
+-rw-r--r--   0        0        0     3457 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_config.py
+-rw-r--r--   0        0        0     5119 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_highlevel.py
+-rw-r--r--   0        0        0     1399 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_main.py
+-rw-r--r--   0        0        0     4760 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_packages.py
+-rw-r--r--   0        0        0    10080 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_project.py
+-rw-r--r--   0        0        0    17567 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_pyd.py
+-rw-r--r--   0        0        0     1574 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stub_source.py
+-rw-r--r--   0        0        0      157 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/bad_test_stub/modules.json
+-rw-r--r--   0        0        0      882 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp32_test_stub/frozen/ntptime.py
+-rw-r--r--   0        0        0      231 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp32_test_stub/frozen/ntptime.pyi
+-rw-r--r--   0        0        0      553 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp32_test_stub/info.json
+-rw-r--r--   0        0        0      347 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp32_test_stub/stubs/machine.py
+-rw-r--r--   0        0        0     3346 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp32_test_stub/stubs/modules.json
+-rw-r--r--   0        0        0      882 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp8266_test_stub/frozen/ntptime.py
+-rw-r--r--   0        0        0      231 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp8266_test_stub/frozen/ntptime.pyi
+-rw-r--r--   0        0        0      570 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp8266_test_stub/info.json
+-rw-r--r--   0        0        0      347 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp8266_test_stub/stubs/machine.py
+-rw-r--r--   0        0        0     3346 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs/esp8266_test_stub/stubs/modules.json
+-rw-r--r--   0        0        0     8511 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs.py
+-rw-r--r--   0        0        0     2447 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_stubs_repo.py
+-rw-r--r--   0        0        0     4534 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_template.py
+-rw-r--r--   0        0        0      157 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_utils/fail.json
+-rw-r--r--   0        0        0      395 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_utils/pass.json
+-rw-r--r--   0        0        0     1088 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_utils/schema.json
+-rw-r--r--   0        0        0    10261 2023-04-17 20:07:39.168921 micropy_cli-4.2.0b3/tests/test_utils.py
+-rw-r--r--   0        0        0    11800 1970-01-01 00:00:00.000000 micropy_cli-4.2.0b3/PKG-INFO
```

### Comparing `micropy_cli-4.2.0b2/CHANGELOG.md` & `micropy_cli-4.2.0b3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,35 @@
 <a name="v4.0.0"></a>
 
+## [4.2.0-beta.3](https://github.com/BradenM/micropy-cli/compare/v4.2.0-beta.2...v4.2.0-beta.3) (2023-04-17)
+
+
+### Features
+
+* **app:** Expose compile, module-defaults flags, integrity in stubs create command. ([885e9d3](https://github.com/BradenM/micropy-cli/commit/885e9d369cad98345e6132315f6fb76694379339))
+* **exc:** `PyDeviceFileIntegrityError` exception. ([a2187c8](https://github.com/BradenM/micropy-cli/commit/a2187c898c9aeb641a63a9237d2469faaf929de5))
+* **pyd:** `NoOpConsumer` implementation. ([5a21ecd](https://github.com/BradenM/micropy-cli/commit/5a21ecd1e85f74a5976aac209457d8273d8596cb))
+* **pydevice:** File integrity support, simple run in pydevice. ([8b7a255](https://github.com/BradenM/micropy-cli/commit/8b7a2557d42cb70430430ad04280dffebd45aeb6))
+* **pyd:** File integrity check support in upydevice backend. ([a3cbf31](https://github.com/BradenM/micropy-cli/commit/a3cbf31f8ff5fd5f0da24661a911f030672d93b7))
+* **pyd:** Implement `remove` across backends. ([f0bba8d](https://github.com/BradenM/micropy-cli/commit/f0bba8d25cd7eb6bdb2567bfde97c22a02088c16))
+* **pyd:** Use noop consumer default for upy `eval`/`eval_script` ([720ace4](https://github.com/BradenM/micropy-cli/commit/720ace4355d5e7a794e6d204a6bccfe0249d5f5d))
+* **utils:** Support compiling createstubs with mpy-cross ([1819197](https://github.com/BradenM/micropy-cli/commit/181919714c6d5d9a5a382e673bd81334164cbb53))
+
+
+### Bug Fixes
+
+* **deps:** Pin dependency typer to 0.7.0 ([30ab97f](https://github.com/BradenM/micropy-cli/commit/30ab97fc450ae5af9f58cf3e5770ce609cba9745))
+* **pyd:** Remove usedforsecurity hash flag for py3.8 ([522a0c3](https://github.com/BradenM/micropy-cli/commit/522a0c3537634950178178628d097944ce554cb3))
+* **pyd:** Support pushing binary files to pydevice in upydevice backend. ([e58c1f2](https://github.com/BradenM/micropy-cli/commit/e58c1f2f90f6e901298dfe54d0b5234818107140))
+
+
+### Miscellaneous Chores
+
+* **release:** Set release to v4.2.0-beta3 ([9ee81a2](https://github.com/BradenM/micropy-cli/commit/9ee81a2f4f63de78716b73b2bc4224a50e58a2c4))
+
 ## [4.2.0-beta.2](https://github.com/BradenM/micropy-cli/compare/v4.2.0-beta.1...v4.2.0-beta.2) (2023-03-27)
 
 
 ### Bug Fixes
 
 * **deps:** Use latest stable typer. ([ec3082e](https://github.com/BradenM/micropy-cli/commit/ec3082ed541b724743f8bc7b5bb19ecce9c9e2bc))
```

### Comparing `micropy_cli-4.2.0b2/LICENSE` & `micropy_cli-4.2.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/README.md` & `micropy_cli-4.2.0b3/README.md`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/app/main.py` & `micropy_cli-4.2.0b3/micropy/app/main.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/app/stubs.py` & `micropy_cli-4.2.0b3/micropy/app/stubs.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,18 +58,20 @@
     def __new__(cls, value: str, backend: Type[MetaPyDeviceBackend]):
         obj = str.__new__(cls, value)
         obj._value_ = value
         obj.backend = backend
         return obj
 
 
-def create_changeset(value: Optional[List[str]]) -> Optional[ListChangeSet]:
+def create_changeset(
+    value: Optional[List[str]], *, replace: bool = False
+) -> Optional[ListChangeSet]:
     if value is None:
         return value
-    return ListChangeSet.from_strings(add=value)
+    return ListChangeSet.from_strings(add=value, replace=replace)
 
 
 @stubs_app.command(name="create")
 def stubs_create(
     ctx: typer.Context,
     port: str = typer.Argument(..., help="Serial port used to connect to device"),
     backend: CreateBackend = typer.Option(CreateBackend.upydevice, help="PyDevice backend."),
@@ -79,25 +81,35 @@
         "--variant",
         help="Create Stubs variant.",
         rich_help_panel="Stubs",
     ),
     module: Optional[List[str]] = typer.Option(
         None, "-m", "--module", help="Modules to add.", rich_help_panel="Stubs"
     ),
+    module_defaults: bool = typer.Option(
+        True, help="Include createstubs default modules.", rich_help_panel="Stubs"
+    ),
     exclude: Optional[List[str]] = typer.Option(
         None, "-e", "--exclude", help="Modules to exclude.", rich_help_panel="Stubs"
     ),
+    compile: bool = typer.Option(
+        True,
+        "-c",
+        "--compile",
+        help="Cross compile to .mpy via mpy-cross.",
+        rich_help_panel="Stubs",
+    ),
 ):
     """Create stubs from micropython-enabled devices.
 
     Utilize Josverl's [micropython-stubber](https://github.com/josverl/micropython-stubber/)
     to generate stubs from your own micropython-enabled device.
 
     """
-    mp: MicroPy = ctx.find_object(MicroPy)
+    mp: MicroPy = ctx.ensure_object(MicroPy)
     log = mp.log
     log.title(f"Connecting to Pyboard @ $[{port}]")
     pyb_log = Log.add_logger("Pyboard", "bright_white")
 
     def _get_desc(name: str, cfg: dict):
         desc = f"{pyb_log.get_service()} {name}"
         return name, cfg | dict(desc=desc)
@@ -114,35 +126,48 @@
             backend=backend.backend,
         )
     except (SystemExit, PyDeviceError):
         log.error(f"Failed to connect, are you sure $[{port}] is correct?")
         return None
 
     log.success("Connected!")
+    if module or exclude:
+        log.title("Preparing createstubs for:")
+        log.info(f"Modules: {', '.join(module or [])}")
+        log.info(f"Exclude: {', '.join(exclude or [])}")
     create_stubs = prepare_create_stubs(
         variant=variant,
-        modules_set=create_changeset(module),
+        modules_set=create_changeset(module, replace=not module_defaults),
         exclude_set=create_changeset(exclude),
+        compile=compile,
     )
+    dev_path = DevicePath("createstubs.mpy") if compile else DevicePath("createstubs.py")
     log.info("Executing stubber on pyboard...")
     try:
-        pyb.run_script(create_stubs.getvalue(), DevicePath("createstubs.py"))
+        pyb.run_script(create_stubs, DevicePath(dev_path))
     except Exception as e:
         # TODO: Handle more usage cases
         log.error(f"Failed to execute script: {str(e)}", exception=e)
         raise
     log.success("Done!")
     log.info("Copying stubs...")
     with tempfile.TemporaryDirectory() as tmpdir:
-        pyb.copy_from(DevicePath("/stubs"), tmpdir)
+        pyb.copy_from(
+            DevicePath("/stubs"),
+            tmpdir,
+            verify_integrity=True,
+            # exclude due to ps1 var possibly different.
+            exclude_integrity={"sys.py", "usys.py"},
+        )
         out_dir = Path(tmpdir)
         stub_path = next(out_dir.iterdir())
         log.info(f"Copied Stubs: $[{stub_path.name}]")
         stub_path = mp.stubs.from_stubber(stub_path, out_dir)
         stub = mp.stubs.add(str(stub_path))
+    pyb.remove(dev_path)
     pyb.disconnect()
     log.success(f"Added {stub.name} to stubs!")
     return stub
 
 
 @stubs_app.command(name="add")
 def stubs_add(ctx: typer.Context, stub_name: str, force: bool = False):
```

### Comparing `micropy_cli-4.2.0b2/micropy/config/config.py` & `micropy_cli-4.2.0b3/micropy/config/config.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/config/config_dict.py` & `micropy_cli-4.2.0b3/micropy/config/config_dict.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/config/config_json.py` & `micropy_cli-4.2.0b3/micropy/config/config_json.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/config/config_source.py` & `micropy_cli-4.2.0b3/micropy/config/config_source.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/data/__init__.py` & `micropy_cli-4.2.0b3/micropy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/data/schemas/firmware.json` & `micropy_cli-4.2.0b3/micropy/data/schemas/firmware.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/data/schemas/stubs.json` & `micropy_cli-4.2.0b3/micropy/data/schemas/stubs.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/exceptions.py` & `micropy_cli-4.2.0b3/micropy/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Micropy Exceptions."""
+from __future__ import annotations
 
 
 class MicropyException(Exception):
     """Generic MicroPy Exception."""
 
 
 class StubError(MicropyException):
@@ -57,7 +58,20 @@
 
 
 class PyDeviceConnectionError(PyDeviceError):
     _default_message = "Failed to connect to pydevice @ {location}."
 
     def __init__(self, location: str):
         super().__init__(self._default_message.format(location=location))
+
+
+class PyDeviceFileIntegrityError(PyDeviceError):
+    _default_message = (
+        "Failed to verify integrity: {device_path} (device={device_sum}, recv={digest})"
+    )
+
+    def __init__(self, device_path: str, device_sum: str, digest: str):
+        super().__init__(
+            self._default_message.format(
+                device_path=device_path, device_sum=device_sum, digest=digest
+            )
+        )
```

### Comparing `micropy_cli-4.2.0b2/micropy/logger.py` & `micropy_cli-4.2.0b3/micropy/logger.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/main.py` & `micropy_cli-4.2.0b3/micropy/main.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/packages/__init__.py` & `micropy_cli-4.2.0b3/micropy/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/packages/package.py` & `micropy_cli-4.2.0b3/micropy/packages/package.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/packages/source.py` & `micropy_cli-4.2.0b3/micropy/packages/source.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/packages/source_package.py` & `micropy_cli-4.2.0b3/micropy/packages/source_package.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/packages/source_path.py` & `micropy_cli-4.2.0b3/micropy/packages/source_path.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/project/checks.py` & `micropy_cli-4.2.0b3/micropy/project/checks.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/project/modules/modules.py` & `micropy_cli-4.2.0b3/micropy/project/modules/modules.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/project/modules/packages.py` & `micropy_cli-4.2.0b3/micropy/project/modules/packages.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/project/modules/stubs.py` & `micropy_cli-4.2.0b3/micropy/project/modules/stubs.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/project/modules/templates.py` & `micropy_cli-4.2.0b3/micropy/project/modules/templates.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/project/project.py` & `micropy_cli-4.2.0b3/micropy/project/project.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/project/template/.gitignore` & `micropy_cli-4.2.0b3/micropy/project/template/.gitignore`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/project/template/.pylintrc` & `micropy_cli-4.2.0b3/micropy/project/template/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/project/template/.vscode/settings.json` & `micropy_cli-4.2.0b3/micropy/project/template/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/project/template.py` & `micropy_cli-4.2.0b3/micropy/project/template.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/pyd/__init__.py` & `micropy_cli-4.2.0b3/micropy/pyd/__init__.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/pyd/abc.py` & `micropy_cli-4.2.0b3/micropy/pyd/abc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import abc
+from io import BytesIO, StringIO
 from pathlib import Path
-from typing import Any, AnyStr, NewType, Protocol
+from typing import Any, AnyStr, Generic, NewType, Protocol, TypeVar
 
 HostPath = NewType("HostPath", str)
 DevicePath = NewType("DevicePath", str)
 
 
 class StartHandler(Protocol):
     def __call__(self, *, name: str = None, size: int | None = None) -> Any:
@@ -107,14 +108,18 @@
         ...
 
     @abc.abstractmethod
     def list_dir(self, path: DevicePath) -> list[DevicePath]:
         ...
 
     @abc.abstractmethod
+    def remove(self, path: DevicePath) -> None:
+        ...
+
+    @abc.abstractmethod
     def copy_dir(
         self,
         source_path: DevicePath,
         target_path: HostPath,
         *,
         consumer: PyDeviceConsumer | None,
         **kwargs,
@@ -132,16 +137,19 @@
         target_path: DevicePath | None = None,
         *,
         consumer: PyDeviceConsumer | None = None,
     ):
         ...
 
 
-class MetaPyDevice(abc.ABC):
-    pydevice: MetaPyDeviceBackend
+AnyBackend = TypeVar("AnyBackend", bound=MetaPyDeviceBackend)
+
+
+class MetaPyDevice(abc.ABC, Generic[AnyBackend]):
+    pydevice: AnyBackend
     stream_consumer: StreamConsumer | None
     message_consumer: MessageConsumer | None
 
     @abc.abstractmethod
     def connect(self) -> None:
         ...
 
@@ -150,13 +158,21 @@
         ...
 
     @abc.abstractmethod
     def copy_to(self, source_path: HostPath, target_path: DevicePath) -> None:
         ...
 
     @abc.abstractmethod
-    def copy_from(self, source_path: DevicePath, target_path: HostPath) -> None:
+    def copy_from(
+        self, source_path: DevicePath, target_path: HostPath, *, verify_integrity: bool = True
+    ) -> None:
         ...
 
     @abc.abstractmethod
-    def run_script(self, content: AnyStr, target_path: DevicePath | None = None):
+    def remove(self, target_path: DevicePath) -> None:
+        ...
+
+    @abc.abstractmethod
+    def run_script(
+        self, content: AnyStr | StringIO | BytesIO, target_path: DevicePath | None = None
+    ):
         ...
```

### Comparing `micropy_cli-4.2.0b2/micropy/pyd/backend_rshell.py` & `micropy_cli-4.2.0b3/micropy/pyd/backend_rshell.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,7 +226,10 @@
         with self.repl():
             try:
                 out_bytes = self.eval(_contents, consumer=consumer)
             except PyboardError as e:
                 raise Exception(str(e)) from e
             out = out_bytes.decode("utf-8")
             return out
+
+    def remove(self, path: DevicePath) -> None:
+        self._rsh.rm(str(path))
```

### Comparing `micropy_cli-4.2.0b2/micropy/pyd/consumers.py` & `micropy_cli-4.2.0b3/micropy/pyd/consumers.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,7 +68,16 @@
     on_start: StartHandler
     on_update: UpdateHandler
     on_end: EndHandler
 
 
 class MessageHandlers(NamedTuple):
     on_message: MessageHandler
+
+
+def _no_op(*args, **kwargs):
+    return None
+
+
+NoOpStreamConsumer = StreamHandlers(on_start=_no_op, on_update=_no_op, on_end=_no_op)
+NoOpMessageConsumer = MessageHandlers(on_message=_no_op)
+NoOpConsumer = ConsumerDelegate(NoOpMessageConsumer, NoOpMessageConsumer)
```

### Comparing `micropy_cli-4.2.0b2/micropy/pyd/pydevice.py` & `micropy_cli-4.2.0b3/micropy/pyd/pydevice.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
+from io import BytesIO, StringIO
 from pathlib import Path
-from typing import AnyStr, Type
+from typing import AnyStr, Generic, Optional, Type
 
 from .abc import (
+    AnyBackend,
     DevicePath,
     HostPath,
     MessageConsumer,
     MetaPyDevice,
     MetaPyDeviceBackend,
     StreamConsumer,
 )
 from .backend_upydevice import UPyDeviceBackend
 from .consumers import ConsumerDelegate
 
 
-class PyDevice(MetaPyDevice):
-    pydevice: MetaPyDeviceBackend
+class PyDevice(MetaPyDevice[AnyBackend], Generic[AnyBackend]):
+    pydevice: AnyBackend
     consumer: ConsumerDelegate
 
     def __init__(
         self,
         location: str,
         *,
         backend: Type[MetaPyDeviceBackend] = UPyDeviceBackend,
@@ -30,31 +32,66 @@
         delegate_cls: Type[ConsumerDelegate] = ConsumerDelegate,
     ):
         self.pydevice = backend().establish(location)
         self.consumer = delegate_cls(stream_consumer, message_consumer)
         if auto_connect and self.pydevice:
             self.pydevice.connect()
 
-    def copy_from(self, source_path: DevicePath, target_path: HostPath) -> None:
+    def copy_from(
+        self,
+        source_path: DevicePath,
+        target_path: HostPath,
+        *,
+        verify_integrity: bool = True,
+        exclude_integrity: Optional[set[str]] = None,
+    ) -> None:
         src_path = Path(str(source_path))
         # 'is_dir/file' only works on existing paths.
         if not src_path.suffix:
             return self.pydevice.copy_dir(
-                DevicePath(source_path), target_path, consumer=self.consumer
+                DevicePath(source_path),
+                target_path,
+                consumer=self.consumer,
+                verify_integrity=verify_integrity,
+                exclude_integrity=exclude_integrity,
             )
-        return self.pydevice.pull_file(DevicePath(source_path), target_path, consumer=self.consumer)
+        return self.pydevice.pull_file(
+            DevicePath(source_path),
+            target_path,
+            consumer=self.consumer,
+            verify_integrity=verify_integrity,
+        )
 
-    def copy_to(self, source_path: HostPath, target_path: DevicePath) -> None:
+    def copy_to(self, source_path: HostPath, target_path: DevicePath, **kwargs) -> None:
         src_path = Path(str(source_path))
         host_exists = src_path.exists()
         if (host_exists and src_path.is_dir()) or (not host_exists and not src_path.suffix):
             raise RuntimeError("Copying dirs to device is not yet supported!")
-        return self.pydevice.push_file(source_path, target_path, consumer=self.consumer)
+        return self.pydevice.push_file(source_path, target_path, consumer=self.consumer, **kwargs)
+
+    def remove(self, target_path: DevicePath) -> None:
+        return self.pydevice.remove(target_path)
 
     def connect(self):
         return self.pydevice.connect()
 
     def disconnect(self):
         return self.pydevice.disconnect()
 
-    def run_script(self, content: AnyStr, target_path: DevicePath | None = None):
-        return self.pydevice.eval_script(content, target_path, consumer=self.consumer)
+    def run_script(
+        self, content: AnyStr | StringIO | BytesIO, target_path: DevicePath | None = None
+    ):
+        _content = (
+            content
+            if isinstance(
+                content,
+                (
+                    str,
+                    bytes,
+                ),
+            )
+            else content.read()
+        )
+        return self.pydevice.eval_script(_content, target_path, consumer=self.consumer)
+
+    def run(self, content: str) -> str | None:
+        return self.pydevice.eval(content, consumer=self.consumer)
```

### Comparing `micropy_cli-4.2.0b2/micropy/stubs/__init__.py` & `micropy_cli-4.2.0b3/micropy/stubs/__init__.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/stubs/manifest.py` & `micropy_cli-4.2.0b3/micropy/stubs/manifest.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/stubs/repo.py` & `micropy_cli-4.2.0b3/micropy/stubs/repo.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/stubs/repo_package.py` & `micropy_cli-4.2.0b3/micropy/stubs/repo_package.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/stubs/repositories/micropy.py` & `micropy_cli-4.2.0b3/micropy/stubs/repositories/micropy.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/stubs/repositories/micropython.py` & `micropy_cli-4.2.0b3/micropy/stubs/repositories/micropython.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/stubs/source.py` & `micropy_cli-4.2.0b3/micropy/stubs/source.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/stubs/stubs.py` & `micropy_cli-4.2.0b3/micropy/stubs/stubs.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/utils/__init__.py` & `micropy_cli-4.2.0b3/micropy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/utils/helpers.py` & `micropy_cli-4.2.0b3/micropy/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/micropy/utils/stub.py` & `micropy_cli-4.2.0b3/micropy/utils/stub.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,26 +84,29 @@
 
 def prepare_create_stubs(
     *,
     variant: Optional[stub_board.CreateStubsVariant] = None,
     modules_set: Optional[stub_board.ListChangeSet] = None,
     problem_set: Optional[stub_board.ListChangeSet] = None,
     exclude_set: Optional[stub_board.ListChangeSet] = None,
-) -> io.StringIO:
+    compile: bool = False,
+) -> io.StringIO | io.BytesIO:
     if stub_board is None:
         raise ImportError("micropython-stubber requires a python version of >= 3.8")
     variant = variant or stub_board.CreateStubsVariant.BASE
     ctx = codemod.CodemodContext()
     code_mod = stub_board.CreateStubsCodemod(
         ctx, variant=variant, modules=modules_set, problematic=problem_set, excluded=exclude_set
     )
     create_stubs = cst.parse_module(locate_create_stubs().read_text())
     result = code_mod.transform_module_impl(create_stubs).code
     result_io = io.StringIO(result)
     minified_io = io.StringIO()
     minify.minify(result_io, minified_io, keep_report=True, diff=False)
     minified_io.seek(0)
     # TODO: compile w/ mpy-cross
-    # compiled_io = io.BytesIO()
-    # minify.cross_compile(minified_io, compiled_io)
-    # compiled_io.seek(0)
+    if compile:
+        compiled_io = io.BytesIO()
+        minify.cross_compile(minified_io, compiled_io)
+        compiled_io.seek(0)
+        return compiled_io
     return minified_io
```

### Comparing `micropy_cli-4.2.0b2/micropy/utils/validate.py` & `micropy_cli-4.2.0b3/micropy/utils/validate.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/pyproject.toml` & `micropy_cli-4.2.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micropy-cli"
-version = "4.2.0-beta.2"
+version = "4.2.0-beta.3"
 description = "Micropython Project Management Tool with VSCode support, Linting, Intellisense, Dependency Management, and more!"
 authors = ["Braden Mars <bradenmars@bradenmars.me>"]
 license = "MIT"
 packages = [{ include = "micropy" }]
 include = [
     { path = "tests", format = "sdist" },
     "README.md",
@@ -63,15 +63,15 @@
 attrs = "==22.2.0"
 typing-extensions = "4.5.0"
 pydantic = "1.10.7"
 distlib = "0.3.6"
 importlib-metadata = { version = "==5.2.0", python = '<3.10' }
 micropython-stubber = "==1.13.1.post1"
 libcst = "0.4.9"
-typer = {version = "^0.7.0", extras = ["all"]}
+typer = {version = "0.7.0", extras = ["all"]}
 
 [tool.poetry.group.dev.dependencies]
 bump2version = "^0.5.11"
 pre-commit = "^3.0.2"
 mypy = { version = "^1.0", extras = ["dmypy"] }
 types-requests = "^2.27.14"
 pylint = "^2.7"
@@ -81,15 +81,15 @@
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 pyupgrade = "^3.3.1"
 isort = "^5.12.0"
 black = ">=22.10,<23.0"
-ruff = "^0.0.259"
+ruff = "^0.0.261"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.1"
 pytest-cov = "^4.0"
```

### Comparing `micropy_cli-4.2.0b2/tests/app/conftest.py` & `micropy_cli-4.2.0b3/tests/app/conftest.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/app/test_main.py` & `micropy_cli-4.2.0b3/tests/app/test_main.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/app/test_stubs.py` & `micropy_cli-4.2.0b3/tests/app/test_stubs.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     else:
         assert result.add[0].children == expected.add[0].children
         assert result.add[1].children == expected.add[1].children
 
 
 @pytest.fixture()
 def pydevice_mock(mocker: MockerFixture):
-    def mock_copy_from(dev_path, tmp_dir):
+    def mock_copy_from(dev_path, tmp_dir, **kwargs):
         stub_dir = Path(tmp_dir) / "stubs"
         stub_dir.mkdir()
 
     pyb_mock = mocker.MagicMock(PyDevice, autospec=True)
     pyb_mock.return_value.copy_from = mock_copy_from
     return pyb_mock
```

### Comparing `micropy_cli-4.2.0b2/tests/conftest.py` & `micropy_cli-4.2.0b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/data/archive_test_stub.tar.gz` & `micropy_cli-4.2.0b3/tests/data/archive_test_stub.tar.gz`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/data/esp32_test_stub/frozen/ntptime.py` & `micropy_cli-4.2.0b3/tests/data/esp32_test_stub/frozen/ntptime.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/data/esp32_test_stub/info.json` & `micropy_cli-4.2.0b3/tests/data/esp32_test_stub/info.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/data/esp32_test_stub/stubs/modules.json` & `micropy_cli-4.2.0b3/tests/data/esp32_test_stub/stubs/modules.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/data/esp8266_test_stub/frozen/ntptime.py` & `micropy_cli-4.2.0b3/tests/data/esp8266_test_stub/frozen/ntptime.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/data/esp8266_test_stub/info.json` & `micropy_cli-4.2.0b3/tests/data/esp8266_test_stub/info.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/data/esp8266_test_stub/stubs/modules.json` & `micropy_cli-4.2.0b3/tests/data/esp8266_test_stub/stubs/modules.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/data/fware_test_stub/frozen/utarfile.py` & `micropy_cli-4.2.0b3/tests/data/fware_test_stub/frozen/utarfile.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/data/fware_test_stub/frozen/utarfile.pyi` & `micropy_cli-4.2.0b3/tests/data/fware_test_stub/frozen/utarfile.pyi`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/data/fware_test_stub/frozen/utokenize.py` & `micropy_cli-4.2.0b3/tests/data/fware_test_stub/frozen/utokenize.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/data/fware_test_stub/info.json` & `micropy_cli-4.2.0b3/tests/data/fware_test_stub/info.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/data/project_test/.vscode/settings.json` & `micropy_cli-4.2.0b3/tests/data/project_test/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/data/test_repo.json` & `micropy_cli-4.2.0b3/tests/data/test_repo.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/data/test_source.xml` & `micropy_cli-4.2.0b3/tests/data/test_source.xml`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_config.py` & `micropy_cli-4.2.0b3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_highlevel.py` & `micropy_cli-4.2.0b3/tests/test_highlevel.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_main.py` & `micropy_cli-4.2.0b3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_packages.py` & `micropy_cli-4.2.0b3/tests/test_packages.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_project.py` & `micropy_cli-4.2.0b3/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_pyd.py` & `micropy_cli-4.2.0b3/tests/test_pyd.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
+import hashlib
 import stat
 import sys
 from pathlib import PurePosixPath
 from typing import Literal, Type
 from unittest.mock import ANY, MagicMock
 
 import pytest
 from micropy.exceptions import PyDeviceError
 from micropy.pyd import backend_rshell, backend_upydevice, consumers
-from micropy.pyd.abc import MetaPyDeviceBackend, PyDeviceConsumer
+from micropy.pyd.abc import DevicePath, MetaPyDeviceBackend, PyDeviceConsumer
 from micropy.pyd.pydevice import PyDevice
 from pytest_mock import MockFixture
 
 
 @pytest.fixture
 def mock_upy(mocker: MockFixture):
     mock_upy = mocker.patch.object(backend_upydevice, "upydevice", autospec=True)
@@ -23,14 +24,20 @@
 @pytest.fixture
 def mock_upy_uos(mocker: MockFixture):
     mock_uos = mocker.patch.object(backend_upydevice, "UOS", autospec=True)
     return mock_uos
 
 
 @pytest.fixture
+def mock_upy_retry(mocker: MockFixture):
+    mock_retry = mocker.patch.object(backend_upydevice, "retry", autospec=True)
+    return mock_retry
+
+
+@pytest.fixture
 def mock_rsh(mocker: MockFixture):
     mock_rsh = mocker.patch.object(backend_rshell, "rsh", autospec=True)
     mock_rsh.connect = mocker.Mock()
     mock_rsh.find_serial_device_by_port = mocker.Mock()
     mock_rsh.cp = mocker.Mock()
     return mock_rsh
 
@@ -156,18 +163,15 @@
         m = pymock
         pyd = self.pyd_cls().establish(MOCK_PORT)
         pyd.connect()
         pyd._pydevice.exec_raw = mocker.Mock(return_value=["", ""])
         pyd.eval("abc", **with_consumer)
         has_cons = "consumer" in with_consumer
         if m.is_upy:
-            if has_cons:
-                m.device.cmd.assert_called_once_with("abc", follow=True, pipe=mocker.ANY)
-            else:
-                m.device.cmd.assert_called_once_with("abc")
+            m.device.cmd.assert_called_once_with("abc", follow=True, pipe=mocker.ANY)
         else:
             if has_cons:
                 pyd._pydevice.exec_raw.assert_called_once_with("abc", data_consumer=mocker.ANY)
             else:
                 pyd._pydevice.exec_raw.assert_called_once_with("abc", data_consumer=None)
 
     def test_eval_script(self, pymock, mocker: MockFixture, with_consumer):
@@ -196,30 +200,113 @@
             0,  # pos
             b"Hi there",  # read,
             8,  # pos
             None,  # close
         ]
         return cmd_effects
 
-    def test_read_file(self, pymock):
+    def test_read_file(self, mock_upy_retry, pymock):
         m = pymock
         if m.is_rsh:
+            # upy only
             return
+        # content size
+        m.mock_uos.return_value.stat.side_effect = ["ENOENT", [0, 0, 0, 0, 0, 0, 8]]
+        # chunk size will default to 8/4
+        m.device.cmd.side_effect = [8, b"Hi", b" t", b"he", b"re"]
         pyd = self.pyd_cls().establish(MOCK_PORT)
-        m.device.cmd.side_effect = self.read_file_effects
-        res = pyd.read_file("/some/path")
+        res = pyd.read_file("/some/path", verify_integrity=False)
         assert res == "Hi there"
+        mock_upy_retry.assert_not_called()
+        assert m.device.cmd.call_count == 5
 
-    def test_pull_file(self, pymock, tmp_path):
+    def test_read_file__with_integrity(self, mock_upy_retry, pymock):
+        m = pymock
+        if m.is_rsh:
+            # upy only
+            return
+        # content size
+        m.mock_uos.return_value.stat.side_effect = ["ENOENT", [0, 0, 0, 0, 0, 0, 8]]
+        # chunk size will default to 8/4
+        chunks = [b"Hi", b" t", b"he", b"re"]
+        chunks_hash = hashlib.sha256()
+        for chunk in chunks:
+            chunks_hash.update(chunk)
+        m.device.cmd.side_effect = [8, *chunks, chunks_hash.hexdigest()]
+        pyd = self.pyd_cls().establish(MOCK_PORT)
+        res = pyd.read_file("/some/path", verify_integrity=True)
+        assert res == "Hi there"
+        mock_upy_retry.assert_not_called()
+        assert m.device.cmd.call_count == 6
+
+    def test_read_file__with_integrity_fail(self, mock_upy_retry, pymock, mocker: MockFixture):
+        m = pymock
+        if m.is_rsh:
+            # upy only
+            return
+        # content size
+        m.mock_uos.return_value.stat.side_effect = ["ENOENT", [0, 0, 0, 0, 0, 0, 8]]
+        # chunk size will default to 8/4
+        chunks = [b"Hi", b" t", b"he", b"re"]
+        m.device.cmd.side_effect = [8, *chunks, "notrightsha"]
+        reset_mock = mocker.MagicMock()
+        pyd = self.pyd_cls().establish(MOCK_PORT)
+        pyd.reset = reset_mock
+        pyd.read_file("/some/path", verify_integrity=True)
+        assert reset_mock.call_count == 4
+        assert m.device.cmd.call_count == 6
+
+    def test_read_file__bad_chunk(self, mock_upy_retry, pymock, mocker: MockFixture):
+        m = pymock
+        if m.is_rsh:
+            # upy only
+            return
+        # content size
+        m.mock_uos.return_value.stat.side_effect = ["ENOENT", [0, 0, 0, 0, 0, 0, 8]]
+        # chunk size will default to 8/4
+        chunks = [b"Hi", b"", b" t", b"he", b"re"]
+        m.device.cmd.side_effect = [8, *chunks]
+        m.mock.Device.return_value.reset = mocker.MagicMock(return_value=None)
+        pyd = self.pyd_cls().establish(MOCK_PORT)
+        res = pyd.read_file("/some/path", verify_integrity=False)
+        assert res == "Hi there"
+        mock_upy_retry.assert_not_called()
+        assert m.device.cmd.call_count == 6
+        assert m.mock.Device.return_value.reset.call_count == 1
+
+    def test_read_file__error_chunk(self, mock_upy_retry, pymock, mocker: MockFixture):
+        m = pymock
+        if m.is_rsh:
+            # upy only
+            return
+        # content size
+        m.mock_uos.return_value.stat.side_effect = ["ENOENT", [0, 0, 0, 0, 0, 0, 8]]
+        # chunk size will default to 8/4
+        chunks = [b"Hi", RuntimeError, b" t", b"he", b"re"]
+        m.device.cmd.side_effect = [8, *chunks]
+        reset_mock = mocker.MagicMock()
+        pyd = self.pyd_cls().establish(MOCK_PORT)
+        pyd.reset = reset_mock
+        pyd.read_file("/some/path", verify_integrity=True)
+        assert reset_mock.call_count == 5
+        assert m.device.cmd.call_count == 4
+
+    def test_pull_file(self, pymock, tmp_path, mock_upy_retry):
         m = pymock
         pyd = self.pyd_cls().establish(MOCK_PORT)
         pyd.connect()
         if m.is_upy:
-            m.device.cmd.side_effect = self.read_file_effects
-            pyd.pull_file("/some/path", (tmp_path / "out.txt"))
+            m.mock_uos.return_value.stat.side_effect = [
+                "ENOENT",  # resolve root
+                "ENOENT",  # resolve root
+                [0, 0, 0, 0, 0, 0, 8],
+            ]
+            # chunk size will default to 8/4
+            m.device.cmd.side_effect = [8, b"Hi", b" t", b"he", b"re"]
+            pyd.pull_file("/some/path", (tmp_path / "out.txt"), verify_integrity=False)
             assert (tmp_path / "out.txt").read_text() == "Hi there"
         else:
             m.mock.find_serial_device_by_port.return_value.name_path = "/"
             pyd.pull_file("/some/path", (tmp_path / "out.txt"))
             m.mock.cp.assert_called_once_with("/some/path", str(tmp_path / "out.txt"))
 
     def test_iter_files(self, pymock):
@@ -295,33 +382,65 @@
 
     def test_copy_from(self, mock_backend, path_type, mocker):
         pyd = PyDevice(MOCK_PORT, backend=mock_backend)
         ptype, p = path_type
         pyd.copy_from(p, "/host/path")
         if ptype == "dir":
             mock_backend.return_value.copy_dir.assert_called_once_with(
-                p, "/host/path", consumer=mocker.ANY
+                p,
+                "/host/path",
+                consumer=mocker.ANY,
+                verify_integrity=mocker.ANY,
+                exclude_integrity=None,
+            )
+        else:
+            mock_backend.return_value.pull_file.assert_called_once_with(
+                p,
+                "/host/path",
+                consumer=mocker.ANY,
+                verify_integrity=mocker.ANY,
+            )
+
+    def test_copy_from__integrity(self, mock_backend, path_type, mocker):
+        pyd = PyDevice(MOCK_PORT, backend=mock_backend)
+        ptype, p = path_type
+        if ptype == "dir":
+            pyd.copy_from(p, "/host/path", verify_integrity=True, exclude_integrity={"abc.py"})
+        else:
+            pyd.copy_from(p, "/host/path", verify_integrity=True)
+        if ptype == "dir":
+            mock_backend.return_value.copy_dir.assert_called_once_with(
+                p,
+                "/host/path",
+                consumer=mocker.ANY,
+                verify_integrity=True,
+                exclude_integrity={"abc.py"},
             )
         else:
             mock_backend.return_value.pull_file.assert_called_once_with(
-                p, "/host/path", consumer=mocker.ANY
+                p, "/host/path", consumer=mocker.ANY, verify_integrity=True
             )
 
     def test_copy_to(self, mock_backend, path_type, mocker):
         pyd = PyDevice(MOCK_PORT, backend=mock_backend)
         ptype, p = path_type
         if ptype == "dir":
             with pytest.raises(RuntimeError):
                 pyd.copy_to("/host/path", p)
         else:
             pyd.copy_to("/host/path/f.txt", p)
             mock_backend.return_value.push_file.assert_called_once_with(
                 "/host/path/f.txt", p, consumer=mocker.ANY
             )
 
+    def test_remove(self, mock_backend):
+        pyd = PyDevice(MOCK_PORT, backend=mock_backend)
+        pyd.remove(DevicePath("/some/path"))
+        mock_backend.return_value.remove.assert_called_once_with("/some/path")
+
 
 class TestConsumers:
     @pytest.mark.parametrize(
         "on_desc,expected_tqdm",
         [
             [None, dict(total=5, unit="B", unit_scale=True, unit_divisor=1024, bar_format=ANY)],
             [
```

### Comparing `micropy_cli-4.2.0b2/tests/test_stub_source.py` & `micropy_cli-4.2.0b3/tests/test_stub_source.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_stubs/esp32_test_stub/frozen/ntptime.py` & `micropy_cli-4.2.0b3/tests/test_stubs/esp32_test_stub/frozen/ntptime.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_stubs/esp32_test_stub/info.json` & `micropy_cli-4.2.0b3/tests/test_stubs/esp32_test_stub/info.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_stubs/esp32_test_stub/stubs/modules.json` & `micropy_cli-4.2.0b3/tests/test_stubs/esp32_test_stub/stubs/modules.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_stubs/esp8266_test_stub/frozen/ntptime.py` & `micropy_cli-4.2.0b3/tests/test_stubs/esp8266_test_stub/frozen/ntptime.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_stubs/esp8266_test_stub/info.json` & `micropy_cli-4.2.0b3/tests/test_stubs/esp8266_test_stub/info.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_stubs/esp8266_test_stub/stubs/modules.json` & `micropy_cli-4.2.0b3/tests/test_stubs/esp8266_test_stub/stubs/modules.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_stubs.py` & `micropy_cli-4.2.0b3/tests/test_stubs.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_stubs_repo.py` & `micropy_cli-4.2.0b3/tests/test_stubs_repo.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_template.py` & `micropy_cli-4.2.0b3/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_utils/schema.json` & `micropy_cli-4.2.0b3/tests/test_utils/schema.json`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/tests/test_utils.py` & `micropy_cli-4.2.0b3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `micropy_cli-4.2.0b2/PKG-INFO` & `micropy_cli-4.2.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropy-cli
-Version: 4.2.0b2
+Version: 4.2.0b3
 Summary: Micropython Project Management Tool with VSCode support, Linting, Intellisense, Dependency Management, and more!
 Home-page: https://github.com/BradenM/micropy-cli
 License: MIT
 Keywords: micropython,stubs,linting,vscode,intellisense
 Author: Braden Mars
 Author-email: bradenmars@bradenmars.me
 Requires-Python: >=3.8,<3.12
@@ -42,15 +42,15 @@
 Requires-Dist: python-minifier (==2.8.1)
 Requires-Dist: questionary (==1.10.0)
 Requires-Dist: requests (==2.28.2)
 Requires-Dist: requirements-parser (==0.2.0)
 Requires-Dist: rshell (>=0.0.31,<0.0.32) ; python_version < "3.10" and sys_platform == "win32"
 Requires-Dist: rshell (>=0.0.31,<0.0.32) ; sys_platform != "win32"
 Requires-Dist: tqdm (==4.65.0)
-Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Requires-Dist: typer[all] (==0.7.0)
 Requires-Dist: typing-extensions (==4.5.0)
 Requires-Dist: upydevice (==0.3.8)
 Project-URL: Documentation, https://micropy-cli.readthedocs.io
 Project-URL: Repository, https://github.com/BradenM/micropy-cli
 Description-Content-Type: text/markdown
 
 # Micropy Cli [![PyPI][pypi-img]][pypi-url] [![PyPI - Python Version][pypiv-img]][pypi-url] [![Github - Test Micropy Cli][build-img]][build-url] [![Coverage Status][cover-img]][cover-url]
```

