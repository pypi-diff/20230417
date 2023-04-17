# Comparing `tmp/pyinsteon-1.4.1.tar.gz` & `tmp/pyinsteon-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinsteon-1.4.1.tar", last modified: Tue Mar 21 20:50:35 2023, max compression
+gzip compressed data, was "pyinsteon-1.4.2.tar", last modified: Mon Apr 17 20:57:29 2023, max compression
```

## Comparing `pyinsteon-1.4.1.tar` & `pyinsteon-1.4.2.tar`

### file list

```diff
@@ -1,238 +1,239 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.315112 pyinsteon-1.4.1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1547 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/DESCRIPTION.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1067 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/LICENSE.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       53 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2494 2023-03-21 20:50:35.315112 pyinsteon-1.4.1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2144 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/README.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.205112 pyinsteon-1.4.1/pyinsteon/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3724 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      126 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/__main__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2917 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/pyinsteon/address.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.215112 pyinsteon-1.4.1/pyinsteon/aldb/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      183 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/pyinsteon/aldb/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5199 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/aldb/aldb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    19321 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/aldb/aldb_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1841 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/aldb/aldb_battery.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8984 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/aldb/aldb_record.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4042 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/aldb/mock_modem_aldb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3920 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/aldb/modem_aldb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3743 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/aldb/no_aldb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    21739 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/commands.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.225112 pyinsteon-1.4.1/pyinsteon/config/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5115 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/config/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1125 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/config/derived_property.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3681 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/config/device_flag.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      603 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/config/extended_property.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      418 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/config/modem_config.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2150 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/config/momentary_delay.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1794 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/config/op_flag_property.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3017 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/config/op_flag_property_byte.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      624 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/config/operating_flag.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5463 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/config/radio_button.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1692 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/config/ramp_rate.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3635 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/config/relay_mode.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3445 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/config/toggle_button.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10950 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/constants.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.225112 pyinsteon-1.4.1/pyinsteon/data_types/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       32 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/data_types/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5126 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/data_types/all_link_record_flags.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4242 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/data_types/im_config_flags.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3663 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/data_types/io_sensor_config_flags.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8465 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/data_types/message_flags.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5551 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/data_types/user_data.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      226 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/default_link.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.235112 pyinsteon-1.4.1/pyinsteon/device_types/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/pyinsteon/device_types/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1283 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/device_types/access_control.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6666 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/device_types/battery_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    20054 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/device_types/climate_control.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11276 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/device_types/device_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1183 2022-08-03 19:37:40.000000 pyinsteon-1.4.1/pyinsteon/device_types/device_commands.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    32988 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/device_types/dimmable_lighting_control.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2469 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/device_types/energy_management.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4964 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/pyinsteon/device_types/general_controller.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      486 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/device_types/hub.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14472 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/device_types/i3_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    41731 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/device_types/ipdb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      517 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/pyinsteon/device_types/mock_modem.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7987 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/device_types/modem_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5226 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/device_types/on_off_controller_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4225 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/device_types/on_off_responder_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5172 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/device_types/open_close_controller_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4092 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/device_types/open_close_responder_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      646 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/device_types/plm.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26934 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/device_types/security_health_safety.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14495 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/device_types/sensors_actuators.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    25431 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/device_types/switched_lighting_control.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      137 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/device_types/unknown_device.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4446 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/device_types/variable_controller_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4143 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/device_types/variable_responder_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2294 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/device_types/window_coverings.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7184 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/device_types/x10.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3889 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/device_types/x10_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3364 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/events.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.245112 pyinsteon-1.4.1/pyinsteon/groups/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1450 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/groups/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      888 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/groups/fan.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1778 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/groups/group_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      607 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/groups/on_level.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1438 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/groups/on_off.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1146 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/groups/open_close.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4480 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/groups/thermostat.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      935 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/groups/wet_dry.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.255112 pyinsteon-1.4.1/pyinsteon/handlers/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4317 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      688 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/all_link_cleanup_failure_report.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      756 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/all_link_cleanup_status_report.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      998 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/all_link_completed.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1740 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/all_link_record_response.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      735 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/cancel_all_linking.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.275112 pyinsteon-1.4.1/pyinsteon/handlers/from_device/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      293 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      551 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/all_link_cleanup_command.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      901 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/assign_to_all_link_group.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1948 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/broadcast_command.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      911 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/delete_from_all_link_group.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1414 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/ext_get_response.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      580 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/manual_change.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      542 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/off.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      660 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/off_all_link_cleanup.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      560 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/off_fast.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      689 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/off_fast_all_link_cleanup.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      577 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/on_fast.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      676 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/on_fast_all_link_cleanup.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      569 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/on_level.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      657 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/on_level_all_link_cleanup.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2174 2023-01-31 20:55:03.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/receive_aldb_record.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      850 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/thermostat_cool_set_point.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      846 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/thermostat_heat_set_point.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      831 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/thermostat_humidity.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      928 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/thermostat_mode.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      846 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/thermostat_temperature.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1692 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/from_device/x10_received.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      909 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/get_first_all_link_record.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1032 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/get_im_configuration.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      854 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/get_im_info.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      845 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/get_next_all_link_record.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1531 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/inbound_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1882 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/manage_all_link_record.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2858 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/outbound_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1188 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/read_eeprom.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1787 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/read_eeprom_response.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      948 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/send_all_link.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      427 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/send_all_link_off.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/send_all_link_on.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1560 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/set_im_configuration.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      961 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/start_all_linking.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.295112 pyinsteon-1.4.1/pyinsteon/handlers/to_device/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      491 2023-01-17 15:33:19.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1588 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/all_link_cleanup_command.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3741 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/direct_command.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1150 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/engine_version_request.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      826 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/enter_linking_mode.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      705 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/enter_unlinking_mode.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1642 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/extended_get.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1930 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/extended_set.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1011 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/get_operating_flags.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      562 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/id_request.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      761 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/night_mode_off.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      754 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/night_mode_on.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      733 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/off.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      634 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/off_all_link_cleanup.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      746 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/off_fast.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      802 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/on_fast.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      881 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/on_level.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      704 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/on_level_all_link_cleanup.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      688 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/peek.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      532 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/ping.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      694 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/poke.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1046 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/product_data_request.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1382 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/read_aldb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1249 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/set_leds.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      771 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/set_msb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1638 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/set_operating_flags.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1966 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/status_request.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1392 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/temperature_down.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1384 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/temperature_up.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1701 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/thermostat_cool_set_point.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1710 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/thermostat_heat_set_point.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1609 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/thermostat_mode.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1311 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/trigger_scene_off.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1412 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/trigger_scene_on.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1338 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/write_aldb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2069 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/to_device/x10_send.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2172 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/handlers/write_eeprom.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      457 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/listener_exception_handler.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.305112 pyinsteon-1.4.1/pyinsteon/managers/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      187 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/managers/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9814 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/pyinsteon/managers/aldb_im_read_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5038 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/managers/aldb_im_write_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10560 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/managers/aldb_read_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3426 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/managers/aldb_write_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10515 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/managers/device_id_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8762 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/pyinsteon/managers/device_link_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13780 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/managers/device_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2465 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/managers/ext_get_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1362 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/managers/ext_prop_read_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1928 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/managers/ext_prop_write_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6700 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/managers/get_set_ext_property_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5706 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/managers/get_set_op_flag_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3447 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/managers/heartbeat_manager.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.305112 pyinsteon-1.4.1/pyinsteon/managers/link_manager/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8816 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/managers/link_manager/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1310 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/pyinsteon/managers/link_manager/default_links.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2704 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/managers/low_batter_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6770 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/managers/on_level_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5027 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/managers/peek_poke_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12007 2023-03-21 20:28:02.000000 pyinsteon-1.4.1/pyinsteon/managers/saved_devices_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11025 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/pyinsteon/managers/scene_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7286 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/managers/thermostat_status_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1086 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/pyinsteon/managers/utils.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2008 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/managers/wet_dry_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4954 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/managers/x10_manager.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.315112 pyinsteon-1.4.1/pyinsteon/protocol/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3137 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/pyinsteon/protocol/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    31052 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/protocol/command_to_msg.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6120 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/protocol/http_reader_writer.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8549 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/protocol/http_transport.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      111 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/protocol/hub_connection_exception.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.315112 pyinsteon-1.4.1/pyinsteon/protocol/messages/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1896 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/protocol/messages/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4046 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/protocol/messages/inbound.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1367 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/protocol/messages/message_definition.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14193 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/protocol/messages/message_definitions.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11565 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/protocol/messages/outbound.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.315112 pyinsteon-1.4.1/pyinsteon/protocol/mock/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/pyinsteon/protocol/mock/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1925 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/protocol/mock/mock_reader.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8033 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/protocol/mock/mock_transport.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15192 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/protocol/msg_to_topic.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      838 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/protocol/msg_to_url.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9176 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/protocol/protocol.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2074 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/protocol/serial_transport.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      811 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/protocol/topic_converters.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       83 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/pyinsteon/run_tool.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1217 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/subscriber_base.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.315112 pyinsteon-1.4.1/pyinsteon/tools/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    18580 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/tools/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    24420 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/tools/advanced.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10429 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/tools/aldb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10133 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/tools/commands.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17206 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/tools/config.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1873 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/tools/log_filter.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7748 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/pyinsteon/tools/scenes.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    49434 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/tools/tools_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3246 2023-03-02 20:10:08.000000 pyinsteon-1.4.1/pyinsteon/tools/utils.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5934 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyinsteon/topics.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12422 2023-01-25 15:15:30.000000 pyinsteon-1.4.1/pyinsteon/utils.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4753 2022-07-18 19:50:59.000000 pyinsteon-1.4.1/pyinsteon/x10_address.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-21 20:50:35.215112 pyinsteon-1.4.1/pyinsteon.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2494 2023-03-21 20:50:34.000000 pyinsteon-1.4.1/pyinsteon.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8610 2023-03-21 20:50:35.000000 pyinsteon-1.4.1/pyinsteon.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-03-21 20:50:34.000000 pyinsteon-1.4.1/pyinsteon.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       56 2023-03-21 20:50:34.000000 pyinsteon-1.4.1/pyinsteon.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-01-17 15:49:42.000000 pyinsteon-1.4.1/pyinsteon.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       68 2023-03-21 20:50:34.000000 pyinsteon-1.4.1/pyinsteon.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-03-21 20:50:34.000000 pyinsteon-1.4.1/pyinsteon.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6539 2023-03-21 20:46:57.000000 pyinsteon-1.4.1/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      799 2023-03-21 20:50:35.325112 pyinsteon-1.4.1/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.914636 pyinsteon-1.4.2/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1547 2023-02-09 23:41:45.000000 pyinsteon-1.4.2/DESCRIPTION.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1067 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/LICENSE.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       53 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2494 2023-04-17 20:57:29.914636 pyinsteon-1.4.2/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2144 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/README.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.890637 pyinsteon-1.4.2/pyinsteon/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3724 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      126 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/__main__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2917 2023-02-09 23:41:45.000000 pyinsteon-1.4.2/pyinsteon/address.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.894636 pyinsteon-1.4.2/pyinsteon/aldb/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      183 2023-02-09 23:41:45.000000 pyinsteon-1.4.2/pyinsteon/aldb/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5199 2023-04-17 20:56:19.000000 pyinsteon-1.4.2/pyinsteon/aldb/aldb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    19321 2023-04-17 20:56:19.000000 pyinsteon-1.4.2/pyinsteon/aldb/aldb_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1841 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/aldb/aldb_battery.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8984 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/aldb/aldb_record.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4042 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/aldb/mock_modem_aldb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3920 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/aldb/modem_aldb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3743 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/aldb/no_aldb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    21913 2023-04-17 20:56:26.000000 pyinsteon-1.4.2/pyinsteon/commands.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.894636 pyinsteon-1.4.2/pyinsteon/config/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5073 2023-04-17 20:56:26.000000 pyinsteon-1.4.2/pyinsteon/config/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1125 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/config/derived_property.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3681 2023-03-20 19:36:03.000000 pyinsteon-1.4.2/pyinsteon/config/device_flag.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      603 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/config/extended_property.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      418 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/config/modem_config.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2150 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/config/momentary_delay.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1794 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/config/op_flag_property.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3457 2023-04-17 20:56:26.000000 pyinsteon-1.4.2/pyinsteon/config/op_flag_property_byte.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      624 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/config/operating_flag.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5463 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/config/radio_button.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1692 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/config/ramp_rate.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3635 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/config/relay_mode.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3445 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/config/toggle_button.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10950 2023-03-20 19:36:03.000000 pyinsteon-1.4.2/pyinsteon/constants.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.894636 pyinsteon-1.4.2/pyinsteon/data_types/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       32 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/data_types/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5126 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/data_types/all_link_record_flags.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4242 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/data_types/im_config_flags.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3663 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/data_types/io_sensor_config_flags.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8465 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/data_types/message_flags.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5551 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/data_types/user_data.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      226 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/default_link.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.898636 pyinsteon-1.4.2/pyinsteon/device_types/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-02-09 23:41:45.000000 pyinsteon-1.4.2/pyinsteon/device_types/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1283 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/device_types/access_control.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6666 2023-03-20 19:36:03.000000 pyinsteon-1.4.2/pyinsteon/device_types/battery_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    20054 2023-04-14 18:38:06.000000 pyinsteon-1.4.2/pyinsteon/device_types/climate_control.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11276 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/device_types/device_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1183 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/device_types/device_commands.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    32875 2023-04-17 20:56:26.000000 pyinsteon-1.4.2/pyinsteon/device_types/dimmable_lighting_control.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2469 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/device_types/energy_management.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4964 2023-02-09 23:41:45.000000 pyinsteon-1.4.2/pyinsteon/device_types/general_controller.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      486 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/device_types/hub.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15774 2023-04-17 20:56:26.000000 pyinsteon-1.4.2/pyinsteon/device_types/i3_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    41731 2023-03-20 19:36:03.000000 pyinsteon-1.4.2/pyinsteon/device_types/ipdb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      517 2023-02-09 23:41:45.000000 pyinsteon-1.4.2/pyinsteon/device_types/mock_modem.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7987 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/device_types/modem_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5226 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/device_types/on_off_controller_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4225 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/device_types/on_off_responder_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5172 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/device_types/open_close_controller_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4092 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/device_types/open_close_responder_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      646 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/device_types/plm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    26934 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/device_types/security_health_safety.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14495 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/device_types/sensors_actuators.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    25597 2023-04-17 20:56:26.000000 pyinsteon-1.4.2/pyinsteon/device_types/switched_lighting_control.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      137 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/device_types/unknown_device.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4446 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/device_types/variable_controller_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4143 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/device_types/variable_responder_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2294 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/device_types/window_coverings.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7184 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/device_types/x10.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3889 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/device_types/x10_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3364 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/events.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.898636 pyinsteon-1.4.2/pyinsteon/groups/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1450 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/groups/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      888 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/groups/fan.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1778 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/groups/group_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      607 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/groups/on_level.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1438 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/groups/on_off.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1146 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/groups/open_close.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4480 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/groups/thermostat.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      935 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/groups/wet_dry.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.902637 pyinsteon-1.4.2/pyinsteon/handlers/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4317 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/handlers/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      688 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/all_link_cleanup_failure_report.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      756 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/all_link_cleanup_status_report.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      998 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/all_link_completed.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1740 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/all_link_record_response.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      735 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/cancel_all_linking.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.902637 pyinsteon-1.4.2/pyinsteon/handlers/from_device/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      293 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      551 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/all_link_cleanup_command.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      901 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/assign_to_all_link_group.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1948 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/broadcast_command.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      911 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/delete_from_all_link_group.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1702 2023-04-17 20:56:26.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/ext_get_response.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      580 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/manual_change.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      542 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/off.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      660 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/off_all_link_cleanup.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      560 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/off_fast.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      689 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/off_fast_all_link_cleanup.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      577 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/on_fast.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      676 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/on_fast_all_link_cleanup.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      569 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/on_level.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      657 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/on_level_all_link_cleanup.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2174 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/receive_aldb_record.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      850 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/thermostat_cool_set_point.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      846 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/thermostat_heat_set_point.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      831 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/thermostat_humidity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      928 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/thermostat_mode.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      846 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/thermostat_temperature.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1692 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/from_device/x10_received.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      909 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/handlers/get_first_all_link_record.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1032 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/get_im_configuration.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      854 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/get_im_info.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      845 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/get_next_all_link_record.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1531 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/inbound_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1882 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/manage_all_link_record.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2858 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/outbound_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1188 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/handlers/read_eeprom.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1787 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/read_eeprom_response.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      948 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/send_all_link.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      427 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/send_all_link_off.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/send_all_link_on.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1560 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/set_im_configuration.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      961 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/start_all_linking.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.906637 pyinsteon-1.4.2/pyinsteon/handlers/to_device/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      491 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1588 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/all_link_cleanup_command.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3741 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/direct_command.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1150 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/engine_version_request.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      826 2023-03-07 05:38:59.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/enter_linking_mode.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      705 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/enter_unlinking_mode.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1711 2023-04-17 20:56:26.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/extended_get.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1930 2023-03-20 19:36:03.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/extended_set.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      934 2023-04-17 20:56:26.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/factory_reset.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1011 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/get_operating_flags.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      562 2023-01-23 13:39:25.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/id_request.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      761 2023-03-20 19:36:03.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/night_mode_off.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      754 2023-03-20 19:36:03.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/night_mode_on.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      733 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/off.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      634 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/off_all_link_cleanup.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      746 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/off_fast.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      802 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/on_fast.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      881 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/on_level.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      704 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/on_level_all_link_cleanup.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      688 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/peek.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      532 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/ping.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      694 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/poke.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1046 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/product_data_request.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1382 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/read_aldb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1249 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/set_leds.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      771 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/set_msb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1638 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/set_operating_flags.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1966 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/status_request.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1392 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/temperature_down.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1384 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/temperature_up.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1701 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/thermostat_cool_set_point.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1710 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/thermostat_heat_set_point.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1609 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/thermostat_mode.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1311 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/trigger_scene_off.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1412 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/trigger_scene_on.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1338 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/write_aldb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2069 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/handlers/to_device/x10_send.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2172 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/handlers/write_eeprom.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      457 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/listener_exception_handler.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.910637 pyinsteon-1.4.2/pyinsteon/managers/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      187 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/managers/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9814 2023-02-09 23:42:43.000000 pyinsteon-1.4.2/pyinsteon/managers/aldb_im_read_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5038 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/managers/aldb_im_write_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10560 2023-04-17 20:56:19.000000 pyinsteon-1.4.2/pyinsteon/managers/aldb_read_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3426 2023-02-20 18:35:53.000000 pyinsteon-1.4.2/pyinsteon/managers/aldb_write_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10515 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/managers/device_id_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8762 2023-02-09 23:41:45.000000 pyinsteon-1.4.2/pyinsteon/managers/device_link_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13780 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/managers/device_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2465 2023-03-20 19:36:03.000000 pyinsteon-1.4.2/pyinsteon/managers/ext_get_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1362 2023-03-20 19:36:03.000000 pyinsteon-1.4.2/pyinsteon/managers/ext_prop_read_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1962 2023-04-17 20:56:26.000000 pyinsteon-1.4.2/pyinsteon/managers/ext_prop_write_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6700 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/managers/get_set_ext_property_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5676 2023-04-17 20:56:26.000000 pyinsteon-1.4.2/pyinsteon/managers/get_set_op_flag_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3447 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/managers/heartbeat_manager.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.910637 pyinsteon-1.4.2/pyinsteon/managers/link_manager/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8816 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/managers/link_manager/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1310 2023-02-09 23:41:45.000000 pyinsteon-1.4.2/pyinsteon/managers/link_manager/default_links.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2704 2023-02-24 20:31:03.000000 pyinsteon-1.4.2/pyinsteon/managers/low_batter_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6770 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/managers/on_level_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5027 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/managers/peek_poke_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12007 2023-03-20 12:21:27.000000 pyinsteon-1.4.2/pyinsteon/managers/saved_devices_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11025 2023-02-16 15:24:23.000000 pyinsteon-1.4.2/pyinsteon/managers/scene_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7302 2023-04-17 20:56:26.000000 pyinsteon-1.4.2/pyinsteon/managers/thermostat_status_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1086 2023-02-09 23:41:45.000000 pyinsteon-1.4.2/pyinsteon/managers/utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2008 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/managers/wet_dry_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4954 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/managers/x10_manager.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.910637 pyinsteon-1.4.2/pyinsteon/protocol/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3137 2023-02-09 23:41:45.000000 pyinsteon-1.4.2/pyinsteon/protocol/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    31497 2023-04-17 20:56:26.000000 pyinsteon-1.4.2/pyinsteon/protocol/command_to_msg.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6120 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/protocol/http_reader_writer.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8549 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/protocol/http_transport.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      111 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/protocol/hub_connection_exception.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.914636 pyinsteon-1.4.2/pyinsteon/protocol/messages/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1896 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/protocol/messages/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4046 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/protocol/messages/inbound.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1367 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/protocol/messages/message_definition.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14193 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/protocol/messages/message_definitions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11565 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/protocol/messages/outbound.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.914636 pyinsteon-1.4.2/pyinsteon/protocol/mock/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-02-09 23:41:45.000000 pyinsteon-1.4.2/pyinsteon/protocol/mock/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1925 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/protocol/mock/mock_reader.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8033 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/protocol/mock/mock_transport.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15192 2023-02-09 23:42:58.000000 pyinsteon-1.4.2/pyinsteon/protocol/msg_to_topic.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      838 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/protocol/msg_to_url.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9176 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/protocol/protocol.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2074 2023-02-02 01:25:31.000000 pyinsteon-1.4.2/pyinsteon/protocol/serial_transport.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      811 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/protocol/topic_converters.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       83 2023-02-09 23:41:45.000000 pyinsteon-1.4.2/pyinsteon/run_tool.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1217 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/subscriber_base.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.914636 pyinsteon-1.4.2/pyinsteon/tools/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    18580 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/tools/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    24420 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/tools/advanced.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10429 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/tools/aldb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10133 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/tools/commands.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17206 2023-03-20 19:36:03.000000 pyinsteon-1.4.2/pyinsteon/tools/config.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1873 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/tools/log_filter.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7748 2023-02-09 23:41:45.000000 pyinsteon-1.4.2/pyinsteon/tools/scenes.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    49450 2023-04-17 20:56:26.000000 pyinsteon-1.4.2/pyinsteon/tools/tools_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3246 2023-02-19 22:07:54.000000 pyinsteon-1.4.2/pyinsteon/tools/utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5966 2023-04-17 20:56:26.000000 pyinsteon-1.4.2/pyinsteon/topics.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12422 2023-04-14 18:36:09.000000 pyinsteon-1.4.2/pyinsteon/utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4753 2022-08-05 17:55:10.000000 pyinsteon-1.4.2/pyinsteon/x10_address.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-17 20:57:29.894636 pyinsteon-1.4.2/pyinsteon.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2494 2023-04-17 20:57:29.000000 pyinsteon-1.4.2/pyinsteon.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8656 2023-04-17 20:57:29.000000 pyinsteon-1.4.2/pyinsteon.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-17 20:57:29.000000 pyinsteon-1.4.2/pyinsteon.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       56 2023-04-17 20:57:29.000000 pyinsteon-1.4.2/pyinsteon.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-17 20:57:27.000000 pyinsteon-1.4.2/pyinsteon.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       68 2023-04-17 20:57:29.000000 pyinsteon-1.4.2/pyinsteon.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-04-17 20:57:29.000000 pyinsteon-1.4.2/pyinsteon.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6539 2023-04-17 20:56:26.000000 pyinsteon-1.4.2/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      799 2023-04-17 20:57:29.914636 pyinsteon-1.4.2/setup.cfg
```

### Comparing `pyinsteon-1.4.1/DESCRIPTION.rst` & `pyinsteon-1.4.2/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/LICENSE.rst` & `pyinsteon-1.4.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/PKG-INFO` & `pyinsteon-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinsteon
-Version: 1.4.1
+Version: 1.4.2
 Summary: Open-source Insteon home automation module running on Python 3.
 Author-email: The pyinsteon authors <pyinsteon@harrisnj.net>
 License: MIT License
 Project-URL: Source Code, https://github.com/pyinsteon/pyinsteon
 Project-URL: Bug Reports, https://github.com/pyinsteon/pyinsteon/issues
 Keywords: home,automation,insteon,python,python3
 Platform: any
```

### Comparing `pyinsteon-1.4.1/README.rst` & `pyinsteon-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/__init__.py` & `pyinsteon-1.4.2/pyinsteon/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/address.py` & `pyinsteon-1.4.2/pyinsteon/address.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/aldb/aldb.py` & `pyinsteon-1.4.2/pyinsteon/aldb/aldb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/aldb/aldb_base.py` & `pyinsteon-1.4.2/pyinsteon/aldb/aldb_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/aldb/aldb_battery.py` & `pyinsteon-1.4.2/pyinsteon/aldb/aldb_battery.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/aldb/aldb_record.py` & `pyinsteon-1.4.2/pyinsteon/aldb/aldb_record.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/aldb/mock_modem_aldb.py` & `pyinsteon-1.4.2/pyinsteon/aldb/mock_modem_aldb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/aldb/modem_aldb.py` & `pyinsteon-1.4.2/pyinsteon/aldb/modem_aldb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/aldb/no_aldb.py` & `pyinsteon-1.4.2/pyinsteon/aldb/no_aldb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/commands.py` & `pyinsteon-1.4.2/pyinsteon/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     ENTER_LINKING_MODE,
     ENTER_UNLINKING_MODE,
     EXTENDED_GET_RESPONSE,
     EXTENDED_GET_SET,
     EXTENDED_READ_WRITE_ALDB,
     EXTENDED_RECEIVED,
     EXTENDED_TRIGGER_ALL_LINK,
+    FACTORY_RESET,
     FX_USERNAME,
     GET_INSTEON_ENGINE_VERSION,
     GET_OPERATING_FLAGS,
     ID_REQUEST,
     INSTANT_CHANGE,
     IO_ALARM_DATA_REQUEST,
     IO_ALARM_DATA_RESPONSE,
@@ -647,14 +648,23 @@
     cmd2=None,
     ud_allowed=False,
     ud_required=False,
     userdata=None,
     use_group=False,
 )
 commands.add(
+    topic=FACTORY_RESET,
+    cmd1=0x34,
+    cmd2=0x00,
+    ud_allowed=True,
+    ud_required=False,
+    userdata=None,
+    use_group=False,
+)
+commands.add(
     topic=NIGHT_MODE_ON,
     cmd1=0x3B,
     cmd2=None,
     ud_allowed=False,
     ud_required=False,
     userdata=None,
     use_group=False,
```

### Comparing `pyinsteon-1.4.1/pyinsteon/config/__init__.py` & `pyinsteon-1.4.2/pyinsteon/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,14 @@
 
 # Derived Properties
 MOMENTARY_DELAY = "momentary_delay"
 RADIO_BUTTON_GROUPS = "radio_button_groups"
 RAMP_RATE_IN_SEC = "ramp_rate_in_seconds"
 RELAY_MODE = "relay_mode"
 TOGGLE_BUTTON = "toggle_button"
-OPS_FLAGS_PROPERTY = "ops_flags_property"
 
 # Modem properties
 MODEM_CONFIG = "modem_config"
 DISABLE_AUTO_LINKING = "disable_auto_linking"
 MONITOR_MODE = "monitor_mode"
 AUTO_LED = "auto_led"
 DEADMAN = "deadman"
```

### Comparing `pyinsteon-1.4.1/pyinsteon/config/derived_property.py` & `pyinsteon-1.4.2/pyinsteon/config/derived_property.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/config/device_flag.py` & `pyinsteon-1.4.2/pyinsteon/config/device_flag.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/config/extended_property.py` & `pyinsteon-1.4.2/pyinsteon/config/extended_property.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/config/momentary_delay.py` & `pyinsteon-1.4.2/pyinsteon/config/momentary_delay.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/config/op_flag_property.py` & `pyinsteon-1.4.2/pyinsteon/config/op_flag_property.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/config/op_flag_property_byte.py` & `pyinsteon-1.4.2/pyinsteon/config/op_flag_property_byte.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 """Operating flag byte for a property read/write process.
 
 For use with `ExtendedPropertyReadManager` and `ExtendedPropertyWriteManager`.
 
+- Receives a list of operating flags and the associated bit.
+- Stores the value of a property byte just like any other property.
+- Updates the associated operating flags with the correct value based on the bit mapping.
+- For bits that do not have an operating flag, the underlying `_value` property will determine the bit value.
+
 """
 from typing import Dict
 
 from ..constants import PropertyType
 from ..utils import bit_is_set, set_bit
-from .derived_property import DerivedProperty
+from .device_flag import DeviceFlagBase
 from .operating_flag import OperatingFlag
 
 
 def _value(prop: OperatingFlag):
     return prop.new_value if prop.is_dirty else prop.value
 
 
-class OpFlagPropertyByte(DerivedProperty):
+class OpFlagPropertyByte(DeviceFlagBase):
     """Operating flag byte for a property read/write process.
 
     For use with `ExtendedPropertyReadManager` and `ExtendedPropertyWriteManager`.
     """
 
     def __init__(
         self, address, name, flags: Dict[int, OperatingFlag], is_read_only=False
     ):
         """Init the DerivedProperty class."""
         super().__init__(
             address,
+            "derived_property",
             name,
             int,
             is_reversed=False,
             is_read_only=is_read_only,
         )
         self._flags: Dict[int, OperatingFlag] = flags
         self._prop_type = PropertyType.HIDDEN
@@ -50,25 +56,25 @@
             if not prop.is_loaded:
                 return False
         return True
 
     @property
     def value(self):
         """Return the value of the flag."""
-        byte_value = 0x00
+        byte_value = self._value if self._value is not None else 0x00
         for bit, prop in self._flags.items():
             if prop.value is None:
                 return None
             byte_value = set_bit(byte_value, bit, prop.value)
         return byte_value
 
     @property
     def new_value(self):
         """Return the new value of the flag."""
-        byte_value = 0x00
+        byte_value = self._value
         for bit, prop in self._flags.items():
             if prop.value is None:
                 return None
             value = _value(prop)
             byte_value = set_bit(byte_value, bit, value)
         return byte_value
 
@@ -88,13 +94,14 @@
 
         Only use this method to update the value of the flag from the value
         of the device.
 
         This method updates the `is_loaded` property and clears the `new value` and
         `is_dirty` properties.
         """
+        super().load(value=value)
         for bit, prop in self._flags.items():
             if value is None:
                 new_val = None
             else:
                 new_val = bit_is_set(value, bit)
             prop.load(new_val)
```

### Comparing `pyinsteon-1.4.1/pyinsteon/config/operating_flag.py` & `pyinsteon-1.4.2/pyinsteon/config/operating_flag.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/config/radio_button.py` & `pyinsteon-1.4.2/pyinsteon/config/radio_button.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/config/ramp_rate.py` & `pyinsteon-1.4.2/pyinsteon/config/ramp_rate.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/config/relay_mode.py` & `pyinsteon-1.4.2/pyinsteon/config/relay_mode.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/config/toggle_button.py` & `pyinsteon-1.4.2/pyinsteon/config/toggle_button.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/constants.py` & `pyinsteon-1.4.2/pyinsteon/constants.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/data_types/all_link_record_flags.py` & `pyinsteon-1.4.2/pyinsteon/data_types/all_link_record_flags.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/data_types/im_config_flags.py` & `pyinsteon-1.4.2/pyinsteon/data_types/im_config_flags.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/data_types/io_sensor_config_flags.py` & `pyinsteon-1.4.2/pyinsteon/data_types/io_sensor_config_flags.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/data_types/message_flags.py` & `pyinsteon-1.4.2/pyinsteon/data_types/message_flags.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/data_types/user_data.py` & `pyinsteon-1.4.2/pyinsteon/data_types/user_data.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/access_control.py` & `pyinsteon-1.4.2/pyinsteon/device_types/access_control.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/battery_base.py` & `pyinsteon-1.4.2/pyinsteon/device_types/battery_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/climate_control.py` & `pyinsteon-1.4.2/pyinsteon/device_types/climate_control.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/device_base.py` & `pyinsteon-1.4.2/pyinsteon/device_types/device_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/device_commands.py` & `pyinsteon-1.4.2/pyinsteon/device_types/device_commands.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/dimmable_lighting_control.py` & `pyinsteon-1.4.2/pyinsteon/device_types/dimmable_lighting_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -826,16 +826,14 @@
             self._address, status_type=2
         )
         for group, group_prop in self._groups.items():
             if isinstance(group_prop, OnLevel):
                 self._handlers[group]["manual_change"] = ManualChangeInbound(
                     self._address, group
                 )
-        self._register_default_ext_prop_read_managers()
-        self._register_default_ext_prop_write_managers()
 
     def _subscribe_to_handelers_and_managers(self):
         """Subscribe methods to handlers and managers."""
         super()._subscribe_to_handelers_and_managers()
         for group, group_prop in self._groups.items():
             if isinstance(group_prop, OnLevel):
                 self._handlers[group]["manual_change"].subscribe(
```

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/energy_management.py` & `pyinsteon-1.4.2/pyinsteon/device_types/energy_management.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/general_controller.py` & `pyinsteon-1.4.2/pyinsteon/device_types/general_controller.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/i3_base.py` & `pyinsteon-1.4.2/pyinsteon/device_types/i3_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,124 +1,143 @@
 """I3 device base classes."""
 import asyncio
 from collections import namedtuple
-from typing import Dict, List
+from typing import Dict, List, Union
 
 from ..config import (
     ACK_A_SCENE,
     BLUE_LED_OFF,
     BRIGHTNESS_MAX,
     BRIGHTNESS_MIN,
     BRIGHTNESS_START,
     CLEANUP_REPORT_OFF,
     DETACH_LOAD_ON,
     DISABLE_BUTTONS,
+    DO_NOT_ROTATE_TO_OFF,
     GREEN_LED_OFF,
     INSTEON_OFF,
     KEY_BEEP_ON,
     LED_BLINK_ON_ERROR_ON,
     LED_BLINK_ON_TX_ON,
     LED_BRIGHTNESS,
     LED_OFF,
     LOAD_SENSE_2_ON,
     LOAD_SENSE_ON,
-    MOD_SYNC_SYNC,
-    NIGHT_LEDS_ON,
     NIGHT_MODE_LED_BRIGHTNESS,
     NIGHT_MODE_MAX_LEVEL,
     NIGHT_MODE_ON,
     NIGHT_MODE_RAMP_RATE,
     NO_CACHE,
     ON_LEVEL,
-    OPS_FLAGS_PROPERTY,
+    OPERATING_FLAGS,
     PROGRAM_LOCK_ON,
     RAMP_RATE,
     RED_LED_OFF,
     RELAY_MODE_OFF,
     RESUME_DIM_ON,
     RF_DISABLE_ON,
     SKIP_SOME_HOPS,
     TEND_ON,
     USE_LOCAL_PROFILE,
     YAKETY_YAK,
 )
 from ..config.extended_property import ExtendedProperty
 from ..config.op_flag_property_byte import OpFlagPropertyByte
-from ..config.operating_flag import OperatingFlag
 from ..constants import PropertyType, ResponseStatus
+from ..handlers.to_device.factory_reset import FactoryResetCommand
 from ..handlers.to_device.night_mode_off import NightModeOffCommand
 from ..handlers.to_device.night_mode_on import NightModeOnCommand
 from ..managers.ext_prop_read_manager import ExtendedPropertyReadManager
 from ..managers.ext_prop_write_manager import ExtendedPropertyWriteManager
 from ..utils import multiple_status
 from .on_off_responder_base import OnOffResponderBase
 from .variable_responder_base import VariableResponderBase
 
-OP_FLAG_PROP_1 = f"{OPS_FLAGS_PROPERTY}_1"
-OP_FLAG_PROP_2 = f"{OPS_FLAGS_PROPERTY}_2"
-OP_FLAG_PROP_3 = f"{OPS_FLAGS_PROPERTY}_3"
+OP_FLAG_1F_00 = f"{OPERATING_FLAGS}_1f_00"
+OP_FLAG_1F_05 = f"{OPERATING_FLAGS}_1f_05"
+OP_FLAG_1F_07 = f"{OPERATING_FLAGS}_1f_07"
 
 READ_MGRS = "ext_prop_read_mgrs"
 WRITE_MGRS = "ext_prop_write_mgrs"
 NIGHT_MODE_OFF = "night_mode_off"
 
 OpsFlagDef = namedtuple(
     "OpsFlagDef", ["name", "group", "bit", "set_cmd", "unset_cmd", "prop_type"]
 )
 ExtProp = namedtuple("ExtProp", ["name", "value_type", "is_read_only", "prop_type"])
 
 
 def _default_ops_flags(dimmable: bool) -> List[OpsFlagDef]:
     """Return a list of default operating flags for i3 devices."""
+    show = PropertyType.STANDARD if dimmable else PropertyType.HIDDEN
     return [
         # Group 0
         OpsFlagDef(PROGRAM_LOCK_ON, 0, 0, 0x00, 0x01, PropertyType.STANDARD),
         OpsFlagDef(LED_BLINK_ON_TX_ON, 0, 1, 0x02, 0x03, PropertyType.STANDARD),
         OpsFlagDef(LED_OFF, 0, 4, 0x08, 0x09, PropertyType.STANDARD),
         OpsFlagDef(KEY_BEEP_ON, 0, 5, 0x0A, 0x0B, PropertyType.STANDARD),
         OpsFlagDef(RF_DISABLE_ON, 0, 6, 0x0C, 0x0D, PropertyType.ADVANCED),
         OpsFlagDef(INSTEON_OFF, 0, 7, 0x0E, 0x0F, PropertyType.ADVANCED),
         # Group 5
         OpsFlagDef(TEND_ON, 5, 0, None, None, PropertyType.HIDDEN),
         # -- Night mode is set with (cmd1: 0x3B  cmd2: 0xXX) and (cmd2: 0x3C  cmd2: 0xXX)
-        OpsFlagDef(NIGHT_MODE_ON, 5, 1, None, None, PropertyType.HIDDEN),
-        OpsFlagDef(LED_BLINK_ON_ERROR_ON, 5, 2, None, None, PropertyType.ADVANCED),
+        OpsFlagDef(NIGHT_MODE_ON, 5, 1, None, None, PropertyType.STANDARD),
+        OpsFlagDef(LED_BLINK_ON_ERROR_ON, 5, 2, None, None, PropertyType.STANDARD),
         OpsFlagDef(CLEANUP_REPORT_OFF, 5, 3, None, None, PropertyType.HIDDEN),
         OpsFlagDef(DISABLE_BUTTONS, 5, 4, None, None, PropertyType.HIDDEN),
         # -- DETACH_LOAD_ON: future feature set/unset with 0x12, 0x13
         OpsFlagDef(DETACH_LOAD_ON, 5, 5, 0x12, 0x13, PropertyType.HIDDEN),
         OpsFlagDef(ACK_A_SCENE, 5, 6, 0x1C, 0x1D, PropertyType.HIDDEN),
-        OpsFlagDef(RELAY_MODE_OFF, 5, 7, 0x1E, 0x1F, PropertyType.HIDDEN),
+        OpsFlagDef(RELAY_MODE_OFF, 5, 7, 0x1EC, 0x1F, show),
         # Group 7
         OpsFlagDef(YAKETY_YAK, 7, 0, None, None, PropertyType.HIDDEN),
         OpsFlagDef(RED_LED_OFF, 7, 1, 0x28, 0x29, PropertyType.STANDARD),
         OpsFlagDef(SKIP_SOME_HOPS, 7, 2, 0x2A, 0x2B, PropertyType.HIDDEN),
         OpsFlagDef(GREEN_LED_OFF, 7, 3, 0x2C, 0x0D, PropertyType.STANDARD),
         OpsFlagDef(BLUE_LED_OFF, 7, 4, 0x2E, 0x2F, PropertyType.STANDARD),
         OpsFlagDef(NO_CACHE, 7, 5, 0x30, 0x31, PropertyType.HIDDEN),
+        OpsFlagDef(DO_NOT_ROTATE_TO_OFF, 7, 6, 0x32, 0x33, show),
     ]
 
 
 def _default_ext_props(dimmable=True) -> List[ExtProp]:
     """Return a list of default extended properties for i3 devices."""
     show_dim = PropertyType.STANDARD if dimmable else PropertyType.HIDDEN
     show_dim_adv = PropertyType.ADVANCED if dimmable else PropertyType.HIDDEN
     return [
-        ExtProp(NIGHT_MODE_LED_BRIGHTNESS, int, False, PropertyType.HIDDEN),
-        ExtProp(NIGHT_MODE_RAMP_RATE, int, False, PropertyType.HIDDEN),
+        ExtProp(NIGHT_MODE_LED_BRIGHTNESS, int, False, PropertyType.STANDARD),
+        ExtProp(NIGHT_MODE_RAMP_RATE, int, False, PropertyType.STANDARD),
         ExtProp(RAMP_RATE, int, False, show_dim_adv),
         ExtProp(ON_LEVEL, int, False, show_dim),
         ExtProp(LED_BRIGHTNESS, int, False, PropertyType.STANDARD),
-        ExtProp(BRIGHTNESS_MIN, int, False, PropertyType.HIDDEN),
-        ExtProp(BRIGHTNESS_MAX, int, False, PropertyType.HIDDEN),
-        ExtProp(BRIGHTNESS_START, int, False, PropertyType.HIDDEN),
-        ExtProp(NIGHT_MODE_MAX_LEVEL, int, False, PropertyType.HIDDEN),
+        ExtProp(BRIGHTNESS_MIN, int, False, show_dim),
+        ExtProp(BRIGHTNESS_MAX, int, False, show_dim),
+        ExtProp(BRIGHTNESS_START, int, False, show_dim),
+        ExtProp(NIGHT_MODE_MAX_LEVEL, int, False, PropertyType.STANDARD),
     ]
 
 
+def _group_1_properties(properties: Dict[str, ExtendedProperty]):
+    """Return a set of properties that represent the 2E 01 properties."""
+    return {
+        2: properties[OP_FLAG_1F_00],
+        3: properties[OP_FLAG_1F_05],
+        4: properties[OP_FLAG_1F_07],
+        5: properties[RAMP_RATE],
+        6: properties[ON_LEVEL],
+        7: properties[LED_BRIGHTNESS],
+        8: properties[BRIGHTNESS_MAX],
+        9: properties[BRIGHTNESS_MIN],
+        10: properties[BRIGHTNESS_START],
+        11: properties[NIGHT_MODE_MAX_LEVEL],
+        12: properties[NIGHT_MODE_LED_BRIGHTNESS],
+        13: properties[NIGHT_MODE_RAMP_RATE],
+    }
+
+
 # pylint: disable=no-member
 # pylint: disable=super-with-arguments
 class I3Base:
     """I3 device type base class."""
 
     def __init__(
         self, address, cat, subcat, firmware=0x00, description="", model="", **kwargs
@@ -135,32 +154,32 @@
             model=model,
             **kwargs,
         )
 
     async def async_read_ext_properties(self, group=None) -> ResponseStatus:
         """Get the device extended properties."""
         responses = []
-        for _, mgr in self._managers[READ_MGRS].items():
+        for mgr in self._managers[READ_MGRS]:
             response = await mgr.async_send()
             responses.append(response)
-        await asyncio.sleep(0.5)
+            await asyncio.sleep(0.2)
         return multiple_status(*responses)
 
-    async def async_write_op_flags(self):
+    async def async_write_op_flags(self) -> ResponseStatus:
         """Write the operating flags to the device."""
         responses = []
         if prop := self._operating_flags.get(NIGHT_MODE_ON):
             if prop.is_dirty:
                 response = await self.async_set_night_mode(prop.new_value)
                 responses.append(response)
         response = await self._op_flags_manager.async_write()
         responses.append(response)
         return multiple_status(*responses)
 
-    async def async_write_ext_properties(self):
+    async def async_write_ext_properties(self) -> ResponseStatus:
         """Write the extended properties."""
         responses = [ResponseStatus.SUCCESS]
         for cmd in self._managers[WRITE_MGRS]:
             if cmd.is_dirty:
                 responses.append(await cmd.async_write())
         return multiple_status(*responses)
 
@@ -168,22 +187,65 @@
         """Set the device night mode on or off."""
         cmd = NIGHT_MODE_ON if on else NIGHT_MODE_OFF
         for _ in range(0, 3):
             response = await self._managers[cmd].async_send()
             await asyncio.sleep(0.5)
         return response
 
-    def _register_handlers_and_managers(self):
+    async def async_factory_reset(self) -> ResponseStatus:
+        """Reset this device to factory defaults."""
+        cmd = FactoryResetCommand(self._address, self._cat, self._subcat)
+        return await cmd.async_send()
+
+    def _register_handlers_and_managers(self) -> None:
         super(I3Base, self)._register_handlers_and_managers()
         self._managers[NIGHT_MODE_ON] = NightModeOnCommand(self._address)
         self._managers[NIGHT_MODE_OFF] = NightModeOffCommand(self._address)
-        self._register_default_ext_prop_read_managers()
+        group_0 = {
+            7: self._properties[RAMP_RATE],
+            8: self._properties[ON_LEVEL],
+            9: self._properties[LED_BRIGHTNESS],
+        }
+        self._add_ext_prop_read_manager(
+            properties=group_0,
+            cmd2=0x00,
+            data1_read=0x00,
+            data2_read=0x00,
+            data3_read=0x00,
+            data1_resp=0x00,
+            data2_resp=0x01,
+            data3_resp=None,
+        )
+
+        # Cat   Subcat  Model   Device      Data1
+        # 0x01  0x57    PS01    i3 Paddle   0x05
+        # 0x01	0x58    DS01    i3 Dial     0x04
+        # 0x01	0x59    KP014   i3 Keypad   0x01
+        # 0x02	0x3F    WR01    i3 Outlet   0x03
+        data2_map = {
+            0x57: 0x05,
+            0x58: 0x04,
+            0x59: 0x01,
+            0x3F: 0x03,
+        }
+        group_1 = _group_1_properties(self._properties)
+        if data1_resp := data2_map.get(self._subcat):
+            self._add_ext_prop_read_manager(
+                properties=group_1,
+                cmd2=0x01,
+                data1_read=0x00,
+                data2_read=0x00,
+                data3_read=0x00,
+                data1_resp=data1_resp,
+                data2_resp=None,
+                data3_resp=None,
+            )
         self._register_default_ext_prop_write_managers()
 
-    def _subscribe_to_handelers_and_managers(self):
+    def _subscribe_to_handelers_and_managers(self) -> None:
         super(I3Base, self)._subscribe_to_handelers_and_managers()
         self._managers[NIGHT_MODE_ON].subscribe(self._handle_night_mode)
         self._managers[NIGHT_MODE_OFF].subscribe(self._handle_night_mode)
 
     def _handle_night_mode(self, night_mode) -> None:
         """Handle the night mode on/off response."""
         if prop := self._operating_flags.get(NIGHT_MODE_ON):
@@ -191,15 +253,15 @@
 
     def _register_default_op_flags_and_props(
         self,
         dimmable: bool,
         ops_flags_1: Dict[int, str],
         ops_flags_2: Dict[int, str],
         ops_flags_3: Dict[int, str],
-    ):
+    ) -> None:
         for flag in _default_ops_flags(dimmable):
             self._add_operating_flag(
                 name=flag.name,
                 group=flag.group,
                 bit=flag.bit,
                 set_cmd=flag.set_cmd,
                 unset_cmd=flag.unset_cmd,
@@ -211,140 +273,120 @@
                 address=self._address,
                 name=prop.name,
                 value_type=prop.value_type,
                 is_reversed=False,
                 is_read_only=prop.is_read_only,
                 prop_type=prop.prop_type,
             )
-        # Dummy flag needed for Extended Properties group 1
-        self._operating_flags[MOD_SYNC_SYNC] = OperatingFlag(
-            address=self._address,
-            name=MOD_SYNC_SYNC,
-            value_type=bool,
-            prop_type=PropertyType.HIDDEN,
-        )
-        self._operating_flags[NIGHT_LEDS_ON] = OperatingFlag(
-            address=self._address,
-            name=NIGHT_LEDS_ON,
-            value_type=bool,
-            prop_type=PropertyType.HIDDEN,
-        )
-        ops_flags_1_all = {
+
+        ops_flags_1f_00_all = {
             0: PROGRAM_LOCK_ON,
             1: LED_BLINK_ON_TX_ON,
             4: LED_OFF,
             5: KEY_BEEP_ON,
             6: RF_DISABLE_ON,
             7: INSTEON_OFF,
         }
-        ops_flags_1_all.update(ops_flags_1)
-        ops_flags_2_all = {
+        ops_flags_1f_00_all.update(ops_flags_1)
+        ops_flags_1f_05_all = {
             1: NIGHT_MODE_ON,
             2: LED_BLINK_ON_ERROR_ON,
             3: CLEANUP_REPORT_OFF,
             4: DISABLE_BUTTONS,
             5: DETACH_LOAD_ON,
             6: ACK_A_SCENE,
             7: RELAY_MODE_OFF,
         }
-        ops_flags_2_all.update(ops_flags_2)
-        ops_flags_3_all = {
+        ops_flags_1f_05_all.update(ops_flags_2)
+        ops_flags_1f_07_all = {
             0: YAKETY_YAK,
-            1: MOD_SYNC_SYNC,
+            1: RED_LED_OFF,
             2: SKIP_SOME_HOPS,
-            3: RELAY_MODE_OFF,
-            4: NIGHT_LEDS_ON,
+            3: GREEN_LED_OFF,
+            4: BLUE_LED_OFF,
             5: NO_CACHE,
+            6: DO_NOT_ROTATE_TO_OFF,
         }
-        ops_flags_3_all.update(ops_flags_3)
-        self._add_extended_prop_byte(OP_FLAG_PROP_1, ops_flags_1_all)
-        self._add_extended_prop_byte(OP_FLAG_PROP_2, ops_flags_2_all)
-        self._add_extended_prop_byte(OP_FLAG_PROP_3, ops_flags_3_all)
+        ops_flags_1f_07_all.update(ops_flags_3)
+        self._add_extended_prop_byte(OP_FLAG_1F_00, ops_flags_1f_00_all)
+        self._add_extended_prop_byte(OP_FLAG_1F_05, ops_flags_1f_05_all)
+        self._add_extended_prop_byte(OP_FLAG_1F_07, ops_flags_1f_07_all)
 
-    def _add_extended_prop_byte(self, name: str, op_flag_map: Dict[int, str]):
+    def _add_extended_prop_byte(self, name: str, op_flag_map: Dict[int, str]) -> None:
         """Add an extended property to hold the operating flags used in an extended write."""
         ops_flags = {
             index: self._operating_flags[name] for index, name in op_flag_map.items()
         }
         self._properties[name] = OpFlagPropertyByte(
             address=self._address, name=name, flags=ops_flags
         )
 
-    def _register_default_ext_prop_read_managers(self):
-        group_0 = {
-            7: self._properties[RAMP_RATE],
-            8: self._properties[ON_LEVEL],
-            9: self._properties[LED_BRIGHTNESS],
-        }
-        self._managers[READ_MGRS] = self._managers.get(READ_MGRS, {})
-        self._managers[READ_MGRS][0] = ExtendedPropertyReadManager(
-            address=self._address,
-            properties=group_0,
-            cmd2=0x00,
-            data1_read=0x00,
-            data2_read=0x00,
-            data3_read=0x00,
-            data1_resp=0x00,
-            data2_resp=0x01,
-            data3_resp=None,
-        )
-        # group_1 = {
-        #     2: self._properties[OP_FLAG_PROP_1],
-        #     3: self._properties[OP_FLAG_PROP_2],
-        #     4: self._properties[OP_FLAG_PROP_3],
-        #     # 5: self._properties[RAMP_RATE],
-        #     # 6: self._properties[ON_LEVEL],
-        #     # 7: self._properties[LED_BRIGHTNESS],
-        #     8: self._properties[BRIGHTNESS_MAX],
-        #     9: self._properties[BRIGHTNESS_MIN],
-        #     10: self._properties[BRIGHTNESS_START],
-        #     11: self._properties[NIGHT_MODE_MAX_LEVEL],
-        #     12: self._properties[NIGHT_MODE_LED_BRIGHTNESS],
-        #     13: self._properties[NIGHT_MODE_RAMP_RATE],
-        # }
-        # self._managers[READ_MGRS][1] = ExtendedPropertyReadManager(
-        #     address=self._address,
-        #     properties=group_1,
-        #     cmd2=0x01,
-        #     data1_read=0x00,
-        #     data2_read=0x00,
-        #     data3_read=0x00,
-        #     data1_resp=0x01,
-        #     data2_resp=None,
-        #     data3_resp=None,
-        # )
-
-    def _register_default_ext_prop_write_managers(self):
-        self._managers[WRITE_MGRS] = self._managers.get(WRITE_MGRS, [])
-
-        led = {3: self._properties[LED_BRIGHTNESS]}
-        self._managers[WRITE_MGRS].append(
-            ExtendedPropertyWriteManager(
-                address=self._address, properties=led, cmd2=0, data1=0x01, data2=0x07
+    def _add_ext_prop_read_manager(
+        self,
+        properties: Dict[int, ExtendedProperty],
+        cmd2: int = 0,
+        data1_read: int = 0,
+        data2_read: int = 0,
+        data3_read: int = None,
+        data1_resp: int = 0,
+        data2_resp: int = 1,
+        data3_resp: int = None,
+    ) -> None:
+        self._managers[READ_MGRS] = self._managers.get(READ_MGRS, [])
+        self._managers[READ_MGRS].append(
+            ExtendedPropertyReadManager(
+                address=self._address,
+                properties=properties,
+                cmd2=cmd2,
+                data1_read=data1_read,
+                data2_read=data2_read,
+                data3_read=data3_read,
+                data1_resp=data1_resp,
+                data2_resp=data2_resp,
+                data3_resp=data3_resp,
             )
         )
 
+    def _register_default_ext_prop_write_managers(self) -> None:
+        led = {3: self._properties[LED_BRIGHTNESS]}
+        self._add_ext_prop_write_manager(properties=led, cmd2=0, data1=0x01, data2=0x07)
         on_level = {3: self._properties[ON_LEVEL]}
-        self._managers[WRITE_MGRS].append(
-            ExtendedPropertyWriteManager(
-                address=self._address,
-                properties=on_level,
-                cmd2=0,
-                data1=0x01,
-                data2=0x06,
-            )
+        self._add_ext_prop_write_manager(
+            properties=on_level,
+            cmd2=0,
+            data1=0x01,
+            data2=0x06,
         )
         ramp_rate = {3: self._properties[RAMP_RATE]}
+        self._add_ext_prop_write_manager(
+            properties=ramp_rate,
+            cmd2=0,
+            data1=0x01,
+            data2=0x05,
+        )
+        group_1 = _group_1_properties(self._properties)
+        self._add_ext_prop_write_manager(
+            properties=group_1, data2=None, cmd2=0x01, data1=0x02
+        )
+
+    def _add_ext_prop_write_manager(
+        self,
+        properties: Dict[int, ExtendedProperty],
+        data2: Union[int, None],
+        cmd2: int = 0,
+        data1: int = 0,
+    ) -> None:
+        self._managers[WRITE_MGRS] = self._managers.get(WRITE_MGRS, [])
         self._managers[WRITE_MGRS].append(
             ExtendedPropertyWriteManager(
                 address=self._address,
-                properties=ramp_rate,
-                cmd2=0,
-                data1=0x01,
-                data2=0x05,
+                properties=properties,
+                cmd2=cmd2,
+                data1=data1,
+                data2=data2,
             )
         )
 
 
 # pylint: disable=super-with-arguments
 class I3VariableResponderBase(I3Base, VariableResponderBase):
     """I3 variable responder base class."""
```

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/ipdb.py` & `pyinsteon-1.4.2/pyinsteon/device_types/ipdb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/mock_modem.py` & `pyinsteon-1.4.2/pyinsteon/device_types/mock_modem.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/modem_base.py` & `pyinsteon-1.4.2/pyinsteon/device_types/modem_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/on_off_controller_base.py` & `pyinsteon-1.4.2/pyinsteon/device_types/on_off_controller_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/on_off_responder_base.py` & `pyinsteon-1.4.2/pyinsteon/device_types/on_off_responder_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/open_close_controller_base.py` & `pyinsteon-1.4.2/pyinsteon/device_types/open_close_controller_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/open_close_responder_base.py` & `pyinsteon-1.4.2/pyinsteon/device_types/open_close_responder_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/plm.py` & `pyinsteon-1.4.2/pyinsteon/device_types/plm.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/security_health_safety.py` & `pyinsteon-1.4.2/pyinsteon/device_types/security_health_safety.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/sensors_actuators.py` & `pyinsteon-1.4.2/pyinsteon/device_types/sensors_actuators.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/switched_lighting_control.py` & `pyinsteon-1.4.2/pyinsteon/device_types/switched_lighting_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     RED_LED_OFF,
     RESUME_DIM_ON,
     REVERSED_ON,
     RF_DISABLE_ON,
     THREE_WAY_ON,
     TOGGLE_BUTTON,
     TRIGGER_GROUP_MASK,
+    USE_LOCAL_PROFILE,
     X10_HOUSE,
     X10_UNIT,
 )
 from ..config.radio_button import RadioButtonGroupsProperty
 from ..config.toggle_button import ToggleButtonProperty
 from ..constants import PropertyType, ResponseStatus, ToggleMode
 from ..events import OFF_EVENT, OFF_FAST_EVENT, ON_EVENT, ON_FAST_EVENT
@@ -659,16 +660,19 @@
     def _register_op_flags_and_props(self):
         self._add_operating_flag(
             LOAD_SENSE_ON, 0, 2, 4, 5, prop_type=PropertyType.ADVANCED
         )
         self._add_operating_flag(
             LOAD_SENSE_2_ON, 0, 3, 6, 7, prop_type=PropertyType.ADVANCED
         )
+        self._add_operating_flag(
+            USE_LOCAL_PROFILE, 7, 7, 0x34, 0x35, prop_type=PropertyType.HIDDEN
+        )
         self._register_default_op_flags_and_props(
             dimmable=False,
             ops_flags_1={2: LOAD_SENSE_ON, 3: LOAD_SENSE_2_ON},
             ops_flags_2={},
-            ops_flags_3={},
+            ops_flags_3={7: USE_LOCAL_PROFILE},
         )
         self._operating_flags[RED_LED_OFF].property_type = PropertyType.HIDDEN
         self._operating_flags[GREEN_LED_OFF].property_type = PropertyType.HIDDEN
         self._operating_flags[BLUE_LED_OFF].property_type = PropertyType.HIDDEN
```

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/variable_controller_base.py` & `pyinsteon-1.4.2/pyinsteon/device_types/variable_controller_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/variable_responder_base.py` & `pyinsteon-1.4.2/pyinsteon/device_types/variable_responder_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/window_coverings.py` & `pyinsteon-1.4.2/pyinsteon/device_types/window_coverings.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/x10.py` & `pyinsteon-1.4.2/pyinsteon/device_types/x10.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/device_types/x10_base.py` & `pyinsteon-1.4.2/pyinsteon/device_types/x10_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/events.py` & `pyinsteon-1.4.2/pyinsteon/events.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/groups/__init__.py` & `pyinsteon-1.4.2/pyinsteon/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/groups/fan.py` & `pyinsteon-1.4.2/pyinsteon/groups/fan.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/groups/group_base.py` & `pyinsteon-1.4.2/pyinsteon/groups/group_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/groups/on_level.py` & `pyinsteon-1.4.2/pyinsteon/groups/on_level.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/groups/on_off.py` & `pyinsteon-1.4.2/pyinsteon/groups/on_off.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/groups/open_close.py` & `pyinsteon-1.4.2/pyinsteon/groups/open_close.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/groups/thermostat.py` & `pyinsteon-1.4.2/pyinsteon/groups/thermostat.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/groups/wet_dry.py` & `pyinsteon-1.4.2/pyinsteon/groups/wet_dry.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/__init__.py` & `pyinsteon-1.4.2/pyinsteon/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/all_link_cleanup_failure_report.py` & `pyinsteon-1.4.2/pyinsteon/handlers/all_link_cleanup_failure_report.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/all_link_cleanup_status_report.py` & `pyinsteon-1.4.2/pyinsteon/handlers/all_link_cleanup_status_report.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/all_link_completed.py` & `pyinsteon-1.4.2/pyinsteon/handlers/all_link_completed.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/all_link_record_response.py` & `pyinsteon-1.4.2/pyinsteon/handlers/all_link_record_response.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/cancel_all_linking.py` & `pyinsteon-1.4.2/pyinsteon/handlers/cancel_all_linking.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/all_link_cleanup_command.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/all_link_cleanup_command.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/assign_to_all_link_group.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/assign_to_all_link_group.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/broadcast_command.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/broadcast_command.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/delete_from_all_link_group.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/delete_from_all_link_group.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/ext_get_response.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/ext_get_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,14 +20,22 @@
             message_type=MessageFlagType.DIRECT,
         )
         self._cmd2 = cmd2
         self._data1 = data1
         self._data2 = data2
         self._data3 = data3
 
+        topic = f"handler.{self._address.id}.{EXTENDED_GET_RESPONSE}"
+        for group in (cmd2, data1, data2, data3):
+            if group is None:
+                topic = f"{topic}.x"
+            else:
+                topic = f"{topic}.{group}"
+        self._subscriber_topic = topic
+
     @inbound_handler
     def handle_response(self, cmd1, cmd2, target, user_data, hops_left):
         """Handle the Extended Get response from a device."""
         # pylint: disable=too-many-boolean-expressions
         if (
             cmd2 == self._cmd2
             and (self._data1 is None or user_data["d1"] == self._data1)
```

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/manual_change.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/manual_change.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/off.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/off.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/off_all_link_cleanup.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/off_all_link_cleanup.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/off_fast.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/off_fast.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/off_fast_all_link_cleanup.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/off_fast_all_link_cleanup.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/on_fast.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/on_fast.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/on_fast_all_link_cleanup.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/on_fast_all_link_cleanup.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/on_level.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/on_level.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/on_level_all_link_cleanup.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/on_level_all_link_cleanup.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/receive_aldb_record.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/receive_aldb_record.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/thermostat_cool_set_point.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/thermostat_cool_set_point.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/thermostat_heat_set_point.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/thermostat_heat_set_point.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/thermostat_humidity.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/thermostat_humidity.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/thermostat_mode.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/thermostat_mode.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/thermostat_temperature.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/thermostat_temperature.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/from_device/x10_received.py` & `pyinsteon-1.4.2/pyinsteon/handlers/from_device/x10_received.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/get_first_all_link_record.py` & `pyinsteon-1.4.2/pyinsteon/handlers/get_first_all_link_record.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/get_im_configuration.py` & `pyinsteon-1.4.2/pyinsteon/handlers/get_im_configuration.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/get_im_info.py` & `pyinsteon-1.4.2/pyinsteon/handlers/get_im_info.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/get_next_all_link_record.py` & `pyinsteon-1.4.2/pyinsteon/handlers/get_next_all_link_record.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/inbound_base.py` & `pyinsteon-1.4.2/pyinsteon/handlers/inbound_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/manage_all_link_record.py` & `pyinsteon-1.4.2/pyinsteon/handlers/manage_all_link_record.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/outbound_base.py` & `pyinsteon-1.4.2/pyinsteon/handlers/outbound_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/read_eeprom.py` & `pyinsteon-1.4.2/pyinsteon/handlers/read_eeprom.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/read_eeprom_response.py` & `pyinsteon-1.4.2/pyinsteon/handlers/read_eeprom_response.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/send_all_link.py` & `pyinsteon-1.4.2/pyinsteon/handlers/send_all_link.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/set_im_configuration.py` & `pyinsteon-1.4.2/pyinsteon/handlers/set_im_configuration.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/start_all_linking.py` & `pyinsteon-1.4.2/pyinsteon/handlers/start_all_linking.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/all_link_cleanup_command.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/all_link_cleanup_command.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/direct_command.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/direct_command.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/engine_version_request.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/engine_version_request.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/enter_linking_mode.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/enter_linking_mode.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/enter_unlinking_mode.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/enter_unlinking_mode.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/extended_get.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/extended_get.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,19 +17,23 @@
         super().__init__(topic=EXTENDED_GET_SET, address=address)
         self._cmd2 = cmd2
         self._data1 = data1
         self._data2 = data2
         self._data3 = data3
 
     # pylint: disable=arguments-differ
-    async def async_send(self, group=0):
+    async def async_send(self, group=0, crc=False):
         """Send Get Operating Flags message asyncronously."""
         self._data1 = group
         response = await super().async_send(
-            cmd2=self._cmd2, data1=self._data1, data2=self._data2, data3=self._data3
+            cmd2=self._cmd2,
+            data1=self._data1,
+            data2=self._data2,
+            data3=self._data3,
+            crc=crc,
         )
         self._data1 = None
         return response
 
     @ack_handler
     async def async_handle_ack(self, cmd1, cmd2, user_data):
         """Handle the ACK response.
```

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/extended_set.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/extended_set.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/get_operating_flags.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/get_operating_flags.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/id_request.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/id_request.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/night_mode_off.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/night_mode_off.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/night_mode_on.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/night_mode_on.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/off.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/off.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/off_all_link_cleanup.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/off_all_link_cleanup.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/off_fast.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/off_fast.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/on_fast.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/on_fast.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/on_level.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/on_level.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/on_level_all_link_cleanup.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/on_level_all_link_cleanup.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/peek.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/peek.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/ping.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/ping.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/poke.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/poke.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/product_data_request.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/product_data_request.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/read_aldb.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/read_aldb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/set_leds.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/set_leds.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/set_msb.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/set_msb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/set_operating_flags.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/set_operating_flags.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/status_request.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/status_request.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/temperature_down.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/temperature_down.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/temperature_up.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/temperature_up.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/thermostat_cool_set_point.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/thermostat_cool_set_point.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/thermostat_heat_set_point.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/thermostat_heat_set_point.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/thermostat_mode.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/thermostat_mode.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/trigger_scene_off.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/trigger_scene_off.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/trigger_scene_on.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/trigger_scene_on.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/write_aldb.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/write_aldb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/to_device/x10_send.py` & `pyinsteon-1.4.2/pyinsteon/handlers/to_device/x10_send.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/handlers/write_eeprom.py` & `pyinsteon-1.4.2/pyinsteon/handlers/write_eeprom.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/aldb_im_read_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/aldb_im_read_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/aldb_im_write_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/aldb_im_write_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/aldb_read_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/aldb_read_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/aldb_write_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/aldb_write_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/device_id_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/device_id_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/device_link_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/device_link_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/device_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/device_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/ext_get_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/ext_get_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/ext_prop_read_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/ext_prop_read_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/ext_prop_write_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/ext_prop_write_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,8 +55,9 @@
             if response == ResponseStatus.SUCCESS:
                 self._load_prop_values()
         return response
 
     def _load_prop_values(self):
         """Load the new value to the property value."""
         for _, prop in self._props.items():
-            prop.load(prop.new_value)
+            if prop.is_dirty:
+                prop.load(prop.new_value)
```

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/get_set_ext_property_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/get_set_ext_property_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/get_set_op_flag_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/get_set_op_flag_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,18 +101,17 @@
             await asyncio.sleep(0.01)
             retries += 1
         return result
 
     async def async_write(self):
         """Set the operating flags."""
         results = []
-        for name in self._op_flags:
+        for name, flag_info in self._flags.items():
             if self._op_flags[name].is_dirty:
-                flat_info = self._flags[name]
-                result = await self._async_write(flat_info)
+                result = await self._async_write(flag_info)
                 results.append(result)
         return multiple_status(*results)
 
     async def _async_write(self, flag_info):
         flag = self._op_flags[flag_info.name]
         should_set = not flag.new_value if flag.is_reversed else flag.new_value
         cmd = flag_info.set_cmd if should_set else flag_info.unset_cmd
```

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/heartbeat_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/heartbeat_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/link_manager/__init__.py` & `pyinsteon-1.4.2/pyinsteon/managers/link_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/link_manager/default_links.py` & `pyinsteon-1.4.2/pyinsteon/managers/link_manager/default_links.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/low_batter_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/low_batter_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/on_level_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/on_level_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/peek_poke_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/peek_poke_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/saved_devices_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/saved_devices_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/scene_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/scene_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/thermostat_status_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/thermostat_status_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,21 +44,21 @@
     """Thermostat status manager."""
 
     def __init__(self, address):
         """Init the GetThermostatStatus class."""
         self._address = Address(address)
         self._get_status_command = ExtendedGetCommand(self._address, cmd2=0x02)
         self._get_set_point_command = ExtendedGetCommand(
-            address=self._address, cmd2=0x00, data1=0x00, data2=0x00, data3=0x00
+            address=self._address, cmd2=0x00, data1=0x00, data2=0x00, data3=0x01
         )
         self._status_response = ExtendedGetResponseHandler(
-            self._address, cmd2=0x02, data1=0x00, data2=0x01, data3=None
+            self._address, cmd2=0x02, data1=0x01, data2=None, data3=None
         )
         self._set_point_response = ExtendedGetResponseHandler(
-            self._address, cmd2=0x00, data1=0x00, data2=0x01, data3=0x00
+            self._address, cmd2=0x00, data1=0x00, data2=0x01, data3=0x01
         )
         self._response_status = asyncio.Queue()
         self._response_set_point = asyncio.Queue()
         self._status_response.subscribe(self._status_received)
         self._set_point_response.subscribe(self._set_point_received)
 
         self._status_received_topic = (
@@ -103,15 +103,15 @@
     async def _status(self):
         """Send the status command and call set point command."""
         while not self._response_status.empty():
             self._response_status.get_nowait()
         retries = 3
         response_status = ResponseStatus.FAILURE
         while retries:
-            response = await self._get_status_command.async_send()
+            response = await self._get_status_command.async_send(crc=True)
             if response == ResponseStatus.SUCCESS:
                 try:
                     response_status = await asyncio.wait_for(
                         self._response_status.get(), TIMEOUT
                     )
                     return response_status
                 except asyncio.TimeoutError:
@@ -124,15 +124,15 @@
     async def _set_point(self):
         """Send the set point command."""
         while not self._response_set_point.empty():
             self._response_set_point.get_nowait()
         retries = 3
         response_set_point = ResponseStatus.FAILURE
         while retries:
-            response = await self._get_set_point_command.async_send()
+            response = await self._get_set_point_command.async_send(crc=True)
             if response == ResponseStatus.SUCCESS:
                 try:
                     return await asyncio.wait_for(
                         self._response_set_point.get(), TIMEOUT
                     )
                 except asyncio.TimeoutError:
                     _LOGGER.debug("Set point response timed out")
```

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/utils.py` & `pyinsteon-1.4.2/pyinsteon/managers/utils.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/wet_dry_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/wet_dry_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/managers/x10_manager.py` & `pyinsteon-1.4.2/pyinsteon/managers/x10_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/protocol/__init__.py` & `pyinsteon-1.4.2/pyinsteon/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/protocol/command_to_msg.py` & `pyinsteon-1.4.2/pyinsteon/protocol/command_to_msg.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 from math import ceil
 
 from .. import pub
 from ..address import Address
 from ..commands import commands
 from ..constants import (
+    DeviceCategory,
     DoorCommand,
     IOModuleControlCommand,
     PoolControlCommand,
     RampRate,
     SprinklerControlCommand,
     ThermostatCommand,
     ThermostatZoneInfo,
@@ -29,14 +30,15 @@
     DOOR_CONTROL,
     DOOR_STATUS_REPORT,
     ENTER_LINKING_MODE,
     ENTER_UNLINKING_MODE,
     EXTENDED_GET_SET,
     EXTENDED_READ_WRITE_ALDB,
     EXTENDED_TRIGGER_ALL_LINK,
+    FACTORY_RESET,
     FX_USERNAME,
     GET_INSTEON_ENGINE_VERSION,
     GET_OPERATING_FLAGS,
     ID_REQUEST,
     INSTANT_CHANGE,
     IO_ALARM_DATA_REQUEST,
     IO_GET_SENSOR_ALARM_DELTA,
@@ -556,14 +558,28 @@
 
 @topic_to_command_handler(register_list=COMMAND_REGISTER, topic=BEEP)
 def beep(address: Address, topic=pub.AUTO_TOPIC):
     """Create a BEEP command."""
     _create_direct_message(topic=topic, address=address)
 
 
+@topic_to_command_handler(register_list=COMMAND_REGISTER, topic=FACTORY_RESET)
+def factory_reset(
+    address: Address, cat: DeviceCategory, subcat: int, topic=pub.AUTO_TOPIC
+):
+    """Create a FACTORY RESET command."""
+    user_data = UserData(
+        {
+            "d1": int(cat),
+            "d2": subcat,
+        }
+    )
+    _create_direct_message(topic=topic, address=address, user_data=user_data)
+
+
 @topic_to_command_handler(register_list=COMMAND_REGISTER, topic=NIGHT_MODE_OFF)
 def night_mode_off(address: Address, topic=pub.AUTO_TOPIC):
     """Create a NIGHT MODE OFF command."""
     _create_direct_message(topic=topic, address=address, cmd2=0x00)
 
 
 @topic_to_command_handler(register_list=COMMAND_REGISTER, topic=NIGHT_MODE_ON)
```

### Comparing `pyinsteon-1.4.1/pyinsteon/protocol/http_reader_writer.py` & `pyinsteon-1.4.2/pyinsteon/protocol/http_reader_writer.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/protocol/http_transport.py` & `pyinsteon-1.4.2/pyinsteon/protocol/http_transport.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/protocol/messages/__init__.py` & `pyinsteon-1.4.2/pyinsteon/protocol/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/protocol/messages/inbound.py` & `pyinsteon-1.4.2/pyinsteon/protocol/messages/inbound.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/protocol/messages/message_definition.py` & `pyinsteon-1.4.2/pyinsteon/protocol/messages/message_definition.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/protocol/messages/message_definitions.py` & `pyinsteon-1.4.2/pyinsteon/protocol/messages/message_definitions.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/protocol/messages/outbound.py` & `pyinsteon-1.4.2/pyinsteon/protocol/messages/outbound.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/protocol/mock/mock_reader.py` & `pyinsteon-1.4.2/pyinsteon/protocol/mock/mock_reader.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/protocol/mock/mock_transport.py` & `pyinsteon-1.4.2/pyinsteon/protocol/mock/mock_transport.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/protocol/msg_to_topic.py` & `pyinsteon-1.4.2/pyinsteon/protocol/msg_to_topic.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/protocol/msg_to_url.py` & `pyinsteon-1.4.2/pyinsteon/protocol/msg_to_url.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/protocol/protocol.py` & `pyinsteon-1.4.2/pyinsteon/protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/protocol/serial_transport.py` & `pyinsteon-1.4.2/pyinsteon/protocol/serial_transport.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/protocol/topic_converters.py` & `pyinsteon-1.4.2/pyinsteon/protocol/topic_converters.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/subscriber_base.py` & `pyinsteon-1.4.2/pyinsteon/subscriber_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/tools/__init__.py` & `pyinsteon-1.4.2/pyinsteon/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/tools/advanced.py` & `pyinsteon-1.4.2/pyinsteon/tools/advanced.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/tools/aldb.py` & `pyinsteon-1.4.2/pyinsteon/tools/aldb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/tools/commands.py` & `pyinsteon-1.4.2/pyinsteon/tools/commands.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/tools/config.py` & `pyinsteon-1.4.2/pyinsteon/tools/config.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/tools/log_filter.py` & `pyinsteon-1.4.2/pyinsteon/tools/log_filter.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/tools/scenes.py` & `pyinsteon-1.4.2/pyinsteon/tools/scenes.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/tools/tools_base.py` & `pyinsteon-1.4.2/pyinsteon/tools/tools_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     "group": bytes,
     "humidity": bytes,
     "link_mode": bool,
     "logging_mode": bool,
     "master": Address,
     "monitor_mode": bool,
     "on_level": bytes,
+    "on": bool,
     "open_level": bytes,
     "relay_mode": RelayMode,
     "seconds": bytes,
     "temperature": bytes,
     "thermostat_mode": ThermostatMode,
     "toggle_mode": ToggleMode,
 }
```

### Comparing `pyinsteon-1.4.1/pyinsteon/tools/utils.py` & `pyinsteon-1.4.2/pyinsteon/tools/utils.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/topics.py` & `pyinsteon-1.4.2/pyinsteon/topics.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 THERMOSTAT_COOL_SET_POINT_STATUS = "thermostat_cool_set_point_status"
 THERMOSTAT_HEAT_SET_POINT_STATUS = "thermostat_heat_set_point_status"
 LEAK_DETECTOR_ANNOUNCE = "leak_detector_announce"
 SET_SPRINKLER_PROGRAM = "set_sprinkler_program"
 SPRINKLER_GET_PROGRAM_RESPONSE = "sprinkler_get_program_response"
 IO_SET_SENSOR_NOMINAL_VALUE = "io_set_sensor_nominal_value"
 IO_ALARM_DATA_RESPONSE = "io_alarm_data_response"
+FACTORY_RESET = "factory_reset"
 
 ALDB_LINK_CHANGED = "aldb.link_changed"
 
 ENGINE_VERSION = "engine_version"
 ALDB_STATUS_CHANGED = "aldb_status_changed"
 EXTENDED_PROPERTIES_CHANGED = "extended_properties_changed"
```

### Comparing `pyinsteon-1.4.1/pyinsteon/utils.py` & `pyinsteon-1.4.2/pyinsteon/utils.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon/x10_address.py` & `pyinsteon-1.4.2/pyinsteon/x10_address.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.4.1/pyinsteon.egg-info/PKG-INFO` & `pyinsteon-1.4.2/pyinsteon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinsteon
-Version: 1.4.1
+Version: 1.4.2
 Summary: Open-source Insteon home automation module running on Python 3.
 Author-email: The pyinsteon authors <pyinsteon@harrisnj.net>
 License: MIT License
 Project-URL: Source Code, https://github.com/pyinsteon/pyinsteon
 Project-URL: Bug Reports, https://github.com/pyinsteon/pyinsteon/issues
 Keywords: home,automation,insteon,python,python3
 Platform: any
```

### Comparing `pyinsteon-1.4.1/pyinsteon.egg-info/SOURCES.txt` & `pyinsteon-1.4.2/pyinsteon.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,15 @@
 pyinsteon/handlers/to_device/all_link_cleanup_command.py
 pyinsteon/handlers/to_device/direct_command.py
 pyinsteon/handlers/to_device/engine_version_request.py
 pyinsteon/handlers/to_device/enter_linking_mode.py
 pyinsteon/handlers/to_device/enter_unlinking_mode.py
 pyinsteon/handlers/to_device/extended_get.py
 pyinsteon/handlers/to_device/extended_set.py
+pyinsteon/handlers/to_device/factory_reset.py
 pyinsteon/handlers/to_device/get_operating_flags.py
 pyinsteon/handlers/to_device/id_request.py
 pyinsteon/handlers/to_device/night_mode_off.py
 pyinsteon/handlers/to_device/night_mode_on.py
 pyinsteon/handlers/to_device/off.py
 pyinsteon/handlers/to_device/off_all_link_cleanup.py
 pyinsteon/handlers/to_device/off_fast.py
```

### Comparing `pyinsteon-1.4.1/pyproject.toml` & `pyinsteon-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "pyinsteon"
-version     = "1.4.1"
+version     = "1.4.2"
 license     = {text = "MIT License"}
 description = "Open-source Insteon home automation module running on Python 3."
 readme      = "DESCRIPTION.rst"
 authors     = [
     {name = "The pyinsteon authors", email = "pyinsteon@harrisnj.net"}
 ]
 keywords    = ["home", "automation", "insteon", "python", "python3"]
```

### Comparing `pyinsteon-1.4.1/setup.cfg` & `pyinsteon-1.4.2/setup.cfg`

 * *Files identical despite different names*

