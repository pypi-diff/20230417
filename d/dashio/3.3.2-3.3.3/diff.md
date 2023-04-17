# Comparing `tmp/dashio-3.3.2.tar.gz` & `tmp/dashio-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashio-3.3.2.tar", last modified: Mon Mar 27 06:17:44 2023, max compression
+gzip compressed data, was "dashio-3.3.3.tar", last modified: Thu Mar 30 02:50:41 2023, max compression
```

## Comparing `dashio-3.3.2.tar` & `dashio-3.3.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:17:44.816154 dashio-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-27 06:17:24.000000 dashio-3.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-03-27 06:17:44.816154 dashio-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-03-27 06:17:24.000000 dashio-3.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:17:44.804154 dashio-3.3.2/dashio/
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/action_station.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:17:44.808153 dashio-3.3.2/dashio/action_station_services/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/action_station_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/action_station_services/action_station_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/action_station_services/as_servicel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/action_station_services/clock_servicel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/action_station_services/modbus_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/action_station_services/task_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/action_station_services/timer_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/bleconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/dashconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:17:44.808153 dashio-3.3.2/dashio/iotcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/audio_visual_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/button_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/device_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/dial.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/knob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/ring_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/textbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/iotcontrol/time_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/mqttconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/serialconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/tcpconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/zeroconf_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-03-27 06:17:24.000000 dashio-3.3.2/dashio/zmqconnection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:17:44.804154 dashio-3.3.2/dashio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-03-27 06:17:44.000000 dashio-3.3.2/dashio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-03-27 06:17:44.000000 dashio-3.3.2/dashio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 06:17:44.000000 dashio-3.3.2/dashio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 06:17:44.000000 dashio-3.3.2/dashio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-27 06:17:44.000000 dashio-3.3.2/dashio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-27 06:17:44.000000 dashio-3.3.2/dashio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-27 06:17:24.000000 dashio-3.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-27 06:17:44.816154 dashio-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-27 06:17:24.000000 dashio-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 06:17:44.816154 dashio-3.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_button_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_dashconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_dashdevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_device_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_dial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_knob.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_mqttconntection.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_tcpconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_textbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_time_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 06:17:24.000000 dashio-3.3.2/tests/test_zqmconnection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 02:50:41.791557 dashio-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-30 02:50:33.000000 dashio-3.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-03-30 02:50:41.791557 dashio-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-03-30 02:50:33.000000 dashio-3.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 02:50:41.783557 dashio-3.3.3/dashio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/action_station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 02:50:41.783557 dashio-3.3.3/dashio/action_station_services/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/action_station_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/action_station_services/action_station_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/action_station_services/as_servicel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/action_station_services/clock_servicel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/action_station_services/modbus_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/action_station_services/task_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/action_station_services/timer_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/bleconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/dashconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 02:50:41.787557 dashio-3.3.3/dashio/iotcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/audio_visual_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/button_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/device_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/knob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/ring_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/textbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/time_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/mqttconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/serialconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/tcpconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/zeroconf_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/zmqconnection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 02:50:41.783557 dashio-3.3.3/dashio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-03-30 02:50:41.000000 dashio-3.3.3/dashio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-03-30 02:50:41.000000 dashio-3.3.3/dashio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 02:50:41.000000 dashio-3.3.3/dashio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 02:50:41.000000 dashio-3.3.3/dashio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-30 02:50:41.000000 dashio-3.3.3/dashio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-30 02:50:41.000000 dashio-3.3.3/dashio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-30 02:50:33.000000 dashio-3.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-30 02:50:41.791557 dashio-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-30 02:50:33.000000 dashio-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 02:50:41.791557 dashio-3.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_button_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_dashconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_dashdevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_device_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_knob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_mqttconntection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_tcpconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_textbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_time_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_zqmconnection.py
```

### Comparing `dashio-3.3.2/LICENSE` & `dashio-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/PKG-INFO` & `dashio-3.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashio
-Version: 3.3.2
+Version: 3.3.3
 Summary: DashIO interface library
 Home-page: https://dashio.io
 Download-URL: https://github.com/dashio-connect/python-dashio
 Author: James Boulton
 Author-email: james@dashio.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dashio-3.3.2/README.md` & `dashio-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/__init__.py` & `dashio-3.3.3/dashio/__init__.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/action_station.py` & `dashio-3.3.3/dashio/action_station.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/action_station_services/action_station_service_config.py` & `dashio-3.3.3/dashio/action_station_services/action_station_service_config.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/action_station_services/as_servicel.py` & `dashio-3.3.3/dashio/action_station_services/as_servicel.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/action_station_services/clock_servicel.py` & `dashio-3.3.3/dashio/action_station_services/clock_servicel.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/action_station_services/modbus_service.py` & `dashio-3.3.3/dashio/action_station_services/modbus_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/action_station_services/task_service.py` & `dashio-3.3.3/dashio/action_station_services/task_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/action_station_services/timer_service.py` & `dashio-3.3.3/dashio/action_station_services/timer_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/bleconnection.py` & `dashio-3.3.3/dashio/bleconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/constants.py` & `dashio-3.3.3/dashio/constants.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/dashconnection.py` & `dashio-3.3.3/dashio/dashconnection.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,28 +129,30 @@
     close() :
         close the connection
     """
     def _on_connect(self, client, userdata, flags, msg):
         if msg == 0:
             self._connected = True
             self._disconnected = False
+            self._connecting = False
             for device_id in self._device_id_list:
                 control_topic = f"{self.username}/{device_id}/control"
                 self._dash_c.subscribe(control_topic, 0)
             for device_id in self._device_id_rx_list:
                 data_topic = f"{self.username}/{device_id}/data"
                 self._dash_c.subscribe(data_topic, 0)
             self._send_dash_announce()
             logging.debug("connected OK")
         else:
             logging.debug("Bad connection Returned code=%s", msg)
 
     def _on_disconnect(self, client, userdata, msg):
         logging.debug("disconnecting reason  %s", msg)
         self._connected = False
+        self._connecting = False
         self._disconnected = True
         self.disconnect_timeout = 1.0
 
     def _on_message(self, client, obj, msg):
         data = str(msg.payload, "utf-8").strip()
         logging.debug("DASH RX:\n%s", data)
         self.tx_zmq_pub.send_multipart([msg.payload, self._b_zmq_connection_uuid])
@@ -244,14 +246,15 @@
         """
 
         threading.Thread.__init__(self, daemon=True)
 
         self.context = context or zmq.Context.instance()
         self._connected = False
         self._disconnected = True
+        self._connecting = True
         self.zmq_connection_uuid = "DASH:" + shortuuid.uuid()
         self._b_zmq_connection_uuid = self.zmq_connection_uuid.encode('utf-8')
         self._device_id_list = []
         self._device_id_rx_list = []
         # self.LWD = "OFFLINE"
         self.running = True
         self.username = username
@@ -279,14 +282,15 @@
         # self.dash_c.on_log = self.__on_log
         # self.dash_c.will_set(self.data_topic, self.LWD, qos=1, retain=False)
         # Connect
         if username and password:
             self._dash_c.username_pw_set(username, password)
             try:
                 self._dash_c.connect(host, port)
+                self._connecting = True
             except mqtt.socket.gaierror as error:
                 logging.debug("No connection to internet: %s", str(error))
         # Start subscribe, with QoS level 0
         self.rx_zmq_sub = self.context.socket(zmq.SUB)
         self.disconnect_timeout = 15.0
         self.start()
 
@@ -348,19 +352,20 @@
                 elif msg_to == b"DASH":
                     data_topic = f"{self.username}/{device_id}/announce"
                 else:
                     data_topic = f"{self.username}/{device_id}/data"
                 if self._connected and data_topic:
                     logging.debug("DASH TX:\n%s", data.decode().rstrip())
                     self._dash_c.publish(data_topic, data.decode())
-            if self._disconnected:
+            if self._disconnected and not self._connecting:
                 self.disconnect_timeout = min(self.disconnect_timeout, 900)
                 time.sleep(self.disconnect_timeout)
                 try:
                     self._dash_c.connect(self.host, self.port)
+                    self._connecting = True
                 except mqtt.socket.gaierror as error:
                     logging.debug("No connection to internet: %s", str(error))
                 self.disconnect_timeout = self.disconnect_timeout * 2
 
         self._dash_c.loop_stop()
         self.tx_zmq_pub.close()
         self.rx_zmq_sub.close()
```

### Comparing `dashio-3.3.2/dashio/device.py` & `dashio-3.3.3/dashio/device.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/__init__.py` & `dashio-3.3.3/dashio/iotcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/alarm.py` & `dashio-3.3.3/dashio/iotcontrol/alarm.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/audio_visual_display.py` & `dashio-3.3.3/dashio/iotcontrol/audio_visual_display.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/button.py` & `dashio-3.3.3/dashio/iotcontrol/button.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/button_group.py` & `dashio-3.3.3/dashio/iotcontrol/button_group.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/chart.py` & `dashio-3.3.3/dashio/iotcontrol/chart.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/color_picker.py` & `dashio-3.3.3/dashio/iotcontrol/color_picker.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/control.py` & `dashio-3.3.3/dashio/iotcontrol/control.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/device_view.py` & `dashio-3.3.3/dashio/iotcontrol/device_view.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/dial.py` & `dashio-3.3.3/dashio/iotcontrol/dial.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/direction.py` & `dashio-3.3.3/dashio/iotcontrol/direction.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/enums.py` & `dashio-3.3.3/dashio/iotcontrol/enums.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/event.py` & `dashio-3.3.3/dashio/iotcontrol/event.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/event_log.py` & `dashio-3.3.3/dashio/iotcontrol/event_log.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/knob.py` & `dashio-3.3.3/dashio/iotcontrol/knob.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/label.py` & `dashio-3.3.3/dashio/iotcontrol/label.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/map.py` & `dashio-3.3.3/dashio/iotcontrol/map.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/menu.py` & `dashio-3.3.3/dashio/iotcontrol/menu.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/ring_buffer.py` & `dashio-3.3.3/dashio/iotcontrol/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/selector.py` & `dashio-3.3.3/dashio/iotcontrol/selector.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/slider.py` & `dashio-3.3.3/dashio/iotcontrol/slider.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/textbox.py` & `dashio-3.3.3/dashio/iotcontrol/textbox.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/iotcontrol/time_graph.py` & `dashio-3.3.3/dashio/iotcontrol/time_graph.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/ip.py` & `dashio-3.3.3/dashio/ip.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/load_config.py` & `dashio-3.3.3/dashio/load_config.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/mqttconnection.py` & `dashio-3.3.3/dashio/mqttconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/serialconnection.py` & `dashio-3.3.3/dashio/serialconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/tcpconnection.py` & `dashio-3.3.3/dashio/tcpconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/zeroconf_service.py` & `dashio-3.3.3/dashio/zeroconf_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio/zmqconnection.py` & `dashio-3.3.3/dashio/zmqconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/dashio.egg-info/PKG-INFO` & `dashio-3.3.3/dashio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashio
-Version: 3.3.2
+Version: 3.3.3
 Summary: DashIO interface library
 Home-page: https://dashio.io
 Download-URL: https://github.com/dashio-connect/python-dashio
 Author: James Boulton
 Author-email: james@dashio.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dashio-3.3.2/dashio.egg-info/SOURCES.txt` & `dashio-3.3.3/dashio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/setup.cfg` & `dashio-3.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/setup.py` & `dashio-3.3.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="dashio",
-    version="3.3.2",
+    version="3.3.3",
     description="DashIO interface library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="James Boulton",
     author_email="james@dashio.com",
     url="https://dashio.io",
     download_url="https://github.com/dashio-connect/python-dashio",
```

### Comparing `dashio-3.3.2/tests/test_button.py` & `dashio-3.3.3/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/tests/test_button_group.py` & `dashio-3.3.3/tests/test_button_group.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/tests/test_chart.py` & `dashio-3.3.3/tests/test_chart.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/tests/test_dashdevice.py` & `dashio-3.3.3/tests/test_dashdevice.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/tests/test_device_view.py` & `dashio-3.3.3/tests/test_device_view.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/tests/test_dial.py` & `dashio-3.3.3/tests/test_dial.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/tests/test_direction.py` & `dashio-3.3.3/tests/test_direction.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/tests/test_event_log.py` & `dashio-3.3.3/tests/test_event_log.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/tests/test_knob.py` & `dashio-3.3.3/tests/test_knob.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/tests/test_label.py` & `dashio-3.3.3/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/tests/test_map.py` & `dashio-3.3.3/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/tests/test_menu.py` & `dashio-3.3.3/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/tests/test_selector.py` & `dashio-3.3.3/tests/test_selector.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/tests/test_slider.py` & `dashio-3.3.3/tests/test_slider.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/tests/test_textbox.py` & `dashio-3.3.3/tests/test_textbox.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.2/tests/test_time_graph.py` & `dashio-3.3.3/tests/test_time_graph.py`

 * *Files identical despite different names*

