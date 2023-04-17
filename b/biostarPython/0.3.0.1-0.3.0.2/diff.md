# Comparing `tmp/biostarPython-0.3.0.1.tar.gz` & `tmp/biostarPython-0.3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biostarPython-0.3.0.1.tar", last modified: Mon Feb  6 19:00:56 2023, max compression
+gzip compressed data, was "biostarPython-0.3.0.2.tar", last modified: Mon Apr 17 11:06:28 2023, max compression
```

## Comparing `biostarPython-0.3.0.1.tar` & `biostarPython-0.3.0.2.tar`

### file list

```diff
@@ -1,147 +1,148 @@
-drwxrwxrwx   0        0        0        0 2023-02-06 19:00:56.038229 biostarPython-0.3.0.1/
--rw-rw-rw-   0        0        0     1083 2022-03-24 17:21:59.000000 biostarPython-0.3.0.1/LICENSE
--rw-rw-rw-   0        0        0       27 2022-03-24 17:21:59.000000 biostarPython-0.3.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4767 2023-02-06 19:00:56.038229 biostarPython-0.3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4272 2023-02-06 18:50:37.000000 biostarPython-0.3.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-06 19:00:55.814873 biostarPython-0.3.0.1/biostarPython/
--rw-rw-rw-   0        0        0    78848 2023-02-06 18:56:54.000000 biostarPython-0.3.0.1/biostarPython/__init__.py
--rw-rw-rw-   0        0        0    60024 2022-03-24 17:21:59.000000 biostarPython-0.3.0.1/biostarPython/event_code.json
-drwxrwxrwx   0        0        0        0 2023-02-06 19:00:55.878657 biostarPython-0.3.0.1/biostarPython/proto/
--rw-rw-rw-   0        0        0     5509 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/access.proto
--rw-rw-rw-   0        0        0     3920 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/action.proto
--rw-rw-rw-   0        0        0      369 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/admin.proto
--rw-rw-rw-   0        0        0     2147 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/apb_zone.proto
--rw-rw-rw-   0        0        0     3899 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/auth.proto
--rw-rw-rw-   0        0        0     7636 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/card.proto
--rw-rw-rw-   0        0        0     1313 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/cert.proto
--rw-rw-rw-   0        0        0     5879 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/connect.proto
--rw-rw-rw-   0        0        0     6542 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/connect_master.proto
--rw-rw-rw-   0        0        0    10458 2023-02-06 11:17:19.000000 biostarPython-0.3.0.1/biostarPython/proto/device.proto
--rw-rw-rw-   0        0        0     4633 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/display.proto
--rw-rw-rw-   0        0        0     3535 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/door.proto
--rw-rw-rw-   0        0        0      467 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/err.proto
--rw-rw-rw-   0        0        0     4876 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/event.proto
--rw-rw-rw-   0        0        0     6366 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/face.proto
--rw-rw-rw-   0        0        0     2999 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/finger.proto
--rw-rw-rw-   0        0        0     1711 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/fire_zone.proto
--rw-rw-rw-   0        0        0     2879 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/gateway.proto
--rw-rw-rw-   0        0        0     1575 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/input.proto
--rw-rw-rw-   0        0        0     1912 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/interlock_zone.proto
--rw-rw-rw-   0        0        0     2557 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/intrusion_zone.proto
--rw-rw-rw-   0        0        0     3361 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/lift.proto
--rw-rw-rw-   0        0        0     1751 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/lift_zone.proto
--rw-rw-rw-   0        0        0     1701 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/lock_zone.proto
--rw-rw-rw-   0        0        0      702 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/login.proto
--rw-rw-rw-   0        0        0     1620 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/master.proto
--rw-rw-rw-   0        0        0     2669 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/network.proto
--rw-rw-rw-   0        0        0     1701 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/operator.proto
--rw-rw-rw-   0        0        0     2146 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/rs485.proto
--rw-rw-rw-   0        0        0      999 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/rtsp.proto
--rw-rw-rw-   0        0        0     4265 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/schedule.proto
--rw-rw-rw-   0        0        0     2541 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/server.proto
--rw-rw-rw-   0        0        0     1759 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/status.proto
--rw-rw-rw-   0        0        0     1881 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/system.proto
--rw-rw-rw-   0        0        0     2914 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/tenant.proto
--rw-rw-rw-   0        0        0     2492 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/thermal.proto
--rw-rw-rw-   0        0        0     3178 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/time.proto
--rw-rw-rw-   0        0        0     2083 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/timed_apb_zone.proto
--rw-rw-rw-   0        0        0     2652 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/tna.proto
--rw-rw-rw-   0        0        0     7870 2022-12-08 09:59:04.000000 biostarPython-0.3.0.1/biostarPython/proto/user.proto
--rw-rw-rw-   0        0        0     1417 2023-02-06 11:17:19.000000 biostarPython-0.3.0.1/biostarPython/proto/voip.proto
--rw-rw-rw-   0        0        0     2873 2022-12-08 09:59:05.000000 biostarPython-0.3.0.1/biostarPython/proto/wiegand.proto
--rw-rw-rw-   0        0        0      655 2022-12-08 09:59:05.000000 biostarPython-0.3.0.1/biostarPython/proto/zone.proto
-drwxrwxrwx   0        0        0        0 2023-02-06 19:00:56.037217 biostarPython-0.3.0.1/biostarPython/service/
--rw-rw-rw-   0        0        0    12356 2023-02-06 12:17:26.000000 biostarPython-0.3.0.1/biostarPython/service/access_pb2.py
--rw-rw-rw-   0        0        0    33559 2023-02-06 12:17:56.000000 biostarPython-0.3.0.1/biostarPython/service/access_pb2_grpc.py
--rw-rw-rw-   0        0        0     8837 2023-02-06 12:18:06.000000 biostarPython-0.3.0.1/biostarPython/service/action_pb2.py
--rw-rw-rw-   0        0        0     5567 2023-02-06 12:18:12.000000 biostarPython-0.3.0.1/biostarPython/service/action_pb2_grpc.py
--rw-rw-rw-   0        0        0     1444 2023-02-06 11:47:28.000000 biostarPython-0.3.0.1/biostarPython/service/admin_pb2.py
--rw-rw-rw-   0        0        0     2385 2023-02-06 12:18:30.000000 biostarPython-0.3.0.1/biostarPython/service/admin_pb2_grpc.py
--rw-rw-rw-   0        0        0     5469 2023-02-06 12:19:16.000000 biostarPython-0.3.0.1/biostarPython/service/apb_zone_pb2.py
--rw-rw-rw-   0        0        0    12846 2023-02-06 12:19:23.000000 biostarPython-0.3.0.1/biostarPython/service/apb_zone_pb2_grpc.py
--rw-rw-rw-   0        0        0     7147 2023-02-06 12:19:32.000000 biostarPython-0.3.0.1/biostarPython/service/auth_pb2.py
--rw-rw-rw-   0        0        0     5414 2023-02-06 12:19:37.000000 biostarPython-0.3.0.1/biostarPython/service/auth_pb2_grpc.py
--rw-rw-rw-   0        0        0    16712 2023-02-06 12:19:55.000000 biostarPython-0.3.0.1/biostarPython/service/card_pb2.py
--rw-rw-rw-   0        0        0    31385 2023-02-06 12:20:01.000000 biostarPython-0.3.0.1/biostarPython/service/card_pb2_grpc.py
--rw-rw-rw-   0        0        0     3070 2023-02-06 11:47:28.000000 biostarPython-0.3.0.1/biostarPython/service/cert_pb2.py
--rw-rw-rw-   0        0        0     5802 2023-02-06 12:21:25.000000 biostarPython-0.3.0.1/biostarPython/service/cert_pb2_grpc.py
--rw-rw-rw-   0        0        0    14626 2023-02-06 12:21:38.000000 biostarPython-0.3.0.1/biostarPython/service/connect_master_pb2.py
--rw-rw-rw-   0        0        0    45962 2023-02-06 12:21:55.000000 biostarPython-0.3.0.1/biostarPython/service/connect_master_pb2_grpc.py
--rw-rw-rw-   0        0        0    12845 2023-02-06 12:23:00.000000 biostarPython-0.3.0.1/biostarPython/service/connect_pb2.py
--rw-rw-rw-   0        0        0    30822 2023-02-06 12:23:07.000000 biostarPython-0.3.0.1/biostarPython/service/connect_pb2_grpc.py
--rw-rw-rw-   0        0        0    19124 2023-02-06 12:23:18.000000 biostarPython-0.3.0.1/biostarPython/service/device_pb2.py
--rw-rw-rw-   0        0        0    31489 2023-02-06 12:23:25.000000 biostarPython-0.3.0.1/biostarPython/service/device_pb2_grpc.py
--rw-rw-rw-   0        0        0    10192 2023-02-06 12:23:41.000000 biostarPython-0.3.0.1/biostarPython/service/display_pb2.py
--rw-rw-rw-   0        0        0    21817 2023-02-06 12:24:17.000000 biostarPython-0.3.0.1/biostarPython/service/display_pb2_grpc.py
--rw-rw-rw-   0        0        0     7898 2023-02-06 12:24:39.000000 biostarPython-0.3.0.1/biostarPython/service/door_pb2.py
--rw-rw-rw-   0        0        0    13931 2023-02-06 12:25:03.000000 biostarPython-0.3.0.1/biostarPython/service/door_pb2_grpc.py
--rw-rw-rw-   0        0        0     1682 2023-02-06 11:47:28.000000 biostarPython-0.3.0.1/biostarPython/service/err_pb2.py
--rw-rw-rw-   0        0        0      863 2023-02-06 11:47:28.000000 biostarPython-0.3.0.1/biostarPython/service/err_pb2_grpc.py
--rw-rw-rw-   0        0        0    10235 2023-02-06 12:25:29.000000 biostarPython-0.3.0.1/biostarPython/service/event_pb2.py
--rw-rw-rw-   0        0        0    21250 2023-02-06 12:25:35.000000 biostarPython-0.3.0.1/biostarPython/service/event_pb2_grpc.py
--rw-rw-rw-   0        0        0    13004 2023-02-06 12:25:46.000000 biostarPython-0.3.0.1/biostarPython/service/face_pb2.py
--rw-rw-rw-   0        0        0    20741 2023-02-06 12:25:51.000000 biostarPython-0.3.0.1/biostarPython/service/face_pb2_grpc.py
--rw-rw-rw-   0        0        0     6996 2023-02-06 12:25:58.000000 biostarPython-0.3.0.1/biostarPython/service/finger_pb2.py
--rw-rw-rw-   0        0        0     9867 2023-02-06 12:26:06.000000 biostarPython-0.3.0.1/biostarPython/service/finger_pb2_grpc.py
--rw-rw-rw-   0        0        0     4475 2023-02-06 12:26:36.000000 biostarPython-0.3.0.1/biostarPython/service/fire_zone_pb2.py
--rw-rw-rw-   0        0        0    10020 2023-02-06 12:26:43.000000 biostarPython-0.3.0.1/biostarPython/service/fire_zone_pb2_grpc.py
--rw-rw-rw-   0        0        0     6559 2023-02-06 12:26:49.000000 biostarPython-0.3.0.1/biostarPython/service/gateway_pb2.py
--rw-rw-rw-   0        0        0    16652 2023-02-06 12:26:54.000000 biostarPython-0.3.0.1/biostarPython/service/gateway_pb2_grpc.py
--rw-rw-rw-   0        0        0     4047 2023-02-06 12:27:00.000000 biostarPython-0.3.0.1/biostarPython/service/input_pb2.py
--rw-rw-rw-   0        0        0     5452 2023-02-06 12:27:06.000000 biostarPython-0.3.0.1/biostarPython/service/input_pb2_grpc.py
--rw-rw-rw-   0        0        0     4971 2023-02-06 12:27:31.000000 biostarPython-0.3.0.1/biostarPython/service/interlock_zone_pb2.py
--rw-rw-rw-   0        0        0    10275 2023-02-06 12:27:52.000000 biostarPython-0.3.0.1/biostarPython/service/interlock_zone_pb2_grpc.py
--rw-rw-rw-   0        0        0     6228 2023-02-06 12:28:04.000000 biostarPython-0.3.0.1/biostarPython/service/intrusion_zone_pb2.py
--rw-rw-rw-   0        0        0    11913 2023-02-06 12:28:10.000000 biostarPython-0.3.0.1/biostarPython/service/intrusion_zone_pb2_grpc.py
--rw-rw-rw-   0        0        0     7728 2023-02-06 12:28:18.000000 biostarPython-0.3.0.1/biostarPython/service/lift_pb2.py
--rw-rw-rw-   0        0        0    14035 2023-02-06 12:28:28.000000 biostarPython-0.3.0.1/biostarPython/service/lift_pb2_grpc.py
--rw-rw-rw-   0        0        0     4410 2023-02-06 12:29:00.000000 biostarPython-0.3.0.1/biostarPython/service/lift_zone_pb2.py
--rw-rw-rw-   0        0        0     9935 2023-02-06 12:29:06.000000 biostarPython-0.3.0.1/biostarPython/service/lift_zone_pb2_grpc.py
--rw-rw-rw-   0        0        0     4262 2023-02-06 12:29:19.000000 biostarPython-0.3.0.1/biostarPython/service/lock_zone_pb2.py
--rw-rw-rw-   0        0        0     9935 2023-02-06 12:29:25.000000 biostarPython-0.3.0.1/biostarPython/service/lock_zone_pb2_grpc.py
--rw-rw-rw-   0        0        0     2146 2023-02-06 11:47:29.000000 biostarPython-0.3.0.1/biostarPython/service/login_pb2.py
--rw-rw-rw-   0        0        0     5309 2023-02-06 12:29:40.000000 biostarPython-0.3.0.1/biostarPython/service/login_pb2_grpc.py
--rw-rw-rw-   0        0        0     4199 2023-02-06 12:29:56.000000 biostarPython-0.3.0.1/biostarPython/service/master_pb2.py
--rw-rw-rw-   0        0        0     8744 2023-02-06 13:00:42.000000 biostarPython-0.3.0.1/biostarPython/service/master_pb2_grpc.py
--rw-rw-rw-   0        0        0     6294 2023-02-06 13:00:55.000000 biostarPython-0.3.0.1/biostarPython/service/network_pb2.py
--rw-rw-rw-   0        0        0    10351 2023-02-06 13:01:06.000000 biostarPython-0.3.0.1/biostarPython/service/network_pb2_grpc.py
--rw-rw-rw-   0        0        0     4298 2023-02-06 13:01:14.000000 biostarPython-0.3.0.1/biostarPython/service/operator_pb2.py
--rw-rw-rw-   0        0        0    11508 2023-02-06 13:01:20.000000 biostarPython-0.3.0.1/biostarPython/service/operator_pb2_grpc.py
--rw-rw-rw-   0        0        0     5400 2023-02-06 13:02:38.000000 biostarPython-0.3.0.1/biostarPython/service/rs485_pb2.py
--rw-rw-rw-   0        0        0     9955 2023-02-06 13:02:44.000000 biostarPython-0.3.0.1/biostarPython/service/rs485_pb2_grpc.py
--rw-rw-rw-   0        0        0     2774 2023-02-06 13:02:52.000000 biostarPython-0.3.0.1/biostarPython/service/rtsp_pb2.py
--rw-rw-rw-   0        0        0     5414 2023-02-06 13:03:01.000000 biostarPython-0.3.0.1/biostarPython/service/rtsp_pb2_grpc.py
--rw-rw-rw-   0        0        0     9817 2023-02-06 13:05:03.000000 biostarPython-0.3.0.1/biostarPython/service/schedule_pb2.py
--rw-rw-rw-   0        0        0    22706 2023-02-06 13:05:09.000000 biostarPython-0.3.0.1/biostarPython/service/schedule_pb2_grpc.py
--rw-rw-rw-   0        0        0     6292 2023-02-06 13:05:18.000000 biostarPython-0.3.0.1/biostarPython/service/server_pb2.py
--rw-rw-rw-   0        0        0    10209 2023-02-06 13:05:28.000000 biostarPython-0.3.0.1/biostarPython/service/server_pb2_grpc.py
--rw-rw-rw-   0        0        0     4278 2023-02-06 13:05:36.000000 biostarPython-0.3.0.1/biostarPython/service/status_pb2.py
--rw-rw-rw-   0        0        0     5490 2023-02-06 13:05:42.000000 biostarPython-0.3.0.1/biostarPython/service/status_pb2_grpc.py
--rw-rw-rw-   0        0        0     4022 2023-02-06 13:05:47.000000 biostarPython-0.3.0.1/biostarPython/service/system_pb2.py
--rw-rw-rw-   0        0        0     5490 2023-02-06 13:05:53.000000 biostarPython-0.3.0.1/biostarPython/service/system_pb2_grpc.py
--rw-rw-rw-   0        0        0     6702 2023-02-06 13:06:24.000000 biostarPython-0.3.0.1/biostarPython/service/tenant_pb2.py
--rw-rw-rw-   0        0        0    18059 2023-02-06 13:06:29.000000 biostarPython-0.3.0.1/biostarPython/service/tenant_pb2_grpc.py
--rw-rw-rw-   0        0        0     5743 2023-02-06 13:06:35.000000 biostarPython-0.3.0.1/biostarPython/service/thermal_pb2.py
--rw-rw-rw-   0        0        0     7140 2023-02-06 13:06:40.000000 biostarPython-0.3.0.1/biostarPython/service/thermal_pb2_grpc.py
--rw-rw-rw-   0        0        0     7426 2023-02-06 13:06:47.000000 biostarPython-0.3.0.1/biostarPython/service/time_pb2.py
--rw-rw-rw-   0        0        0    14295 2023-02-06 13:06:53.000000 biostarPython-0.3.0.1/biostarPython/service/time_pb2_grpc.py
--rw-rw-rw-   0        0        0     5385 2023-02-06 13:07:01.000000 biostarPython-0.3.0.1/biostarPython/service/timed_apb_zone_pb2.py
--rw-rw-rw-   0        0        0    13402 2023-02-06 13:07:05.000000 biostarPython-0.3.0.1/biostarPython/service/timed_apb_zone_pb2_grpc.py
--rw-rw-rw-   0        0        0     6041 2023-02-06 13:07:11.000000 biostarPython-0.3.0.1/biostarPython/service/tna_pb2.py
--rw-rw-rw-   0        0        0     8364 2023-02-06 13:07:17.000000 biostarPython-0.3.0.1/biostarPython/service/tna_pb2_grpc.py
--rw-rw-rw-   0        0        0    16453 2023-02-06 13:07:31.000000 biostarPython-0.3.0.1/biostarPython/service/user_pb2.py
--rw-rw-rw-   0        0        0    39790 2023-02-06 13:07:38.000000 biostarPython-0.3.0.1/biostarPython/service/user_pb2_grpc.py
--rw-rw-rw-   0        0        0     3440 2023-02-06 13:07:47.000000 biostarPython-0.3.0.1/biostarPython/service/voip_pb2.py
--rw-rw-rw-   0        0        0     5414 2023-02-06 13:07:52.000000 biostarPython-0.3.0.1/biostarPython/service/voip_pb2_grpc.py
--rw-rw-rw-   0        0        0     6784 2023-02-06 13:08:01.000000 biostarPython-0.3.0.1/biostarPython/service/wiegand_pb2.py
--rw-rw-rw-   0        0        0    10091 2023-02-06 13:08:06.000000 biostarPython-0.3.0.1/biostarPython/service/wiegand_pb2_grpc.py
--rw-rw-rw-   0        0        0     1896 2023-02-06 11:47:29.000000 biostarPython-0.3.0.1/biostarPython/service/zone_pb2.py
--rw-rw-rw-   0        0        0      159 2023-02-06 11:47:29.000000 biostarPython-0.3.0.1/biostarPython/service/zone_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-02-06 19:00:55.820872 biostarPython-0.3.0.1/biostarPython.egg-info/
--rw-rw-rw-   0        0        0     4767 2023-02-06 19:00:55.000000 biostarPython-0.3.0.1/biostarPython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5068 2023-02-06 19:00:55.000000 biostarPython-0.3.0.1/biostarPython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-06 19:00:55.000000 biostarPython-0.3.0.1/biostarPython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-02-06 19:00:55.000000 biostarPython-0.3.0.1/biostarPython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-02-06 19:00:55.000000 biostarPython-0.3.0.1/biostarPython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-06 19:00:56.039234 biostarPython-0.3.0.1/setup.cfg
--rw-rw-rw-   0        0        0      999 2023-02-06 18:56:57.000000 biostarPython-0.3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:06:28.036917 biostarPython-0.3.0.2/
+-rw-rw-rw-   0        0        0     1083 2022-03-24 17:21:59.000000 biostarPython-0.3.0.2/LICENSE
+-rw-rw-rw-   0        0        0       27 2022-03-24 17:21:59.000000 biostarPython-0.3.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4904 2023-04-17 11:06:28.035896 biostarPython-0.3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4409 2023-04-17 11:05:20.000000 biostarPython-0.3.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 11:06:27.904577 biostarPython-0.3.0.2/biostarPython/
+-rw-rw-rw-   0        0        0     1121 2023-03-20 13:04:17.000000 biostarPython-0.3.0.2/biostarPython/Log Events.py
+-rw-rw-rw-   0        0        0    79274 2023-04-17 11:04:47.000000 biostarPython-0.3.0.2/biostarPython/__init__.py
+-rw-rw-rw-   0        0        0    60024 2022-03-24 17:21:59.000000 biostarPython-0.3.0.2/biostarPython/event_code.json
+drwxrwxrwx   0        0        0        0 2023-04-17 11:06:27.949116 biostarPython-0.3.0.2/biostarPython/proto/
+-rw-rw-rw-   0        0        0     5509 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/access.proto
+-rw-rw-rw-   0        0        0     3920 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/action.proto
+-rw-rw-rw-   0        0        0      369 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/admin.proto
+-rw-rw-rw-   0        0        0     2147 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/apb_zone.proto
+-rw-rw-rw-   0        0        0     3899 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/auth.proto
+-rw-rw-rw-   0        0        0     7636 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/card.proto
+-rw-rw-rw-   0        0        0     1313 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/cert.proto
+-rw-rw-rw-   0        0        0     5879 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/connect.proto
+-rw-rw-rw-   0        0        0     6542 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/connect_master.proto
+-rw-rw-rw-   0        0        0    10458 2023-02-06 11:17:19.000000 biostarPython-0.3.0.2/biostarPython/proto/device.proto
+-rw-rw-rw-   0        0        0     4633 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/display.proto
+-rw-rw-rw-   0        0        0     3535 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/door.proto
+-rw-rw-rw-   0        0        0      467 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/err.proto
+-rw-rw-rw-   0        0        0     4876 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/event.proto
+-rw-rw-rw-   0        0        0     6366 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/face.proto
+-rw-rw-rw-   0        0        0     2999 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/finger.proto
+-rw-rw-rw-   0        0        0     1711 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/fire_zone.proto
+-rw-rw-rw-   0        0        0     2879 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/gateway.proto
+-rw-rw-rw-   0        0        0     1575 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/input.proto
+-rw-rw-rw-   0        0        0     1912 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/interlock_zone.proto
+-rw-rw-rw-   0        0        0     2557 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/intrusion_zone.proto
+-rw-rw-rw-   0        0        0     3361 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/lift.proto
+-rw-rw-rw-   0        0        0     1751 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/lift_zone.proto
+-rw-rw-rw-   0        0        0     1701 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/lock_zone.proto
+-rw-rw-rw-   0        0        0      702 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/login.proto
+-rw-rw-rw-   0        0        0     1620 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/master.proto
+-rw-rw-rw-   0        0        0     2669 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/network.proto
+-rw-rw-rw-   0        0        0     1701 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/operator.proto
+-rw-rw-rw-   0        0        0     2146 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/rs485.proto
+-rw-rw-rw-   0        0        0      999 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/rtsp.proto
+-rw-rw-rw-   0        0        0     4265 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/schedule.proto
+-rw-rw-rw-   0        0        0     2541 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/server.proto
+-rw-rw-rw-   0        0        0     1759 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/status.proto
+-rw-rw-rw-   0        0        0     1881 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/system.proto
+-rw-rw-rw-   0        0        0     2914 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/tenant.proto
+-rw-rw-rw-   0        0        0     2492 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/thermal.proto
+-rw-rw-rw-   0        0        0     3178 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/time.proto
+-rw-rw-rw-   0        0        0     2083 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/timed_apb_zone.proto
+-rw-rw-rw-   0        0        0     2652 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/tna.proto
+-rw-rw-rw-   0        0        0     7870 2022-12-08 09:59:04.000000 biostarPython-0.3.0.2/biostarPython/proto/user.proto
+-rw-rw-rw-   0        0        0     1417 2023-02-06 11:17:19.000000 biostarPython-0.3.0.2/biostarPython/proto/voip.proto
+-rw-rw-rw-   0        0        0     2873 2022-12-08 09:59:05.000000 biostarPython-0.3.0.2/biostarPython/proto/wiegand.proto
+-rw-rw-rw-   0        0        0      655 2022-12-08 09:59:05.000000 biostarPython-0.3.0.2/biostarPython/proto/zone.proto
+drwxrwxrwx   0        0        0        0 2023-04-17 11:06:28.035896 biostarPython-0.3.0.2/biostarPython/service/
+-rw-rw-rw-   0        0        0    12356 2023-02-06 12:17:26.000000 biostarPython-0.3.0.2/biostarPython/service/access_pb2.py
+-rw-rw-rw-   0        0        0    33559 2023-02-06 12:17:56.000000 biostarPython-0.3.0.2/biostarPython/service/access_pb2_grpc.py
+-rw-rw-rw-   0        0        0     8837 2023-02-06 12:18:06.000000 biostarPython-0.3.0.2/biostarPython/service/action_pb2.py
+-rw-rw-rw-   0        0        0     5567 2023-02-06 12:18:12.000000 biostarPython-0.3.0.2/biostarPython/service/action_pb2_grpc.py
+-rw-rw-rw-   0        0        0     1444 2023-02-06 11:47:28.000000 biostarPython-0.3.0.2/biostarPython/service/admin_pb2.py
+-rw-rw-rw-   0        0        0     2385 2023-02-06 12:18:30.000000 biostarPython-0.3.0.2/biostarPython/service/admin_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5469 2023-02-06 12:19:16.000000 biostarPython-0.3.0.2/biostarPython/service/apb_zone_pb2.py
+-rw-rw-rw-   0        0        0    12846 2023-02-06 12:19:23.000000 biostarPython-0.3.0.2/biostarPython/service/apb_zone_pb2_grpc.py
+-rw-rw-rw-   0        0        0     7147 2023-02-06 12:19:32.000000 biostarPython-0.3.0.2/biostarPython/service/auth_pb2.py
+-rw-rw-rw-   0        0        0     5414 2023-02-06 12:19:37.000000 biostarPython-0.3.0.2/biostarPython/service/auth_pb2_grpc.py
+-rw-rw-rw-   0        0        0    16712 2023-02-06 12:19:55.000000 biostarPython-0.3.0.2/biostarPython/service/card_pb2.py
+-rw-rw-rw-   0        0        0    31385 2023-02-06 12:20:01.000000 biostarPython-0.3.0.2/biostarPython/service/card_pb2_grpc.py
+-rw-rw-rw-   0        0        0     3070 2023-02-06 11:47:28.000000 biostarPython-0.3.0.2/biostarPython/service/cert_pb2.py
+-rw-rw-rw-   0        0        0     5802 2023-02-06 12:21:25.000000 biostarPython-0.3.0.2/biostarPython/service/cert_pb2_grpc.py
+-rw-rw-rw-   0        0        0    14626 2023-02-06 12:21:38.000000 biostarPython-0.3.0.2/biostarPython/service/connect_master_pb2.py
+-rw-rw-rw-   0        0        0    45962 2023-02-06 12:21:55.000000 biostarPython-0.3.0.2/biostarPython/service/connect_master_pb2_grpc.py
+-rw-rw-rw-   0        0        0    12845 2023-02-06 12:23:00.000000 biostarPython-0.3.0.2/biostarPython/service/connect_pb2.py
+-rw-rw-rw-   0        0        0    30822 2023-02-06 12:23:07.000000 biostarPython-0.3.0.2/biostarPython/service/connect_pb2_grpc.py
+-rw-rw-rw-   0        0        0    19124 2023-02-06 12:23:18.000000 biostarPython-0.3.0.2/biostarPython/service/device_pb2.py
+-rw-rw-rw-   0        0        0    31489 2023-02-06 12:23:25.000000 biostarPython-0.3.0.2/biostarPython/service/device_pb2_grpc.py
+-rw-rw-rw-   0        0        0    10192 2023-02-06 12:23:41.000000 biostarPython-0.3.0.2/biostarPython/service/display_pb2.py
+-rw-rw-rw-   0        0        0    21817 2023-02-06 12:24:17.000000 biostarPython-0.3.0.2/biostarPython/service/display_pb2_grpc.py
+-rw-rw-rw-   0        0        0     7898 2023-02-06 12:24:39.000000 biostarPython-0.3.0.2/biostarPython/service/door_pb2.py
+-rw-rw-rw-   0        0        0    13931 2023-02-06 12:25:03.000000 biostarPython-0.3.0.2/biostarPython/service/door_pb2_grpc.py
+-rw-rw-rw-   0        0        0     1682 2023-02-06 11:47:28.000000 biostarPython-0.3.0.2/biostarPython/service/err_pb2.py
+-rw-rw-rw-   0        0        0      863 2023-02-06 11:47:28.000000 biostarPython-0.3.0.2/biostarPython/service/err_pb2_grpc.py
+-rw-rw-rw-   0        0        0    10235 2023-02-06 12:25:29.000000 biostarPython-0.3.0.2/biostarPython/service/event_pb2.py
+-rw-rw-rw-   0        0        0    21250 2023-02-06 12:25:35.000000 biostarPython-0.3.0.2/biostarPython/service/event_pb2_grpc.py
+-rw-rw-rw-   0        0        0    13004 2023-02-06 12:25:46.000000 biostarPython-0.3.0.2/biostarPython/service/face_pb2.py
+-rw-rw-rw-   0        0        0    20741 2023-02-06 12:25:51.000000 biostarPython-0.3.0.2/biostarPython/service/face_pb2_grpc.py
+-rw-rw-rw-   0        0        0     6996 2023-02-06 12:25:58.000000 biostarPython-0.3.0.2/biostarPython/service/finger_pb2.py
+-rw-rw-rw-   0        0        0     9867 2023-02-06 12:26:06.000000 biostarPython-0.3.0.2/biostarPython/service/finger_pb2_grpc.py
+-rw-rw-rw-   0        0        0     4475 2023-02-06 12:26:36.000000 biostarPython-0.3.0.2/biostarPython/service/fire_zone_pb2.py
+-rw-rw-rw-   0        0        0    10020 2023-02-06 12:26:43.000000 biostarPython-0.3.0.2/biostarPython/service/fire_zone_pb2_grpc.py
+-rw-rw-rw-   0        0        0     6559 2023-02-06 12:26:49.000000 biostarPython-0.3.0.2/biostarPython/service/gateway_pb2.py
+-rw-rw-rw-   0        0        0    16652 2023-02-06 12:26:54.000000 biostarPython-0.3.0.2/biostarPython/service/gateway_pb2_grpc.py
+-rw-rw-rw-   0        0        0     4047 2023-02-06 12:27:00.000000 biostarPython-0.3.0.2/biostarPython/service/input_pb2.py
+-rw-rw-rw-   0        0        0     5452 2023-02-06 12:27:06.000000 biostarPython-0.3.0.2/biostarPython/service/input_pb2_grpc.py
+-rw-rw-rw-   0        0        0     4971 2023-02-06 12:27:31.000000 biostarPython-0.3.0.2/biostarPython/service/interlock_zone_pb2.py
+-rw-rw-rw-   0        0        0    10275 2023-02-06 12:27:52.000000 biostarPython-0.3.0.2/biostarPython/service/interlock_zone_pb2_grpc.py
+-rw-rw-rw-   0        0        0     6228 2023-02-06 12:28:04.000000 biostarPython-0.3.0.2/biostarPython/service/intrusion_zone_pb2.py
+-rw-rw-rw-   0        0        0    11913 2023-02-06 12:28:10.000000 biostarPython-0.3.0.2/biostarPython/service/intrusion_zone_pb2_grpc.py
+-rw-rw-rw-   0        0        0     7728 2023-02-06 12:28:18.000000 biostarPython-0.3.0.2/biostarPython/service/lift_pb2.py
+-rw-rw-rw-   0        0        0    14035 2023-02-06 12:28:28.000000 biostarPython-0.3.0.2/biostarPython/service/lift_pb2_grpc.py
+-rw-rw-rw-   0        0        0     4410 2023-02-06 12:29:00.000000 biostarPython-0.3.0.2/biostarPython/service/lift_zone_pb2.py
+-rw-rw-rw-   0        0        0     9935 2023-02-06 12:29:06.000000 biostarPython-0.3.0.2/biostarPython/service/lift_zone_pb2_grpc.py
+-rw-rw-rw-   0        0        0     4262 2023-02-06 12:29:19.000000 biostarPython-0.3.0.2/biostarPython/service/lock_zone_pb2.py
+-rw-rw-rw-   0        0        0     9935 2023-02-06 12:29:25.000000 biostarPython-0.3.0.2/biostarPython/service/lock_zone_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2146 2023-02-06 11:47:29.000000 biostarPython-0.3.0.2/biostarPython/service/login_pb2.py
+-rw-rw-rw-   0        0        0     5309 2023-02-06 12:29:40.000000 biostarPython-0.3.0.2/biostarPython/service/login_pb2_grpc.py
+-rw-rw-rw-   0        0        0     4199 2023-02-06 12:29:56.000000 biostarPython-0.3.0.2/biostarPython/service/master_pb2.py
+-rw-rw-rw-   0        0        0     8744 2023-02-06 13:00:42.000000 biostarPython-0.3.0.2/biostarPython/service/master_pb2_grpc.py
+-rw-rw-rw-   0        0        0     6294 2023-02-06 13:00:55.000000 biostarPython-0.3.0.2/biostarPython/service/network_pb2.py
+-rw-rw-rw-   0        0        0    10351 2023-02-06 13:01:06.000000 biostarPython-0.3.0.2/biostarPython/service/network_pb2_grpc.py
+-rw-rw-rw-   0        0        0     4298 2023-02-06 13:01:14.000000 biostarPython-0.3.0.2/biostarPython/service/operator_pb2.py
+-rw-rw-rw-   0        0        0    11508 2023-02-06 13:01:20.000000 biostarPython-0.3.0.2/biostarPython/service/operator_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5400 2023-02-06 13:02:38.000000 biostarPython-0.3.0.2/biostarPython/service/rs485_pb2.py
+-rw-rw-rw-   0        0        0     9955 2023-02-06 13:02:44.000000 biostarPython-0.3.0.2/biostarPython/service/rs485_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2774 2023-02-06 13:02:52.000000 biostarPython-0.3.0.2/biostarPython/service/rtsp_pb2.py
+-rw-rw-rw-   0        0        0     5414 2023-02-06 13:03:01.000000 biostarPython-0.3.0.2/biostarPython/service/rtsp_pb2_grpc.py
+-rw-rw-rw-   0        0        0     9817 2023-02-06 13:05:03.000000 biostarPython-0.3.0.2/biostarPython/service/schedule_pb2.py
+-rw-rw-rw-   0        0        0    22706 2023-02-06 13:05:09.000000 biostarPython-0.3.0.2/biostarPython/service/schedule_pb2_grpc.py
+-rw-rw-rw-   0        0        0     6292 2023-02-06 13:05:18.000000 biostarPython-0.3.0.2/biostarPython/service/server_pb2.py
+-rw-rw-rw-   0        0        0    10209 2023-02-06 13:05:28.000000 biostarPython-0.3.0.2/biostarPython/service/server_pb2_grpc.py
+-rw-rw-rw-   0        0        0     4278 2023-02-06 13:05:36.000000 biostarPython-0.3.0.2/biostarPython/service/status_pb2.py
+-rw-rw-rw-   0        0        0     5490 2023-02-06 13:05:42.000000 biostarPython-0.3.0.2/biostarPython/service/status_pb2_grpc.py
+-rw-rw-rw-   0        0        0     4022 2023-02-06 13:05:47.000000 biostarPython-0.3.0.2/biostarPython/service/system_pb2.py
+-rw-rw-rw-   0        0        0     5490 2023-02-06 13:05:53.000000 biostarPython-0.3.0.2/biostarPython/service/system_pb2_grpc.py
+-rw-rw-rw-   0        0        0     6702 2023-02-06 13:06:24.000000 biostarPython-0.3.0.2/biostarPython/service/tenant_pb2.py
+-rw-rw-rw-   0        0        0    18059 2023-02-06 13:06:29.000000 biostarPython-0.3.0.2/biostarPython/service/tenant_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5743 2023-02-06 13:06:35.000000 biostarPython-0.3.0.2/biostarPython/service/thermal_pb2.py
+-rw-rw-rw-   0        0        0     7140 2023-02-06 13:06:40.000000 biostarPython-0.3.0.2/biostarPython/service/thermal_pb2_grpc.py
+-rw-rw-rw-   0        0        0     7426 2023-02-06 13:06:47.000000 biostarPython-0.3.0.2/biostarPython/service/time_pb2.py
+-rw-rw-rw-   0        0        0    14295 2023-02-06 13:06:53.000000 biostarPython-0.3.0.2/biostarPython/service/time_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5385 2023-02-06 13:07:01.000000 biostarPython-0.3.0.2/biostarPython/service/timed_apb_zone_pb2.py
+-rw-rw-rw-   0        0        0    13402 2023-02-06 13:07:05.000000 biostarPython-0.3.0.2/biostarPython/service/timed_apb_zone_pb2_grpc.py
+-rw-rw-rw-   0        0        0     6041 2023-02-06 13:07:11.000000 biostarPython-0.3.0.2/biostarPython/service/tna_pb2.py
+-rw-rw-rw-   0        0        0     8364 2023-02-06 13:07:17.000000 biostarPython-0.3.0.2/biostarPython/service/tna_pb2_grpc.py
+-rw-rw-rw-   0        0        0    16453 2023-02-06 13:07:31.000000 biostarPython-0.3.0.2/biostarPython/service/user_pb2.py
+-rw-rw-rw-   0        0        0    39790 2023-02-06 13:07:38.000000 biostarPython-0.3.0.2/biostarPython/service/user_pb2_grpc.py
+-rw-rw-rw-   0        0        0     3440 2023-02-06 13:07:47.000000 biostarPython-0.3.0.2/biostarPython/service/voip_pb2.py
+-rw-rw-rw-   0        0        0     5414 2023-02-06 13:07:52.000000 biostarPython-0.3.0.2/biostarPython/service/voip_pb2_grpc.py
+-rw-rw-rw-   0        0        0     6784 2023-02-06 13:08:01.000000 biostarPython-0.3.0.2/biostarPython/service/wiegand_pb2.py
+-rw-rw-rw-   0        0        0    10091 2023-02-06 13:08:06.000000 biostarPython-0.3.0.2/biostarPython/service/wiegand_pb2_grpc.py
+-rw-rw-rw-   0        0        0     1896 2023-02-06 11:47:29.000000 biostarPython-0.3.0.2/biostarPython/service/zone_pb2.py
+-rw-rw-rw-   0        0        0      159 2023-02-06 11:47:29.000000 biostarPython-0.3.0.2/biostarPython/service/zone_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:06:27.908580 biostarPython-0.3.0.2/biostarPython.egg-info/
+-rw-rw-rw-   0        0        0     4904 2023-04-17 11:06:27.000000 biostarPython-0.3.0.2/biostarPython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5096 2023-04-17 11:06:27.000000 biostarPython-0.3.0.2/biostarPython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 11:06:27.000000 biostarPython-0.3.0.2/biostarPython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-17 11:06:27.000000 biostarPython-0.3.0.2/biostarPython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-17 11:06:27.000000 biostarPython-0.3.0.2/biostarPython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 11:06:28.036917 biostarPython-0.3.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      999 2023-04-17 11:02:28.000000 biostarPython-0.3.0.2/setup.py
```

### Comparing `biostarPython-0.3.0.1/LICENSE` & `biostarPython-0.3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/PKG-INFO` & `biostarPython-0.3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: biostarPython
-Version: 0.3.0.1
+Version: 0.3.0.2
 Summary: Python client for Suprema GSDK with included callable classes.
 Home-page: https://github.com/gcartlidge/biostarPython
 Author: SupremaUK
 Author-email: gcartlidge@supremainc.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >3.5.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #Python Client for Suprema GSDK<br>
+0.3.0.2 - Fixed no response recieved from some user commands, also added newEventFilter() under event service, to create a new Filter. 
 0.3.0.0 - Support for BS3, VOIP, RTSP and Wiegand User ID <br>
 0.2.1.4 - Version Push <br>
 0.2.1.2 - Fixed issue with importing none existent package <br>
 0.2.1.0 - Addes getJobCode, setJobCode, setJobCodeMulti and setAccessGroupMulti to the UserSvc<br>
 0.2.0.1 - Added searchInfoToConnectInfo(self, searchInfo, isAsync) under ConnectSvc, allowing generation of Connection Parameters directly from search results<br>
 0.2.0.0 - Upgraded support for gRPC to the newest version supported by python (Regenerated .py files from .proto)<br>
 0.1.9.0 - Added zone services, LockZone, APBZone, TimedAPBZone, FireZone, InterlockZone and IntrusionZone are included.
```

### Comparing `biostarPython-0.3.0.1/README.md` & `biostarPython-0.3.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #Python Client for Suprema GSDK<br>
+0.3.0.2 - Fixed no response recieved from some user commands, also added newEventFilter() under event service, to create a new Filter. 
 0.3.0.0 - Support for BS3, VOIP, RTSP and Wiegand User ID <br>
 0.2.1.4 - Version Push <br>
 0.2.1.2 - Fixed issue with importing none existent package <br>
 0.2.1.0 - Addes getJobCode, setJobCode, setJobCodeMulti and setAccessGroupMulti to the UserSvc<br>
 0.2.0.1 - Added searchInfoToConnectInfo(self, searchInfo, isAsync) under ConnectSvc, allowing generation of Connection Parameters directly from search results<br>
 0.2.0.0 - Upgraded support for gRPC to the newest version supported by python (Regenerated .py files from .proto)<br>
 0.1.9.0 - Added zone services, LockZone, APBZone, TimedAPBZone, FireZone, InterlockZone and IntrusionZone are included.
```

### Comparing `biostarPython-0.3.0.1/biostarPython/__init__.py` & `biostarPython-0.3.0.2/biostarPython/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.0.1"
+__version__ = "0.3.0.2"
 __author__ = 'SupremaUK'
 __credits__ = 'SupremaInc'
 
 from os.path import dirname
 from sys import exc_info
 from json import load as jsonload
 from biostarPython.service import access_pb2_grpc, action_pb2_grpc, admin_pb2_grpc, apb_zone_pb2_grpc, auth_pb2_grpc, card_pb2_grpc, cert_pb2_grpc, connect_master_pb2_grpc, connect_pb2_grpc, device_pb2_grpc, display_pb2_grpc, door_pb2_grpc, err_pb2_grpc, event_pb2_grpc, face_pb2_grpc, finger_pb2_grpc, fire_zone_pb2_grpc, gateway_pb2_grpc, input_pb2_grpc, interlock_zone_pb2_grpc, intrusion_zone_pb2_grpc, lift_pb2_grpc, lift_zone_pb2_grpc, lock_zone_pb2_grpc, login_pb2_grpc, network_pb2_grpc, operator_pb2_grpc, rs485_pb2_grpc, schedule_pb2_grpc, server_pb2_grpc, status_pb2_grpc, system_pb2_grpc, tenant_pb2_grpc, thermal_pb2_grpc, timed_apb_zone_pb2_grpc, time_pb2_grpc, tna_pb2_grpc, user_pb2_grpc, voip_pb2_grpc, wiegand_pb2_grpc, rtsp_pb2_grpc, voip_pb2_grpc
@@ -566,15 +566,15 @@
     try:
       self.stub.DeleteAllMulti(user_pb2_grpc.user__pb2.DeleteAllMultiRequest(deviceIDs=deviceIDs))
     except grpc.RpcError as e:
       logger.error(f'Cannot delete all users multi: {e}')
       raise
   def getFinger(self, deviceID, userIDs):
     try:
-      self.stub.GetFinger(user_pb2_grpc.user__pb2.GetFingerRequest(deviceID=deviceID, userIDs=userIDs))
+      response = self.stub.GetFinger(user_pb2_grpc.user__pb2.GetFingerRequest(deviceID=deviceID, userIDs=userIDs))
       return response.userFingers
     except grpc.RpcError as e:
       logger.error(f'Cannot get user fingers: {e}')
       raise
   def setFinger(self, deviceID, userFingers):
     try:
       self.stub.SetFinger(user_pb2_grpc.user__pb2.SetFingerRequest(deviceID=deviceID, userFingers=userFingers))
@@ -585,15 +585,15 @@
     try:
       self.stub.SetFingerMulti(user_pb2_grpc.user__pb2.SetFingerMultiRequest(deviceIDs=deviceIDs, userFingers=userFingers))
     except grpc.RpcError as e:
       logger.error(f'Cannot set user fingers multi: {e}')
       raise
   def getCard(self, deviceID, userIDs):
     try:
-      self.stub.GetCard(user_pb2_grpc.user__pb2.GetCardRequest(deviceID=deviceID, userIDs=userIDs))
+      response = self.stub.GetCard(user_pb2_grpc.user__pb2.GetCardRequest(deviceID=deviceID, userIDs=userIDs))
       return response.userCards
     except grpc.RpcError as e:
       logger.error(f'Cannot get user cards: {e}')
       raise
   def setCard(self, deviceID, userCards):
     try:
       self.stub.SetCard(user_pb2_grpc.user__pb2.SetCardRequest(deviceID=deviceID, userCards=userCards))
@@ -604,15 +604,15 @@
     try:
       self.stub.SetCardMulti(user_pb2_grpc.user__pb2.SetCardMultiRequest(deviceIDs=deviceIDs, userCards=userCards))
     except grpc.RpcError as e:
       logger.error(f'Cannot set user cards multi: {e}')
       raise   
   def getFace(self, deviceID, userIDs):
     try:
-      self.stub.GetFace(user_pb2_grpc.user__pb2.GetFaceRequest(deviceID=deviceID, userIDs=userIDs))
+      response = self.stub.GetFace(user_pb2_grpc.user__pb2.GetFaceRequest(deviceID=deviceID, userIDs=userIDs))
       return response.userFaces
     except grpc.RpcError as e:
       logger.error(f'Cannot get user faces: {e}')
       raise      
   def setFace(self, deviceID, userFaces):
     try:
       self.stub.SetFace(user_pb2_grpc.user__pb2.SetFaceRequest(deviceID=deviceID, userFaces=userFaces))
@@ -946,15 +946,15 @@
     try:
       self.stub.SetQRConfigMulti(card_pb2_grpc.card__pb2.SetQRConfigMultiRequest(deviceIDs=deviceIDs,config=config))
     except grpc.RpcError as e:
       logger.error(f'Cannot set multiple QRconfig: {e}')
       raise
 class EventSvc:
   stub = None
-
+  newEventFilter = event_pb2_grpc.event__pb2.EventFilter
   def __init__(self, channel): 
     try:
       self.stub = event_pb2_grpc.EventStub(channel)
     except grpc.RpcError as e:
       logger.error(f'Cannot get the event stub: {e}')
       raise
   def getLog(self, deviceID, startEventID, maxNumOfLog):
@@ -1096,14 +1096,20 @@
       raise
   def handleUserPhrase(self, serverReq, errCode, userPhrase):
     try:
       self.stub.HandleUserPhrase(server_pb2_grpc.server__pb2.HandleUserPhraseRequest(deviceID=serverReq.deviceID, seqNO=serverReq.seqNO, errCode=errCode, userPhrase=userPhrase))
     except grpc.RpcError as e:
       logger.error(f'Cannot handle userPhrase: {e}')
       raise      
+  def handleGlobalAPB(self, serverReq, errCode, zoneID):
+    try:
+      self.stub.HandleGlobalAPB(server_pb2_grpc.server__pb2.HandleGlobalAPBRequest(deviceID=serverReq.deviceID, seqNO=serverReq.seqNO, errCode=errCode, zoneID=zoneID))
+    except grpc.RpcError as e:
+      logger.error(f'Cannot handle Global APB: {e}')
+      raise 
 class SystemSvc:
   stub = None
   def __init__(self, channel):
     try:
       self.stub = system_pb2_grpc.SystemStub(channel)
     except grpc.RpcError as e:
       logger.error(f'Cannot get the system stub: {e}')
```

### Comparing `biostarPython-0.3.0.1/biostarPython/event_code.json` & `biostarPython-0.3.0.2/biostarPython/event_code.json`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/access.proto` & `biostarPython-0.3.0.2/biostarPython/proto/access.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/action.proto` & `biostarPython-0.3.0.2/biostarPython/proto/action.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/apb_zone.proto` & `biostarPython-0.3.0.2/biostarPython/proto/apb_zone.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/auth.proto` & `biostarPython-0.3.0.2/biostarPython/proto/auth.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/card.proto` & `biostarPython-0.3.0.2/biostarPython/proto/card.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/cert.proto` & `biostarPython-0.3.0.2/biostarPython/proto/cert.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/connect.proto` & `biostarPython-0.3.0.2/biostarPython/proto/connect.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/connect_master.proto` & `biostarPython-0.3.0.2/biostarPython/proto/connect_master.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/device.proto` & `biostarPython-0.3.0.2/biostarPython/proto/device.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/display.proto` & `biostarPython-0.3.0.2/biostarPython/proto/display.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/door.proto` & `biostarPython-0.3.0.2/biostarPython/proto/door.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/event.proto` & `biostarPython-0.3.0.2/biostarPython/proto/event.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/face.proto` & `biostarPython-0.3.0.2/biostarPython/proto/face.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/finger.proto` & `biostarPython-0.3.0.2/biostarPython/proto/finger.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/fire_zone.proto` & `biostarPython-0.3.0.2/biostarPython/proto/fire_zone.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/gateway.proto` & `biostarPython-0.3.0.2/biostarPython/proto/gateway.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/input.proto` & `biostarPython-0.3.0.2/biostarPython/proto/input.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/interlock_zone.proto` & `biostarPython-0.3.0.2/biostarPython/proto/interlock_zone.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/intrusion_zone.proto` & `biostarPython-0.3.0.2/biostarPython/proto/intrusion_zone.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/lift.proto` & `biostarPython-0.3.0.2/biostarPython/proto/lift.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/lift_zone.proto` & `biostarPython-0.3.0.2/biostarPython/proto/lift_zone.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/lock_zone.proto` & `biostarPython-0.3.0.2/biostarPython/proto/lock_zone.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/login.proto` & `biostarPython-0.3.0.2/biostarPython/proto/login.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/master.proto` & `biostarPython-0.3.0.2/biostarPython/proto/master.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/network.proto` & `biostarPython-0.3.0.2/biostarPython/proto/network.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/operator.proto` & `biostarPython-0.3.0.2/biostarPython/proto/operator.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/rs485.proto` & `biostarPython-0.3.0.2/biostarPython/proto/rs485.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/rtsp.proto` & `biostarPython-0.3.0.2/biostarPython/proto/rtsp.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/schedule.proto` & `biostarPython-0.3.0.2/biostarPython/proto/schedule.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/server.proto` & `biostarPython-0.3.0.2/biostarPython/proto/server.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/status.proto` & `biostarPython-0.3.0.2/biostarPython/proto/status.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/system.proto` & `biostarPython-0.3.0.2/biostarPython/proto/system.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/tenant.proto` & `biostarPython-0.3.0.2/biostarPython/proto/tenant.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/thermal.proto` & `biostarPython-0.3.0.2/biostarPython/proto/thermal.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/time.proto` & `biostarPython-0.3.0.2/biostarPython/proto/time.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/timed_apb_zone.proto` & `biostarPython-0.3.0.2/biostarPython/proto/timed_apb_zone.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/tna.proto` & `biostarPython-0.3.0.2/biostarPython/proto/tna.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/user.proto` & `biostarPython-0.3.0.2/biostarPython/proto/user.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/voip.proto` & `biostarPython-0.3.0.2/biostarPython/proto/voip.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/wiegand.proto` & `biostarPython-0.3.0.2/biostarPython/proto/wiegand.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/proto/zone.proto` & `biostarPython-0.3.0.2/biostarPython/proto/zone.proto`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/access_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/access_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/access_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/access_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/action_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/action_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/action_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/action_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/admin_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/admin_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/admin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/apb_zone_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/apb_zone_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/apb_zone_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/apb_zone_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/auth_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/auth_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/card_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/card_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/card_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/card_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/cert_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/cert_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/cert_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/cert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/connect_master_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/connect_master_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/connect_master_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/connect_master_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/connect_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/connect_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/connect_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/connect_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/device_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/device_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/device_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/device_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/display_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/display_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/display_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/display_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/door_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/door_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/door_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/door_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/err_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/err_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/err_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/err_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/event_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/event_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/event_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/event_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/face_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/face_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/face_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/face_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/finger_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/finger_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/finger_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/finger_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/fire_zone_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/fire_zone_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/fire_zone_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/fire_zone_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/gateway_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/gateway_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/gateway_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/gateway_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/input_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/input_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/input_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/input_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/interlock_zone_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/interlock_zone_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/interlock_zone_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/interlock_zone_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/intrusion_zone_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/intrusion_zone_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/intrusion_zone_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/intrusion_zone_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/lift_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/lift_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/lift_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/lift_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/lift_zone_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/lift_zone_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/lift_zone_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/lift_zone_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/lock_zone_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/lock_zone_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/lock_zone_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/lock_zone_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/login_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/login_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/login_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/login_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/master_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/master_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/master_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/master_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/network_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/network_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/network_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/network_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/operator_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/operator_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/operator_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/operator_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/rs485_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/rs485_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/rs485_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/rs485_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/rtsp_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/rtsp_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/rtsp_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/rtsp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/schedule_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/schedule_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/schedule_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/schedule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/server_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/server_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/server_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/server_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/status_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/status_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/status_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/system_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/system_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/system_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/system_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/tenant_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/tenant_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/tenant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/thermal_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/thermal_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/thermal_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/thermal_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/time_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/time_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/time_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/time_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/timed_apb_zone_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/timed_apb_zone_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/timed_apb_zone_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/timed_apb_zone_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/tna_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/tna_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/tna_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/tna_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/user_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/user_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/user_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/voip_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/voip_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/voip_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/voip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/wiegand_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/wiegand_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/wiegand_pb2_grpc.py` & `biostarPython-0.3.0.2/biostarPython/service/wiegand_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython/service/zone_pb2.py` & `biostarPython-0.3.0.2/biostarPython/service/zone_pb2.py`

 * *Files identical despite different names*

### Comparing `biostarPython-0.3.0.1/biostarPython.egg-info/PKG-INFO` & `biostarPython-0.3.0.2/biostarPython.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: biostarPython
-Version: 0.3.0.1
+Version: 0.3.0.2
 Summary: Python client for Suprema GSDK with included callable classes.
 Home-page: https://github.com/gcartlidge/biostarPython
 Author: SupremaUK
 Author-email: gcartlidge@supremainc.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >3.5.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #Python Client for Suprema GSDK<br>
+0.3.0.2 - Fixed no response recieved from some user commands, also added newEventFilter() under event service, to create a new Filter. 
 0.3.0.0 - Support for BS3, VOIP, RTSP and Wiegand User ID <br>
 0.2.1.4 - Version Push <br>
 0.2.1.2 - Fixed issue with importing none existent package <br>
 0.2.1.0 - Addes getJobCode, setJobCode, setJobCodeMulti and setAccessGroupMulti to the UserSvc<br>
 0.2.0.1 - Added searchInfoToConnectInfo(self, searchInfo, isAsync) under ConnectSvc, allowing generation of Connection Parameters directly from search results<br>
 0.2.0.0 - Upgraded support for gRPC to the newest version supported by python (Regenerated .py files from .proto)<br>
 0.1.9.0 - Added zone services, LockZone, APBZone, TimedAPBZone, FireZone, InterlockZone and IntrusionZone are included.
```

### Comparing `biostarPython-0.3.0.1/biostarPython.egg-info/SOURCES.txt` & `biostarPython-0.3.0.2/biostarPython.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
+biostarPython/Log Events.py
 biostarPython/__init__.py
 biostarPython/event_code.json
 biostarPython.egg-info/PKG-INFO
 biostarPython.egg-info/SOURCES.txt
 biostarPython.egg-info/dependency_links.txt
 biostarPython.egg-info/requires.txt
 biostarPython.egg-info/top_level.txt
```

### Comparing `biostarPython-0.3.0.1/setup.py` & `biostarPython-0.3.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name='biostarPython',
-    version='0.3.0.1',
+    version='0.3.0.2',
     author_email = 'gcartlidge@supremainc.com',
     author = 'SupremaUK',
     description = 'Python client for Suprema GSDK with included callable classes.',
     long_description=README,
     long_description_content_type="text/markdown",
     url = 'https://github.com/gcartlidge/biostarPython',
     packages=['biostarPython','biostarPython.service','biostarPython.proto'],
```

