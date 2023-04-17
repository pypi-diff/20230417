# Comparing `tmp/aliyun-iot-linkkit-1.2.7.tar.gz` & `tmp/aliyun-iot-linkkit-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-iot-linkkit-1.2.7.tar", last modified: Wed Mar 15 09:48:43 2023, max compression
+gzip compressed data, was "dist/aliyun-iot-linkkit-1.2.8.tar", last modified: Mon Apr 17 02:01:22 2023, max compression
```

## Comparing `aliyun-iot-linkkit-1.2.7.tar` & `aliyun-iot-linkkit-1.2.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-03-15 09:48:43.000000 aliyun-iot-linkkit-1.2.7/
--rw-r--r--   0 xicai.cxc   (502) staff       (20)     1204 2023-03-15 09:48:43.000000 aliyun-iot-linkkit-1.2.7/PKG-INFO
-drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-03-15 09:48:43.000000 aliyun-iot-linkkit-1.2.7/linkkit/
--rw-r--r--   0 xicai.cxc   (502) staff       (20)   125864 2023-03-13 06:48:22.000000 aliyun-iot-linkkit-1.2.7/linkkit/linkkit.py
--rw-r--r--   0 xicai.cxc   (502) staff       (20)       16 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.7/linkkit/__init__.py
--rw-r--r--   0 xicai.cxc   (502) staff       (20)    19761 2020-10-30 09:09:42.000000 aliyun-iot-linkkit-1.2.7/linkkit/h2client.py
-drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-03-15 09:48:43.000000 aliyun-iot-linkkit-1.2.7/linksdktest/
--rw-r--r--   0 xicai.cxc   (502) staff       (20)        0 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.7/linksdktest/__init__.py
-drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-03-15 09:48:43.000000 aliyun-iot-linkkit-1.2.7/linksdktest/common/
--rw-r--r--   0 xicai.cxc   (502) staff       (20)      361 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.7/linksdktest/common/__init__.py
--rw-r--r--   0 xicai.cxc   (502) staff       (20)     3558 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.7/linksdktest/common/var.py
--rw-r--r--   0 xicai.cxc   (502) staff       (20)        0 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.7/linksdktest/common/method.py
-drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-03-15 09:48:43.000000 aliyun-iot-linkkit-1.2.7/aliyun_iot_linkkit.egg-info/
--rw-r--r--   0 xicai.cxc   (502) staff       (20)     1204 2023-03-15 09:48:43.000000 aliyun-iot-linkkit-1.2.7/aliyun_iot_linkkit.egg-info/PKG-INFO
--rw-r--r--   0 xicai.cxc   (502) staff       (20)      396 2023-03-15 09:48:43.000000 aliyun-iot-linkkit-1.2.7/aliyun_iot_linkkit.egg-info/SOURCES.txt
--rw-r--r--   0 xicai.cxc   (502) staff       (20)       23 2023-03-15 09:48:43.000000 aliyun-iot-linkkit-1.2.7/aliyun_iot_linkkit.egg-info/requires.txt
--rw-r--r--   0 xicai.cxc   (502) staff       (20)       20 2023-03-15 09:48:43.000000 aliyun-iot-linkkit-1.2.7/aliyun_iot_linkkit.egg-info/top_level.txt
--rw-r--r--   0 xicai.cxc   (502) staff       (20)        1 2023-03-15 09:48:43.000000 aliyun-iot-linkkit-1.2.7/aliyun_iot_linkkit.egg-info/dependency_links.txt
--rw-r--r--   0 xicai.cxc   (502) staff       (20)      579 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.7/README.md
--rw-r--r--   0 xicai.cxc   (502) staff       (20)      704 2023-03-13 06:44:27.000000 aliyun-iot-linkkit-1.2.7/setup.py
--rw-r--r--   0 xicai.cxc   (502) staff       (20)       38 2023-03-15 09:48:43.000000 aliyun-iot-linkkit-1.2.7/setup.cfg
+drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)     1561 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/PKG-INFO
+drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/linkkit/
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)   124142 2023-04-07 06:44:24.000000 aliyun-iot-linkkit-1.2.8/linkkit/linkkit.py
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)       16 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.8/linkkit/__init__.py
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)    19761 2020-10-30 09:09:42.000000 aliyun-iot-linkkit-1.2.8/linkkit/h2client.py
+drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/linksdktest/
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)        0 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.8/linksdktest/__init__.py
+drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/linksdktest/common/
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)      361 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.8/linksdktest/common/__init__.py
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)     3558 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.8/linksdktest/common/var.py
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)        0 2022-12-15 05:41:47.000000 aliyun-iot-linkkit-1.2.8/linksdktest/common/method.py
+drwxr-xr-x   0 xicai.cxc   (502) staff       (20)        0 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/aliyun_iot_linkkit.egg-info/
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)     1561 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/aliyun_iot_linkkit.egg-info/PKG-INFO
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)      396 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/aliyun_iot_linkkit.egg-info/SOURCES.txt
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)       17 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/aliyun_iot_linkkit.egg-info/requires.txt
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)       20 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/aliyun_iot_linkkit.egg-info/top_level.txt
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)        1 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/aliyun_iot_linkkit.egg-info/dependency_links.txt
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)      840 2023-04-03 12:41:56.000000 aliyun-iot-linkkit-1.2.8/README.md
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)      695 2023-04-07 06:41:26.000000 aliyun-iot-linkkit-1.2.8/setup.py
+-rw-r--r--   0 xicai.cxc   (502) staff       (20)       38 2023-04-17 02:01:22.000000 aliyun-iot-linkkit-1.2.8/setup.cfg
```

### Comparing `aliyun-iot-linkkit-1.2.7/linkkit/linkkit.py` & `aliyun-iot-linkkit-1.2.8/linkkit/linkkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,29 +30,29 @@
 import socket
 import string
 import time
 import re
 import sys
 from enum import Enum
 import paho.mqtt.client as mqtt
-from linkkit import h2client
-
 
 REQUIRED_MAJOR_VERSION = 3
 REQUIRED_MINOR_VERSION = 5
 
+
 # check Python version
 def lk_check_python_version(major_version, minor_version):
     version = sys.version_info
     if version[0] < major_version or (version[0] == major_version and version[1] < minor_version):
-        print("WARNING: linkit requires Python %d.%d or higher, and the current version is %s" % (major_version, minor_version, sys.version))
-    
-lk_check_python_version(REQUIRED_MAJOR_VERSION, REQUIRED_MINOR_VERSION)
+        print("WARNING: linkit requires Python %d.%d or higher, and the current version is %s" % (
+            major_version, minor_version, sys.version))
 
 
+lk_check_python_version(REQUIRED_MAJOR_VERSION, REQUIRED_MINOR_VERSION)
+
 
 class LinkKit(object):
     TAG_KEY = "attrKey"
     TAG_VALUE = "attrValue"
 
     class LinkKitState(Enum):
         INITIALIZED = 1
@@ -60,82 +60,93 @@
         CONNECTED = 3
         DISCONNECTING = 4
         DISCONNECTED = 5
         DESTRUCTING = 6
         DESTRUCTED = 7
 
     class ErrorCode(Enum):
-        #0x100开头的表示为网关相关的错误码
+        # 0x100开头的表示为网关相关的错误码
         NULL_SUBDEV_ERR = -0x101         # 输入的子设备信息为空错误
         SUBDEV_NOT_ARRAY_ERR = -0x102    # 输入数据并非数组错误
         ARRAY_LENGTH_ERR = -0x103        # 数组长度错误
-        #0x300开头的表示为动态注册相关的错误码
-        DYNREG_AUTH_FAILED = -0x301      # 免白动态注册认证失败
-        DYNREG_AUTH_NWL_FAILED = -0x302
-        #0x400开头表示为OTA有关的错误
+        # 0x300开头的表示为动态注册相关的错误码
+        DYNREG_AUTH_FAILED = -0x301      # 预注册动态注册认证失败
+        DYNREG_AUTH_NWL_FAILED = -0x302  # 免白动态注册认证失败
+        # 0x400开头表示为OTA有关的错误
         OTA_INVALID_PARAM = -0x401       # 参数非法
         OTA_DIGEST_MISMATCH = -0x402     # 校验和不通过
         OTA_PUB_FAILED = -0x403          # 上报失败
         OTA_INVALID_SIGN_METHOD = -0x404 # 非法校验方法
         OTA_DOWNLOAD_FAIL = -0x405       # 下载失败
         OTA_INVALID_URL = -0X406         # 无法访问HTTP链接
         OTA_INVALID_PATH = -0X407        # 存储路径打开失败
         SUCCESS = 0
 
     class StateError(Exception):
         def __init__(self, err):
             Exception.__init__(self, err)
-            
+
     class Shadow(object):
         def __init__(self):
             self.__version = None
             self.__timestamp = None
             self.__state = None
             self.__metadata = None
             self.__latest_shadow_lock = threading.Lock()
             self.__latest_received_time = None
             self.__lastest_received_payload = None
-            
+
         def get_version(self):
             with self.__latest_shadow_lock:
                 return self.__version
+
         def get_metadata(self):
             with self.__latest_shadow_lock:
                 return self.__metadata
+
         def get_state(self):
             with self.__latest_shadow_lock:
                 return self.__state
+
         def set_state(self, state):
             with self.__latest_shadow_lock:
                 self.__state = state
+
         def set_metadata(self, metadata):
             with self.__latest_shadow_lock:
                 self.__metadata = metadata
+
         def set_version(self, version):
             with self.__latest_shadow_lock:
                 self.__version = version
+
         def set_timestamp(self, timestamp):
             with self.__latest_shadow_lock:
                 self.__timestamp = timestamp
+
         def set_latest_recevied_time(self, timestamp):
             with self.__latest_shadow_lock:
                 self.__latest_received_time = timestamp
+
         def get_latest_recevied_time(self):
             with self.__latest_shadow_lock:
-                return self.__latest_received_time 
+                return self.__latest_received_time
+
         def set_latest_recevied_payload(self, payload):
             with self.__latest_shadow_lock:
                 self.__latest_received_payload = payload
+
         def get_latest_recevied_payload(self):
             with self.__latest_shadow_lock:
-                return self.__latest_received_payload 
-                
+                return self.__latest_received_payload
+
         def to_dict(self):
-            return {'state':self.__state, 'metadata':self.__metadata, 'version':self.__version, 'timestamp':self.__timestamp}
-        
+            return {'state': self.__state, 'metadata': self.__metadata, 'version': self.__version,
+                    'timestamp': self.__timestamp}
+
         def to_json_string(self):
             return json.dumps(self.to_dict())
 
     class __HandlerTask(object):
 
         def __init__(self, logger=None):
             self.__logger = logger
@@ -253,37 +264,23 @@
                     self.__callback()
                 if self.__logger is not None:
                     self.__logger.debug("LoopThread thread exit")
             except Exception as e:
                 self.__logger.error("LoopThread thread Exception:" + str(e))
             self.__started = False
             self.__req_wait.set()
-            
-    class __H2FileUploadSink(h2client.H2FileUploadSink):
-        def __init__(self, linkkit_instance):
-            self.__lk_instance = linkkit_instance
-            
-        def on_file_upload_start(self, id, upload_file_info, user_data):
-            self.__lk_instance._on_file_upload_start(id, upload_file_info, user_data)
-        
-        def on_file_upload_end(self, id, upload_file_info, upload_file_result, user_data):
-            self.__lk_instance._on_file_upload_end(id, upload_file_info, upload_file_result, user_data)
-            
-        def on_file_upload_progress(self, id, upload_file_result, upload_file_info, user_data):
-            self.__lk_instance._on_file_upload_progress(id, upload_file_result,
-                                                        upload_file_info, user_data)
-            
+
     def _on_file_upload_start(self, id, upload_file_info, user_data):
         if self.__on_file_upload_begin != None:
             self.__on_file_upload_begin(id, upload_file_info, self.__user_data)
 
     def _on_file_upload_end(self, id, upload_file_info, upload_file_result, user_data):
         if self.__on_file_upload_end != None:
             self.__on_file_upload_end(id, upload_file_info, upload_file_result, self.__user_data)
-    
+
     def _on_file_upload_progress(self, id, upload_file_result, upload_file_info, user_data):
         pass
 
     class __LinkKitLog(object):
         def __init__(self):
             self.__logger = logging.getLogger("linkkit")
             self.__enabled = False
@@ -344,15 +341,15 @@
 DKqC5JlR3XC321Y9YeRq4VzW9v493kHMB65jUr9TU/Qr6cf9tveCX4XSQRjbgbME\
 HMUfpIBvFSDJ3gyICh3WZlXi/EjJKSZp4A==\n\
 -----END CERTIFICATE-----"
 
     def __init__(self, host_name, product_key, device_name, device_secret, auth_type=None,
                  username=None, client_id=None, password=None, instance_id=None,
                  product_secret=None, user_data=None):
-            
+
         # logging configs
         self.__just_for_pycharm_autocomplete = False
 
         def __str_is_empty(value):
             if value is None or value == "":
                 return True
             else:
@@ -384,18 +381,17 @@
         self.__device_interface_info = ""
         self.__device_mac = None
         self.__cellular_IMEI = None
         self.__cellular_ICCID = None
         self.__cellular_IMSI = None
         self.__cellular_MSISDN = None
         self.__mqtt_client = None
-        self.__sdk_version = "1.2.7"
+        self.__sdk_version = "1.2.8"
         self.__sdk_program_language = "Python"
         self.__endpoint = None
-        self.__h2_endpoint = None
         self.__instance_id = instance_id
 
         self.__mqtt_port = 1883
         self.__mqtt_protocol = "MQTTv311"
         self.__mqtt_transport = "TCP"
         self.__mqtt_secure = "TLS"
         self.__mqtt_keep_alive = 60
@@ -404,17 +400,19 @@
         self.__mqtt_max_queued_message = 40
         self.__mqtt_auto_reconnect_min_sec = 1
         self.__mqtt_auto_reconnect_max_sec = 60
         self.__mqtt_auto_reconnect_sec = 0
         self.__mqtt_request_timeout = 10
         # 动态注册(免预注册)的flag
         self.__dynamic_register_nwl_flag = 0
+        # 动态注册(预注册)的flag
+        self.__dynamic_register_flag = 0
         self.__linkkit_state = LinkKit.LinkKitState.INITIALIZED
         self.__aliyun_broker_ca_data = self.__ALIYUN_BROKER_CA_DATA
-        
+
         self.__latest_shadow = LinkKit.Shadow()
         self.__auth_type = auth_type
         self.__username = username
         self.__client_id = client_id
         self.__password = password
 
         # aliyun IoT callbacks
@@ -423,43 +421,42 @@
         # mqtt callbacks
         self.__on_connect = None
         self.__on_disconnect = None
         self.__on_publish_topic = None
         self.__on_subscribe_topic = None
         self.__on_unsubscribe_topic = None
         self.__on_topic_message = None
-        
+
         self.__on_topic_rrpc_message = None
         self.__on_subscribe_rrpc_topic = None
         self.__on_unsubscribe_rrpc_topic = None
 
-
         # thing model callbacks
         self.__on_thing_create = None
         self.__on_thing_enable = None
         self.__on_thing_disable = None
         self.__on_thing_raw_data_arrived = None
         self.__on_thing_raw_data_post = None
         self.__on_thing_call_service = None
         self.__on_thing_prop_changed = None
         self.__on_thing_event_post = None
         self.__on_thing_prop_post = None
         self.__on_thing_shadow_get = None
         self.__on_thing_device_info_update = None
         self.__on_thing_device_info_delete = None
-        
+
         self.__on_file_upload_begin = None
         self.__on_file_upload_end = None
 
         self.__user_topics = {}
         self.__user_topics_subscribe_request = {}
         self.__user_topics_unsubscribe_request = {}
         self.__user_topics_request_lock = threading.Lock()
         self.__user_topics_unsubscribe_request_lock = threading.Lock()
-        
+
         self.__user_rrpc_topics = {}
         self.__user_rrpc_topics_lock = threading.RLock()
         self.__user_rrpc_topics_subscribe_request = {}
         self.__user_rrpc_topics_unsubscribe_request = {}
         self.__user_rrpc_topics_subscribe_request_lock = threading.RLock()
         self.__user_rrpc_topics_unsubscribe_request_lock = threading.RLock()
         self.__user_rrpc_request_ids = []
@@ -474,45 +471,47 @@
         self.__thing_topic_prop_set = '/sys/%s/%s/thing/service/property/set' % \
                                       (self.__product_key, self.__device_name)
         self.__thing_topic_prop_set_reply = self.__thing_topic_prop_set + "_reply"
         self.__thing_topic_prop_get = '/sys/%s/%s/thing/service/property/get' % \
                                       (self.__product_key, self.__device_name)
         self.__thing_topic_event_post_pattern = '/sys/%s/%s/thing/event/%s/post'
         self.__gateway_topic_add_subdev_topo = '/sys/%s/%s/thing/topo/add' % \
-                                       (self.__product_key, self.__device_name)
+                                               (self.__product_key, self.__device_name)
         self.__gateway_topic_add_subdev_topo_reply = self.__gateway_topic_add_subdev_topo + "_reply"
 
         self.__gateway_topic_delete_subdev_topo = '/sys/%s/%s/thing/topo/delete' % \
-                                       (self.__product_key, self.__device_name)
+                                                  (self.__product_key, self.__device_name)
         self.__gateway_topic_delete_subdev_topo_reply = self.__gateway_topic_delete_subdev_topo + "_reply"
 
         self.__gateway_topic_login_subdev = '/ext/session/%s/%s/combine/batch_login' % \
-                                       (self.__product_key, self.__device_name)
+                                            (self.__product_key, self.__device_name)
         self.__gateway_topic_login_subdev_reply = self.__gateway_topic_login_subdev + "_reply"
 
         self.__gateway_topic_logout_subdev = '/ext/session/%s/%s/combine/batch_logout' % \
-                                       (self.__product_key, self.__device_name)
+                                             (self.__product_key, self.__device_name)
         self.__gateway_topic_logout_subdev_reply = self.__gateway_topic_logout_subdev + "_reply"
 
         self.__gateway_topic_register_subdev = '/sys/%s/%s/thing/sub/register' % \
-                                       (self.__product_key, self.__device_name)
+                                               (self.__product_key, self.__device_name)
         self.__gateway_topic_register_subdev_reply = self.__gateway_topic_register_subdev + "_reply"
 
         self.__gateway_topic_product_register_subdev = '/sys/%s/%s/thing/proxy/provisioning/product_register' % \
-                                       (self.__product_key, self.__device_name)
+                                                       (self.__product_key, self.__device_name)
         self.__gateway_topic_product_register_subdev_reply = self.__gateway_topic_product_register_subdev + "_reply"
 
         self.__gateway_topic_topo_change = '/sys/%s/%s/thing/topo/change' % \
-                                       (self.__product_key, self.__device_name)
+                                           (self.__product_key, self.__device_name)
         self.__dynamic_register_nwl_topic = '/ext/regnwl'
+        self.__dynamic_register_topic = '/ext/register'
 
         self.__ota_report_version_topic = '/ota/device/inform/%s/%s' % (self.__product_key, self.__device_name)
         self.__ota_push_topic = '/ota/device/upgrade/%s/%s' % (self.__product_key, self.__device_name)
         self.__ota_pull_topic = '/sys/%s/%s/thing/ota/firmware/get' % (self.__product_key, self.__device_name)
-        self.__ota_pull_reply_topic = '/sys/%s/%s/thing/ota/firmware/get_reply' % (self.__product_key, self.__device_name)
+        self.__ota_pull_reply_topic = '/sys/%s/%s/thing/ota/firmware/get_reply' % (
+            self.__product_key, self.__device_name)
 
         self.__thing_prop_post_mid = {}
         self.__thing_prop_post_mid_lock = threading.Lock()
         self.__thing_prop_set_reply_mid = {}
         self.__thing_prop_set_reply_mid_lock = threading.Lock()
         self.__gateway_add_subdev_topo_mid = {}
         self.__gateway_add_subdev_topo_mid_lock = threading.Lock()
@@ -524,22 +523,21 @@
         self.__thing_events = set()
         self.__thing_request_id_max = 1000000
         self.__thing_request_value = 0
         self.__thing_request_id = {}
         self.__thing_request_id_lock = threading.Lock()
         self.__thing_event_post_mid = {}
         self.__thing_event_post_mid_lock = threading.Lock()
-        
+
         self.__thing_topic_shadow_get = '/shadow/get/%s/%s' % \
-                                       (self.__product_key, self.__device_name)
+                                        (self.__product_key, self.__device_name)
         self.__thing_topic_shadow_update = '/shadow/update/%s/%s' % \
-                                       (self.__product_key, self.__device_name)
+                                           (self.__product_key, self.__device_name)
         self.__thing_shadow_mid = {}
-        self.__thing_shadow_mid_lock = threading.Lock()                        
-                                       
+        self.__thing_shadow_mid_lock = threading.Lock()
 
         # service topic
         self.__thing_topic_service_pattern = '/sys/%s/%s/thing/service/%s'
         self.__thing_topic_services = set()
         self.__thing_topic_services_reply = set()
         self.__thing_services = set()
         self.__thing_answer_service_mid = {}
@@ -550,19 +548,21 @@
         self.__thing_topic_raw_up_reply = self.__thing_topic_raw_up + "_reply"
         self.__thing_topic_raw_down = '/sys/%s/%s/thing/model/down_raw' % (self.__product_key, self.__device_name)
         self.__thing_topic_raw_down_reply = self.__thing_topic_raw_down + "_reply"
         self.__thing_raw_up_mid = {}
         self.__thing_raw_up_mid_lock = threading.Lock()
         self.__thing_raw_down_reply_mid = {}
         self.__thing_raw_down_reply_mid_lock = threading.Lock()
-        
+
         # thing topic - device_info
-        self.__thing_topic_update_device_info_up = '/sys/%s/%s/thing/deviceinfo/update' % (self.__product_key, self.__device_name)
+        self.__thing_topic_update_device_info_up = '/sys/%s/%s/thing/deviceinfo/update' % (
+        self.__product_key, self.__device_name)
         self.__thing_topic_update_device_info_reply = self.__thing_topic_update_device_info_up + "_reply"
-        self.__thing_topic_delete_device_info_up = '/sys/%s/%s/thing/deviceinfo/delete' % (self.__product_key, self.__device_name)
+        self.__thing_topic_delete_device_info_up = '/sys/%s/%s/thing/deviceinfo/delete' % (
+        self.__product_key, self.__device_name)
         self.__thing_topic_delete_device_info_reply = self.__thing_topic_delete_device_info_up + "_reply"
         self.__thing_update_device_info_up_mid = {}
         self.__thing_update_device_info_up_mid_lock = threading.Lock()
         self.__thing_delete_device_info_up_mid = {}
         self.__thing_delete_device_info_up_mid_lock = threading.Lock()
 
         # properties
@@ -619,18 +619,14 @@
         self.__handler_task.register_cmd_callback(self.__handler_task_cmd_on_publish,
                                                   self.__handler_task_on_publish_callback)
         self.__handler_task.register_cmd_callback(self.__handler_task_cmd_on_subscribe,
                                                   self.__handler_task_on_subscribe_callback)
         self.__handler_task.register_cmd_callback(self.__handler_task_cmd_on_unsubscribe,
                                                   self.__handler_task_on_unsubscribe_callback)
         self.__handler_task.start()
-        
-        self.__h2_client = None
-        self.__h2_client_lock = threading.RLock()
-
         pass
 
     @property
     def on_device_dynamic_register(self):
         return None
 
     @on_device_dynamic_register.setter
@@ -681,19 +677,19 @@
     @property
     def on_topic_message(self):
         return None
 
     @on_topic_message.setter
     def on_topic_message(self, value):
         self.__on_topic_message = value
-        
+
     @property
     def on_topic_rrpc_message(self):
         return None
-    
+
     @on_topic_rrpc_message.setter
     def on_topic_rrpc_message(self, value):
         self.__on_topic_rrpc_message = value
 
     @property
     def on_thing_create(self):
         return None
@@ -725,27 +721,27 @@
     @on_thing_raw_data_arrived.setter
     def on_thing_raw_data_arrived(self, value):
         self.__on_thing_raw_data_arrived = value
 
     @property
     def on_thing_raw_data_post(self):
         return self.__on_thing_raw_data_post
-    
+
     @property
     def on_thing_device_info_update(self):
         return self.__on_thing_device_info_update
-    
+
     @on_thing_device_info_update.setter
     def on_thing_device_info_update(self, value):
         self.__on_thing_device_info_update = value
-    
+
     @property
     def on_thing_device_info_delete(self):
         return self.__on_thing_device_info_delete
-    
+
     @on_thing_device_info_delete.setter
     def on_thing_device_info_delete(self, value):
         self.__on_thing_device_info_delete = value
 
     @on_thing_raw_data_post.setter
     def on_thing_raw_data_post(self, value):
         self.__on_thing_raw_data_post = value
@@ -777,38 +773,38 @@
     @property
     def on_thing_prop_post(self):
         return self.__on_thing_prop_post
 
     @on_thing_prop_post.setter
     def on_thing_prop_post(self, value):
         self.__on_thing_prop_post = value
-        
+
     @property
     def on_thing_shadow_get(self):
         return self.__on_thing_shadow_get
-    
+
     @on_thing_shadow_get.setter
     def on_thing_shadow_get(self, value):
         self.__on_thing_shadow_get = value
 
     @property
     def on_file_upload_begin(self):
         return self.__on_file_upload_begin
-        
+
     @on_file_upload_begin.setter
     def on_file_upload_begin(self, value):
         self.__on_file_upload_begin = value
-        
+
     @property
     def on_file_upload_end(self):
         return self.__on_file_upload_end
-        
+
     @on_file_upload_end.setter
     def on_file_upload_end(self, value):
-        self.__on_file_upload_end = value 
+        self.__on_file_upload_end = value
 
     @property
     def on_gateway_add_subdev_topo_reply(self):
         return None
 
     @on_gateway_add_subdev_topo_reply.setter
     def on_gateway_add_subdev_topo_reply(self, value):
@@ -824,23 +820,23 @@
 
     @property
     def on_gateway_login_subdev_reply(self):
         return None
 
     @on_gateway_login_subdev_reply.setter
     def on_gateway_login_subdev_reply(self, value):
-        self.__on_gateway_login_subdev_reply= value
+        self.__on_gateway_login_subdev_reply = value
 
     @property
     def on_gateway_logout_subdev_reply(self):
         return None
 
     @on_gateway_logout_subdev_reply.setter
     def on_gateway_logout_subdev_reply(self, value):
-        self.__on_gateway_logout_subdev_reply= value
+        self.__on_gateway_logout_subdev_reply = value
 
     @property
     def on_gateway_register_subdev_reply(self):
         return None
 
     @on_gateway_register_subdev_reply.setter
     def on_gateway_register_subdev_reply(self, value):
@@ -873,15 +869,15 @@
     @property
     def on_gateway_topo_change(self):
         return None
 
     @on_gateway_topo_change.setter
     def on_gateway_topo_change(self, value):
         self.__on_gateway_topo_change = value
-        
+
     def enable_logger(self, level):
         self.__link_log.config_logger(level)
         self.__link_log.enable_logger()
         if self.__mqtt_client is not None:
             self.__mqtt_client.enable_logger(self.__PahoLog)
         self.__PahoLog.setLevel(level)
 
@@ -890,19 +886,17 @@
         if self.__mqtt_client is not None:
             self.__mqtt_client.disable_logger()
 
     def config_logger(self, level):
         self.__link_log.config_logger(level)
         if self.__mqtt_client is not None:
             self.__PahoLog.setLevel(level)
-            
-    def config_http2(self, endpoint = None):
-        if self.__linkkit_state is not LinkKit.LinkKitState.INITIALIZED:
-            raise LinkKit.StateError("not in INITIALIZED state")
-        self.__h2_endpoint = endpoint
+
+    def config_http2(self, endpoint=None):
+        raise LinkKit.StateError("not supported any more")
 
     def config_mqtt(self, port=1883, protocol="MQTTv311", transport="TCP",
                     secure="TLS", keep_alive=60, clean_session=True,
                     max_inflight_message=20, max_queued_message=40,
                     auto_reconnect_min_sec=1,
                     auto_reconnect_max_sec=60,
                     cadata=None,
@@ -921,21 +915,21 @@
             raise ValueError("keep_alive range wrong")
         if clean_session is not True and clean_session is not False:
             raise ValueError("clean session wrong")
         if max_queued_message < 0:
             raise ValueError("max_queued_message wrong")
         if max_inflight_message < 0:
             raise ValueError("max_inflight_message wrong")
-        if auto_reconnect_min_sec < 1 or auto_reconnect_min_sec > 120*60:
+        if auto_reconnect_min_sec < 1 or auto_reconnect_min_sec > 120 * 60:
             raise ValueError("auto_reconnect_min_sec wrong")
-        if auto_reconnect_max_sec < 1 or auto_reconnect_max_sec > 120*60:
+        if auto_reconnect_max_sec < 1 or auto_reconnect_max_sec > 120 * 60:
             raise ValueError("auto_reconnect_max_sec wrong")
         if auto_reconnect_min_sec > auto_reconnect_max_sec:
             raise ValueError("auto_reconnect_max_sec less than auto_reconnect_min_sec")
-        
+
         self.__link_log.info("config_mqtt enter")
         if self.__linkkit_state == LinkKit.LinkKitState.INITIALIZED:
             if port is not None:
                 self.__mqtt_port = port
             if protocol is not None:
                 self.__mqtt_protocol = protocol
             if transport is not None:
@@ -955,128 +949,58 @@
             if auto_reconnect_max_sec is not None:
                 self.__mqtt_auto_reconnect_max_sec = auto_reconnect_max_sec
             if cadata is not None:
                 self.__aliyun_broker_ca_data = cadata
             if endpoint is not None:
                 self.__endpoint = endpoint
 
-
     def config_device_info(self, interface_info):
         if self.__linkkit_state is not LinkKit.LinkKitState.INITIALIZED:
             raise LinkKit.StateError("LinkKit object not in INITIALIZED")
         if not isinstance(interface_info, str):
             raise ValueError("interface info must be string")
         if len(interface_info) > 160:
             return 1
         self.__device_interface_info = interface_info
         return 0
-    
+
     def get_product(self):
         return self.__product_key
-    
+
     def get_device_name(self):
         return self.__device_name
-    
+
     def get_endpoint(self):
         return self.__endpoint;
-    
+
     def get_h2_endpoint(self):
-        return self.__h2_endpoint;
-    
+        raise LinkKit.StateError("not supported any more")
+
     def get_actual_endpoint(self):
-        return self.__generate_endpoint();
-    
+        return self.__generate_endpoint()
+
     def get_actual_h2_endpoint(self):
-        if self.__h2_client:
-            return self.get_actual_endpoint()
-        else:
-            return self.__try_generate_custom_h2_endpoint();
-    
+        raise LinkKit.StateError("not supported any more")
+
     def __load_json(self, payload):
         return json.loads(self.__to_str(payload))
 
     def __to_str(self, payload):
         if type(payload) is bytes:
             return str(payload, 'utf-8')
         else:
             return payload
-        
-    def __try_open_h2_client(self):
-        with self.__h2_client_lock:
-            if not self.__h2_client: 
-                self.__h2_client = h2client.H2Client(self.__host_name,
-                                                     self.__product_key,
-                                                     self.__device_name,
-                                                     self.__device_secret,
-                                                     endpoint=self.__try_generate_custom_h2_endpoint())
-                self.__h2_client.open()
-                
-    def __try_generate_custom_h2_endpoint(self):
-        if self.__h2_endpoint:
-            return self.__h2_endpoint
-        elif self.__endpoint and self.__endpoint.find('.iot-as-mqtt.') > 0:
-            return self.__endpoint.replace('.iot-as-mqtt.', '.iot-as-http2.')
-        else:
-            return None
-    
-                
-    def __try_close_h2_client(self):
-        with self.__h2_client_lock:
-            if self.__h2_client:
-                self.__h2_client.close()
-                self.__h2_client = None
-                
-    def _get_h2_client(self):
-        self.__try_open_h2_client()
-        return self.__h2_client
-                
-    
-    def upload_file_sync(self, local_filename, remote_filename = None, over_write = True, 
-                         timeout = None):
-        """
-        upload a file to the cloud and block the request
-        
-        Parameters
-        ----------
-        local_filename : str
-            the path of local file
-        remote_filename: str, optional
-            the filename on the cloud
-        over_write: boolean, optional
-            if true, overwrite the file. The default value is True
-        timeout: int or float, optional
-            timeout can be an int or float. If timeout is not specified or None, there is no limit to the wait time.
-            
-        Returns 
-        ----------
-        UploadFileResult
-            upload_size, total_size, file_store_id, code, exception
-            code is 0 if success.
-            
-        Exceptions
-        ----------
-        ValueError
-        Exception
-        
-        """
-        sink = self.__H2FileUploadSink(self)
-        self.__try_open_h2_client()
-        return self.__h2_client.upload_file_sync(local_filename,
-                                           remote_filename,
-                                            over_write, timeout, sink, None)
-        
-        
-    def upload_file_async(self, local_filename, remote_filename = None, over_write = True):
-        sink = self.__H2FileUploadSink(self)
-        self.__try_open_h2_client()
-        return self.__h2_client.upload_file_async(local_filename,
-                                           remote_filename,
-                                            over_write, sink, None)
-        
-        
+
+    def upload_file_sync(self, local_filename, remote_filename=None, over_write=True,
+                         timeout=None):
+        raise LinkKit.StateError("not supported any more")
+
+    def upload_file_async(self, local_filename, remote_filename=None, over_write=True):
+        raise LinkKit.StateError("not supported any more")
+
     def __upload_device_interface_info(self):
         request_id = self.__get_thing_request_id()
         payload = {
             "id": request_id,
             "version": "1.0",
             "params": [
                 {
@@ -1102,16 +1026,15 @@
             if rc == mqtt.MQTT_ERR_SUCCESS:
                 self.__device_info_mid[mid] = self.__timestamp()
                 return 0
             else:
                 return 1
 
     def destruct(self):
-        self.__try_close_h2_client()
-        
+
         if self.__linkkit_state is LinkKit.LinkKitState.DESTRUCTED:
             raise LinkKit.StateError("LinkKit object has already destructed")
         self.__link_log.debug("destruct enter")
         if self.__linkkit_state == LinkKit.LinkKitState.CONNECTED or \
                 self.__linkkit_state == LinkKit.LinkKitState.CONNECTING:
             self.__linkkit_state = LinkKit.LinkKitState.DESTRUCTING
             if self.__connect_async_req:
@@ -1125,15 +1048,15 @@
             if self.__connect_async_req:
                 with self.__worker_loop_exit_req_lock:
                     self.__worker_loop_exit_req = True
             self.__handler_task.stop()
             self.__handler_task.wait_stop()
             self.__linkkit_state = LinkKit.LinkKitState.DESTRUCTED
         pass
-    
+
     def destroy(self):
         self.destruct()
 
     def check_state(self):
         return self.__linkkit_state
 
     @staticmethod
@@ -1142,14 +1065,15 @@
         generate radom string
         """
         random_str = ""
         for i in range(randomlength):
             random_str += random.choice(string.digits + string.ascii_letters)
         return random_str
 
+    # 基于HTTPS的一型一密预注册
     def __dynamic_register_device(self):
         pk = self.__product_key
         ps = self.__product_secret
         dn = self.__device_name
         random_str = self.__generate_random_str(15)
         context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH, cadata=self.__aliyun_broker_ca_data)
         sign_content = "deviceName%sproductKey%srandom%s" % (dn, pk, random_str)
@@ -1173,15 +1097,15 @@
                     return 0, reply_obj_data["deviceSecret"]
                     pass
             else:
                 return 1, reply_obj["message"]
 
     def __config_mqtt_client_internal(self):
         self.__link_log.info("start connect")
-        
+
         timestamp = str(int(time.time()))
         if self.__mqtt_secure == "TLS":
             securemode = 2
         else:
             securemode = 3
         if self.__device_interface_info:
             sii_option = 'sii=%s,' % (self.__device_interface_info)
@@ -1198,43 +1122,57 @@
             sign_content = "clientId%sdeviceName%sproductKey%stimestamp%s" % (
                 self.__product_key + "&" + self.__device_name,
                 self.__device_name,
                 self.__product_key,
                 timestamp)
             password = hmac.new(self.__device_secret.encode("utf-8"), sign_content.encode("utf-8"),
                                 hashlib.sha1).hexdigest()
-        elif self.__auth_type == "regnwl":
-            # 通过一型一密免预注册协议发起认证
-            self.__dynamic_register_nwl_flag = 1
+        # 通过username, passwd, cilentid直连接入的方式
+        elif self.__is_valid_str(self.__client_id) and self.__is_valid_str(self.__username) and self.__is_valid_str(
+                self.__password):
+            # 如果已经通过基于mqtt的免预注册一型一密协议获取到了client_id, user_name, password
+            client_id = self.__client_id
+            username = self.__username
+            password = self.__password
+        # 基于mqtt协议的一型一密，包括预注册和非预注册两种, 尝试去获取username, clientid和password
+        elif self.__is_valid_str(self.__product_secret):
+            if self.__auth_type == "regnwl":
+                # 通过一型一密免预注册协议发起认证
+                self.__dynamic_register_nwl_flag = 1
+            elif self.__auth_type == "register":
+                # 通过一型一密预注册协议发起认证
+                self.__dynamic_register_flag = 1
+            else:
+                raise LinkKit.StateError("unknow dynreg param error")
+
+            auth_type_str = self.__auth_type
             random_str = self.__generate_random_str(15)
             if self.__is_valid_str(self.__instance_id):
-                client_id = "%s.%s|random=%s,authType=regnwl,securemode=2,signmethod=hmacsha256,instanceId=%s|" % (self.__device_name, self.__product_key, random_str, self.__instance_id)
+                client_id = "%s.%s|random=%s,authType=%s,securemode=2,signmethod=hmacsha256,instanceId=%s|" % (
+                    self.__device_name, self.__product_key, random_str, auth_type_str, self.__instance_id)
             else:
-                client_id = "%s.%s|random=%s,authType=regnwl,securemode=2,signmethod=hmacsha256|" % (self.__device_name, self.__product_key, random_str)
+                client_id = "%s.%s|random=%s,authType=%s,securemode=2,signmethod=hmacsha256|" % (
+                    self.__device_name, self.__product_key, random_str, auth_type_str)
             username = "%s&%s" % (self.__device_name, self.__product_key)
             password_src = "deviceName%sproductKey%srandom%s" % (self.__device_name, self.__product_key, random_str)
-            password = hmac.new(self.__product_secret.encode("utf-8"), password_src.encode("utf-8"), hashlib.sha256).hexdigest()
-        elif self.__is_valid_str(self.__client_id) and self.__is_valid_str(self.__username) and self.__is_valid_str(self.__password):
-            # 如果已经通过一型一密免预注册协议获取到了client_id, user_name, password
-            client_id = self.__client_id
-            username = self.__username
-            password = self.__password
+            password = hmac.new(self.__product_secret.encode("utf-8"), password_src.encode("utf-8"),
+                                hashlib.sha256).hexdigest()
         else:
             raise LinkKit.StateError("unknow auth error")
 
         # mqtt client start initialize
         mqtt_protocol_version = mqtt.MQTTv311
         if self.__mqtt_protocol == "MQTTv311":
             mqtt_protocol_version = mqtt.MQTTv311
         elif self.__mqtt_protocol == "MQTTv31":
             mqtt_protocol_version = mqtt.MQTTv31
         self.__mqtt_client = mqtt.Client(client_id=client_id,
                                          clean_session=self.__mqtt_clean_session,
                                          protocol=mqtt_protocol_version)
-       
+
         if self.__link_log.is_enabled():
             self.__mqtt_client.enable_logger(self.__PahoLog)
         self.__mqtt_client.username_pw_set(username, password)
         self.__mqtt_client.on_connect = self.__on_internal_connect
         self.__mqtt_client.on_disconnect = self.__on_internal_disconnect
         self.__mqtt_client.on_message = self.__on_internal_message
         self.__mqtt_client.on_publish = self.__on_internal_publish
@@ -1258,15 +1196,15 @@
             return self.__endpoint
         elif self.__host_name == "127.0.0.1" or self.__host_name == "localhost":
             return self.__host_name
         elif self.__is_valid_str(self.__instance_id):
             return self.__instance_id + ".mqtt.iothub.aliyuncs.com"
         else:
             return "%s.iot-as-mqtt.%s.aliyuncs.com" % \
-                                        (self.__product_key, self.__host_name)
+                   (self.__product_key, self.__host_name)
 
     def connect(self):
         raise LinkKit.StateError("not supported")
 
     def connect_async(self):
         self.__link_log.debug("connect_async")
         if self.__linkkit_state not in (LinkKit.LinkKitState.INITIALIZED, LinkKit.LinkKitState.DISCONNECTED):
@@ -1378,18 +1316,18 @@
             ret = self.__mqtt_client.unsubscribe(unsubscribe_topics)
             rc, mid = ret
             if rc == mqtt.MQTT_ERR_SUCCESS:
                 self.__user_topics_unsubscribe_request[mid] = unsubscribe_topics
                 return ret
             else:
                 return 1, None
-            
+
     def __make_rrpc_topic(self, topic):
         return '/ext/rrpc/+%s' % (topic)
-            
+
     def subscribe_rrpc_topic(self, topic):
         if self.__linkkit_state is not LinkKit.LinkKitState.CONNECTED:
             raise LinkKit.StateError("not in CONNECTED state")
         qos = 0
         if isinstance(topic, str):
             if topic is None or len(topic) == 0:
                 raise ValueError('Invalid topic.')
@@ -1446,15 +1384,15 @@
             with self.__user_rrpc_topics_lock:
                 if topic not in self.__user_rrpc_topics:
                     return 1, None
             rrpc_topic = self.__make_rrpc_topic(topic)
             unsubscribe_topics.append(rrpc_topic)
             with self.__user_rrpc_topics_lock:
                 del self.__user_rrpc_topics[topic]
-            
+
         elif isinstance(topic, list):
             for one_topic in topic:
                 self.__check_topic_string(one_topic)
                 one_topic = self.__tidy_topic(one_topic)
                 with self.__user_rrpc_topics_lock:
                     if one_topic in self.__user_rrpc_topics:
                         rrpc_topic = self.__make_rrpc_topic(one_topic)
@@ -1479,18 +1417,20 @@
         session_flag_internal = {'session present': session_flag}
         self.__handler_task.post_message(self.__handler_task_cmd_on_connect,
                                          (client, user_data, session_flag_internal, rc))
 
     def __loop_forever_internal(self):
         self.__link_log.debug("enter")
         self.__linkkit_state = LinkKit.LinkKitState.CONNECTING
-        if self.__device_secret is None or self.__device_secret == "":
-            lack_other_auth_info = not self.__is_valid_str(self.__username) or not self.__is_valid_str(self.__client_id) or not self.__is_valid_str(self.__password)
-            # 需要预注册的一型一密
-            if self.__auth_type != "regnwl" and lack_other_auth_info:
+
+        # 为了保持存量设备兼容，保留了基于https的需要预注册的一型一密的预注册
+        if not self.__is_valid_str(self.__device_secret) and self.__is_valid_str(self.__product_secret):
+            lack_other_auth_info = not self.__is_valid_str(self.__username) or not self.__is_valid_str(
+                self.__client_id) or not self.__is_valid_str(self.__password)
+            if not self.__is_valid_str(self.__auth_type) and lack_other_auth_info:
                 rc, value = self.__dynamic_register_device()
                 try:
                     self.__on_device_dynamic_register(rc, value, self.__user_data)
                     if rc == 0:
                         self.__device_secret = value
                     else:
                         self.__link_log.error("dynamic register device fail:" + value)
@@ -1557,19 +1497,28 @@
 
             if self.__worker_loop_exit_req:
                 if self.__linkkit_state == LinkKit.LinkKitState.DESTRUCTING:
                     self.__handler_task.stop()
                     self.__linkkit_state = LinkKit.LinkKitState.DESTRUCTED
                 break
             self.__reconnect_wait()
-            # 下面这段逻辑，表示在一型一密免白情况下，由于三元组不对，导致无法与服务器建连,因此需要退出，否则会一直重试
+            # 在mqtt + 一型一密免预注册的情况下，由于三元组不对，导致无法与服务器建连,因此需要退出，否则会一直重试
             if 1 == self.__dynamic_register_nwl_flag:
                 if self.__on_device_dynamic_register_nwl_reply is not None:
-                    self.__on_device_dynamic_register_nwl_reply(LinkKit.ErrorCode.DYNREG_AUTH_NWL_FAILED.value, None, None, None)
+                    self.__on_device_dynamic_register_nwl_reply(LinkKit.ErrorCode.DYNREG_AUTH_NWL_FAILED.value, None,
+                                                                None, None)
                 self.__linkkit_state = LinkKit.LinkKitState.DISCONNECTED
+                self.__dynamic_register_nwl_flag = 0
+                break
+            # 在mqtt + 一型一密预注册的情况下，由于三元组不对，导致无法与服务器建连,因此需要退出，否则会一直重试
+            if 1 == self.__dynamic_register_flag:
+                if self.__on_device_dynamic_register is not None:
+                    self.__on_device_dynamic_register(LinkKit.ErrorCode.DYNREG_AUTH_FAILED.value, None, None)
+                self.__linkkit_state = LinkKit.LinkKitState.DISCONNECTED
+                self.__dynamic_register_flag = 0
                 break
 
     def __clean_timeout_message(self):
         # self.__link_log.debug("__clean_timeout_message enter")
         expire_timestamp = self.__timestamp() - self.__mqtt_request_timeout * 1000
         with self.__thing_prop_post_mid_lock:
             self.__clean_timeout_message_item(self.__thing_prop_post_mid, expire_timestamp)
@@ -1661,15 +1610,15 @@
                     post_topic = self.__thing_topic_event_post_pattern % \
                                  (self.__product_key, self.__device_name, event)
                     self.__thing_topic_event_post[event] = post_topic
                     self.__thing_topic_event_post_reply.add(post_topic + "_reply")
                 # service topic
                 for service in self.__thing_services:
                     self.__thing_topic_services.add(self.__thing_topic_service_pattern %
-                                                       (self.__product_key, self.__device_name, service))
+                                                    (self.__product_key, self.__device_name, service))
 
         except Exception as e:
             self.__link_log.info("file open error:" + str(e))
             return 2
         self.__thing_setup_state = True
         return 0
 
@@ -1688,66 +1637,68 @@
             raise LinkKit.StateError("not in CONNECTED state")
         with self.__thing_raw_down_reply_mid_lock:
             rc, mid = self.__mqtt_client.publish(self.__thing_topic_raw_down_reply, payload, 0)
             if rc == mqtt.MQTT_ERR_SUCCESS:
                 self.__thing_raw_down_reply_mid[mid] = self.__timestamp()
                 return 0
         return 1
-    
+
     def thing_update_device_info(self, payload):
         if self.__linkkit_state is not LinkKit.LinkKitState.CONNECTED:
             raise LinkKit.StateError("not in CONNECTED state")
         if not self.__thing_setup_state or not self.__thing_enable_state:
             raise LinkKit.StateError("not in SETUP & ENABLE state")
             return 1, None
         request_id = self.__get_thing_request_id()
         with self.__thing_update_device_info_up_mid_lock:
-            rc, mid = self.__mqtt_client.publish(self.__thing_topic_update_device_info_up, 
-                                                 self.__pack_alink_request(request_id, "thing.deviceinfo.update", payload),
-                                                  0)
+            rc, mid = self.__mqtt_client.publish(self.__thing_topic_update_device_info_up,
+                                                 self.__pack_alink_request(request_id, "thing.deviceinfo.update",
+                                                                           payload),
+                                                 0)
             if rc == mqtt.MQTT_ERR_SUCCESS:
                 self.__thing_update_device_info_up_mid[mid] = self.__timestamp()
                 return rc, request_id
         return 1, None
-    
+
     def thing_delete_device_info(self, payload):
         if self.__linkkit_state is not LinkKit.LinkKitState.CONNECTED:
             raise LinkKit.StateError("not in CONNECTED state")
         if not self.__thing_setup_state or not self.__thing_enable_state:
             return 1
         request_id = self.__get_thing_request_id()
         with self.__thing_delete_device_info_up_mid_lock:
             rc, mid = self.__mqtt_client.publish(self.__thing_topic_delete_device_info_up,
-                                                  self.__pack_alink_request(request_id, "thing.deviceinfo.delete", payload),
-                                                   0)
+                                                 self.__pack_alink_request(request_id, "thing.deviceinfo.delete",
+                                                                           payload),
+                                                 0)
             if rc == mqtt.MQTT_ERR_SUCCESS:
                 self.__thing_delete_device_info_up_mid[mid] = self.__timestamp()
                 return rc, request_id
         return 1, None
-    
+
     def thing_update_tags(self, tagMap):
         if not isinstance(tagMap, dict):
             raise ValueError("tagMap must be a dictionary")
             return 1, None
-        
+
         payload = []
         for (k, v) in tagMap.items():
             payload.append({LinkKit.TAG_KEY: k, LinkKit.TAG_VALUE: v})
         return self.thing_update_device_info(payload)
-    
+
     def thing_remove_tags(self, tagKeys):
         if not isinstance(tagKeys, list) and not isinstance(tagKeys, tuple):
             raise ValueError("tagKeys must be a list or tuple")
             return 1, None
-        
+
         payload = []
         for tagKey in tagKeys:
             payload.append({LinkKit.TAG_KEY: tagKey})
         return self.thing_delete_device_info(payload)
-    
+
     def __pack_alink_request(self, request_id, method, params):
         request = {
             "id": request_id,
             "version": "1.0",
             "params": params,
             "method": method
         }
@@ -1767,15 +1718,15 @@
         }
 
         item = self.__pop_rrpc_service('alink_' + str(request_id))
         if item:
             service_reply_topic = item['topic']
         else:
             service_reply_topic = self.__thing_topic_service_pattern % (self.__product_key,
-                                                                        self.__device_name, 
+                                                                        self.__device_name,
                                                                         identifier + "_reply")
         with self.__thing_answer_service_mid_lock:
             rc, mid = self.__mqtt_client.publish(service_reply_topic, json.dumps(response), 0)
             if rc == mqtt.MQTT_ERR_SUCCESS:
                 self.__thing_answer_service_mid[mid] = self.__timestamp()
                 return 0
         return 1
@@ -1903,15 +1854,15 @@
             if code != 200:
                 self.__link_log.error("upload device info reply error:%s" % reply_message)
             try:
                 if self.__on_thing_device_info_update != None:
                     self.__on_thing_device_info_update(request_id, code, data, reply_message, self.__user_data)
             except Exception as e:
                 self.__link_log.error("__on_thing_device_info_update process raise exception:%s" % e)
-            pass          
+            pass
         elif message.topic == self.__thing_topic_prop_post_reply:
             payload = self.__load_json(message.payload)
             request_id = payload["id"]
             code = payload["code"]
             data = payload["data"]
             reply_message = payload["message"]
             try:
@@ -2075,28 +2026,42 @@
                 msg = payload['message']
                 self.__back_thing_request_id(request_id)
                 if self.__on_gateway_product_register_subdev_reply is not None:
                     self.__on_gateway_product_register_subdev_reply(request_id, code, data, msg, self.__user_data)
             except Exception as e:
                 self.__link_log.error("__on_gateway_product_register_subdev_reply process raise exception:%s" % e)
             pass
+        elif message.topic == self.__dynamic_register_topic:
+            try:
+                payload = self.__load_json(message.payload)
+                device_secret = payload["deviceSecret"]
+                self.disconnect()
+                self.__dynamic_register_flag = 0
+                if self.__on_device_dynamic_register is not None:
+                    self.__on_device_dynamic_register(LinkKit.ErrorCode.SUCCESS.value, device_secret, None)
+            except Exception as e:
+                self.__link_log.error("__on_device_dynamic_register process raise exception:%s" % e)
+            pass
+
         elif message.topic == self.__dynamic_register_nwl_topic:
             # 一型一密免动态注册获取到username和token
             try:
                 payload = self.__load_json(message.payload)
                 client_id = payload["clientId"]
-                client_id = client_id + '|authType=connwl,securemode=-2,_ss=1,ext=3,lan=%s,_v=%s|' % (self.__sdk_program_language, self.__sdk_version)
+                client_id = client_id + '|authType=connwl,securemode=-2,_ss=1,ext=3,lan=%s,_v=%s|' % (
+                    self.__sdk_program_language, self.__sdk_version)
                 product_key = payload["productKey"]
                 device_name = payload["deviceName"]
                 username = device_name + '&' + product_key
                 password = payload['deviceToken']
+                self.disconnect()
+                self.__dynamic_register_nwl_flag = 0
                 if self.__on_device_dynamic_register_nwl_reply is not None:
-                    self.__on_device_dynamic_register_nwl_reply(LinkKit.ErrorCode.SUCCESS.value, client_id, username, password)
-                    self.disconnect()
-                    self.__dynamic_register_nwl_flag = 0
+                    self.__on_device_dynamic_register_nwl_reply(LinkKit.ErrorCode.SUCCESS.value, client_id, username,
+                                                                password)
             except Exception as e:
                 self.__link_log.error("__on_device_dynamic_register_nwl_reply process raise exception:%s" % e)
             pass
         elif message.topic == self.__ota_push_topic or message.topic == self.__ota_pull_reply_topic:
             try:
                 payload = json.loads(self.__to_str(message.payload))
                 data = payload.setdefault("data", "")
@@ -2120,15 +2085,16 @@
                 ota_notice_type = 0
                 if message.topic == self.__ota_push_topic:
                     ota_notice_type = 1
                 else:
                     ota_notice_type = 2
 
                 if self.__on_ota_message_arrived is not None:
-                    self.__on_ota_message_arrived(ota_notice_type, version, size, url, sign_method, sign, module, str(extra))
+                    self.__on_ota_message_arrived(ota_notice_type, version, size, url, sign_method, sign, module,
+                                                  str(extra))
 
             except Exception as e:
                 self.__link_log.error("__on_ota_message_arrived process raise exception:%s" % e)
             pass
         elif self.__on_topic_message is not None:
             try:
                 self.__on_topic_message(message.topic, message.payload, message.qos, self.__user_data)
@@ -2188,26 +2154,26 @@
 
         rc = self.__mqtt_client.publish(self.__ota_report_version_topic, payload, 0)
         if rc == mqtt.MQTT_ERR_SUCCESS:
             return LinkKit.ErrorCode.SUCCESS
         else:
             return LinkKit.ErrorCode.OTA_PUB_FAILED
 
-    def download_ota_firmware(self, url, local_path, sign_method, sign, download_step=10*1024):
+    def download_ota_firmware(self, url, local_path, sign_method, sign, download_step=10 * 1024):
         if not self.__is_valid_str(url) or not self.__is_valid_str(local_path) or not self.__is_valid_str(sign_method) \
                 or not self.__is_valid_str(sign):
             return LinkKit.ErrorCode.OTA_INVALID_PARAM
 
         context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH, cadata=self.__aliyun_broker_ca_data)
 
         try:
             conn = urllib.request.urlopen(url, context=context)
         except Exception as e:
             # Return code error (e.g. 404, 501, ...)
-            self.__link_log.error('HTTPError: {} %s' %e)
+            self.__link_log.error('HTTPError: {} %s' % e)
             return LinkKit.ErrorCode.OTA_INVALID_URL
         else:
             # 200
             self.__link_log.info('https return 200')
 
             try:
                 file = open(local_path, 'wb')
@@ -2236,146 +2202,146 @@
                     return LinkKit.ErrorCode.SUCCESS
                 else:
                     self.__link_log.error('sign mismatch, expect:' + firmware_sign + ", actually:" + sign)
                     return LinkKit.ErrorCode.OTA_DIGEST_MISMATCH
 
     def __parse_raw_topic(self, topic):
         return re.search('/ext/rrpc/.*?(/.*)', topic).group(1)
-    
+
     def __tidy_topic(self, topic):
         if topic == None:
             return None
         topic = topic.strip()
         if len(topic) == 0:
             return None
         if topic[0] != '/':
             topic = '/' + topic
         return topic
-    
+
     def __push_rrpc_service(self, item):
         with self.__user_rrpc_request_ids_lock:
             if len(self.__user_rrpc_request_ids) > self.__user_rrpc_request_max_len:
                 removed_item = self.__user_rrpc_request_ids.pop(0)
                 del self.__user_rrpc_request_id_index_map[removed_item['id']]
-                
+
         self.__user_rrpc_request_ids.append(item)
         self.__user_rrpc_request_id_index_map[item['id']] = 0
-    
+
     def __pop_rrpc_service(self, id):
         with self.__user_rrpc_request_ids_lock:
             if id not in self.__user_rrpc_request_id_index_map:
-                return None            
-            del self.__user_rrpc_request_id_index_map[id]            
+                return None
+            del self.__user_rrpc_request_id_index_map[id]
             for index in range(0, len(self.__user_rrpc_request_ids)):
                 item = self.__user_rrpc_request_ids[index]
                 if item['id'] == id:
                     del self.__user_rrpc_request_ids[index]
                     return item
             return None
-        
+
     def thing_answer_rrpc(self, id, response):
         item = self.__pop_rrpc_service("rrpc_" + id)
         if item == None:
             self.__link_log.error("answer_rrpc_topic, the id does not exist: %s" % id)
             return 1, None
         rc, mid = self.__mqtt_client.publish(item['topic'], response, 0)
         self.__link_log.debug('reply topic:%s' % item['topic'])
         return rc, mid
-    
-    
+
     def __try_parse_rrpc_topic(self, message):
         self.__link_log.debug('receive a rrpc topic:%s' % message.topic)
         raw_topic = self.__parse_raw_topic(message.topic)
         # if it is a service, log it...
         if raw_topic.startswith('/sys') and raw_topic in self.__thing_topic_services:
             identifier = raw_topic.split('/', 6)[6]
             payload = self.__load_json(self.__to_str(message.payload))
             try:
                 request_id = payload["id"]
                 params = payload["params"]
                 item_id = 'alink_' + request_id
-                item = {'id':item_id, 'request_id':request_id, 'payload': payload, 'identifier':identifier, 'topic':message.topic}
+                item = {'id': item_id, 'request_id': request_id, 'payload': payload, 'identifier': identifier,
+                        'topic': message.topic}
                 self.__push_rrpc_service(item)
                 self.__on_thing_call_service(identifier, request_id, params, self.__user_data)
             except Exception as e:
                 self.__link_log.error("on_thing_call_service raise exception: %s" % e)
             return
-        
+
         # parse
         with self.__user_rrpc_topics_subscribe_request_lock:
             with self.__user_rrpc_topics_lock:
                 if raw_topic not in self.__user_rrpc_topics:
                     self.__link_log.error("%s is not in the rrpc-subscribed list" % raw_topic)
                     return
         if not self.__on_topic_rrpc_message:
             return
         try:
             rrpc_id = message.topic.split('/', 4)[3]
             item_id = 'rrpc_' + rrpc_id
-            item = {'id':item_id, 'payload': message.payload, 'topic':message.topic} 
+            item = {'id': item_id, 'payload': message.payload, 'topic': message.topic}
             self.__push_rrpc_service(item)
             self.__on_topic_rrpc_message(rrpc_id, message.topic,
-                                                    message.payload, 
-                                                    message.qos,
-                                                    self.__user_data)
-            #self.__mqtt_client.publish(message.topic, response, 0)
-            #self.__link_log.debug('reply topic:%s' % message.topic)
+                                         message.payload,
+                                         message.qos,
+                                         self.__user_data)
+            # self.__mqtt_client.publish(message.topic, response, 0)
+            # self.__link_log.debug('reply topic:%s' % message.topic)
         except Exception as e:
             self.__link_log.error("on_topic_rrpc_message process raise exception:%r" % e)
-    
+
     def __try_parse_try_shadow(self, payload):
-        try:          
+        try:
             self.__latest_shadow.set_latest_recevied_time(self.__timestamp())
             self.__latest_shadow.set_latest_recevied_payload(payload)
-            
+
             # parse the pay load
             msg = self.__load_json(payload)
             # set version
             if 'version' in msg:
                 self.__latest_shadow.set_version(msg['version'])
             elif 'payload' in msg and 'version' in msg['payload']:
                 self.__latest_shadow.set_version(msg['payload']['version'])
-                
+
             # set timestamp
             if 'timestamp' in msg:
                 self.__latest_shadow.set_timestamp(msg['timestamp'])
             elif 'payload' in msg and 'timestamp' in msg['payload']:
                 self.__latest_shadow.set_timestamp(msg['payload']['timestamp'])
-                
+
             # set state and metadata
             if 'payload' in msg and msg['payload']['status'] == 'success':
                 if 'state' in msg['payload']:
                     self.__latest_shadow.set_state(msg['payload']['state'])
                 if 'metadata' in msg['payload']:
-                    self.__latest_shadow.set_metadata(msg['payload']['metadata'])                             
+                    self.__latest_shadow.set_metadata(msg['payload']['metadata'])
         except Exception as e:
             pass
-    
+
     def thing_update_shadow(self, reported, version):
         request = {
             'state': {'reported': reported},
             'method': 'update',
             'version': version
         }
         return self.__thing_update_shadow(request)
-            
+
     def thing_get_shadow(self):
-        request = {'method':'get'}
+        request = {'method': 'get'}
         return self.__thing_update_shadow(request)
-    
+
     def local_get_latest_shadow(self):
         return self.__latest_shadow
-    
+
     def __thing_update_shadow(self, request):
         if self.__linkkit_state is not LinkKit.LinkKitState.CONNECTED:
             raise LinkKit.StateError("not in CONNECTED state")
         if not self.__thing_setup_state or not self.__thing_enable_state:
             return 1, None
         with self.__thing_shadow_mid_lock:
-            rc, mid = self.__mqtt_client.publish(self.__thing_topic_shadow_update, 
+            rc, mid = self.__mqtt_client.publish(self.__thing_topic_shadow_update,
                                                  json.dumps(request), 1)
             if rc == mqtt.MQTT_ERR_SUCCESS:
                 self.__thing_shadow_mid[mid] = self.__timestamp()
                 return 0, mid
             else:
                 return 1, None
 
@@ -2389,15 +2355,15 @@
         client, user_data, message = value
         self.__on_internal_async_message(message)
 
     def __on_internal_connect(self, client, user_data, session_flag, rc):
         self.__link_log.info("__on_internal_connect")
         if rc == 0:
             self.__reset_reconnect_wait()
-            #self.__upload_device_interface_info()
+            # self.__upload_device_interface_info()
             self.__handler_task.post_message(self.__handler_task_cmd_on_connect, (client, user_data, session_flag, rc))
 
     def __handler_task_on_connect_callback(self, value):
         client, user_data, session_flag, rc = value
         self.__link_log.info("__on_internal_connect enter")
         self.__link_log.debug("session:%d, return code:%d" % (session_flag['session present'], rc))
         if rc == 0:
@@ -2429,19 +2395,19 @@
         else:
             self.__link_log.error("__on_internal_disconnect enter from wrong state:%r" % self.__linkkit_state)
 
             return
         self.__user_topics.clear()
         self.__user_topics_subscribe_request.clear()
         self.__user_topics_unsubscribe_request.clear()
-        
+
         self.__user_rrpc_topics.clear()
         self.__user_rrpc_topics_subscribe_request.clear()
         self.__user_rrpc_topics_unsubscribe_request.clear()
-        
+
         self.__thing_prop_post_mid.clear()
         self.__thing_event_post_mid.clear()
         self.__thing_answer_service_mid.clear()
         self.__thing_raw_down_reply_mid.clear()
         self.__thing_raw_up_mid.clear()
         self.__thing_shadow_mid.clear()
         self.__device_info_mid.clear()
@@ -2470,15 +2436,15 @@
 
         pass
 
     def __on_internal_publish(self, client, user_data, mid):
         self.__handler_task.post_message(self.__handler_task_cmd_on_publish, (client, user_data, mid))
 
     def __gateway_add_subdev_topo(self, subdev_array):
-        request_params = [ ]
+        request_params = []
         for subdev in subdev_array:
             ret = self.__validate_subdev_param(subdev, 3)
             if ret != 0:
                 return ret, None
 
             pk = subdev[0]
             dn = subdev[1]
@@ -2491,15 +2457,15 @@
             params = {
                 "productKey": pk,
                 "deviceName": dn,
                 "clientId": client_id,
                 "timestamp": millis,
                 "signmethod": "hmacSha256",
                 "sign": sign
-                }
+            }
             request_params.append(params)
         request_id = self.__get_thing_request_id()
         if request_id is None:
             return 1, None
         request = {
             "id": request_id,
             "version": "1.0",
@@ -2511,15 +2477,15 @@
                 self.__gateway_add_subdev_topo_mid[mid] = self.__timestamp()
                 return 0, request_id
             else:
                 return 1, None
         pass
 
     def gateway_add_subdev_topo(self, subdev_array):
-         return self.__gateway_add_subdev_topo(subdev_array)
+        return self.__gateway_add_subdev_topo(subdev_array)
 
     def __validate_subdev_param(self, subdev, expected_len):
         if subdev is None:
             return LinkKit.ErrorCode.NULL_SUBDEV_ERR.value
         if not isinstance(subdev, list):
             return LinkKit.ErrorCode.SUBDEV_NOT_ARRAY_ERR.value
         if len(subdev) < expected_len:
@@ -2537,15 +2503,15 @@
 
             pk = subdev[0]
             dn = subdev[1]
 
             params = {
                 "productKey": pk,
                 "deviceName": dn,
-                }
+            }
             request_params.append(params)
         request_id = self.__get_thing_request_id()
         if request_id is None:
             return 1, None
         request = {
             "id": request_id,
             "version": "1.0",
@@ -2557,18 +2523,18 @@
                 self.__gateway_delete_subdev_topo_mid[mid] = self.__timestamp()
                 return 0, request_id
             else:
                 return 1, None
         pass
 
     def gateway_delete_subdev_topo(self, subdev_array):
-         return self.__gateway_delete_subdev_topo(subdev_array)
+        return self.__gateway_delete_subdev_topo(subdev_array)
 
     def __gateway_login_subdev(self, subdev_array):
-        device_list = [ ]
+        device_list = []
         for subdev in subdev_array:
             ret = self.__validate_subdev_param(subdev, 3)
             if ret != 0:
                 return ret, None
 
             pk = subdev[0]
             dn = subdev[1]
@@ -2581,15 +2547,15 @@
             dev_params = {
                 "productKey": pk,
                 "deviceName": dn,
                 "clientId": client_id,
                 "timestamp": millis,
                 "cleanSession": "false",
                 "sign": sign
-                }
+            }
             device_list.append(dev_params)
         request_params = {
             "signMethod": "hmacSha256",
             "deviceList": device_list,
         }
         request_id = self.__get_thing_request_id()
         if request_id is None:
@@ -2597,20 +2563,20 @@
         request = {
             "id": request_id,
             "version": "1.0",
             "params": request_params,
         }
         rc, mid = self.__mqtt_client.publish(self.__gateway_topic_login_subdev, json.dumps(request), 0)
         if rc == mqtt.MQTT_ERR_SUCCESS:
-             return 0, request_id
+            return 0, request_id
         else:
-             return 1, None
+            return 1, None
 
     def gateway_login_subdev(self, subdev_array):
-         return self.__gateway_login_subdev(subdev_array)
+        return self.__gateway_login_subdev(subdev_array)
 
     def gateway_logout_subdev(self, subdev_array):
         return self.__gateway_logout_subdev(subdev_array)
 
     def __gateway_logout_subdev(self, subdev_array):
         request_params = []
         for subdev in subdev_array:
@@ -2620,59 +2586,59 @@
 
             pk = subdev[0]
             dn = subdev[1]
 
             params = {
                 "productKey": pk,
                 "deviceName": dn,
-                }
+            }
             request_params.append(params)
         request_id = self.__get_thing_request_id()
         if request_id is None:
             return 1, None
         request = {
             "id": request_id,
             "version": "1.0",
             "params": request_params,
         }
         rc, mid = self.__mqtt_client.publish(self.__gateway_topic_logout_subdev, json.dumps(request), 0)
         if rc == mqtt.MQTT_ERR_SUCCESS:
-           return 0, request_id
+            return 0, request_id
         else:
-           return 1, None
+            return 1, None
         pass
 
     def __gateway_register_subdev(self, subdev_array):
-        request_params = [ ]
+        request_params = []
         for subdev in subdev_array:
             ret = self.__validate_subdev_param(subdev, 2)
             if ret != 0:
                 return ret, None
 
             pk = subdev[0]
             dn = subdev[1]
 
             params = {
                 "productKey": pk,
                 "deviceName": dn,
-                }
+            }
             request_params.append(params)
         request_id = self.__get_thing_request_id()
         if request_id is None:
             return 1, None
         request = {
             "id": request_id,
             "version": "1.0",
             "params": request_params,
         }
         rc, mid = self.__mqtt_client.publish(self.__gateway_topic_register_subdev, json.dumps(request), 0)
         if rc == mqtt.MQTT_ERR_SUCCESS:
-           return 0, request_id
+            return 0, request_id
         else:
-           return 1, None
+            return 1, None
 
     def gateway_register_subdev(self, subdev_array):
         return self.__gateway_register_subdev(subdev_array)
 
     def gateway_product_register_subdev(self, subdev_array):
         return self.__gateway_product_register_subdev(subdev_array)
 
@@ -2692,33 +2658,33 @@
             sign = hmac.new(ps.encode("utf-8"), sign_content.encode("utf-8"), hashlib.sha256).hexdigest()
             dev_params = {
                 "productKey": pk,
                 "deviceName": dn,
                 "random": random_str,
                 "signMethod": "hmacSha256",
                 "sign": sign
-                }
+            }
             device_list.append(dev_params)
         request_params = {
             "proxieds": device_list,
         }
         request_id = self.__get_thing_request_id()
         if request_id is None:
             return 1, None
         request = {
             "id": request_id,
             "version": "1.0",
             "params": request_params,
         }
         rc, mid = self.__mqtt_client.publish(self.__gateway_topic_product_register_subdev, json.dumps(request), 0)
         if rc == mqtt.MQTT_ERR_SUCCESS:
-             self.__link_log.debug("mid for product dynamic register:%d" % mid)
-             return 0, request_id
+            self.__link_log.debug("mid for product dynamic register:%d" % mid)
+            return 0, request_id
         else:
-             return 1, None
+            return 1, None
 
     def __handler_task_on_publish_callback(self, value):
         client, user_data, mid = value
         self.__link_log.debug("__on_internal_publish message:%d" % mid)
         with self.__thing_event_post_mid_lock:
             if mid in self.__thing_event_post_mid:
                 self.__thing_event_post_mid.pop(mid)
@@ -2836,15 +2802,15 @@
                 self.__user_rrpc_topics_unsubscribe_request.pop(mid)
                 if self.__on_unsubscribe_rrpc_topic:
                     try:
                         self.__on_unsubscribe_rrpc_topic(mid, self.__user_data)
                     except Exception as err:
                         self.__link_log.error('Caught exception in on_unsubscribe_rrpc_topic: %s', err)
                 return
-            
+
         with self.__user_topics_unsubscribe_request_lock:
             if mid in self.__user_topics_unsubscribe_request:
                 unsubscribe_request = self.__user_topics_unsubscribe_request.pop(mid)
                 pass
         if unsubscribe_request is not None:
             for t in unsubscribe_request:
                 self.__link_log.debug("__user_topics:%s" % str(self.__user_topics))
@@ -2875,8 +2841,7 @@
         if user_str is None or user_str == "":
             return False
         return True
 
     @staticmethod
     def __timestamp():
         return int(time.time() * 1000)
-
```

### Comparing `aliyun-iot-linkkit-1.2.7/linkkit/h2client.py` & `aliyun-iot-linkkit-1.2.8/linkkit/h2client.py`

 * *Files identical despite different names*

### Comparing `aliyun-iot-linkkit-1.2.7/linksdktest/common/var.py` & `aliyun-iot-linkkit-1.2.8/linksdktest/common/var.py`

 * *Files identical despite different names*

### Comparing `aliyun-iot-linkkit-1.2.7/README.md` & `aliyun-iot-linkkit-1.2.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,7 +16,19 @@
 * [UPDATE] fix the onConnect callback invoked at wrong time issue
 
 ### 1.2.3
 * [UPDATE] fix tsl parsing error for simplified tsl products
 
 ### 1.2.4
 * [UPDATE] add gateway feature
+
+### 1.2.5
+* [UPDATE] add mqtt dynamic-register without pre-registration feature
+
+### 1.2.6
+* [UPDATE] set Endpoint parameter with default value
+
+### 1.2.7
+* [UPDATE] add ota feature
+
+### 1.2.8
+* [UPDATE] add mqtt dynamic-register with pre-registration feature
```

### Comparing `aliyun-iot-linkkit-1.2.7/setup.py` & `aliyun-iot-linkkit-1.2.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", mode='r', encoding='UTF-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aliyun-iot-linkkit",
-    version="1.2.7",
+    version="1.2.8",
     author="Aliyun IoT Linkkit Python SDK",
     author_email="xicai.cxc@alibaba-inc.com",
     description="Aliyun IoT Linkkit SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
-    install_requires=['paho-mqtt', 'hyper', 'crcmod'],
+    install_requires=['paho-mqtt', 'crcmod'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
 )
```

