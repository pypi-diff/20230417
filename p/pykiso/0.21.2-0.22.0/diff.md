# Comparing `tmp/pykiso-0.21.2.tar.gz` & `tmp/pykiso-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykiso-0.21.2.tar", max compression
+gzip compressed data, was "pykiso-0.22.0.tar", max compression
```

## Comparing `pykiso-0.21.2.tar` & `pykiso-0.22.0.tar`

### file list

```diff
@@ -1,110 +1,112 @@
--rw-r--r--   0        0        0    14194 2023-02-09 10:51:23.525275 pykiso-0.21.2/LICENSE
--rw-r--r--   0        0        0     5740 2023-02-09 10:51:23.525275 pykiso-0.21.2/README.md
--rw-r--r--   0        0        0     3545 2023-02-09 10:51:23.635275 pykiso-0.21.2/pyproject.toml
--rw-r--r--   0        0        0     1921 2023-02-09 10:51:23.635275 pykiso-0.21.2/src/pykiso/__init__.py
--rw-r--r--   0        0        0      642 2023-02-09 10:51:23.720275 pykiso-0.21.2/src/pykiso/__main__.py
--rw-r--r--   0        0        0     9480 2023-02-09 10:51:23.720275 pykiso-0.21.2/src/pykiso/auxiliary.py
--rw-r--r--   0        0        0     7193 2023-02-09 10:51:23.720275 pykiso-0.21.2/src/pykiso/cli.py
--rw-r--r--   0        0        0    11837 2023-02-09 10:51:23.721275 pykiso-0.21.2/src/pykiso/config_parser.py
--rw-r--r--   0        0        0     5559 2023-02-09 10:51:23.721275 pykiso-0.21.2/src/pykiso/connector.py
--rw-r--r--   0        0        0     2436 2023-02-09 10:51:23.721275 pykiso-0.21.2/src/pykiso/exceptions.py
--rw-r--r--   0        0        0     4509 2023-02-09 10:51:23.721275 pykiso-0.21.2/src/pykiso/global_config.py
--rw-r--r--   0        0        0      410 2023-02-09 10:51:23.721275 pykiso-0.21.2/src/pykiso/interfaces/__init__.py
--rw-r--r--   0        0        0    13651 2023-02-09 10:51:23.721275 pykiso-0.21.2/src/pykiso/interfaces/dt_auxiliary.py
--rw-r--r--   0        0        0     8975 2023-02-09 10:51:23.722276 pykiso-0.21.2/src/pykiso/interfaces/mp_auxiliary.py
--rw-r--r--   0        0        0     4318 2023-02-09 10:51:23.722276 pykiso-0.21.2/src/pykiso/interfaces/simple_auxiliary.py
--rw-r--r--   0        0        0     8665 2023-02-09 10:51:23.722276 pykiso-0.21.2/src/pykiso/interfaces/thread_auxiliary.py
--rw-r--r--   0        0        0      516 2023-02-09 10:51:23.722276 pykiso-0.21.2/src/pykiso/lib/__init__.py
--rw-r--r--   0        0        0      552 2023-02-09 10:51:23.723276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/__init__.py
--rw-r--r--   0        0        0     8415 2023-02-09 10:51:23.723276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/acroname_auxiliary.py
--rw-r--r--   0        0        0     7916 2023-02-09 10:51:23.723276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/communication_auxiliary.py
--rw-r--r--   0        0        0    12655 2023-02-09 10:51:23.723276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/dut_auxiliary.py
--rw-r--r--   0        0        0     2014 2023-02-09 10:51:23.723276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/__init__.py
--rw-r--r--   0        0        0    10145 2023-02-09 10:51:23.724275 pykiso-0.21.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_auxiliary.py
--rw-r--r--   0        0        0    19216 2023-02-09 10:51:23.724275 pykiso-0.21.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_cli.py
--rw-r--r--   0        0        0     5029 2023-02-09 10:51:23.724275 pykiso-0.21.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_instruments.py
--rw-r--r--   0        0        0    16676 2023-02-09 10:51:23.724275 pykiso-0.21.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_scpi_commands.py
--rw-r--r--   0        0        0    14219 2023-02-09 10:51:23.724275 pykiso-0.21.2/src/pykiso/lib/auxiliaries/mp_proxy_auxiliary.py
--rw-r--r--   0        0        0    12009 2023-02-09 10:51:23.725276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/proxy_auxiliary.py
--rw-r--r--   0        0        0    17111 2023-02-09 10:51:23.725276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/record_auxiliary.py
--rw-r--r--   0        0        0     2645 2023-02-09 10:51:23.725276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/__init__.py
--rw-r--r--   0        0        0     6511 2023-02-09 10:51:23.725276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/response_templates.py
--rw-r--r--   0        0        0    14146 2023-02-09 10:51:23.726276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/scenario.py
--rw-r--r--   0        0        0     3889 2023-02-09 10:51:23.726276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulated_auxiliary.py
--rw-r--r--   0        0        0     4288 2023-02-09 10:51:23.726276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulation.py
--rw-r--r--   0        0        0      718 2023-02-09 10:51:23.726276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/__init__.py
--rw-r--r--   0        0        0      599 2023-02-09 10:51:23.726276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/common/__init__.py
--rw-r--r--   0        0        0     5284 2023-02-09 10:51:23.726276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_base_auxiliary.py
--rw-r--r--   0        0        0    12677 2023-02-09 10:51:23.726276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_callback.py
--rw-r--r--   0        0        0     1517 2023-02-09 10:51:23.727275 pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_exceptions.py
--rw-r--r--   0        0        0     1570 2023-02-09 10:51:23.727275 pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_request.py
--rw-r--r--   0        0        0     2664 2023-02-09 10:51:23.727275 pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_response.py
--rw-r--r--   0        0        0     1404 2023-02-09 10:51:23.727275 pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_utils.py
--rw-r--r--   0        0        0    12568 2023-02-09 10:51:23.727275 pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/uds_auxiliary.py
--rw-r--r--   0        0        0    11194 2023-02-09 10:51:23.727275 pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/uds_server_auxiliary.py
--rw-r--r--   0        0        0    13528 2023-02-09 10:51:23.728276 pykiso-0.21.2/src/pykiso/lib/auxiliaries/ykush_auxiliary.py
--rw-r--r--   0        0        0      548 2023-02-09 10:51:23.728276 pykiso-0.21.2/src/pykiso/lib/connectors/__init__.py
--rw-r--r--   0        0        0     3999 2023-02-09 10:51:23.728276 pykiso-0.21.2/src/pykiso/lib/connectors/cc_example.py
--rw-r--r--   0        0        0    13274 2023-02-09 10:51:23.728276 pykiso-0.21.2/src/pykiso/lib/connectors/cc_fdx_lauterbach.py
--rw-r--r--   0        0        0     1446 2023-02-09 10:51:23.728276 pykiso-0.21.2/src/pykiso/lib/connectors/cc_flasher_example.py
--rw-r--r--   0        0        0     4804 2023-02-09 10:51:23.729276 pykiso-0.21.2/src/pykiso/lib/connectors/cc_mp_proxy.py
--rw-r--r--   0        0        0    14164 2023-02-09 10:51:23.729276 pykiso-0.21.2/src/pykiso/lib/connectors/cc_pcan_can.py
--rw-r--r--   0        0        0    11002 2023-02-09 10:51:23.729276 pykiso-0.21.2/src/pykiso/lib/connectors/cc_process.py
--rw-r--r--   0        0        0     5019 2023-02-09 10:51:23.729276 pykiso-0.21.2/src/pykiso/lib/connectors/cc_proxy.py
--rw-r--r--   0        0        0     2048 2023-02-09 10:51:23.729276 pykiso-0.21.2/src/pykiso/lib/connectors/cc_raw_loopback.py
--rw-r--r--   0        0        0    14011 2023-02-09 10:51:23.730275 pykiso-0.21.2/src/pykiso/lib/connectors/cc_rtt_segger.py
--rw-r--r--   0        0        0     5547 2023-02-09 10:51:23.730275 pykiso-0.21.2/src/pykiso/lib/connectors/cc_serial.py
--rw-r--r--   0        0        0      538 2023-02-09 10:51:23.730275 pykiso-0.21.2/src/pykiso/lib/connectors/cc_socket_can/__init__.py
--rw-r--r--   0        0        0     7195 2023-02-09 10:51:23.730275 pykiso-0.21.2/src/pykiso/lib/connectors/cc_socket_can/cc_socket_can.py
--rw-r--r--   0        0        0     7903 2023-02-09 10:51:23.731276 pykiso-0.21.2/src/pykiso/lib/connectors/cc_socket_can/socketcan_to_trc.py
--rw-r--r--   0        0        0     3215 2023-02-09 10:51:23.731276 pykiso-0.21.2/src/pykiso/lib/connectors/cc_tcp_ip.py
--rw-r--r--   0        0        0     5729 2023-02-09 10:51:23.731276 pykiso-0.21.2/src/pykiso/lib/connectors/cc_uart.py
--rw-r--r--   0        0        0     2981 2023-02-09 10:51:23.731276 pykiso-0.21.2/src/pykiso/lib/connectors/cc_udp.py
--rw-r--r--   0        0        0     3425 2023-02-09 10:51:23.731276 pykiso-0.21.2/src/pykiso/lib/connectors/cc_udp_server.py
--rw-r--r--   0        0        0     2276 2023-02-09 10:51:23.731276 pykiso-0.21.2/src/pykiso/lib/connectors/cc_usb.py
--rw-r--r--   0        0        0     7128 2023-02-09 10:51:23.731276 pykiso-0.21.2/src/pykiso/lib/connectors/cc_vector_can.py
--rw-r--r--   0        0        0     7019 2023-02-09 10:51:23.732276 pykiso-0.21.2/src/pykiso/lib/connectors/cc_visa.py
--rw-r--r--   0        0        0     3918 2023-02-09 10:51:23.732276 pykiso-0.21.2/src/pykiso/lib/connectors/flash_jlink.py
--rw-r--r--   0        0        0     8380 2023-02-09 10:51:23.732276 pykiso-0.21.2/src/pykiso/lib/connectors/flash_lauterbach.py
--rw-r--r--   0        0        0      530 2023-02-09 10:51:23.732276 pykiso-0.21.2/src/pykiso/lib/robot_framework/__init__.py
--rw-r--r--   0        0        0     4193 2023-02-09 10:51:23.732276 pykiso-0.21.2/src/pykiso/lib/robot_framework/acroname_auxiliary.py
--rw-r--r--   0        0        0     2380 2023-02-09 10:51:23.732276 pykiso-0.21.2/src/pykiso/lib/robot_framework/aux_interface.py
--rw-r--r--   0        0        0     3361 2023-02-09 10:51:23.733276 pykiso-0.21.2/src/pykiso/lib/robot_framework/communication_auxiliary.py
--rw-r--r--   0        0        0     3639 2023-02-09 10:51:23.733276 pykiso-0.21.2/src/pykiso/lib/robot_framework/dut_auxiliary.py
--rw-r--r--   0        0        0    16126 2023-02-09 10:51:23.733276 pykiso-0.21.2/src/pykiso/lib/robot_framework/instrument_control_auxiliary.py
--rw-r--r--   0        0        0     3599 2023-02-09 10:51:23.733276 pykiso-0.21.2/src/pykiso/lib/robot_framework/loader.py
--rw-r--r--   0        0        0     2321 2023-02-09 10:51:23.733276 pykiso-0.21.2/src/pykiso/lib/robot_framework/proxy_auxiliary.py
--rw-r--r--   0        0        0     6606 2023-02-09 10:51:23.733276 pykiso-0.21.2/src/pykiso/lib/robot_framework/record_auxiliary.py
--rw-r--r--   0        0        0     6840 2023-02-09 10:51:23.734276 pykiso-0.21.2/src/pykiso/lib/robot_framework/uds_auxiliary.py
--rw-r--r--   0        0        0     7620 2023-02-09 10:51:23.734276 pykiso-0.21.2/src/pykiso/logging_initializer.py
--rw-r--r--   0        0        0    11744 2023-02-09 10:51:23.734276 pykiso-0.21.2/src/pykiso/message.py
--rw-r--r--   0        0        0      410 2023-02-09 10:51:23.734276 pykiso-0.21.2/src/pykiso/test_coordinator/__init__.py
--rw-r--r--   0        0        0    13097 2023-02-09 10:51:23.734276 pykiso-0.21.2/src/pykiso/test_coordinator/test_case.py
--rw-r--r--   0        0        0    15437 2023-02-09 10:51:23.735276 pykiso-0.21.2/src/pykiso/test_coordinator/test_execution.py
--rw-r--r--   0        0        0     5480 2023-02-09 10:51:23.735276 pykiso-0.21.2/src/pykiso/test_coordinator/test_message_handler.py
--rw-r--r--   0        0        0    16859 2023-02-09 10:51:23.735276 pykiso-0.21.2/src/pykiso/test_coordinator/test_suite.py
--rw-r--r--   0        0        0      515 2023-02-09 10:51:23.736276 pykiso-0.21.2/src/pykiso/test_result/__init__.py
--rw-r--r--   0        0        0    15559 2023-02-09 10:51:23.736276 pykiso-0.21.2/src/pykiso/test_result/assert_step_report.py
--rw-r--r--   0        0        0     1971 2023-02-09 10:51:23.736276 pykiso-0.21.2/src/pykiso/test_result/templates/report_template.css
--rw-r--r--   0        0        0     5351 2023-02-09 10:51:23.823276 pykiso-0.21.2/src/pykiso/test_result/templates/report_template.html.j2
--rw-r--r--   0        0        0     1624 2023-02-09 10:51:23.823276 pykiso-0.21.2/src/pykiso/test_result/templates/report_template_script.js
--rw-r--r--   0        0        0     9917 2023-02-09 10:51:23.823276 pykiso-0.21.2/src/pykiso/test_result/text_result.py
--rw-r--r--   0        0        0     5842 2023-02-09 10:51:23.823276 pykiso-0.21.2/src/pykiso/test_result/xml_result.py
--rw-r--r--   0        0        0      410 2023-02-09 10:51:23.824276 pykiso-0.21.2/src/pykiso/test_setup/__init__.py
--rw-r--r--   0        0        0     9071 2023-02-09 10:51:23.824276 pykiso-0.21.2/src/pykiso/test_setup/config_registry.py
--rw-r--r--   0        0        0    13873 2023-02-09 10:51:23.824276 pykiso-0.21.2/src/pykiso/test_setup/dynamic_loader.py
--rw-r--r--   0        0        0      410 2023-02-09 10:51:23.824276 pykiso-0.21.2/src/pykiso/tool/__init__.py
--rw-r--r--   0        0        0      410 2023-02-09 10:51:23.824276 pykiso-0.21.2/src/pykiso/tool/pykiso_to_pytest/__init__.py
--rw-r--r--   0        0        0     5577 2023-02-09 10:51:23.825276 pykiso-0.21.2/src/pykiso/tool/pykiso_to_pytest/cli.py
--rw-r--r--   0        0        0     3114 2023-02-09 10:51:23.825276 pykiso-0.21.2/src/pykiso/tool/pykiso_to_pytest/templates/conftest_template.jinja2
--rw-r--r--   0        0        0    11816 2023-02-09 10:51:23.825276 pykiso-0.21.2/src/pykiso/tool/show_tag.py
--rw-r--r--   0        0        0      410 2023-02-09 10:51:23.825276 pykiso-0.21.2/src/pykiso/tool/testrail/__init__.py
--rw-r--r--   0        0        0    12414 2023-02-09 10:51:23.825276 pykiso-0.21.2/src/pykiso/tool/testrail/api.py
--rw-r--r--   0        0        0     7584 2023-02-09 10:51:23.825276 pykiso-0.21.2/src/pykiso/tool/testrail/cli.py
--rw-r--r--   0        0        0     5195 2023-02-09 10:51:23.826276 pykiso-0.21.2/src/pykiso/tool/testrail/console.py
--rw-r--r--   0        0        0     8545 2023-02-09 10:51:23.826276 pykiso-0.21.2/src/pykiso/tool/testrail/containers.py
--rw-r--r--   0        0        0     5075 2023-02-09 10:51:23.826276 pykiso-0.21.2/src/pykiso/tool/testrail/extraction.py
--rw-r--r--   0        0        0    12851 2023-02-09 10:51:23.826276 pykiso-0.21.2/src/pykiso/tool/testrail/testrail.py
--rw-r--r--   0        0        0     1661 2023-02-09 10:51:23.826276 pykiso-0.21.2/src/pykiso/types.py
--rw-r--r--   0        0        0     8410 1970-01-01 00:00:00.000000 pykiso-0.21.2/setup.py
--rw-r--r--   0        0        0     8312 1970-01-01 00:00:00.000000 pykiso-0.21.2/PKG-INFO
+-rw-r--r--   0        0        0    14194 2023-04-17 14:37:25.523320 pykiso-0.22.0/LICENSE
+-rw-r--r--   0        0        0     6028 2023-04-17 14:37:25.524320 pykiso-0.22.0/README.md
+-rw-r--r--   0        0        0     4289 2023-04-17 14:37:25.725318 pykiso-0.22.0/pyproject.toml
+-rw-r--r--   0        0        0     1972 2023-04-17 14:37:25.725318 pykiso-0.22.0/src/pykiso/__init__.py
+-rw-r--r--   0        0        0      642 2023-04-17 14:37:25.725318 pykiso-0.22.0/src/pykiso/__main__.py
+-rw-r--r--   0        0        0     9480 2023-04-17 14:37:25.725318 pykiso-0.22.0/src/pykiso/auxiliary.py
+-rw-r--r--   0        0        0     7920 2023-04-17 14:37:25.725318 pykiso-0.22.0/src/pykiso/cli.py
+-rw-r--r--   0        0        0    11837 2023-04-17 14:37:25.726318 pykiso-0.22.0/src/pykiso/config_parser.py
+-rw-r--r--   0        0        0     5559 2023-04-17 14:37:25.726318 pykiso-0.22.0/src/pykiso/connector.py
+-rw-r--r--   0        0        0     2436 2023-04-17 14:37:25.726318 pykiso-0.22.0/src/pykiso/exceptions.py
+-rw-r--r--   0        0        0     4509 2023-04-17 14:37:25.726318 pykiso-0.22.0/src/pykiso/global_config.py
+-rw-r--r--   0        0        0      410 2023-04-17 14:37:25.726318 pykiso-0.22.0/src/pykiso/interfaces/__init__.py
+-rw-r--r--   0        0        0    13651 2023-04-17 14:37:25.726318 pykiso-0.22.0/src/pykiso/interfaces/dt_auxiliary.py
+-rw-r--r--   0        0        0     8975 2023-04-17 14:37:25.726318 pykiso-0.22.0/src/pykiso/interfaces/mp_auxiliary.py
+-rw-r--r--   0        0        0     4318 2023-04-17 14:37:25.727318 pykiso-0.22.0/src/pykiso/interfaces/simple_auxiliary.py
+-rw-r--r--   0        0        0     8665 2023-04-17 14:37:25.727318 pykiso-0.22.0/src/pykiso/interfaces/thread_auxiliary.py
+-rw-r--r--   0        0        0      516 2023-04-17 14:37:25.727318 pykiso-0.22.0/src/pykiso/lib/__init__.py
+-rw-r--r--   0        0        0      552 2023-04-17 14:37:25.727318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/__init__.py
+-rw-r--r--   0        0        0     8415 2023-04-17 14:37:25.727318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/acroname_auxiliary.py
+-rw-r--r--   0        0        0     7916 2023-04-17 14:37:25.728318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/communication_auxiliary.py
+-rw-r--r--   0        0        0    12655 2023-04-17 14:37:25.728318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/dut_auxiliary.py
+-rw-r--r--   0        0        0     2014 2023-04-17 14:37:25.728318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/__init__.py
+-rw-r--r--   0        0        0    10145 2023-04-17 14:37:25.728318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_auxiliary.py
+-rw-r--r--   0        0        0    19216 2023-04-17 14:37:25.728318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_cli.py
+-rw-r--r--   0        0        0     5029 2023-04-17 14:37:25.728318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_instruments.py
+-rw-r--r--   0        0        0    16676 2023-04-17 14:37:25.729318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_scpi_commands.py
+-rw-r--r--   0        0        0    14219 2023-04-17 14:37:25.729318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/mp_proxy_auxiliary.py
+-rw-r--r--   0        0        0    14149 2023-04-17 14:37:25.729318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/proxy_auxiliary.py
+-rw-r--r--   0        0        0    17111 2023-04-17 14:37:25.729318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/record_auxiliary.py
+-rw-r--r--   0        0        0     2645 2023-04-17 14:37:25.730318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/__init__.py
+-rw-r--r--   0        0        0     6511 2023-04-17 14:37:25.730318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/response_templates.py
+-rw-r--r--   0        0        0    14146 2023-04-17 14:37:25.730318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/scenario.py
+-rw-r--r--   0        0        0     3889 2023-04-17 14:37:25.730318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulated_auxiliary.py
+-rw-r--r--   0        0        0     4288 2023-04-17 14:37:25.730318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulation.py
+-rw-r--r--   0        0        0      718 2023-04-17 14:37:25.730318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/__init__.py
+-rw-r--r--   0        0        0      599 2023-04-17 14:37:25.731318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/__init__.py
+-rw-r--r--   0        0        0     3913 2023-04-17 14:37:25.731318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/odx_parser.py
+-rw-r--r--   0        0        0     5284 2023-04-17 14:37:25.731318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_base_auxiliary.py
+-rw-r--r--   0        0        0    12896 2023-04-17 14:37:25.731318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_callback.py
+-rw-r--r--   0        0        0     1517 2023-04-17 14:37:25.731318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_exceptions.py
+-rw-r--r--   0        0        0     1570 2023-04-17 14:37:25.731318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_request.py
+-rw-r--r--   0        0        0     2664 2023-04-17 14:37:25.731318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_response.py
+-rw-r--r--   0        0        0     1404 2023-04-17 14:37:25.731318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_utils.py
+-rw-r--r--   0        0        0    12733 2023-04-17 14:37:25.732318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/uds_auxiliary.py
+-rw-r--r--   0        0        0    17074 2023-04-17 14:37:25.732318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/uds_server_auxiliary.py
+-rw-r--r--   0        0        0    13528 2023-04-17 14:37:25.732318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/ykush_auxiliary.py
+-rw-r--r--   0        0        0      548 2023-04-17 14:37:25.732318 pykiso-0.22.0/src/pykiso/lib/connectors/__init__.py
+-rw-r--r--   0        0        0     3999 2023-04-17 14:37:25.732318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_example.py
+-rw-r--r--   0        0        0    13274 2023-04-17 14:37:25.732318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_fdx_lauterbach.py
+-rw-r--r--   0        0        0     1446 2023-04-17 14:37:25.815317 pykiso-0.22.0/src/pykiso/lib/connectors/cc_flasher_example.py
+-rw-r--r--   0        0        0     4966 2023-04-17 14:37:25.816318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_mp_proxy.py
+-rw-r--r--   0        0        0    19974 2023-04-17 14:37:25.816318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_pcan_can.py
+-rw-r--r--   0        0        0    11002 2023-04-17 14:37:25.816318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_process.py
+-rw-r--r--   0        0        0     5697 2023-04-17 14:37:25.816318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_proxy.py
+-rw-r--r--   0        0        0     2048 2023-04-17 14:37:25.816318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_raw_loopback.py
+-rw-r--r--   0        0        0    14178 2023-04-17 14:37:25.817318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_rtt_segger.py
+-rw-r--r--   0        0        0     5713 2023-04-17 14:37:25.817318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_serial.py
+-rw-r--r--   0        0        0      538 2023-04-17 14:37:25.817318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_socket_can/__init__.py
+-rw-r--r--   0        0        0     7361 2023-04-17 14:37:25.817318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_socket_can/cc_socket_can.py
+-rw-r--r--   0        0        0     8065 2023-04-17 14:37:25.817318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_socket_can/socketcan_to_trc.py
+-rw-r--r--   0        0        0     3215 2023-04-17 14:37:25.818318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_tcp_ip.py
+-rw-r--r--   0        0        0     5893 2023-04-17 14:37:25.818318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_uart.py
+-rw-r--r--   0        0        0     2981 2023-04-17 14:37:25.818318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_udp.py
+-rw-r--r--   0        0        0     3425 2023-04-17 14:37:25.818318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_udp_server.py
+-rw-r--r--   0        0        0     2440 2023-04-17 14:37:25.818318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_usb.py
+-rw-r--r--   0        0        0     7302 2023-04-17 14:37:25.818318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_vector_can.py
+-rw-r--r--   0        0        0     7194 2023-04-17 14:37:25.818318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_visa.py
+-rw-r--r--   0        0        0     4085 2023-04-17 14:37:25.818318 pykiso-0.22.0/src/pykiso/lib/connectors/flash_jlink.py
+-rw-r--r--   0        0        0     8380 2023-04-17 14:37:25.819317 pykiso-0.22.0/src/pykiso/lib/connectors/flash_lauterbach.py
+-rw-r--r--   0        0        0      530 2023-04-17 14:37:25.819317 pykiso-0.22.0/src/pykiso/lib/robot_framework/__init__.py
+-rw-r--r--   0        0        0     4193 2023-04-17 14:37:25.819317 pykiso-0.22.0/src/pykiso/lib/robot_framework/acroname_auxiliary.py
+-rw-r--r--   0        0        0     2380 2023-04-17 14:37:25.819317 pykiso-0.22.0/src/pykiso/lib/robot_framework/aux_interface.py
+-rw-r--r--   0        0        0     3361 2023-04-17 14:37:25.819317 pykiso-0.22.0/src/pykiso/lib/robot_framework/communication_auxiliary.py
+-rw-r--r--   0        0        0     3639 2023-04-17 14:37:25.819317 pykiso-0.22.0/src/pykiso/lib/robot_framework/dut_auxiliary.py
+-rw-r--r--   0        0        0    16126 2023-04-17 14:37:25.820318 pykiso-0.22.0/src/pykiso/lib/robot_framework/instrument_control_auxiliary.py
+-rw-r--r--   0        0        0     3599 2023-04-17 14:37:25.820318 pykiso-0.22.0/src/pykiso/lib/robot_framework/loader.py
+-rw-r--r--   0        0        0     2321 2023-04-17 14:37:25.820318 pykiso-0.22.0/src/pykiso/lib/robot_framework/proxy_auxiliary.py
+-rw-r--r--   0        0        0     6606 2023-04-17 14:37:25.820318 pykiso-0.22.0/src/pykiso/lib/robot_framework/record_auxiliary.py
+-rw-r--r--   0        0        0     6840 2023-04-17 14:37:25.820318 pykiso-0.22.0/src/pykiso/lib/robot_framework/uds_auxiliary.py
+-rw-r--r--   0        0        0     7770 2023-04-17 14:37:25.820318 pykiso-0.22.0/src/pykiso/logging_initializer.py
+-rw-r--r--   0        0        0    11744 2023-04-17 14:37:25.821318 pykiso-0.22.0/src/pykiso/message.py
+-rw-r--r--   0        0        0      410 2023-04-17 14:37:25.821318 pykiso-0.22.0/src/pykiso/test_coordinator/__init__.py
+-rw-r--r--   0        0        0    12735 2023-04-17 14:37:25.821318 pykiso-0.22.0/src/pykiso/test_coordinator/test_case.py
+-rw-r--r--   0        0        0    16086 2023-04-17 14:37:25.821318 pykiso-0.22.0/src/pykiso/test_coordinator/test_execution.py
+-rw-r--r--   0        0        0     5480 2023-04-17 14:37:25.821318 pykiso-0.22.0/src/pykiso/test_coordinator/test_message_handler.py
+-rw-r--r--   0        0        0    16859 2023-04-17 14:37:25.822317 pykiso-0.22.0/src/pykiso/test_coordinator/test_suite.py
+-rw-r--r--   0        0        0      515 2023-04-17 14:37:25.822317 pykiso-0.22.0/src/pykiso/test_result/__init__.py
+-rw-r--r--   0        0        0    16836 2023-04-17 14:37:25.822317 pykiso-0.22.0/src/pykiso/test_result/assert_step_report.py
+-rw-r--r--   0        0        0     8391 2023-04-17 14:37:25.822317 pykiso-0.22.0/src/pykiso/test_result/multi_result.py
+-rw-r--r--   0        0        0     1971 2023-04-17 14:37:25.822317 pykiso-0.22.0/src/pykiso/test_result/templates/report_template.css
+-rw-r--r--   0        0        0     5461 2023-04-17 14:37:25.823317 pykiso-0.22.0/src/pykiso/test_result/templates/report_template.html.j2
+-rw-r--r--   0        0        0     1624 2023-04-17 14:37:25.823317 pykiso-0.22.0/src/pykiso/test_result/templates/report_template_script.js
+-rw-r--r--   0        0        0     9917 2023-04-17 14:37:25.823317 pykiso-0.22.0/src/pykiso/test_result/text_result.py
+-rw-r--r--   0        0        0     5663 2023-04-17 14:37:25.823317 pykiso-0.22.0/src/pykiso/test_result/xml_result.py
+-rw-r--r--   0        0        0      410 2023-04-17 14:37:25.823317 pykiso-0.22.0/src/pykiso/test_setup/__init__.py
+-rw-r--r--   0        0        0     9772 2023-04-17 14:37:25.823317 pykiso-0.22.0/src/pykiso/test_setup/config_registry.py
+-rw-r--r--   0        0        0    14160 2023-04-17 14:37:25.824318 pykiso-0.22.0/src/pykiso/test_setup/dynamic_loader.py
+-rw-r--r--   0        0        0      410 2023-04-17 14:37:25.824318 pykiso-0.22.0/src/pykiso/tool/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-17 14:37:25.824318 pykiso-0.22.0/src/pykiso/tool/pykiso_to_pytest/__init__.py
+-rw-r--r--   0        0        0     5577 2023-04-17 14:37:25.824318 pykiso-0.22.0/src/pykiso/tool/pykiso_to_pytest/cli.py
+-rw-r--r--   0        0        0     3114 2023-04-17 14:37:25.824318 pykiso-0.22.0/src/pykiso/tool/pykiso_to_pytest/templates/conftest_template.jinja2
+-rw-r--r--   0        0        0    11816 2023-04-17 14:37:25.824318 pykiso-0.22.0/src/pykiso/tool/show_tag.py
+-rw-r--r--   0        0        0      410 2023-04-17 14:37:25.824318 pykiso-0.22.0/src/pykiso/tool/testrail/__init__.py
+-rw-r--r--   0        0        0    12414 2023-04-17 14:37:25.825317 pykiso-0.22.0/src/pykiso/tool/testrail/api.py
+-rw-r--r--   0        0        0     7584 2023-04-17 14:37:25.825317 pykiso-0.22.0/src/pykiso/tool/testrail/cli.py
+-rw-r--r--   0        0        0     5195 2023-04-17 14:37:25.825317 pykiso-0.22.0/src/pykiso/tool/testrail/console.py
+-rw-r--r--   0        0        0     8545 2023-04-17 14:37:25.825317 pykiso-0.22.0/src/pykiso/tool/testrail/containers.py
+-rw-r--r--   0        0        0     5075 2023-04-17 14:37:25.825317 pykiso-0.22.0/src/pykiso/tool/testrail/extraction.py
+-rw-r--r--   0        0        0    12851 2023-04-17 14:37:25.825317 pykiso-0.22.0/src/pykiso/tool/testrail/testrail.py
+-rw-r--r--   0        0        0     1794 2023-04-17 14:37:25.825317 pykiso-0.22.0/src/pykiso/types.py
+-rw-r--r--   0        0        0     9371 1970-01-01 00:00:00.000000 pykiso-0.22.0/setup.py
+-rw-r--r--   0        0        0     9260 1970-01-01 00:00:00.000000 pykiso-0.22.0/PKG-INFO
```

### Comparing `pykiso-0.21.2/LICENSE` & `pykiso-0.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/README.md` & `pykiso-0.22.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [![License](https://img.shields.io/badge/Licence-Eclipse%20Public%20License%202.0-lightgrey)](https://opensource.org/licenses/EPL-2.0)
 [![Platforms](https://img.shields.io/badge/Platforms-win64%20linux64%20osx64-lightgrey)]()
 [![Supported python version](https://img.shields.io/pypi/pyversions/pykiso)]()
 [![Build status](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fci.eclipse.org%2Fkiso-testing%2Fjob%2Fkiso-testing%2Fjob%2Fmaster%2F)](https://ci.eclipse.org/kiso-testing/job/kiso-testing/job/master/)
 [![Documentation Status](https://readthedocs.org/projects/kiso-testing/badge/?version=latest)](https://kiso-testing.readthedocs.io/en/latest/?badge=latest)
 [![Test results](https://img.shields.io/jenkins/tests?compact_message&failed_label=failed&jobUrl=https%3A%2F%2Fci.eclipse.org%2Fkiso-testing%2Fjob%2Fkiso-testing%2Fjob%2Fmaster%2F&passed_label=passed&skipped_label=skipped)](https://ci.eclipse.org/kiso-testing/job/kiso-testing/job/master/)
 [![codecov](https://codecov.io/gh/eclipse/kiso-testing/branch/master/graph/badge.svg?token=IBKQ700ABS)](https://codecov.io/gh/eclipse/kiso-testing)
-[![Code quality](https://img.shields.io/lgtm/grade/python/github/eclipse/kiso-testing)]()
+[![CodeFactor](https://www.codefactor.io/repository/github/eclipse/kiso-testing/badge)](https://www.codefactor.io/repository/github/eclipse/kiso-testing)
 [![Last commit](https://img.shields.io/github/last-commit/eclipse/kiso-testing)]()
 [![Commits since latest version](https://img.shields.io/github/commits-since/eclipse/kiso-testing/latest/master)]()
 
 # PyKiso
 
 ![Optional Text](./docs/images/pykiso_logo.png)
 
@@ -21,23 +21,28 @@
 * Blackbox integration tests to make sure my external device interfaces are working as expected
 
 The project will contain:
 * The core python framework (this repository)
 * Framework plugins that are generic enough to be integrated as "native" (this repository)
 * Additional "testApps" for different targets platforms (e.g. stm32, ...) or languages (C, C++, ...) . It could be pure SW or also HW (other repositories)
 
+## Link to Eclipse Project
+https://projects.eclipse.org/projects/iot.kiso-testing
+
 ## Requirements ##
 
 * Python 3.7+
 * pip/poetry (used to get the rest of the requirements)
 
 ## Install ##
 
 ```bash
-pip install pykiso
+pip install pykiso # Core framework
+pip install pykiso[plugins] # For installing all plugins
+pip install pykiso[all] # For installing all what we have to offer
 ```
 
 [Poetry](https://python-poetry.org/) is more appropriate for developers as it automatically creates virtual environments.
 
 ```bash
 cd kiso-testing
 poetry install --all-extras
```

### Comparing `pykiso-0.21.2/pyproject.toml` & `pykiso-0.22.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykiso"
-version = "0.21.2"
+version = "0.22.0"
 description = "Embedded integration testing framework."
 authors = ["Sebastian Fischer <sebastian.fischer@de.bosch.com>"]
 license = "Eclipse Public License - v 2.0"
 readme = "README.md"
 homepage = "https://pypi.org/project/pykiso/"
 repository = "https://github.com/eclipse/kiso-testing"
 documentation = "https://kiso-testing.readthedocs.io/en/latest/"
@@ -38,34 +38,79 @@
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 brainstem = "*"
 PyYAML = "^6.0"
-pylink-square = ">=0.12,<0.15"
-pyserial = "^3.0"
-python-can = {version = "~4.1.0", extras = ["pcan"]}
-PyVISA = "^1.12.0"
-PyVISA-py = "~0.5.3"
 robotframework = "3.2.2"
 unittest-xml-reporting = "^3.2.0"
 click = ">=7.0.0,<9.0.0"
-pykiso-python-uds = "~3.0.2"
 tabulate = ">=0.8.9,<0.10.0"
 Jinja2 = ">=2.11.0,<4.0.0"
 MarkupSafe = "~2.0.1" # Allow support for Jinja2 between 2.11 < x < 3
 importlib-metadata = {version = ">=4.12,<6.0", python = "<3.8"}
 pyreadline3 = {version = "^3.4.1", python = "^3.5"}
 hidapi = "^0.12.0.post2"
 rich = {version = "^13.2.0", optional = true}
 requests = {version = "^2.28.2", optional = true}
+isort = {version = ">=5.11.4",optional = true}
+black = {version = "22.10.0",optional = true}
+pylink-square = {version = ">=0.12,<0.15", optional = true}
+pykiso-python-uds = {version = "~3.0.2", optional = true}
+pyserial = {version = "^3.0", optional = true}
+PyVISA = {version = "^1.12.0", optional = true}
+PyVISA-py = {version = "~0.5.3", optional = true}
+python-can = {version = "^4.0.0", optional = true, extras = ["pcan,vector"]}
 
+[tool.poetry.extras]
+plugins = [
+    "pylink-square",
+    "pykiso-python-uds",
+    "python-can",
+    "pyserial",
+    "PyVISA",
+    "PyVISA-py",
+]
+can = [
+    "pykiso-python-uds",
+    "python-can",
+]
+debugger = [
+    "pylink-square",
+]
+instrument = [
+    "PyVISA",
+    "PyVISA-py",
+]
+serial = [
+    "pyserial",
+]
+testrail = [
+    "rich",
+    "requests",
+]
+pykitest = [
+    "black",
+    "isort",
+]
+all = [
+    "pylink-square",
+    "pykiso-python-uds",
+    "python-can",
+    "pyserial",
+    "PyVISA",
+    "PyVISA-py",
+    "rich",
+    "requests",
+    "isort",
+    "black",
+]
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 black = "22.10.0"
 bump2version = "*"
 coverage = { version = "^6.5", extras = ["toml"] }
 invoke = "*"
 pdbpp = "*"
 pre-commit = "*"
 pylint = "*"
@@ -73,25 +118,14 @@
 pytest-cov = "*"
 pytest-mock = "*"
 Sphinx = "*"
 sphinx-rtd-theme = "*"
 sphinxcontrib-programoutput = "*"
 sphinx-autodoc-typehints = "*"
 
-[tool.poetry.extras]
-testrail = [
-    "rich",
-    "requests",
-]
-
-all = [
-    "rich",
-    "requests",
-]
-
 [tool.poetry.scripts]
 pykiso = 'pykiso.cli:main'
 pykiso-tags = 'pykiso.tool.show_tag:main'
 instrument-control = 'pykiso.lib.auxiliaries.instrument_control_auxiliary.instrument_control_cli:main'
 pykitest = 'pykiso.tool.pykiso_to_pytest.cli:main'
 testrail = "pykiso.tool.testrail.cli:cli_testrail"
 
@@ -111,15 +145,15 @@
 
 [tool.coverage.run]
 omit = [
     "*/tests/*",
     "*/examples/*",
     "*/setup.py",
     "*/tasks.py",
-    "*/src/pykiso/tool/*",
+    "*/src/pykiso/tool/testrail/*",
     "*/src/pykiso/__main__.py",
     "*/src/pykiso/interfaces/thread_auxiliary.py",
     "*/src/pykiso/lib/auxiliaries/acroname_auxiliary.py",
     "*__init__.py",
 ]
 
 [tool.coverage.report]
```

### Comparing `pykiso-0.21.2/src/pykiso/__init__.py` & `pykiso-0.22.0/src/pykiso/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 from .test_coordinator import test_case, test_message_handler, test_suite
 from .test_coordinator.test_case import (
     BasicTest,
     RemoteTest,
     define_test_parameters,
     retry_test_case,
 )
+from .test_coordinator.test_execution import abort
 from .test_coordinator.test_suite import (
     BasicTestSuiteSetup,
     BasicTestSuiteTeardown,
     RemoteTestSuiteSetup,
     RemoteTestSuiteTeardown,
 )
```

### Comparing `pykiso-0.21.2/src/pykiso/__main__.py` & `pykiso-0.22.0/src/pykiso/__main__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/auxiliary.py` & `pykiso-0.22.0/src/pykiso/auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/cli.py` & `pykiso-0.22.0/src/pykiso/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,22 @@
 :module: cli
 
 :synopsis: Entry point to the integration test framework.
 
 .. currentmodule:: cli
 
 """
-import collections
 import logging
 import pprint
 import sys
-import time
 from pathlib import Path
-from typing import Dict, List, NamedTuple, Optional, Tuple
+from typing import Dict, List, Optional, Tuple
 
 import click
 
-from pykiso.test_coordinator.test_execution import ExitCode
-
 from . import __version__
 from .config_parser import parse_config
 from .global_config import Grabber
 from .logging_initializer import initialize_logging
 from .test_coordinator import test_execution
 from .test_setup.config_registry import ConfigRegistry
 from .types import PathType
@@ -112,14 +108,15 @@
 )
 @click.option(
     "-l",
     "--log-path",
     required=False,
     default=None,
     type=click.Path(writable=True),
+    multiple=True,
     help="path to log-file or folder. If not set will log to STDOUT",
 )
 @click.option(
     "--log-level",
     required=False,
     default="INFO",
     type=click.Choice(
@@ -171,15 +168,15 @@
 )
 @click.version_option(__version__)
 @Grabber.grab_cli_config
 @click.pass_context
 def main(
     click_context: click.Context,
     test_configuration_file: Tuple[PathType],
-    log_path: PathType = None,
+    log_path: Tuple[PathType] = None,
     log_level: str = "INFO",
     report_type: str = "text",
     step_report: Optional[PathType] = None,
     pattern: Optional[str] = None,
     failfast: bool = False,
     verbose: bool = False,
 ):
@@ -189,39 +186,59 @@
     the pykiso call. Multiple values must be separated with a comma.
 
     For example: pykiso -c your_config.yaml --branch-level dev,master --variant delta
 
     \f
     :param click_context: click context
     :param test_configuration_file: path to the YAML config file
-    :param log_path: path to an existing directory or file to write logs to
+    :param log_path: path to existing directories or files to write logs to
     :param log_level: any of DEBUG, INFO, WARNING, ERROR
     :param report_type: if "test", the standard report, if "junit", a junit report is generated
     :param variant: allow the user to execute a subset of tests based on variants
     :param branch_level: allow the user to execute a subset of tests based on branch levels
     :param step_report: file path for the step report or None
     :param pattern: overwrite the pattern from the YAML file for easier test development
     :param failfast: stop the test run on the first error or failure
     :param verbose: activate logging for the whole framework
     """
 
-    for config_file in test_configuration_file:
+    for idx, config_file in enumerate(test_configuration_file):
+
+        yaml_name = Path(config_file).stem
         # Set the logging
-        logger = initialize_logging(log_path, log_level, verbose, report_type)
+        if log_path:
+            # Put all logs in one file
+            if len(log_path) == 1:
+                logger = initialize_logging(
+                    log_path[0], log_level, verbose, report_type, yaml_name
+                )
+            # Log in different files for each yaml
+            elif len(log_path) == len(test_configuration_file):
+                logger = initialize_logging(
+                    log_path[idx], log_level, verbose, report_type, yaml_name
+                )
+            else:
+                raise click.UsageError(
+                    f"Mismatch: {len(test_configuration_file)} yaml config files provided but {len(log_path)} log files"
+                )
+        else:
+            log_path = None
+            logger = initialize_logging(log_path, log_level, verbose, report_type)
+
         # Get YAML configuration
         cfg_dict = parse_config(config_file)
         # Run tests
         logger.debug("cfg_dict:\n{}".format(pprint.pformat(cfg_dict)))
 
         ConfigRegistry.register_aux_con(cfg_dict)
 
         user_tags = eval_user_tags(click_context)
 
         exit_code = test_execution.execute(
-            cfg_dict, report_type, user_tags, step_report, pattern, failfast
+            cfg_dict, report_type, yaml_name, user_tags, step_report, pattern, failfast
         )
         ConfigRegistry.delete_aux_con()
         for handler in logging.getLogger().handlers:
             if isinstance(handler, logging.FileHandler):
                 logging.getLogger().removeHandler(handler)
 
     sys.exit(exit_code)
```

### Comparing `pykiso-0.21.2/src/pykiso/config_parser.py` & `pykiso-0.22.0/src/pykiso/config_parser.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/connector.py` & `pykiso-0.22.0/src/pykiso/connector.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/exceptions.py` & `pykiso-0.22.0/src/pykiso/exceptions.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/global_config.py` & `pykiso-0.22.0/src/pykiso/global_config.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/interfaces/dt_auxiliary.py` & `pykiso-0.22.0/src/pykiso/interfaces/dt_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/interfaces/mp_auxiliary.py` & `pykiso-0.22.0/src/pykiso/interfaces/mp_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/interfaces/simple_auxiliary.py` & `pykiso-0.22.0/src/pykiso/interfaces/simple_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/interfaces/thread_auxiliary.py` & `pykiso-0.22.0/src/pykiso/interfaces/thread_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/__init__.py` & `pykiso-0.22.0/src/pykiso/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/__init__.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/acroname_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/acroname_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/communication_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/communication_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/dut_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/dut_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/__init__.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_cli.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_cli.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_instruments.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_instruments.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_scpi_commands.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_scpi_commands.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/mp_proxy_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/mp_proxy_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/proxy_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/proxy_auxiliary.py`

 * *Files 9% similar despite different names*

```diff
@@ -88,17 +88,52 @@
         :param trace_dir: where to place the trace
         :param trace_name: trace's file name
         """
         super().__init__(
             is_proxy_capable=True, tx_task_on=False, rx_task_on=True, **kwargs
         )
         self.channel = com
+        self._open_count = 0
         self.logger = self._init_trace(activate_trace, trace_dir, trace_name)
         self.proxy_channels = self.get_proxy_con(aux_list)
 
+    @property
+    def _open_connections(self) -> int:
+        """A counter monitoring the number of attached running auxiliaries.
+
+        .. warning::
+            Do not set this manually as it can easily result in unexpected behaviours.
+
+
+        :getter: returns the number of currently attached and running auxiliaries.
+        :setter: set by ``CCProxy`` instances when being opened or closed.
+            When no open connection remains and the counter falls back to 0,
+            the ``ProxyAuxiliary`` will be stopped and the attached 'physical'
+            communication channel closed.
+            When the first connection is opened and the counter is increased
+            from 0 to 1, the ``ProxyAuxiliary`` will be started and the attached
+            'physical' communication channel opened.
+        """
+        with self.lock:
+            return self._open_count
+
+    @_open_connections.setter
+    def _open_connections(self, value: int):
+        # locking shouldn't be necessary but we're never too paranoid
+        with self.lock:
+            last_connection_closed = value == 0 and self._open_count == 1
+            first_connection_opened = value == 1 and self._open_count == 0
+            # prevent negative values on invalid initialization
+            if value >= 0:
+                self._open_count = value
+            if last_connection_closed and self.is_instance:
+                self.delete_instance()
+            elif first_connection_opened and not self.is_instance:
+                self.create_instance()
+
     @staticmethod
     def _init_trace(
         activate: bool, t_dir: Optional[str] = None, t_name: Optional[str] = None
     ) -> logging.Logger:
         """Initialize the logging trace for proxy auxiliary received
         message recording.
 
@@ -146,18 +181,17 @@
 
     def get_proxy_con(self, aux_list: List[str]) -> Tuple[CCProxy, ...]:
         """Retrieve all connector associated to all given existing Auxiliaries.
 
         If auxiliary alias exists but auxiliary instance was not created
         yet, create it immediately using ConfigRegistry _aux_cache.
 
-        :param aux_list: list of auxiliary's alias
-
+        :param aux_list: list of auxiliary aliases or instances.
         :return: tuple containing all connectors associated to
-            all given auxiliaries
+            all given auxiliaries.
         """
         channel_inst: List[CCProxy] = []
 
         for aux in aux_list:
             # aux_list can contain a auxiliary instance just grab the
             # channel
             if isinstance(aux, (AuxiliaryInterface, DTAuxiliaryInterface)):
@@ -192,15 +226,15 @@
         # share its API to the user's auxiliaries
         for channel in channel_inst:
             channel._bind_channel_info(self)
 
         return tuple(channel_inst)
 
     @staticmethod
-    def _check_aux_compatibility(aux) -> None:
+    def _check_aux_compatibility(aux: DTAuxiliaryInterface) -> None:
         """Check if the given auxiliary is proxy compatible.
 
         :param aux: auxiliary instance to check
 
         :raises NotImplementedError: if is_proxy_capable flag is False
         """
         if not aux.is_proxy_capable:
@@ -222,19 +256,29 @@
                 raise TypeError(f"Channel {channel} is not compatible!")
 
     def _dispatch_tx_method_to_channels(self) -> None:
         """Attached public run_command method to all connected proxy
         channels.
 
         .. note:: This method use the thread safe method implemented by
-            each proxy channels(attached_tx_callback).
+            each proxy channel (attach_tx_callback).
         """
         for conn in self.proxy_channels:
             conn.attach_tx_callback(self.run_command)
 
+    def _remove_tx_method_from_channels(self) -> None:
+        """Detach public run_command method from all connected proxy
+        channels.
+
+        .. note:: This method use the thread safe method implemented by
+            each proxy channel (detach_tx_callback).
+        """
+        for conn in self.proxy_channels:
+            conn.detach_tx_callback()
+
     @open_connector
     def _create_auxiliary_instance(self) -> bool:
         """Open current associated channel and dispatch tx method.
 
         :return: if channel creation is successful return True otherwise
             False
         """
@@ -245,14 +289,15 @@
     @close_connector
     def _delete_auxiliary_instance(self) -> bool:
         """Close current associated channel.
 
         :return: if channel deletion is successful return True otherwise
             False
         """
+        self._remove_tx_method_from_channels()
         log.internal_info("Auxiliary instance deleted")
         return True
 
     def run_command(self, conn: CChannel, *args: tuple, **kwargs: dict) -> None:
         """Transmit an incoming request from a linked proxy channel
         to the proxy auxiliary's channel.
 
@@ -286,35 +331,38 @@
         proxy connectors.
 
         :param con_use: current proxy channel instance which the command
             comes from
         :param kwargs: named arguments
         """
         for conn in self.proxy_channels:
-            if conn != con_use:
+            if conn != con_use and conn.queue_out is not None:
                 conn.queue_out.put(kwargs)
 
     def _receive_message(self, timeout_in_s: float = 0) -> None:
         """Get a message from the associated channel and dispatch it to
-        the liked proxy channels.
+        the linked proxy channels.
 
         .. note:: this method is called by the rx thread task from the
-            inherit interface class
+            inherited interface class
 
 
         :param timeout_in_s: maximum amount of time (seconds) to wait
             for a message
         """
         try:
             recv_response = self.channel.cc_receive(timeout=timeout_in_s)
             received_data = recv_response.get("msg")
             # if data are received, populate connector's queue_out
             if received_data is not None:
                 self.logger.debug(
-                    f"received response : data {received_data.hex()} || channel : {self.channel.name}"
+                    "received response : data %s || channel : %s",
+                    received_data.hex(),
+                    self.channel.name,
                 )
                 for conn in self.proxy_channels:
-                    conn.queue_out.put(recv_response)
+                    if conn.queue_out is not None:
+                        conn.queue_out.put(recv_response)
         except Exception:
             log.exception(
                 f"encountered error while receiving message via {self.channel}"
             )
```

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/record_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/record_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/__init__.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/response_templates.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/response_templates.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/scenario.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/scenario.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulated_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulated_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulation.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulation.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/__init__.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/common/__init__.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_base_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_base_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_callback.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,20 @@
 from __future__ import annotations
 
 import logging
 import time
 import typing
 from dataclasses import dataclass
 from itertools import cycle
-from typing import Callable, ClassVar, List, Optional, Tuple, Union
+from typing import Callable, ClassVar, Dict, List, Optional, Tuple, Union
 
 from uds import IsoServices
 
+from pykiso.types import OdxRequestConfigDict
+
 if typing.TYPE_CHECKING:
     from pykiso.lib.auxiliaries.udsaux import UdsServerAuxiliary
 
 
 log = logging.getLogger(__name__)
 
 
@@ -56,17 +58,17 @@
         must have two positional arguments: the received request as a list of
         integers and the UdsServerAuxiliary instance.
     """
 
     POSITIVE_RESPONSE_OFFSET: ClassVar[int] = 0x40
 
     # e.g. 0x1003 or [0x10, 0x03]
-    request: Union[int, List[int]]
+    request: Union[int, List[int], OdxRequestConfigDict]
     # e.g. 0x5003 or [0x50, 0x03]
-    response: Optional[Union[int, List[int]]] = None
+    response: Optional[Union[int, List[int], Dict[str, str]]] = None
     # e.g. 0x1011 or b'DATA'
     response_data: Optional[Union[int, bytes]] = None
     # specify zero-padding
     data_length: Optional[int] = None
     # custom callback
     callback: Optional[Callable[[List[int], UdsServerAuxiliary], None]] = None
 
@@ -75,21 +77,23 @@
         self.call_count = 0
 
         if isinstance(self.request, int):
             self.request = list(self.int_to_bytes(self.request))
 
         if isinstance(self.response, int):
             self.response = list(self.int_to_bytes(self.response))
-        elif self.response is None:
+        elif self.response is None and not isinstance(self.request, dict):
             # create positive response based on request
             self.response = [
                 self.request[0] + self.POSITIVE_RESPONSE_OFFSET
             ] + self.request[1:]
 
-        if self.response_data is not None:
+        if self.response_data is not None and not (
+            isinstance(self.response, dict) or self.response is None
+        ):
             # convert response_data and append it to the response
             self.response_data = (
                 list(self.int_to_bytes(self.response_data))
                 if isinstance(self.response_data, int)
                 else list(self.response_data)
             )
             self.response.extend(self.response_data)
```

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_exceptions.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_exceptions.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_request.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_request.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_response.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_response.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/common/uds_utils.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_utils.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/udsaux/uds_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/uds_auxiliary.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,21 @@
 import logging
 import threading
 import time
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Iterator, List, Optional, Union
 
-import can
-from uds import IsoServices
+try:
+    import can
+    from uds import IsoServices
+except ImportError as e:
+    raise ImportError(
+        f"{e.name} dependency missing, consider installing pykiso with 'pip install pykiso[can]'"
+    )
 
 from pykiso.connector import CChannel
 
 from .common import uds_exceptions
 from .common.uds_base_auxiliary import UdsBaseAuxiliary
 from .common.uds_request import UDSCommands
 from .common.uds_response import UdsResponse
```

### Comparing `pykiso-0.21.2/src/pykiso/lib/auxiliaries/ykush_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/auxiliaries/ykush_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/__init__.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_example.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_example.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_fdx_lauterbach.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_fdx_lauterbach.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_flasher_example.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_flasher_example.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_mp_proxy.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_mp_proxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,25 +37,28 @@
 
 log = logging.getLogger(__name__)
 
 
 class CCMpProxy(CChannel):
     """Multiprocessing Proxy CChannel for multi auxiliary usage."""
 
+    # keep an uninitialized proxy variable at class-level to fulfill the existence conditions.
+    # when a CCProxy instance will then set it, it will only be set at instance level but stay
+    # uninitialized at class-level
+    _proxy: MpProxyAuxiliary = None
+    _physical_channel: CChannel = None
+
     def __init__(self, **kwargs):
         """Initialize attributes."""
         kwargs.update(processing=True)
         super().__init__(**kwargs)
         # instantiate directly both queue_in and queue_out
         self.queue_in = multiprocessing.Queue()
         self.queue_out = multiprocessing.Queue()
         self.timeout = 1
-        # used for physical channel attributes access from main auxiliary
-        self._proxy = None
-        self._physical_channel = None
 
     def _bind_channel_info(self, proxy_aux: MpProxyAuxiliary):
         """Bind a :py:class:`~pykiso.lib.auxiliaries.mp_proxy_auxiliary.MpProxyAuxiliary`
         instance that is instanciated in order to handle the connection of
         multiple auxiliaries to a single communication channel in order to
         hide the underlying proxy setup.
```

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_process.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_process.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_proxy.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_proxy.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,23 +38,27 @@
 
 log = logging.getLogger(__name__)
 
 
 class CCProxy(CChannel):
     """Proxy CChannel to bind multiple auxiliaries to a single 'physical' CChannel."""
 
+    # keep an uninitialized proxy variable at class-level to fulfill the existence conditions.
+    # when a CCProxy instance will then set it, it will only be set at instance level but stay
+    # uninitialized at class-level
+    _proxy: ProxyAuxiliary = None
+    _physical_channel: CChannel = None
+
     def __init__(self, **kwargs):
         """Initialize attributes."""
         super().__init__(**kwargs)
         self.queue_out = None
         self.timeout = 1
         self._lock = threading.Lock()
         self._tx_callback = None
-        self._proxy = None
-        self._physical_channel = None
 
     def _bind_channel_info(self, proxy_aux: ProxyAuxiliary):
         """Bind a :py:class:`~pykiso.lib.auxiliaries.proxy_auxiliary.ProxyAuxiliary`
         instance that is instanciated in order to handle the connection of
         multiple auxiliaries to a single communication channel.
 
         This allows to access the real communication channel's attributes
@@ -98,14 +102,26 @@
             log.internal_debug(f"attached function {func.__name__}")
             if self._tx_callback is not None:
                 log.internal_warning(
                     f"function {func.__name__} will replace current transmit callback {self._tx_callback.__name__}"
                 )
             self._tx_callback = func
 
+    def open(self) -> None:
+        super().open()
+        if self._proxy is not None:
+            # will start the proxy_auxiliary if this is the first CCProxy to be opened
+            self._proxy._open_connections += 1
+
+    def close(self) -> None:
+        super().close()
+        if self._proxy is not None:
+            # will stop the proxy_auxiliary if this is the last CCProxy to be closed
+            self._proxy._open_connections -= 1
+
     def _cc_open(self) -> None:
         """Open proxy channel."""
         log.internal_info("Open proxy channel")
         self.queue_out = queue.Queue()
 
     def _cc_close(self) -> None:
         """Close proxy channel."""
```

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_raw_loopback.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_raw_loopback.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_rtt_segger.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_rtt_segger.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,21 @@
 import functools
 import logging
 import threading
 import time
 from pathlib import Path
 from typing import Dict, Optional, Union
 
-import pylink
+try:
+    import pylink
+except ImportError as e:
+    raise ImportError(
+        f"{e.name} dependency missing, consider installing pykiso with 'pip install pykiso[debugger]'"
+    )
+
 
 from pykiso import connector
 from pykiso.message import Message
 
 log = logging.getLogger(__name__)
```

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_serial.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_serial.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,21 @@
 
 """
 
 
 from enum import Enum, IntEnum
 from typing import ByteString, Dict, Optional, Union
 
-import serial
+try:
+    import serial
+except ImportError as e:
+    raise ImportError(
+        f"{e.name} dependency missing, consider installing pykiso with 'pip install pykiso[serial]'"
+    )
+
 
 from pykiso import Message, connector
 
 MessageType = Union[Message, bytes]
 
 
 class ByteSize(IntEnum):
@@ -64,15 +70,15 @@
         timeout: Optional[float] = None,
         xonxoff: bool = False,
         rtscts: bool = False,
         write_timeout: Optional[float] = None,
         dsrdtr: bool = False,
         inter_byte_timeout: Optional[float] = None,
         exclusive: Optional[bool] = None,
-        **kwargs
+        **kwargs,
     ):
         """Init Serial settings
 
         :param port: Device name (e.g. "COM1" for Windows or "/dev/ttyACM0" for Linux)
         :param baudrate: Baud rate such as 9600 or 115200 etc, defaults to 9600
         :param bytesize: Number of data bits. Possible values:
           FIVEBITS, SIXBITS, SEVENBITS, EIGHTBITS, defaults to EIGHTBITS
```

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_socket_can/__init__.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_socket_can/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_socket_can/cc_socket_can.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_socket_can/cc_socket_can.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,22 @@
 
 import logging
 import platform
 import time
 from pathlib import Path
 from typing import Dict, Optional, Union
 
-import can
-import can.bus
+try:
+    import can
+    import can.bus
+except ImportError as e:
+    raise ImportError(
+        f"{e.name} dependency missing, consider installing pykiso with 'pip install pykiso[can]'"
+    )
+
 
 from pykiso import CChannel, Message
 from pykiso.lib.connectors.cc_socket_can.socketcan_to_trc import (
     SocketCan2Trc,
     can,
 )
```

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_socket_can/socketcan_to_trc.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_socket_can/socketcan_to_trc.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,21 @@
 
 import logging
 import subprocess
 import sys
 import time
 from textwrap import dedent
 
-import can
+try:
+    import can
+except ImportError as e:
+    raise ImportError(
+        f"{e.name} dependency missing, consider installing pykiso with 'pip install pykiso[can]'"
+    )
+
 
 log = logging.getLogger(__name__)
 
 
 TRC_HEADER = """\
         ;$FILEVERSION=2.0
         ;$STARTTIME={starttime_days:12.3f}
```

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_tcp_ip.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_tcp_ip.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_uart.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_uart.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,20 @@
 
 """
 
 import struct
 import time
 from typing import Optional
 
-import serial
+try:
+    import serial
+except ImportError as e:
+    raise ImportError(
+        f"{e.name} dependency missing, consider installing pykiso with 'pip install pykiso[serial]'"
+    )
 
 from pykiso import connector, message
 
 
 class IncompleteCCMsgError(Exception):
     def __init__(self, value):
         self.value = value
```

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_udp.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_udp.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_udp_server.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_udp_server.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_usb.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_usb.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,20 @@
 
 .. currentmodule:: cc_usb
 
 
 .. warning: Still under test
 """
 
-import serial
+try:
+    import serial
+except ImportError as e:
+    raise ImportError(
+        f"{e.name} dependency missing, consider installing pykiso with 'pip install pykiso[serial]'"
+    )
 
 from pykiso.lib.connectors import cc_uart
 
 
 class CCUsb(cc_uart.CCUart):
     def __init__(self, serial_port):
         super().__init__(serial_port, baudrate=9600)
```

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_vector_can.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_vector_can.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,18 +18,24 @@
 .. currentmodule:: cc_vector_can
 
 """
 
 import logging
 from typing import Dict, Optional, Union
 
-import can
-import can.bus
-import can.interfaces.vector
-from can.interfaces.vector.canlib import get_channel_configs
+try:
+    import can
+    import can.bus
+    import can.interfaces.vector
+    from can.interfaces.vector.canlib import get_channel_configs
+except ImportError as e:
+    raise ImportError(
+        f"{e.name} dependency missing, consider installing pykiso with 'pip install pykiso[can]'"
+    )
+
 
 from pykiso import CChannel, Message
 
 MessageType = Union[Message, bytes]
 
 log = logging.getLogger(__name__)
```

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/cc_visa.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/cc_visa.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,21 @@
 
 """
 
 import abc
 import logging
 from typing import Dict, Optional
 
-import pyvisa
+try:
+    import pyvisa
+except ImportError as e:
+    raise ImportError(
+        f"{e.name} dependency missing, consider installing pykiso with 'pip install pykiso[instrument]'"
+    )
+
 
 from pykiso import CChannel
 from pykiso.types import MsgType
 
 log = logging.getLogger(__name__)
```

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/flash_jlink.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/flash_jlink.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,21 @@
 
 """
 
 import logging
 import pathlib
 import typing
 
-import pylink
+try:
+    import pylink
+except ImportError as e:
+    raise ImportError(
+        f"{e.name} dependency missing, consider installing pykiso with 'pip install pykiso[debugger]'"
+    )
+
 
 from pykiso import Flasher
 
 PathType = typing.Union[str, pathlib.Path]
 
 log = logging.getLogger(__name__)
```

### Comparing `pykiso-0.21.2/src/pykiso/lib/connectors/flash_lauterbach.py` & `pykiso-0.22.0/src/pykiso/lib/connectors/flash_lauterbach.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/robot_framework/__init__.py` & `pykiso-0.22.0/src/pykiso/lib/robot_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/robot_framework/acroname_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/robot_framework/acroname_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/robot_framework/aux_interface.py` & `pykiso-0.22.0/src/pykiso/lib/robot_framework/aux_interface.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/robot_framework/communication_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/robot_framework/communication_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/robot_framework/dut_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/robot_framework/dut_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/robot_framework/instrument_control_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/robot_framework/instrument_control_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/robot_framework/loader.py` & `pykiso-0.22.0/src/pykiso/lib/robot_framework/loader.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/robot_framework/proxy_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/robot_framework/proxy_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/robot_framework/record_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/robot_framework/record_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/lib/robot_framework/uds_auxiliary.py` & `pykiso-0.22.0/src/pykiso/lib/robot_framework/uds_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/logging_initializer.py` & `pykiso-0.22.0/src/pykiso/logging_initializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,24 +63,26 @@
 
 
 def initialize_logging(
     log_path: PathType,
     log_level: str,
     verbose: bool,
     report_type: str = None,
+    yaml_name: str = None,
 ) -> logging.Logger:
     """Initialize the logging.
 
     Sets the general log level, output file or STDOUT and the
     logging format.
 
     :param log_path: path to the logfile
     :param log_level: any of DEBUG, INFO, WARNING, ERROR
     :param verbose: activate internal kiso logging if True
     :param report_type: expected report type (junit, text,...)
+    :param yaml_name: name of current yaml config file
 
     :returns: configured Logger
     """
     root_logger = logging.getLogger()
     log_format = logging.Formatter(
         "%(asctime)s [%(levelname)s] %(module)s:%(lineno)d: %(message)s"
     )
@@ -110,16 +112,17 @@
                 logging.INTERNAL_INFO,
                 logging.INTERNAL_DEBUG,
             )
 
     # if log_path is given create a file handler
     if log_path is not None:
         log_path = Path(log_path)
-        if log_path.is_dir():
-            fname = time.strftime("%Y-%m-%d_%H-%M-test.log")
+        if log_path.suffix == "":
+            log_path.mkdir(parents=True, exist_ok=True)
+            fname = time.strftime(f"%Y-%m-%d_%H-%M-{yaml_name}.log")
             log_path = log_path / fname
         file_handler = logging.FileHandler(log_path, "a+")
         file_handler.setFormatter(log_format)
         file_handler.setLevel(levels[log_level])
         root_logger.addHandler(file_handler)
 
     # if report_type is junit use sys.stdout as stream
```

### Comparing `pykiso-0.21.2/src/pykiso/message.py` & `pykiso-0.22.0/src/pykiso/message.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/test_coordinator/test_case.py` & `pykiso-0.22.0/src/pykiso/test_coordinator/test_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -241,25 +241,15 @@
                     teardown_timeout,
                     test_ids,
                     tag,
                     *args,
                     **kwargs,
                 )
 
-        NewClass.__doc__ = NewClass.__doc__.format(
-            DecoratedClass=DecoratedClass,
-            suite_id=suite_id,
-            case_id=case_id,
-            auxes=[aux.__class__.__name__ for aux in aux_list or []],
-            setup_timeout=setup_timeout,
-            run_timeout=run_timeout,
-            teardown_timeout=teardown_timeout,
-            test_ids=test_ids,
-            tag=tag,
-        )
+        NewClass.__doc__ = DecoratedClass.__doc__
 
         # Used to display the current test module in the test result
         NewClass.__module__ = DecoratedClass.__module__
         # Passing the name of the decorated class to the new returned class
         # in order to get the test case name and references, i.e. suite_id and case_id
         # in the test results in the console and in the report.
         # Changing __name__ is necessary to make the test name appear in the test results in the console.
```

### Comparing `pykiso-0.21.2/src/pykiso/test_coordinator/test_execution.py` & `pykiso-0.22.0/src/pykiso/test_coordinator/test_execution.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,20 @@
     1. Glob a list of test-suite folders
     2. Generate a list of test-suites with a list of test-cases
     3. Loop per suite
     4. Gather result
 """
 from __future__ import annotations
 
+import os
 from typing import TYPE_CHECKING
 from unittest.loader import VALID_MODULE_NAME
 
+from pykiso.test_result.multi_result import MultiTestResult
+
 if TYPE_CHECKING:
     from .test_case import BasicTest
 
 import enum
 import logging
 import re
 import time
@@ -317,27 +320,43 @@
             current_test_suite = create_test_suite(test_suite_configuration)
             list_of_test_suites.append(current_test_suite)
         except BaseException as e:
             raise TestCollectionError(test_suite_configuration["suite_dir"]) from e
     return list_of_test_suites
 
 
+def abort(reason: str = None) -> None:
+    """Quit ITF test and log an error if a reason is indicated and
+    if any errors occurred it logs them.
+
+    :param reason: reason to abort, defaults to None
+    """
+    if reason:
+        log.critical(reason)
+    log.critical(
+        "Non recoverable error occurred during test execution, aborting test session."
+    )
+    os.kill(os.getpid(), ExitCode.ONE_OR_MORE_TESTS_RAISED_UNEXPECTED_EXCEPTION)
+
+
 def execute(
     config: Dict[str, Any],
     report_type: str = "text",
+    report_name: str = "",
     user_tags: Optional[Dict[str, List[str]]] = None,
     step_report: Optional[Path] = None,
     pattern_inject: Optional[str] = None,
     failfast: bool = False,
 ) -> int:
     """Create test environment based on test configuration.
 
     :param config: dict from converted YAML config file
     :param report_type: str to set the type of report wanted, i.e. test
         or junit
+    :param report_name: name of the junit report
     :param user_tags: test case tags to execute
     :param step_report: file path for the step report or None
     :param pattern_inject: optional pattern that will override
         test_filter_pattern for all suites. Used in test development to
         run specific tests.
     :param failfast: stop the test run on the first error or failure.
 
@@ -366,35 +385,35 @@
                 test_file_pattern.test_class,
                 test_file_pattern.test_case,
             )
 
         log_file_path = get_logging_options().log_path
         # TestRunner selection: generate or not a junit report. Start the tests and publish the results
         if report_type == "junit":
-            junit_report_name = time.strftime("TEST-pykiso-%Y-%m-%d_%H-%M-%S.xml")
+            junit_report_name = time.strftime(f"%Y-%m-%d_%H-%M-%S-{report_name}.xml")
             project_folder = Path.cwd()
             reports_path = project_folder / "reports"
             junit_report_path = reports_path / junit_report_name
             reports_path.mkdir(exist_ok=True)
             with open(junit_report_path, "wb") as junit_output, ResultStream(
                 log_file_path
             ) as stream:
                 test_runner = xmlrunner.XMLTestRunner(
                     output=junit_output,
-                    resultclass=XmlTestResult,
+                    resultclass=MultiTestResult(XmlTestResult, BannerTestResult),
                     failfast=failfast,
                     verbosity=0,
                     stream=stream,
                 )
                 result = test_runner.run(all_tests_to_run)
         else:
             with ResultStream(log_file_path) as stream:
                 test_runner = unittest.TextTestRunner(
                     stream=stream,
-                    resultclass=BannerTestResult,
+                    resultclass=MultiTestResult(BannerTestResult),
                     failfast=failfast,
                     verbosity=0,
                 )
                 result = test_runner.run(all_tests_to_run)
 
         # Generate the html step report
         if step_report is not None:
```

### Comparing `pykiso-0.21.2/src/pykiso/test_coordinator/test_message_handler.py` & `pykiso-0.22.0/src/pykiso/test_coordinator/test_message_handler.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/test_coordinator/test_suite.py` & `pykiso-0.22.0/src/pykiso/test_coordinator/test_suite.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/test_result/__init__.py` & `pykiso-0.22.0/src/pykiso/test_result/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/test_result/assert_step_report.py` & `pykiso-0.22.0/src/pykiso/test_result/assert_step_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,16 +49,19 @@
 
 
 # Global variables
 # Store the Result Step report
 ALL_STEP_REPORT = OrderedDict()
 # Step result keys used by Jinja for columns name
 REPORT_KEYS = ["message", "var_name", "expected_result", "actual_result", "succeed"]
+DEFAULT_TEST_METHOD = ["setup", "teardown", "handle_interaction"]
 # Parent method being reported ; Ignore sub call (assert in an assert)
-_FUNCTION_TO_APPLY = r"|".join(["test", "setup", "teardown", "handle_interaction"])
+_FUNCTION_TO_APPLY = r"|".join(["test", *DEFAULT_TEST_METHOD])
+#: content all assertion methods where the checked value is not shown
+MUTE_CONTENT_ASSERTION = ["assertIsInstance", "assertNotIsInstance"]
 
 # Jinja template location
 SCRIPT_PATH = str(Path(__file__).resolve().parent)
 REPORT_TEMPLATE = "templates/report_template.html.j2"
 
 
 @dataclass
@@ -197,45 +200,77 @@
     if not ALL_STEP_REPORT.get(test_class_name):
         ALL_STEP_REPORT[test_class_name] = OrderedDict()
         # Add test succeed flag
         ALL_STEP_REPORT[test_class_name]["succeed"] = True
         # Add header (mutable object -> dictionary fed during test)
         ALL_STEP_REPORT[test_class_name]["header"] = test.step_report.header
         # Add description of the test -> Always test_run
-        ALL_STEP_REPORT[test_class_name]["description"] = (
-            test._testMethodDoc or "Not provided"
-        )
+        ALL_STEP_REPORT[test_class_name]["description"] = test.__doc__ or "Not provided"
         # Add test file path
         ALL_STEP_REPORT[test_class_name]["file_path"] = inspect.getfile(type(test))
         # Store the result (start, stop, elapsed time)
         ALL_STEP_REPORT[test_class_name]["time_result"] = OrderedDict()
         ALL_STEP_REPORT[test_class_name]["time_result"]["Start Time"] = 0
         # Store the tests list
         ALL_STEP_REPORT[test_class_name]["test_list"] = OrderedDict()
 
     # Create the current test step storage
     if not ALL_STEP_REPORT[test_class_name]["test_list"].get(test_name):
-        ALL_STEP_REPORT[test_class_name]["test_list"][test_name] = []
+        test_method = getattr(test, test_name, None)
+        test_description = test_method.__doc__ or ""
+        ALL_STEP_REPORT[test_class_name]["test_list"][test_name] = {
+            "description": test_description,
+            "steps": [],
+        }
 
 
 def _add_step(
     test_class_name: str,
     test_name: str,
     message: str,
     var_name: str,
     expected: typing.Any,
     received: typing.Any,
 ):
     global ALL_STEP_REPORT, REPORT_KEYS
 
-    ALL_STEP_REPORT[test_class_name]["test_list"][test_name].append(
+    ALL_STEP_REPORT[test_class_name]["test_list"][test_name]["steps"].append(
         dict(zip(REPORT_KEYS, [message, var_name, expected, received, True]))
     )
 
 
+def determine_parent_test_function(test_name: str) -> str:
+    """Determine the parent test function.
+
+    This function attached the nested assertion to the correct parent test
+    function.
+
+    :param test_name: current test function
+
+    :return: parent test function
+    """
+    # the function respect the default test method pattern or in defualt test
+    # function
+    if test_name.lower() in DEFAULT_TEST_METHOD or test_name.startswith("test_"):
+        return test_name
+
+    # collect all methods called from the stack to get the parent test function
+    methods = [frame.function for frame in inspect.stack()]
+
+    # determine if the parent test function is a fixture or a test function
+    fixture = [method for method in methods if method.lower() in DEFAULT_TEST_METHOD]
+    test_function = [method for method in methods if method.startswith("test_")]
+
+    if fixture:
+        return fixture.pop()
+
+    if test_function:
+        return test_function.pop()
+
+
 def assert_decorator(assert_method: types.MethodType):
     """Decorator to gather assertion information
 
     - MyTestClass
         - header: additional data
         - description: test purpose
         - file_path: test location
@@ -267,61 +302,59 @@
         return: The assertion method output if it exists. Otherwise, None
         """
         global _FUNCTION_TO_APPLY
         try:
             # Context
             currentframe = inspect.currentframe()
             f_back = currentframe.f_back
-            test_name = f_back.f_code.co_name
+
+            test_name = determine_parent_test_function(f_back.f_code.co_name)
             test_case_inst: TestCase = assert_method.__self__
             test_class_name = type(test_case_inst).__name__
             assert_name = assert_method.__name__
 
             # filter parent call, only known function recorded
             parent_method = re.findall(_FUNCTION_TO_APPLY, test_name.lower())
-            if parent_method:
-                # get the decorated test fixture name (setUp, tearDown, ...)
-                if parent_method[0] == "handle_interaction":
-                    test_name = f_back.f_locals["func"].__name__
-
-                # Assign variables to signature
-                signature = inspect.signature(assert_method)
-                arguments = signature.bind(*args, **kwargs).arguments
-                test_name = test_case_inst.step_report.current_table or test_name
-
-                # 1. Gather message, var_name, expected, received
-                # 1.1 Get message. default value: ""
-                if test_case_inst.step_report.message:
-                    message = test_case_inst.step_report.message
-                    test_case_inst.step_report.message = ""
-                else:
-                    message = arguments.get("msg", "")
-
-                # ensure message is always present in the arguments
-                # dictionary. (used in _get_expected)
-                if not message and "msg" in signature.parameters:
-                    arguments["msg"] = ""
-
-                # 1.2. Get 'received" value (Always 1st argument)
-                received = list(arguments.values())[0]
-
-                # 1.3. Get variable name
-                var_name = _get_variable_name(f_back, assert_name)
-
-                # 1.4. Get Expected value
-                expected = _get_expected(assert_name, arguments)
-
-                # 2. Update report data
-                # 2.1 Ensure report ready for update
-                _prepare_report(test_case_inst, test_name)
-
-                # 2.2. Add new step
-                _add_step(
-                    test_class_name, test_name, message, var_name, expected, received
-                )
+            # get the decorated test fixture name (setUp, tearDown, ...)
+            if parent_method and parent_method[0] == "handle_interaction":
+                test_name = f_back.f_locals["func"].__name__
+
+            # Assign variables to signature
+            signature = inspect.signature(assert_method)
+            arguments = signature.bind(*args, **kwargs).arguments
+            test_name = test_case_inst.step_report.current_table or test_name
+            # 1. Gather message, var_name, expected, received
+            # 1.1 Get message. default value: ""
+            if test_case_inst.step_report.message:
+                message = test_case_inst.step_report.message
+                test_case_inst.step_report.message = ""
+            else:
+                message = arguments.get("msg", "")
+
+            # ensure message is always present in the arguments
+            # dictionary. (used in _get_expected)
+            if not message and "msg" in signature.parameters:
+                arguments["msg"] = ""
+
+            # 1.2. Get 'received" value (Always 1st argument)
+            assert_value = list(arguments.values())[0]
+            received = assert_value if assert_name not in MUTE_CONTENT_ASSERTION else ""
+
+            # 1.3. Get variable name
+            var_name = _get_variable_name(f_back, assert_name)
+
+            # 1.4. Get Expected value
+            expected = _get_expected(assert_name, arguments)
+
+            # 2. Update report data
+            # 2.1 Ensure report ready for update
+            _prepare_report(test_case_inst, test_name)
+
+            # 2.2. Add new step
+            _add_step(test_class_name, test_name, message, var_name, expected, received)
 
         except Exception as e:
             log.error(f"Unable to update Step due to exception: {e}")
 
         # Run the assert method and mark the test as failed if the AssertionError is raised
         try:
             return assert_method(*args, **kwargs)
```

### Comparing `pykiso-0.21.2/src/pykiso/test_result/templates/report_template.css` & `pykiso-0.22.0/src/pykiso/test_result/templates/report_template.css`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/test_result/templates/report_template.html.j2` & `pykiso-0.22.0/src/pykiso/test_result/templates/report_template.html.j2`

 * *Files 2% similar despite different names*

```diff
@@ -25,32 +25,33 @@
                 {% for key, value in data.items() -%}
                     <u>{{key}}</u>: {{value}}</br>
                 {%- endfor %}
             {%- endfor %}
             </p>
             {#- For each test (setUp, run, tearDown) -#}
             {% for test_name, test_content in class_content["test_list"].items() %}
-                {% set test_success = is_test_success(test_content) -%}
+                {% set test_success = is_test_success(test_content["steps"]) -%}
                 <details {% if not test_success %}open{% endif %}><summary><h3>{{test_name}}
                 {% if test_success -%}<span style="color:green;">Success</span>
                 {% else %}<span style="color:red;">Fail</span>
                 {%- endif %}</h3></summary>
+                <p>{{test_content["description"] | replace("\n", "<br/>\n") }}</p>
                 <table>
                     <thead>
                         <tr>
                             {# Set Columns name from the first row, excluding succeed flag -#}
                             <th scope="col" style="width: 3%">Step</th>
-                            {% for column_name in test_content[0].keys() if column_name != "succeed" -%}
+                            {% for column_name in test_content["steps"][0].keys() if column_name != "succeed" -%}
                                 <th scope="col">{{column_name}}</th>
                             {%- endfor %}
                         </tr>
                     </thead>
                     <tbody>
                         {#- Loop over each assert method called (step-report) -#}
-                        {% for row in test_content -%}
+                        {% for row in test_content["steps"] -%}
                             {# Set cell color variable according to the assert result and emptiness -#}
                             {% if row.pop("succeed") -%}
                                 {% set color_cell = "background-color: rgb(196, 243, 196);" -%}
                                 {% set color_empty_cell = "background-color: rgb(250, 250, 128);" -%}
                             {% else -%}
                                 {% set color_cell = "background-color: rgb(236, 160, 160);" -%}
                                 {% set color_empty_cell = "background-color: rgb(236, 160, 160);" -%}
```

#### html2text {}

```diff
@@ -10,16 +10,18 @@
 \n") }}
 **** Date, Time, Software versions: ****
 {# Add additional information from header key -#} {% for data in [class_content
 ["time_result"], class_content["header"]] -%} {% for key, value in data.items()
 -%} {{key}}: {{value}} {%- endfor %} {%- endfor %}
 {#- For each test (setUp, run, tearDown) -#} {% for test_name, test_content in
 class_content["test_list"].items() %} {% set test_success = is_test_success
-(test_content) -%}
+(test_content["steps"]) -%}
 % if not test_success %}open{% endif %}>
 **** {{test_name}} {% if test_success -%}Success {% else %}Fail {%- endif %}
 ****
+{{test_content["description"] | replace("\n", "
+\n") }}
 Step           {{column_name}}
 {{loop.index}}
  {%- endfor %}
 {%- endfor %}
```

### Comparing `pykiso-0.21.2/src/pykiso/test_result/templates/report_template_script.js` & `pykiso-0.22.0/src/pykiso/test_result/templates/report_template_script.js`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/test_result/text_result.py` & `pykiso-0.22.0/src/pykiso/test_result/text_result.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/test_result/xml_result.py` & `pykiso-0.22.0/src/pykiso/test_result/xml_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
         :return: the wrapped test case's representation.
         """
         *modules, test_case, test_method = self.test_id.split(".")
         return f"{test_method} ({'.'.join(modules)}.{test_case})"
 
 
-class XmlTestResult(BannerTestResult, xmlrunner.runner._XMLTestResult):
+class XmlTestResult(xmlrunner.runner._XMLTestResult):
     """
     Test result class that can express test results in a XML report.
     Used by XMLTestRunner.
     """
 
     def __init__(
         self,
@@ -109,20 +109,15 @@
         :param stream: buffered text interface to a buffered raw stream
         :param descriptions: include description of the test
         :param verbosity: print output into the console
         :param elapsed_times: include the time spend on the test
         :param properties: junit testsuite properties
         :param infoclass: class containing the test information
         """
-        BannerTestResult.__init__(
-            self,
-            stream=stream,
-            descriptions=descriptions,
-            verbosity=verbosity,
-        )
+
         xmlrunner.runner._XMLTestResult.__init__(
             self,
             stream=stream,
             descriptions=descriptions,
             verbosity=verbosity,
             elapsed_times=elapsed_times,
             properties=properties,
```

### Comparing `pykiso-0.21.2/src/pykiso/test_setup/config_registry.py` & `pykiso-0.22.0/src/pykiso/test_setup/config_registry.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 """
 from __future__ import annotations
 
 from collections import defaultdict
 from typing import TYPE_CHECKING, Any, Dict, List, Tuple, Type
 
+from ..exceptions import PykisoError
 from .dynamic_loader import DynamicImportLinker
 
 if TYPE_CHECKING:
     from pykiso.auxiliary import AuxiliaryCommon
     from pykiso.types import (
         AuxiliaryAlias,
         AuxiliaryConfig,
@@ -72,14 +73,15 @@
         return name, config
 
     @staticmethod
     def _make_proxy_aux_config(
         channel_name: ConnectorAlias,
         aux_list: List[AuxiliaryAlias],
         multiprocessing: bool,
+        auto_start: bool,
     ) -> Tuple[AuxiliaryAlias, AuxiliaryConfig]:
         """Craft the configuration dictionary for a proxy auxiliary to be
         attached to all auxiliaries sharing a communication channel.
 
         :param channel_name: name of the 'physical' channel that should
             be attached to the proxy auxiliary (the only direct connection).
         :param multiprocessing: whether the communication channel is
@@ -90,15 +92,15 @@
         from pykiso.lib.auxiliaries.mp_proxy_auxiliary import MpProxyAuxiliary
         from pykiso.lib.auxiliaries.proxy_auxiliary import ProxyAuxiliary
 
         aux_class = ProxyAuxiliary if not multiprocessing else MpProxyAuxiliary
         name = f"proxy_aux_{channel_name}"
         config = {
             "connectors": {"com": channel_name},
-            "config": {"aux_list": aux_list},
+            "config": {"aux_list": aux_list, "auto_start": auto_start},
             "type": f"{aux_class.__module__}:{aux_class.__name__}",
         }
         return name, config
 
     @staticmethod
     def _link_cchannel_to_auxiliaries(
         config: ConfigDict,
@@ -130,27 +132,37 @@
         # 1. Detect required proxy setups
         cchannel_to_auxiliaries = cls._link_cchannel_to_auxiliaries(config)
         proxies = []
 
         # 2. Overwrite auxiliary and connector config with required proxies
         for channel_name, auxiliaries in cchannel_to_auxiliaries.items():
             if len(auxiliaries) < 2:
-                # only one auxiliary holds the channel so there's nothing to patch
+                # only one auxiliary holds the channel so no proxy is required
                 continue
 
             # detect if communication channel is multiprocessing-based
             mp_enabled = False
-            if config["connectors"][channel_name].get("config") is not None:
-                mp_enabled = config["connectors"][channel_name]["config"].get(
-                    "processing", False
-                )
+            channel_cfg = config["connectors"][channel_name].get("config")
+            if channel_cfg is not None:
+                mp_enabled = channel_cfg.get("processing", False)
+
+            # automatically start proxy if at least one auxiliary has the auto_start flag set
+            for auxiliary in auxiliaries:
+                try:
+                    auto_start = config["auxiliaries"][auxiliary]["config"][
+                        "auto_start"
+                    ]
+                except KeyError:
+                    # default value for auto_start is True
+                    auto_start = True
+                    break
 
             # create a proxy auxiliary config for this shared channel
             proxy_aux_name, proxy_aux_cfg = cls._make_proxy_aux_config(
-                channel_name, auxiliaries, mp_enabled
+                channel_name, auxiliaries, mp_enabled, auto_start
             )
             config["auxiliaries"][proxy_aux_name] = proxy_aux_cfg
             proxies.append(proxy_aux_name)
 
             # create a proxy channel config for each of the auxiliaries sharing the channel
             for aux_name in auxiliaries:
                 cc_proxy_name, cc_proxy_cfg = cls._make_proxy_channel_config(
@@ -175,15 +187,20 @@
                 aux_details["type"],
                 aux_cons=aux_details.get("connectors") or dict(),
                 **cfg,
             )
 
         # 5. Finally, import required ProxyAuxiliary instances so that user doesn't have to
         for proxy_aux in proxies:
-            cls._linker._aux_cache.get_instance(proxy_aux)
+            try:
+                cls.get_aux_by_alias(proxy_aux)
+            except PykisoError:
+                # ensure that the created ProxyAuxiliary is stopped if its creation fails
+                cls.delete_aux_con()
+                raise
 
     @classmethod
     def delete_aux_con(cls) -> None:
         """Deregister the import hooks, close all running threads,
         delete all instances.
         """
         cls._linker.uninstall()
```

### Comparing `pykiso-0.21.2/src/pykiso/test_setup/dynamic_loader.py` & `pykiso-0.22.0/src/pykiso/test_setup/dynamic_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,14 +227,20 @@
             f"instantiating {name}: {self.modules[name]}({self.configs[name]})"
         )
         inst = self.modules[name](name=name, **self.configs[name])
         self.instances[name] = inst
         log.internal_debug(f"instantiated {name}")
         return inst
 
+    def delete_all_instances(self) -> None:
+        """Call custom del method if it exists"""
+        for instance in self.instances.values():
+            if callable(getattr(instance, "__del__", None)):
+                instance.__del__()
+
 
 class AuxiliaryCache(ModuleCache):
     """A ModuleCache that specifically provides Auxiliaries.
 
     This has the additional functionality that if an auxiliary has any defined connectors,
     these will be provided automatically.
     """
@@ -351,14 +357,15 @@
         self._aux_cache.provide(name, module, connectors=aux_cons, **config_params)
         self._aux_loader.provide(name)
 
     def uninstall(self):
         """Deregister the import hooks, close all running threads, delete all instances."""
         log.internal_debug("closing and uninstalling all dynamic modules and loaders")
         self._stop_auxiliaries()
+        self._con_cache.delete_all_instances()
         del self._con_cache
         del self._aux_cache
         del self._aux_loader
         for finder in self._finders:
             sys.meta_path.remove(finder)
 
     def _stop_auxiliaries(self):
```

### Comparing `pykiso-0.21.2/src/pykiso/tool/pykiso_to_pytest/cli.py` & `pykiso-0.22.0/src/pykiso/tool/pykiso_to_pytest/cli.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/tool/pykiso_to_pytest/templates/conftest_template.jinja2` & `pykiso-0.22.0/src/pykiso/tool/pykiso_to_pytest/templates/conftest_template.jinja2`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/tool/show_tag.py` & `pykiso-0.22.0/src/pykiso/tool/show_tag.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/tool/testrail/api.py` & `pykiso-0.22.0/src/pykiso/tool/testrail/api.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/tool/testrail/cli.py` & `pykiso-0.22.0/src/pykiso/tool/testrail/cli.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/tool/testrail/console.py` & `pykiso-0.22.0/src/pykiso/tool/testrail/console.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/tool/testrail/containers.py` & `pykiso-0.22.0/src/pykiso/tool/testrail/containers.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/tool/testrail/extraction.py` & `pykiso-0.22.0/src/pykiso/tool/testrail/extraction.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/tool/testrail/testrail.py` & `pykiso-0.22.0/src/pykiso/tool/testrail/testrail.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.21.2/src/pykiso/types.py` & `pykiso-0.22.0/src/pykiso/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,7 +57,16 @@
     test_suite_id: int
 
 
 class ConfigDict(TypedDict):
     auxiliaries: Dict[AuxiliaryAlias, AuxiliaryConfig]
     connectors: Dict[ConnectorAlias, ConnectorConfig]
     test_suite_list: List[SuiteConfig]
+
+
+class OdxParamDict(TypedDict):
+    parameter: str
+
+
+class OdxRequestConfigDict(TypedDict):
+    service: int
+    data: OdxParamDict
```

### Comparing `pykiso-0.21.2/setup.py` & `pykiso-0.22.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,47 +27,62 @@
 {'': ['*'],
  'pykiso.test_result': ['templates/*'],
  'pykiso.tool.pykiso_to_pytest': ['templates/*']}
 
 install_requires = \
 ['Jinja2>=2.11.0,<4.0.0',
  'MarkupSafe>=2.0.1,<2.1.0',
- 'PyVISA-py>=0.5.3,<0.6.0',
- 'PyVISA>=1.12.0,<2.0.0',
  'PyYAML>=6.0,<7.0',
  'brainstem',
  'click>=7.0.0,<9.0.0',
  'hidapi>=0.12.0.post2,<0.13.0',
- 'pykiso-python-uds>=3.0.2,<3.1.0',
- 'pylink-square>=0.12,<0.15',
- 'pyserial>=3.0,<4.0',
- 'python-can[pcan]>=4.1.0,<4.2.0',
  'robotframework==3.2.2',
  'tabulate>=0.8.9,<0.10.0',
  'unittest-xml-reporting>=3.2.0,<4.0.0']
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata>=4.12,<6.0'],
  ':python_version >= "3.5" and python_version < "4.0"': ['pyreadline3>=3.4.1,<4.0.0'],
- 'all': ['rich>=13.2.0,<14.0.0', 'requests>=2.28.2,<3.0.0'],
+ 'all': ['rich>=13.2.0,<14.0.0',
+         'requests>=2.28.2,<3.0.0',
+         'isort>=5.11.4',
+         'black==22.10.0',
+         'pylink-square>=0.12,<0.15',
+         'pykiso-python-uds>=3.0.2,<3.1.0',
+         'pyserial>=3.0,<4.0',
+         'PyVISA>=1.12.0,<2.0.0',
+         'PyVISA-py>=0.5.3,<0.6.0',
+         'python-can[pcan,vector]>=4.0.0,<5.0.0'],
+ 'can': ['pykiso-python-uds>=3.0.2,<3.1.0',
+         'python-can[pcan,vector]>=4.0.0,<5.0.0'],
+ 'debugger': ['pylink-square>=0.12,<0.15'],
+ 'instrument': ['PyVISA>=1.12.0,<2.0.0', 'PyVISA-py>=0.5.3,<0.6.0'],
+ 'plugins': ['pylink-square>=0.12,<0.15',
+             'pykiso-python-uds>=3.0.2,<3.1.0',
+             'pyserial>=3.0,<4.0',
+             'PyVISA>=1.12.0,<2.0.0',
+             'PyVISA-py>=0.5.3,<0.6.0',
+             'python-can[pcan,vector]>=4.0.0,<5.0.0'],
+ 'pykitest': ['isort>=5.11.4', 'black==22.10.0'],
+ 'serial': ['pyserial>=3.0,<4.0'],
  'testrail': ['rich>=13.2.0,<14.0.0', 'requests>=2.28.2,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['instrument-control = '
                      'pykiso.lib.auxiliaries.instrument_control_auxiliary.instrument_control_cli:main',
                      'pykiso = pykiso.cli:main',
                      'pykiso-tags = pykiso.tool.show_tag:main',
                      'pykitest = pykiso.tool.pykiso_to_pytest.cli:main',
                      'testrail = pykiso.tool.testrail.cli:cli_testrail']}
 
 setup_kwargs = {
     'name': 'pykiso',
-    'version': '0.21.2',
+    'version': '0.22.0',
     'description': 'Embedded integration testing framework.',
-    'long_description': '[![License](https://img.shields.io/badge/Licence-Eclipse%20Public%20License%202.0-lightgrey)](https://opensource.org/licenses/EPL-2.0)\n[![Platforms](https://img.shields.io/badge/Platforms-win64%20linux64%20osx64-lightgrey)]()\n[![Supported python version](https://img.shields.io/pypi/pyversions/pykiso)]()\n[![Build status](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fci.eclipse.org%2Fkiso-testing%2Fjob%2Fkiso-testing%2Fjob%2Fmaster%2F)](https://ci.eclipse.org/kiso-testing/job/kiso-testing/job/master/)\n[![Documentation Status](https://readthedocs.org/projects/kiso-testing/badge/?version=latest)](https://kiso-testing.readthedocs.io/en/latest/?badge=latest)\n[![Test results](https://img.shields.io/jenkins/tests?compact_message&failed_label=failed&jobUrl=https%3A%2F%2Fci.eclipse.org%2Fkiso-testing%2Fjob%2Fkiso-testing%2Fjob%2Fmaster%2F&passed_label=passed&skipped_label=skipped)](https://ci.eclipse.org/kiso-testing/job/kiso-testing/job/master/)\n[![codecov](https://codecov.io/gh/eclipse/kiso-testing/branch/master/graph/badge.svg?token=IBKQ700ABS)](https://codecov.io/gh/eclipse/kiso-testing)\n[![Code quality](https://img.shields.io/lgtm/grade/python/github/eclipse/kiso-testing)]()\n[![Last commit](https://img.shields.io/github/last-commit/eclipse/kiso-testing)]()\n[![Commits since latest version](https://img.shields.io/github/commits-since/eclipse/kiso-testing/latest/master)]()\n\n# PyKiso\n\n![Optional Text](./docs/images/pykiso_logo.png)\n\n## Introduction ##\n\n**pykiso** is an integration test framework. With it, it is possible to write\n* Whitebox integration tests directly on my target device\n* Graybox integration tests to make sure the communication-link with my target device is working as expected\n* Blackbox integration tests to make sure my external device interfaces are working as expected\n\nThe project will contain:\n* The core python framework (this repository)\n* Framework plugins that are generic enough to be integrated as "native" (this repository)\n* Additional "testApps" for different targets platforms (e.g. stm32, ...) or languages (C, C++, ...) . It could be pure SW or also HW (other repositories)\n\n## Requirements ##\n\n* Python 3.7+\n* pip/poetry (used to get the rest of the requirements)\n\n## Install ##\n\n```bash\npip install pykiso\n```\n\n[Poetry](https://python-poetry.org/) is more appropriate for developers as it automatically creates virtual environments.\n\n```bash\ncd kiso-testing\npoetry install --all-extras\npoetry shell\n```\n\n### Pre-Commit\n\nTo improve code-quality, a configuration of [pre-commit](https://pre-commit.com/) hooks are available.\nThe following pre-commit hooks are used:\n\n- black\n- flake8\n- isort\n- trailing-whitespace\n- end-of-file-fixer\n- check-docstring-first\n- check-json\n- check-added-large-files\n- check-yaml\n- debug-statements\n\nIf you don\'t have pre-commit installed, you can get it using pip:\n\n```bash\npip install pre-commit\n```\n\nStart using the hooks with\n\n```bash\npre-commit install\n```\n\n## Commit message convention\n\nCommits are sorted into multiple categories based on keywords that can occur at any position as part of the commit message.\n[Category] Keywords\n* [BREAKING CHANGES] BREAKING CHANGE\n* [Features] feat:\n* [Fixes] fix:\n* [Docs] docs:\n* [Styles] style:\n* [Refactors] refactor!:\n* [Performances] perf:\n* [Tests] test:\n* [Build] build:\n* [Ci] ci:\nEach commit is considered only once according to the order of the categories listed above. Merge commits are ignored.\n\nThe tool commitizen can help you to create commits which follows these standards.\n```bash\n# if not yet installed:\npip install -U commitizen==2.20.4\n# helps you to create a commit:\ncz commit\n# or use equivalent short variant:\ncz c\n```\n\n## Generate Changelog\n\nAfter you installed the dev dependencies from the pipfile you are able to\nautogenerate the Changelog.\n\n```bash\ninvoke changelog\n```\n\n## Usage ##\n\nOnce installed the application is bound to `pykiso`, it can be called with the following arguments:\n\n```bash\nUsage: pykiso [OPTIONS]\n\n  Embedded Integration Test Framework - CLI Entry Point.\n\n  TAG Filters: any additional option to be passed to the test as tag through\n  the pykiso call. Multiple values must be separated with a comma.\n\n  For example: pykiso -c your_config.yaml --branch-level dev,master --variant\n  delta\n\nOptions:\n  -c, --test-configuration-file FILE\n                                  path to the test configuration file (in YAML\n                                  format)  [required]\n  -l, --log-path PATH             path to log-file or folder. If not set will\n                                  log to STDOUT\n  --log-level [DEBUG|INFO|WARNING|ERROR]\n                                  set the verbosity of the logging\n  --junit                         enables the generation of a junit report\n  --text                          default, test results are only displayed in\n                                  the console\n  --step-report PATH              generate the step report at the specified\n                                  path\n  --failfast                      stop the test run on the first error or\n                                  failure\n  -v, --verbose                   activate the internal framework logs\n  -p, --pattern TEXT              test filter pattern, e.g. \'test_suite_1.py\'\n                                  or \'test_*.py\'. Or even more granularly\n                                  \'test_suite_1.py::test_class::test_name\'\n  --version                       Show the version and exit.\n  -h, --help                      Show this message and exit.\n```\n\nSuitable config files are available in the `examples` folder.\n\n### Demo using example config ##\n\n```bash\ninvoke run\n```\n\n### Running the Tests ##\n\n```bash\ninvoke test\n```\n\nor\n\n```bash\npytest\n```\n',
+    'long_description': '[![License](https://img.shields.io/badge/Licence-Eclipse%20Public%20License%202.0-lightgrey)](https://opensource.org/licenses/EPL-2.0)\n[![Platforms](https://img.shields.io/badge/Platforms-win64%20linux64%20osx64-lightgrey)]()\n[![Supported python version](https://img.shields.io/pypi/pyversions/pykiso)]()\n[![Build status](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fci.eclipse.org%2Fkiso-testing%2Fjob%2Fkiso-testing%2Fjob%2Fmaster%2F)](https://ci.eclipse.org/kiso-testing/job/kiso-testing/job/master/)\n[![Documentation Status](https://readthedocs.org/projects/kiso-testing/badge/?version=latest)](https://kiso-testing.readthedocs.io/en/latest/?badge=latest)\n[![Test results](https://img.shields.io/jenkins/tests?compact_message&failed_label=failed&jobUrl=https%3A%2F%2Fci.eclipse.org%2Fkiso-testing%2Fjob%2Fkiso-testing%2Fjob%2Fmaster%2F&passed_label=passed&skipped_label=skipped)](https://ci.eclipse.org/kiso-testing/job/kiso-testing/job/master/)\n[![codecov](https://codecov.io/gh/eclipse/kiso-testing/branch/master/graph/badge.svg?token=IBKQ700ABS)](https://codecov.io/gh/eclipse/kiso-testing)\n[![CodeFactor](https://www.codefactor.io/repository/github/eclipse/kiso-testing/badge)](https://www.codefactor.io/repository/github/eclipse/kiso-testing)\n[![Last commit](https://img.shields.io/github/last-commit/eclipse/kiso-testing)]()\n[![Commits since latest version](https://img.shields.io/github/commits-since/eclipse/kiso-testing/latest/master)]()\n\n# PyKiso\n\n![Optional Text](./docs/images/pykiso_logo.png)\n\n## Introduction ##\n\n**pykiso** is an integration test framework. With it, it is possible to write\n* Whitebox integration tests directly on my target device\n* Graybox integration tests to make sure the communication-link with my target device is working as expected\n* Blackbox integration tests to make sure my external device interfaces are working as expected\n\nThe project will contain:\n* The core python framework (this repository)\n* Framework plugins that are generic enough to be integrated as "native" (this repository)\n* Additional "testApps" for different targets platforms (e.g. stm32, ...) or languages (C, C++, ...) . It could be pure SW or also HW (other repositories)\n\n## Link to Eclipse Project\nhttps://projects.eclipse.org/projects/iot.kiso-testing\n\n## Requirements ##\n\n* Python 3.7+\n* pip/poetry (used to get the rest of the requirements)\n\n## Install ##\n\n```bash\npip install pykiso # Core framework\npip install pykiso[plugins] # For installing all plugins\npip install pykiso[all] # For installing all what we have to offer\n```\n\n[Poetry](https://python-poetry.org/) is more appropriate for developers as it automatically creates virtual environments.\n\n```bash\ncd kiso-testing\npoetry install --all-extras\npoetry shell\n```\n\n### Pre-Commit\n\nTo improve code-quality, a configuration of [pre-commit](https://pre-commit.com/) hooks are available.\nThe following pre-commit hooks are used:\n\n- black\n- flake8\n- isort\n- trailing-whitespace\n- end-of-file-fixer\n- check-docstring-first\n- check-json\n- check-added-large-files\n- check-yaml\n- debug-statements\n\nIf you don\'t have pre-commit installed, you can get it using pip:\n\n```bash\npip install pre-commit\n```\n\nStart using the hooks with\n\n```bash\npre-commit install\n```\n\n## Commit message convention\n\nCommits are sorted into multiple categories based on keywords that can occur at any position as part of the commit message.\n[Category] Keywords\n* [BREAKING CHANGES] BREAKING CHANGE\n* [Features] feat:\n* [Fixes] fix:\n* [Docs] docs:\n* [Styles] style:\n* [Refactors] refactor!:\n* [Performances] perf:\n* [Tests] test:\n* [Build] build:\n* [Ci] ci:\nEach commit is considered only once according to the order of the categories listed above. Merge commits are ignored.\n\nThe tool commitizen can help you to create commits which follows these standards.\n```bash\n# if not yet installed:\npip install -U commitizen==2.20.4\n# helps you to create a commit:\ncz commit\n# or use equivalent short variant:\ncz c\n```\n\n## Generate Changelog\n\nAfter you installed the dev dependencies from the pipfile you are able to\nautogenerate the Changelog.\n\n```bash\ninvoke changelog\n```\n\n## Usage ##\n\nOnce installed the application is bound to `pykiso`, it can be called with the following arguments:\n\n```bash\nUsage: pykiso [OPTIONS]\n\n  Embedded Integration Test Framework - CLI Entry Point.\n\n  TAG Filters: any additional option to be passed to the test as tag through\n  the pykiso call. Multiple values must be separated with a comma.\n\n  For example: pykiso -c your_config.yaml --branch-level dev,master --variant\n  delta\n\nOptions:\n  -c, --test-configuration-file FILE\n                                  path to the test configuration file (in YAML\n                                  format)  [required]\n  -l, --log-path PATH             path to log-file or folder. If not set will\n                                  log to STDOUT\n  --log-level [DEBUG|INFO|WARNING|ERROR]\n                                  set the verbosity of the logging\n  --junit                         enables the generation of a junit report\n  --text                          default, test results are only displayed in\n                                  the console\n  --step-report PATH              generate the step report at the specified\n                                  path\n  --failfast                      stop the test run on the first error or\n                                  failure\n  -v, --verbose                   activate the internal framework logs\n  -p, --pattern TEXT              test filter pattern, e.g. \'test_suite_1.py\'\n                                  or \'test_*.py\'. Or even more granularly\n                                  \'test_suite_1.py::test_class::test_name\'\n  --version                       Show the version and exit.\n  -h, --help                      Show this message and exit.\n```\n\nSuitable config files are available in the `examples` folder.\n\n### Demo using example config ##\n\n```bash\ninvoke run\n```\n\n### Running the Tests ##\n\n```bash\ninvoke test\n```\n\nor\n\n```bash\npytest\n```\n',
     'author': 'Sebastian Fischer',
     'author_email': 'sebastian.fischer@de.bosch.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pypi.org/project/pykiso/',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `pykiso-0.21.2/PKG-INFO` & `pykiso-0.22.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykiso
-Version: 0.21.2
+Version: 0.22.0
 Summary: Embedded integration testing framework.
 Home-page: https://pypi.org/project/pykiso/
 License: Eclipse Public License - v 2.0
 Keywords: testing,integration testing,framework,testing framework
 Author: Sebastian Fischer
 Author-email: sebastian.fischer@de.bosch.com
 Requires-Python: >=3.7,<4.0
@@ -26,29 +26,37 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
 Provides-Extra: all
+Provides-Extra: can
+Provides-Extra: debugger
+Provides-Extra: instrument
+Provides-Extra: plugins
+Provides-Extra: pykitest
+Provides-Extra: serial
 Provides-Extra: testrail
 Requires-Dist: Jinja2 (>=2.11.0,<4.0.0)
 Requires-Dist: MarkupSafe (>=2.0.1,<2.1.0)
-Requires-Dist: PyVISA (>=1.12.0,<2.0.0)
-Requires-Dist: PyVISA-py (>=0.5.3,<0.6.0)
+Requires-Dist: PyVISA (>=1.12.0,<2.0.0) ; extra == "plugins" or extra == "instrument" or extra == "all"
+Requires-Dist: PyVISA-py (>=0.5.3,<0.6.0) ; extra == "plugins" or extra == "instrument" or extra == "all"
 Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: black (==22.10.0) ; extra == "pykitest" or extra == "all"
 Requires-Dist: brainstem
 Requires-Dist: click (>=7.0.0,<9.0.0)
 Requires-Dist: hidapi (>=0.12.0.post2,<0.13.0)
 Requires-Dist: importlib-metadata (>=4.12,<6.0) ; python_version < "3.8"
-Requires-Dist: pykiso-python-uds (>=3.0.2,<3.1.0)
-Requires-Dist: pylink-square (>=0.12,<0.15)
+Requires-Dist: isort (>=5.11.4) ; extra == "pykitest" or extra == "all"
+Requires-Dist: pykiso-python-uds (>=3.0.2,<3.1.0) ; extra == "plugins" or extra == "can" or extra == "all"
+Requires-Dist: pylink-square (>=0.12,<0.15) ; extra == "plugins" or extra == "debugger" or extra == "all"
 Requires-Dist: pyreadline3 (>=3.4.1,<4.0.0) ; python_version >= "3.5" and python_version < "4.0"
-Requires-Dist: pyserial (>=3.0,<4.0)
-Requires-Dist: python-can[pcan] (>=4.1.0,<4.2.0)
+Requires-Dist: pyserial (>=3.0,<4.0) ; extra == "plugins" or extra == "serial" or extra == "all"
+Requires-Dist: python-can[pcan,vector] (>=4.0.0,<5.0.0) ; extra == "plugins" or extra == "can" or extra == "all"
 Requires-Dist: requests (>=2.28.2,<3.0.0) ; extra == "testrail" or extra == "all"
 Requires-Dist: rich (>=13.2.0,<14.0.0) ; extra == "testrail" or extra == "all"
 Requires-Dist: robotframework (==3.2.2)
 Requires-Dist: tabulate (>=0.8.9,<0.10.0)
 Requires-Dist: unittest-xml-reporting (>=3.2.0,<4.0.0)
 Project-URL: Documentation, https://kiso-testing.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/eclipse/kiso-testing
@@ -57,15 +65,15 @@
 [![License](https://img.shields.io/badge/Licence-Eclipse%20Public%20License%202.0-lightgrey)](https://opensource.org/licenses/EPL-2.0)
 [![Platforms](https://img.shields.io/badge/Platforms-win64%20linux64%20osx64-lightgrey)]()
 [![Supported python version](https://img.shields.io/pypi/pyversions/pykiso)]()
 [![Build status](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fci.eclipse.org%2Fkiso-testing%2Fjob%2Fkiso-testing%2Fjob%2Fmaster%2F)](https://ci.eclipse.org/kiso-testing/job/kiso-testing/job/master/)
 [![Documentation Status](https://readthedocs.org/projects/kiso-testing/badge/?version=latest)](https://kiso-testing.readthedocs.io/en/latest/?badge=latest)
 [![Test results](https://img.shields.io/jenkins/tests?compact_message&failed_label=failed&jobUrl=https%3A%2F%2Fci.eclipse.org%2Fkiso-testing%2Fjob%2Fkiso-testing%2Fjob%2Fmaster%2F&passed_label=passed&skipped_label=skipped)](https://ci.eclipse.org/kiso-testing/job/kiso-testing/job/master/)
 [![codecov](https://codecov.io/gh/eclipse/kiso-testing/branch/master/graph/badge.svg?token=IBKQ700ABS)](https://codecov.io/gh/eclipse/kiso-testing)
-[![Code quality](https://img.shields.io/lgtm/grade/python/github/eclipse/kiso-testing)]()
+[![CodeFactor](https://www.codefactor.io/repository/github/eclipse/kiso-testing/badge)](https://www.codefactor.io/repository/github/eclipse/kiso-testing)
 [![Last commit](https://img.shields.io/github/last-commit/eclipse/kiso-testing)]()
 [![Commits since latest version](https://img.shields.io/github/commits-since/eclipse/kiso-testing/latest/master)]()
 
 # PyKiso
 
 ![Optional Text](./docs/images/pykiso_logo.png)
 
@@ -77,23 +85,28 @@
 * Blackbox integration tests to make sure my external device interfaces are working as expected
 
 The project will contain:
 * The core python framework (this repository)
 * Framework plugins that are generic enough to be integrated as "native" (this repository)
 * Additional "testApps" for different targets platforms (e.g. stm32, ...) or languages (C, C++, ...) . It could be pure SW or also HW (other repositories)
 
+## Link to Eclipse Project
+https://projects.eclipse.org/projects/iot.kiso-testing
+
 ## Requirements ##
 
 * Python 3.7+
 * pip/poetry (used to get the rest of the requirements)
 
 ## Install ##
 
 ```bash
-pip install pykiso
+pip install pykiso # Core framework
+pip install pykiso[plugins] # For installing all plugins
+pip install pykiso[all] # For installing all what we have to offer
 ```
 
 [Poetry](https://python-poetry.org/) is more appropriate for developers as it automatically creates virtual environments.
 
 ```bash
 cd kiso-testing
 poetry install --all-extras
```

