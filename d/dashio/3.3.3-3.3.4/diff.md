# Comparing `tmp/dashio-3.3.3.tar.gz` & `tmp/dashio-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashio-3.3.3.tar", last modified: Thu Mar 30 02:50:41 2023, max compression
+gzip compressed data, was "dashio-3.3.4.tar", last modified: Mon Apr 17 02:20:18 2023, max compression
```

## Comparing `dashio-3.3.3.tar` & `dashio-3.3.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 02:50:41.791557 dashio-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-30 02:50:33.000000 dashio-3.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-03-30 02:50:41.791557 dashio-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-03-30 02:50:33.000000 dashio-3.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 02:50:41.783557 dashio-3.3.3/dashio/
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/action_station.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 02:50:41.783557 dashio-3.3.3/dashio/action_station_services/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/action_station_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/action_station_services/action_station_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/action_station_services/as_servicel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/action_station_services/clock_servicel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/action_station_services/modbus_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/action_station_services/task_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/action_station_services/timer_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/bleconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/dashconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 02:50:41.787557 dashio-3.3.3/dashio/iotcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/audio_visual_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/button_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/device_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/dial.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/knob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/ring_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/textbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/iotcontrol/time_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/mqttconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/serialconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/tcpconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/zeroconf_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-03-30 02:50:33.000000 dashio-3.3.3/dashio/zmqconnection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 02:50:41.783557 dashio-3.3.3/dashio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-03-30 02:50:41.000000 dashio-3.3.3/dashio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-03-30 02:50:41.000000 dashio-3.3.3/dashio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 02:50:41.000000 dashio-3.3.3/dashio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 02:50:41.000000 dashio-3.3.3/dashio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-30 02:50:41.000000 dashio-3.3.3/dashio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-30 02:50:41.000000 dashio-3.3.3/dashio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-30 02:50:33.000000 dashio-3.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-30 02:50:41.791557 dashio-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-30 02:50:33.000000 dashio-3.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 02:50:41.791557 dashio-3.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_button_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_dashconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_dashdevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_device_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_dial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_knob.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_mqttconntection.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_tcpconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_textbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_time_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 02:50:33.000000 dashio-3.3.3/tests/test_zqmconnection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:20:18.635324 dashio-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-17 02:20:10.000000 dashio-3.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-17 02:20:18.635324 dashio-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-17 02:20:10.000000 dashio-3.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:20:18.627324 dashio-3.3.4/dashio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/action_station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:20:18.627324 dashio-3.3.4/dashio/action_station_services/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/action_station_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/action_station_services/action_station_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/action_station_services/as_servicel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/action_station_services/clock_servicel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/action_station_services/modbus_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/action_station_services/task_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/action_station_services/timer_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/bleconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/dashconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:20:18.631324 dashio-3.3.4/dashio/iotcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/audio_visual_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/button_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/device_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/knob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/ring_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/textbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/iotcontrol/time_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/mqttconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/serialconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/tcpconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/zeroconf_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-17 02:20:10.000000 dashio-3.3.4/dashio/zmqconnection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:20:18.627324 dashio-3.3.4/dashio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-17 02:20:18.000000 dashio-3.3.4/dashio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-17 02:20:18.000000 dashio-3.3.4/dashio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 02:20:18.000000 dashio-3.3.4/dashio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 02:20:18.000000 dashio-3.3.4/dashio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-17 02:20:18.000000 dashio-3.3.4/dashio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-17 02:20:18.000000 dashio-3.3.4/dashio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-17 02:20:10.000000 dashio-3.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-17 02:20:18.635324 dashio-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-17 02:20:10.000000 dashio-3.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:20:18.635324 dashio-3.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_button_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_dashconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_dashdevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_device_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_knob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_mqttconntection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_tcpconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_textbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_time_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:20:10.000000 dashio-3.3.4/tests/test_zqmconnection.py
```

### Comparing `dashio-3.3.3/LICENSE` & `dashio-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/PKG-INFO` & `dashio-3.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: dashio
-Version: 3.3.3
+Version: 3.3.4
 Summary: DashIO interface library
 Home-page: https://dashio.io
 Download-URL: https://github.com/dashio-connect/python-dashio
 Author: James Boulton
 Author-email: james@dashio.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.6.0
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
-# DashIO
+# python-dashio
 
 ![Tests](https://github.com/dashio-connect/python-dashio/actions/workflows/tests.yml/badge.svg)
 
-[**DashIO**](http://dashio.io) - It is a quick effortless way to connect your IoT device to your phone, tablet or iPad using the free **Dash** app. It allows easy setup of controls such as Dials, Text Boxes, Charts, Graphs, Notifications..., from your IoT device. You can define the look and layout of the controls on your phone from your IoT device. There are three methods to connect to your phone; Bluetooth Low Energy (BLE), TCP or MQTT.
+[**python-dashio**](http://www.dashio.io) - It is a quick effortless way to connect your IoT device to your phone, tablet or iPad using the free **Dash** app. It allows easy setup of controls such as Dials, Text Boxes, Charts, Graphs, Notifications..., from your IoT device. You can define the look and layout of the controls on your phone from your IoT device. There are three methods to connect to your phone; Bluetooth Low Energy (BLE), TCP or MQTT.
 
 ## Getting Started
 
 For the big picture on **DashIO**, take a look at our website: <a href="https://dashio.io">dashio.io</a>
 
 ## Documentation
```

### Comparing `dashio-3.3.3/README.md` & `dashio-3.3.4/dashio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,28 @@
-# DashIO
+Metadata-Version: 2.1
+Name: dashio
+Version: 3.3.4
+Summary: DashIO interface library
+Home-page: https://dashio.io
+Download-URL: https://github.com/dashio-connect/python-dashio
+Author: James Boulton
+Author-email: james@dashio.com
+License: MIT
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Operating System :: OS Independent
+Requires-Python: >3.6.0
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE
+
+# python-dashio
 
 ![Tests](https://github.com/dashio-connect/python-dashio/actions/workflows/tests.yml/badge.svg)
 
-[**DashIO**](http://dashio.io) - It is a quick effortless way to connect your IoT device to your phone, tablet or iPad using the free **Dash** app. It allows easy setup of controls such as Dials, Text Boxes, Charts, Graphs, Notifications..., from your IoT device. You can define the look and layout of the controls on your phone from your IoT device. There are three methods to connect to your phone; Bluetooth Low Energy (BLE), TCP or MQTT.
+[**python-dashio**](http://www.dashio.io) - It is a quick effortless way to connect your IoT device to your phone, tablet or iPad using the free **Dash** app. It allows easy setup of controls such as Dials, Text Boxes, Charts, Graphs, Notifications..., from your IoT device. You can define the look and layout of the controls on your phone from your IoT device. There are three methods to connect to your phone; Bluetooth Low Energy (BLE), TCP or MQTT.
 
 ## Getting Started
 
 For the big picture on **DashIO**, take a look at our website: <a href="https://dashio.io">dashio.io</a>
 
 ## Documentation
```

### Comparing `dashio-3.3.3/dashio/__init__.py` & `dashio-3.3.4/dashio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
     ButtonState,
     LabelStyle,
     KnobStyle,
     ChartXAxisLabelsStyle,
     TextFormat,
     DirectionStyle,
     ColorPickerStyle,
-    ControlName
+    ControlName,
+    ButtonStyle
 )
 from .iotcontrol.audio_visual_display import AudioVisualDisplay
 from .iotcontrol.chart import Chart, ChartLine
 from .iotcontrol.slider import Slider
 from .iotcontrol.textbox import TextBox
 from .iotcontrol.button import Button
 from .iotcontrol.time_graph import TimeGraph, TimeGraphLine, DataPoint
```

### Comparing `dashio-3.3.3/dashio/action_station.py` & `dashio-3.3.4/dashio/action_station.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/action_station_services/action_station_service_config.py` & `dashio-3.3.4/dashio/action_station_services/action_station_service_config.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/action_station_services/as_servicel.py` & `dashio-3.3.4/dashio/action_station_services/as_servicel.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/action_station_services/clock_servicel.py` & `dashio-3.3.4/dashio/action_station_services/clock_servicel.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/action_station_services/modbus_service.py` & `dashio-3.3.4/dashio/action_station_services/modbus_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/action_station_services/task_service.py` & `dashio-3.3.4/dashio/action_station_services/task_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/action_station_services/timer_service.py` & `dashio-3.3.4/dashio/action_station_services/timer_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/bleconnection.py` & `dashio-3.3.4/dashio/bleconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/constants.py` & `dashio-3.3.4/dashio/constants.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/dashconnection.py` & `dashio-3.3.4/dashio/dashconnection.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import time
 
 import paho.mqtt.client as mqtt
 import shortuuid
 import zmq
 
 from .constants import CONNECTION_PUB_URL
-
+from .iotcontrol.enums import ConnectionState
 
 class DashControl():
     """Class to stare dash connection info
     """
     def get_state(self) -> str:
         """Not used by this class as its a CFG only control
         """
@@ -127,34 +127,30 @@
     set_connection(username, password):
         change the connection username and password
     close() :
         close the connection
     """
     def _on_connect(self, client, userdata, flags, msg):
         if msg == 0:
-            self._connected = True
-            self._disconnected = False
-            self._connecting = False
+            self._connection_state = ConnectionState.CONNECTED
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
-        self._connected = False
-        self._connecting = False
-        self._disconnected = True
-        self.disconnect_timeout = 1.0
+        self._connection_state = ConnectionState.DISCONNECTED
+        self._disconnect_timeout = 1.0
 
     def _on_message(self, client, obj, msg):
         data = str(msg.payload, "utf-8").strip()
         logging.debug("DASH RX:\n%s", data)
         self.tx_zmq_pub.send_multipart([msg.payload, self._b_zmq_connection_uuid])
 
     def _on_subscribe(self, client, obj, mid, granted_qos):
@@ -170,15 +166,15 @@
         ----------
             device (Device):
                 The Device to add.
         """
         if device.device_id not in self._device_id_list:
             self._device_id_list.append(device.device_id)
             device.register_connection(self)
-            if self._connected:
+            if self._connection_state == ConnectionState.CONNECTED:
                 control_topic = f"{self.username}/{device.device_id}/control"
                 self._dash_c.subscribe(control_topic, 0)
                 self._send_dash_announce()
 
     def _add_device_rx(self, msg_dict):
         """Connect to another device"""
         device_id = msg_dict["deviceID"]
@@ -244,17 +240,15 @@
             use_ssl : Boolean
                 Defaults to True.
         """
 
         threading.Thread.__init__(self, daemon=True)
 
         self.context = context or zmq.Context.instance()
-        self._connected = False
-        self._disconnected = True
-        self._connecting = True
+        self._connection_state = ConnectionState.DISCONNECTED
         self.zmq_connection_uuid = "DASH:" + shortuuid.uuid()
         self._b_zmq_connection_uuid = self.zmq_connection_uuid.encode('utf-8')
         self._device_id_list = []
         self._device_id_rx_list = []
         # self.LWD = "OFFLINE"
         self.running = True
         self.username = username
@@ -282,20 +276,20 @@
         # self.dash_c.on_log = self.__on_log
         # self.dash_c.will_set(self.data_topic, self.LWD, qos=1, retain=False)
         # Connect
         if username and password:
             self._dash_c.username_pw_set(username, password)
             try:
                 self._dash_c.connect(host, port)
-                self._connecting = True
+                self._connection_state = ConnectionState.CONNECTING
             except mqtt.socket.gaierror as error:
                 logging.debug("No connection to internet: %s", str(error))
         # Start subscribe, with QoS level 0
         self.rx_zmq_sub = self.context.socket(zmq.SUB)
-        self.disconnect_timeout = 15.0
+        self._disconnect_timeout = 1.0
         self.start()
 
     def close(self):
         """Close the connection."""
         self.running = False
 
     def _dash_command(self, msg_dict: dict):
@@ -349,23 +343,23 @@
                 if control_type == b'ALM':
                     data_topic = f"{self.username}/{device_id}/alarm"
                     control_type = ""
                 elif msg_to == b"DASH":
                     data_topic = f"{self.username}/{device_id}/announce"
                 else:
                     data_topic = f"{self.username}/{device_id}/data"
-                if self._connected and data_topic:
+                if self._connection_state == ConnectionState.CONNECTED and data_topic:
                     logging.debug("DASH TX:\n%s", data.decode().rstrip())
                     self._dash_c.publish(data_topic, data.decode())
-            if self._disconnected and not self._connecting:
-                self.disconnect_timeout = min(self.disconnect_timeout, 900)
-                time.sleep(self.disconnect_timeout)
+            if self._connection_state == ConnectionState.DISCONNECTED:
+                self._disconnect_timeout = min(self._disconnect_timeout, 900)
+                time.sleep(self._disconnect_timeout)
                 try:
                     self._dash_c.connect(self.host, self.port)
-                    self._connecting = True
+                    self._connection_state = ConnectionState.CONNECTING
                 except mqtt.socket.gaierror as error:
                     logging.debug("No connection to internet: %s", str(error))
-                self.disconnect_timeout = self.disconnect_timeout * 2
+                self._disconnect_timeout = self._disconnect_timeout * 2
 
         self._dash_c.loop_stop()
         self.tx_zmq_pub.close()
         self.rx_zmq_sub.close()
```

### Comparing `dashio-3.3.3/dashio/device.py` & `dashio-3.3.4/dashio/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,20 @@
 
     remove_control(iot_control) :
         Remove a control from the device.
 
     get_control(control_type: str, control_id: str):
         returns the instance of a controla leaded into the device.
 
+    remove_control(control_type, control_id) :
+        Removes the control from the device.
+
+    is_control_loaded(iot_control) :
+         Returns boolean if the control is loaded in the device.
+
     add_all_c64_controls(c64_dict: dict):
         Adds all controls defined in c64_dict into the device.
 
     set_wifi_callback(callback) :
         Set a callback function that is called when the DashIO app provides wifi provisioning information.
 
     unset_wifi_callback() :
@@ -175,15 +181,14 @@
                 continue
             if control.cntrl_type == "DVVW":
                 cfg_list = control.get_cfg(data)
                 for cfg in cfg_list:
                     dvvw_str += self._device_id_str + cfg
             else:
                 cfg_list = control.get_cfg(data)
-                #  logging.debug("CFG: %s", cfg_list)
                 for cfg in cfg_list:
                     reply += self._device_id_str + cfg
         reply += dvvw_str
         return reply
 
     def _send_alarm(self, alarm_id, message_header, message_body):
         payload = self._device_id_str + f"\tALM\t{alarm_id}\t{message_header}\t{message_body}\n"
@@ -203,20 +208,20 @@
             pass
 
     def _send_announce(self):
         payload = self._device_id_str + f"\tWHO\t{self.device_type}\t{self.device_name}\n"
         logging.debug("ANNOUNCE: %s", payload)
         self.tx_zmq_pub.send_multipart([b"DASH", payload.encode('utf-8')])
 
-    def is_control_loaded(self, control_type, control_id) -> bool:
+    def is_control_loaded(self, control_type, control_id: str) -> bool:
         """Is the control loaded in the device?"""
         key = f"{control_type}\t{control_id}"
         return key in self.controls_dict
 
-    def add_all_c64_controls(self, c64_dict):
+    def add_all_c64_controls(self, c64_dict: dict):
         """Loads all the controls in cfg_dict into the device.
 
         Parameters
         ----------
         c64_dict : Dict
             dictionary of the CFG loaded by decode_cfg from a CFG64 or json
         """
```

### Comparing `dashio-3.3.3/dashio/iotcontrol/__init__.py` & `dashio-3.3.4/dashio/iotcontrol/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """The DashIO module is for creating devices, controls and connections for the DashIO app.
 """
 from .enums import Color, Icon, Precision, Keyboard, TextAlignment, SliderBarStyle, DialNumberPosition, DialStyle,\
     SoundName, ChartLineType, TimeGraphLineType, TimeGraphPositionOfKey, ButtonState, LabelStyle, KnobStyle,\
-    TitlePosition, ChartXAxisLabelsStyle, TextFormat, DirectionStyle, ColorPickerStyle, ControlName
+    TitlePosition, ChartXAxisLabelsStyle, TextFormat, DirectionStyle, ColorPickerStyle, ControlName, ButtonStyle
 from .audio_visual_display import AudioVisualDisplay
 from .chart import Chart, ChartLine, ChartConfig
 from .slider import Slider, SliderConfig
 from .textbox import TextBox, TextBoxConfig
 from .button import Button, ButtonConfig
 from .time_graph import TimeGraph, TimeGraphLine, DataPoint, TimeGraphConfig
 from .knob import Knob, KnobConfig
```

### Comparing `dashio-3.3.3/dashio/iotcontrol/alarm.py` & `dashio-3.3.4/dashio/iotcontrol/alarm.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/audio_visual_display.py` & `dashio-3.3.4/dashio/iotcontrol/audio_visual_display.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/button.py` & `dashio-3.3.4/dashio/iotcontrol/button.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,36 +18,38 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from ..constants import BAD_CHARS
-from .control import Control, ControlPosition, ControlConfig, _get_color, _get_icon, _get_title_position
-from .enums import ButtonState, Color, Icon, TitlePosition
+from .control import Control, ControlPosition, ControlConfig, _get_color, _get_icon, _get_title_position, _get_button_style
+from .enums import ButtonState, Color, Icon, TitlePosition, ButtonStyle
 
 
 class ButtonConfig(ControlConfig):
     """ButtonGroupConfig"""
     def __init__(
         self,
         control_id: str,
         title: str,
         title_position: TitlePosition,
         button_enabled: bool,
+        style: ButtonStyle,
         icon_name: Icon,
         on_color: Color,
         off_color: Color,
         text: str,
         control_position: ControlPosition
     ) -> None:
         super().__init__(control_id, title, control_position, title_position)
         self.cfg["text"] = text.translate(BAD_CHARS)
         self.cfg["iconName"] = icon_name.value
         self.cfg["buttonEnabled"] = button_enabled
+        self.cfg["style"] = str(style.value)
         self.cfg["onColor"] = str(on_color.value)
         self.cfg["offColor"] = str(off_color.value)
 
     @classmethod
     def from_dict(cls, cfg_dict: dict):
         """Instantiates ButtonGroupConfig from cfg dictionary
 
@@ -61,14 +63,15 @@
         ButtonGroupConfig
         """
         tmp_cls = cls(
             cfg_dict["controlID"],
             cfg_dict["title"],
             _get_title_position(cfg_dict["titlePosition"]),
             cfg_dict["buttonEnabled"],
+            _get_button_style(cfg_dict["style"]),
             _get_icon(cfg_dict["iconName"]),
             _get_color(cfg_dict["onColor"]),
             _get_color(cfg_dict["offColor"]),
             cfg_dict["text"],
             ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
@@ -86,14 +89,16 @@
         A short title for the button group
     text : str
         The text that appears on the ButtonGroup
     title_position : TitlePosition
         Can be TitlePosition.BOTTOM, TitlePosition.TOP, TitlePosition.OFF
     button_enabled : boolean
         True allows the app to send button events. False disables button pushes
+    stype : ButtonStyle
+        The style of the button. Options are ButtonStyle.BASIC, ButtonStyle.HIGHLIGHT
     icon_name : Icon
         Set the icon for the button
     off_color : Color
         Set the off color
     on_color : Color
         Set the on color
     control_position : ControlPosition
@@ -121,27 +126,29 @@
 
     def __init__(
         self,
         control_id,
         title="A Button",
         title_position=TitlePosition.BOTTOM,
         button_enabled=True,
+        style=ButtonStyle.BASIC,
         icon_name=Icon.NONE,
         on_color=Color.BLUE,
         off_color=Color.RED,
         text="",
         control_position: ControlPosition = None
     ):
         super().__init__("BTTN", control_id)
         self._cfg_columnar.append(
             ButtonConfig(
                 control_id,
                 title,
                 title_position,
                 button_enabled,
+                style,
                 icon_name,
                 on_color,
                 off_color,
                 text,
                 control_position
             )
         )
@@ -163,14 +170,15 @@
         Button
         """
         tmp_cls = cls(
             cfg_dict["controlID"],
             cfg_dict["title"],
             _get_title_position(cfg_dict["titlePosition"]),
             cfg_dict["buttonEnabled"],
+            _get_button_style(cfg_dict.get("style", 'basic')),
             _get_icon(cfg_dict["iconName"]),
             _get_color(cfg_dict["onColor"]),
             _get_color(cfg_dict["offColor"]),
             cfg_dict["text"],
             ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
```

### Comparing `dashio-3.3.3/dashio/iotcontrol/button_group.py` & `dashio-3.3.4/dashio/iotcontrol/button_group.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/chart.py` & `dashio-3.3.4/dashio/iotcontrol/chart.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/color_picker.py` & `dashio-3.3.4/dashio/iotcontrol/color_picker.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/control.py` & `dashio-3.3.4/dashio/iotcontrol/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import json
 import logging
 from ..constants import BAD_CHARS
 from .enums import ColorPickerStyle, DeviceViewStyle, DialNumberPosition, DirectionStyle, ChartXAxisLabelsStyle, Keyboard, KnobStyle, Precision,\
-    TextAlignment, TitlePosition, Icon, Color, TextFormat, LabelStyle, SliderBarStyle, DialStyle, TimeGraphPositionOfKey
+    TextAlignment, TitlePosition, Icon, Color, TextFormat, LabelStyle, SliderBarStyle, DialStyle, TimeGraphPositionOfKey, ButtonStyle
 from .event import Event
 
 
 def _get_icon(icon_str: str) -> Icon:
     icon_name = icon_str.upper().replace(" ", "")
     return Icon[icon_name]
 
@@ -58,17 +58,20 @@
     return Precision(precision_int)
 
 
 def _get_keyboard_type(keyboard_str: str) -> Keyboard:
     t_keyboard = keyboard_str.upper().replace(" ", "")
     return Keyboard[t_keyboard]
 
+def _get_button_style(button_style: str) -> ButtonStyle:
+    btn_style = button_style.upper()
+    return ButtonStyle[btn_style]
 
-def _get_device_view_style(device_vuew_style: str) -> DeviceViewStyle:
-    dvs_name = device_vuew_style.upper().replace(" ", "")
+def _get_device_view_style(device_view_style: str) -> DeviceViewStyle:
+    dvs_name = device_view_style.upper().replace(" ", "")
     return DeviceViewStyle[dvs_name]
 
 
 def _get_color_picker_style(color_picker_style: str) -> ColorPickerStyle:
     cps_name = color_picker_style.upper().replace(" ", "")
     return ColorPickerStyle[cps_name]
 
@@ -138,15 +141,15 @@
         self.x_position_ratio = x_position_ratio
         self.y_position_ratio = y_position_ratio
         self.width_ratio = width_ratio
         self.height_ratio = height_ratio
 
 
 class ControlConfig:
-    """Base COntrolConfig"""
+    """Base ControlConfig"""
     def get_cfg_json(self) -> str:
         """Returns the CFG str for the control called when the iotdashboard app asks for a CFG
 
         Parameters
         ----------
         data : list from IoTDashboard
             The command from IoTDashboard split on \t into a list
@@ -352,14 +355,16 @@
         """
         # Dictionary to store CFG json
         self._cfg_columnar = []
         self._cfg_full_page = []
         self._cfg_full_page_no_columns = 0
         self.cntrl_type = cntrl_type.translate(BAD_CHARS)
         self.control_id = control_id.translate(BAD_CHARS)
+        if not self.control_id:
+            raise ValueError('control_id cannot be an empty string')
         self._message_rx_event = Event()
         self._message_tx_event = Event()
         # This may break things but makes all controls able to be setup from tasks.
         self._message_rx_event += self._message_tx_event
         self._control_hdr_str = f"\t{{device_id}}\t{self.cntrl_type}\t{self.control_id}\t"
 
     def del_configs_columnar(self):
```

### Comparing `dashio-3.3.3/dashio/iotcontrol/device_view.py` & `dashio-3.3.4/dashio/iotcontrol/device_view.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/dial.py` & `dashio-3.3.4/dashio/iotcontrol/dial.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/direction.py` & `dashio-3.3.4/dashio/iotcontrol/direction.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/enums.py` & `dashio-3.3.4/dashio/iotcontrol/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,23 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from enum import Enum
 
 
+class ConnectionState(Enum):
+    """
+    Used Internally for MQTT and DashConntections
+    """
+    CONNECTED = 0
+    CONNECTING = 1
+    DISCONNECTED = 2
+
+
 class ControlName(Enum):
     """
     All the control names
     """
     AVD = "AVD"
     DVVW = "DVVW"
     MENU = "MENU"
@@ -130,14 +139,20 @@
     PLOP = "Plop"
     PLOPPLIPPLIP = "Plop Plip Plip"
     SWITCH = "Switch"
     WHOOSH = "Whoosh"
     BOING = "Boing"
 
 
+class ButtonStyle(Enum):
+    """Button Styles"""
+    BASIC = "basic"
+    HIGHLIGHT = "highlight"
+
+
 class DeviceViewStyle(Enum):
     """DeciveView Styles"""
     BASIC = "BASIC"
     BORDERS = "BORDERS"
 
 
 class ColorPickerStyle(Enum):
```

### Comparing `dashio-3.3.3/dashio/iotcontrol/event.py` & `dashio-3.3.4/dashio/iotcontrol/event.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/event_log.py` & `dashio-3.3.4/dashio/iotcontrol/event_log.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/knob.py` & `dashio-3.3.4/dashio/iotcontrol/knob.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/label.py` & `dashio-3.3.4/dashio/iotcontrol/label.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/map.py` & `dashio-3.3.4/dashio/iotcontrol/map.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/menu.py` & `dashio-3.3.4/dashio/iotcontrol/menu.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/ring_buffer.py` & `dashio-3.3.4/dashio/iotcontrol/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/selector.py` & `dashio-3.3.4/dashio/iotcontrol/selector.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/slider.py` & `dashio-3.3.4/dashio/iotcontrol/slider.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/textbox.py` & `dashio-3.3.4/dashio/iotcontrol/textbox.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/iotcontrol/time_graph.py` & `dashio-3.3.4/dashio/iotcontrol/time_graph.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/ip.py` & `dashio-3.3.4/dashio/ip.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/load_config.py` & `dashio-3.3.4/dashio/load_config.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/mqttconnection.py` & `dashio-3.3.4/dashio/mqttconnection.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,37 +29,36 @@
 
 import paho.mqtt.client as mqtt
 import shortuuid
 import zmq
 
 from .constants import CONNECTION_PUB_URL
 
+from .iotcontrol.enums import ConnectionState
 
 class MQTTConnection(threading.Thread):
     """Setups and manages a connection thread to the MQTT Server."""
 
     def _on_connect(self, client, userdata, flags, msg):
         if msg == 0:
-            self._connected = True
-            self._disconnected = False
+            self._connection_state = ConnectionState.CONNECTED
             for device_id in self._device_id_list:
                 control_topic = f"{self.username}/{device_id}/control"
                 self.mqttc.subscribe(control_topic, 0)
             for device_id in self._device_id_rx_list:
                 data_topic = f"{self.username}/{device_id}/data"
                 self.mqttc.subscribe(data_topic, 0)
             self._send_dash_announce()
             logging.debug("connected OK")
         else:
             logging.debug("Bad connection Returned code=%s", msg)
 
     def _on_disconnect(self, client, userdata, msg):
         logging.debug("disconnecting reason  %s", msg)
-        self._connected = False
-        self._disconnected = True
+        self._connection_state = ConnectionState.DISCONNECTED
 
     def _on_message(self, client, obj, msg):
         data = str(msg.payload, "utf-8").strip()
         logging.debug("MQTT RX:\n%s", data)
         self.tx_zmq_pub.send_multipart([msg.payload, self.b_connection_id])
 
     def _on_subscribe(self, client, obj, mid, granted_qos):
@@ -75,15 +74,15 @@
         ----------
             device (Device):
                 The Device to add.
         """
         if device.device_id not in self._device_id_list:
             self._device_id_list.append(device.device_id)
             device.register_connection(self)
-            if self._connected:
+            if self._connection_state == ConnectionState.CONNECTED:
                 control_topic = f"{self.username}/{device.device_id}/control"
                 self.mqttc.subscribe(control_topic, 0)
                 self._send_dash_announce()
 
     def _add_device_rx(self, msg_dict):
         """Connect to another device"""
         device_id = msg_dict["deviceID"]
@@ -135,27 +134,24 @@
         """
 
         threading.Thread.__init__(self, daemon=True)
 
         self.context = context or zmq.Context.instance()
         self.zmq_connection_uuid = "MQTT:" + shortuuid.uuid()
         self.b_connection_id = self.zmq_connection_uuid.encode('utf-8')
-
-        self._connected = False
-        self._disconnected = True
+        self._connection_state = ConnectionState.DISCONNECTED
         self.connection_topic_list = []
         self._device_id_list = []
         self._device_id_rx_list = []
         self.host = host
         self.port = port
         # self.last_will = "OFFLINE"
         self.running = True
         self.username = username
         self.mqttc = mqtt.Client()
-        self.disconnect_timeout = 15.0
         # Assign event callbacks
         self.mqttc.on_message = self._on_message
         self.mqttc.on_connect = self._on_connect
         self.mqttc.on_disconnect = self._on_disconnect
         self.mqttc.on_subscribe = self._on_subscribe
 
         if use_ssl:
@@ -172,18 +168,19 @@
         self.mqttc.on_log = self._on_log
         # self.mqttc.will_set(self.data_topic, self.last_will, qos=1, retain=False)
         # Connect
         if username and password:
             self.mqttc.username_pw_set(username, password)
         try:
             self.mqttc.connect(self.host, self.port)
+            self._connection_state = ConnectionState.CONNECTING
         except mqtt.socket.gaierror as error:
             logging.debug("No connection to internet: %s", str(error))
         # Start subscribe, with QoS level 0
-        self.disconnect_timeout = 15.0
+        self._disconnect_timeout = 1.0
         self.start()
 
     def _mqtt_command(self, msg_dict: dict):
         logging.debug("MQTT CMD: %s", msg_dict)
         if msg_dict['msgType'] == 'connect':
             self._add_device_rx(msg_dict)
         if msg_dict['msgType'] == 'disconnect':
@@ -227,22 +224,23 @@
                     continue
                 msg_l = data.split(b'\t')
                 try:
                     device_id = msg_l[1].decode().strip()
                 except IndexError:
                     continue
                 data_topic = f"{self.username}/{device_id}/data"
-                if self._connected:
+                if self._connection_state == ConnectionState.CONNECTED:
                     logging.debug("MQTT TX:\n%s", data.decode().rstrip())
                     self.mqttc.publish(data_topic, data.decode())
-            if self._disconnected:
-                self.disconnect_timeout = min(self.disconnect_timeout, 900)
-                time.sleep(self.disconnect_timeout)
+            if self._connection_state == ConnectionState.DISCONNECTED:
+                self._disconnect_timeout = min(self._disconnect_timeout, 900)
+                time.sleep(self._disconnect_timeout)
                 try:
                     self.mqttc.connect(self.host, self.port)
+                    self._connection_state = ConnectionState.CONNECTING
                 except mqtt.socket.gaierror as error:
                     logging.debug("No connection to internet: %s", str(error))
-                self.disconnect_timeout = self.disconnect_timeout * 2
+                self._disconnect_timeout = self._disconnect_timeout * 2
 
         self.mqttc.loop_stop()
         self.tx_zmq_pub.close()
         self.rx_zmq_sub.close()
```

### Comparing `dashio-3.3.3/dashio/serialconnection.py` & `dashio-3.3.4/dashio/serialconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/tcpconnection.py` & `dashio-3.3.4/dashio/tcpconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/zeroconf_service.py` & `dashio-3.3.4/dashio/zeroconf_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio/zmqconnection.py` & `dashio-3.3.4/dashio/zmqconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/dashio.egg-info/PKG-INFO` & `dashio-3.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,12 @@
-Metadata-Version: 2.1
-Name: dashio
-Version: 3.3.3
-Summary: DashIO interface library
-Home-page: https://dashio.io
-Download-URL: https://github.com/dashio-connect/python-dashio
-Author: James Boulton
-Author-email: james@dashio.com
-License: MIT
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Operating System :: OS Independent
-Requires-Python: >3.6.0
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
-# DashIO
+# python-dashio
 
 ![Tests](https://github.com/dashio-connect/python-dashio/actions/workflows/tests.yml/badge.svg)
 
-[**DashIO**](http://dashio.io) - It is a quick effortless way to connect your IoT device to your phone, tablet or iPad using the free **Dash** app. It allows easy setup of controls such as Dials, Text Boxes, Charts, Graphs, Notifications..., from your IoT device. You can define the look and layout of the controls on your phone from your IoT device. There are three methods to connect to your phone; Bluetooth Low Energy (BLE), TCP or MQTT.
+[**python-dashio**](http://www.dashio.io) - It is a quick effortless way to connect your IoT device to your phone, tablet or iPad using the free **Dash** app. It allows easy setup of controls such as Dials, Text Boxes, Charts, Graphs, Notifications..., from your IoT device. You can define the look and layout of the controls on your phone from your IoT device. There are three methods to connect to your phone; Bluetooth Low Energy (BLE), TCP or MQTT.
 
 ## Getting Started
 
 For the big picture on **DashIO**, take a look at our website: <a href="https://dashio.io">dashio.io</a>
 
 ## Documentation
```

### Comparing `dashio-3.3.3/dashio.egg-info/SOURCES.txt` & `dashio-3.3.4/dashio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/setup.cfg` & `dashio-3.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/setup.py` & `dashio-3.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="dashio",
-    version="3.3.3",
+    version="3.3.4",
     description="DashIO interface library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="James Boulton",
     author_email="james@dashio.com",
     url="https://dashio.io",
     download_url="https://github.com/dashio-connect/python-dashio",
```

### Comparing `dashio-3.3.3/tests/test_button.py` & `dashio-3.3.4/tests/test_button.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/tests/test_button_group.py` & `dashio-3.3.4/tests/test_button_group.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/tests/test_chart.py` & `dashio-3.3.4/tests/test_chart.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/tests/test_dashdevice.py` & `dashio-3.3.4/tests/test_dashdevice.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/tests/test_device_view.py` & `dashio-3.3.4/tests/test_device_view.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/tests/test_dial.py` & `dashio-3.3.4/tests/test_dial.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/tests/test_direction.py` & `dashio-3.3.4/tests/test_direction.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/tests/test_event_log.py` & `dashio-3.3.4/tests/test_event_log.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/tests/test_knob.py` & `dashio-3.3.4/tests/test_knob.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/tests/test_label.py` & `dashio-3.3.4/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/tests/test_map.py` & `dashio-3.3.4/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/tests/test_menu.py` & `dashio-3.3.4/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/tests/test_selector.py` & `dashio-3.3.4/tests/test_selector.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/tests/test_slider.py` & `dashio-3.3.4/tests/test_slider.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/tests/test_textbox.py` & `dashio-3.3.4/tests/test_textbox.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.3/tests/test_time_graph.py` & `dashio-3.3.4/tests/test_time_graph.py`

 * *Files identical despite different names*

