# Comparing `tmp/router_log_preprocessor-0.1.4.tar.gz` & `tmp/router_log_preprocessor-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "router_log_preprocessor-0.1.4.tar", max compression
+gzip compressed data, was "router_log_preprocessor-0.1.5.tar", max compression
```

## Comparing `router_log_preprocessor-0.1.4.tar` & `router_log_preprocessor-0.1.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    11382 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.4/LICENSE
--rw-r--r--   0        0        0     8920 2023-04-13 12:24:43.831463 router_log_preprocessor-0.1.4/README.md
--rw-r--r--   0        0        0      794 2023-04-14 18:52:31.036646 router_log_preprocessor-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      626 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.4/router_log_preprocessor/__init__.py
--rw-r--r--   0        0        0      886 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.4/router_log_preprocessor/__main__.py
--rw-r--r--   0        0        0     1031 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__init__.py
--rw-r--r--   0        0        0      605 2023-04-04 18:59:52.867206 router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      619 2023-04-04 18:59:52.871206 router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc
--rw-r--r--   0        0        0     1263 2023-04-04 18:59:52.903206 router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc
--rw-r--r--   0        0        0     1317 2023-04-14 18:44:34.268234 router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc
--rw-r--r--   0        0        0      850 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/domain/_dnsmasq_dhcp.py
--rw-r--r--   0        0        0     1251 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/domain/_message.py
--rw-r--r--   0        0        0     1560 2023-04-14 18:44:28.564220 router_log_preprocessor-0.1.4/router_log_preprocessor/domain/_wlc.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/__init__.py
--rw-r--r--   0        0        0      190 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      842 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc
--rw-r--r--   0        0        0     1045 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/abc.py
--rw-r--r--   0        0        0      724 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__init__.py
--rw-r--r--   0        0        0      302 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2723 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc
--rw-r--r--   0        0        0     1898 2023-04-14 18:44:34.272234 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc
--rw-r--r--   0        0        0     4217 2023-04-13 12:50:18.950272 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc
--rw-r--r--   0        0        0     2906 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/_known_clients.py
--rw-r--r--   0        0        0     2644 2023-04-14 18:44:28.588220 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/_mapper.py
--rw-r--r--   0        0        0     5820 2023-04-13 12:50:17.498262 router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/_trapper.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/__init__.py
--rw-r--r--   0        0        0      195 2023-04-04 18:59:52.839205 router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1582 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc
--rw-r--r--   0        0        0     2062 2023-04-04 19:21:23.727171 router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc
--rw-r--r--   0        0        0     2081 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/handler.py
--rw-r--r--   0        0        0     2723 2023-04-04 19:21:22.431159 router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/server.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/__init__.py
--rw-r--r--   0        0        0      198 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1049 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc
--rw-r--r--   0        0        0      350 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/__pycache__/typing.cpython-38.pyc
--rw-r--r--   0        0        0     1310 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc
--rw-r--r--   0        0        0     1680 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py
--rw-r--r--   0        0        0      771 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/typing.py
--rw-r--r--   0        0        0     2361 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/wlc.py
--rw-r--r--   0        0        0     2327 2023-04-05 19:10:32.809547 router_log_preprocessor-0.1.4/router_log_preprocessor/settings.py
--rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/util/__init__.py
--rw-r--r--   0        0        0      189 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.4/router_log_preprocessor/util/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1200 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.4/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc
--rw-r--r--   0        0        0     3026 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.4/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc
--rw-r--r--   0        0        0     2071 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/util/logging.py
--rw-r--r--   0        0        0     3588 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.4/router_log_preprocessor/util/rfc3164_parser.py
--rw-r--r--   0        0        0    10333 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.4/setup.py
--rw-r--r--   0        0        0     9790 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11382 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.5/LICENSE
+-rw-r--r--   0        0        0     8920 2023-04-13 12:24:43.831463 router_log_preprocessor-0.1.5/README.md
+-rw-r--r--   0        0        0      794 2023-04-17 19:20:50.639422 router_log_preprocessor-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      626 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.5/router_log_preprocessor/__init__.py
+-rw-r--r--   0        0        0      886 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.5/router_log_preprocessor/__main__.py
+-rw-r--r--   0        0        0     1031 2023-04-04 18:58:30.998235 router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__init__.py
+-rw-r--r--   0        0        0      605 2023-04-04 18:59:52.867206 router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      619 2023-04-04 18:59:52.871206 router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc
+-rw-r--r--   0        0        0     1263 2023-04-04 18:59:52.903206 router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc
+-rw-r--r--   0        0        0     1317 2023-04-14 18:44:34.268234 router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc
+-rw-r--r--   0        0        0      850 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/domain/_dnsmasq_dhcp.py
+-rw-r--r--   0        0        0     1251 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/domain/_message.py
+-rw-r--r--   0        0        0     1560 2023-04-14 18:44:28.564220 router_log_preprocessor-0.1.5/router_log_preprocessor/domain/_wlc.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/__init__.py
+-rw-r--r--   0        0        0      190 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      842 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc
+-rw-r--r--   0        0        0     1045 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/abc.py
+-rw-r--r--   0        0        0      724 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__init__.py
+-rw-r--r--   0        0        0      302 2023-04-04 18:59:52.863206 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2723 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc
+-rw-r--r--   0        0        0     1898 2023-04-14 18:44:34.272234 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc
+-rw-r--r--   0        0        0     4217 2023-04-13 12:50:18.950272 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc
+-rw-r--r--   0        0        0     2906 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/_known_clients.py
+-rw-r--r--   0        0        0     2644 2023-04-14 18:44:28.588220 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/_mapper.py
+-rw-r--r--   0        0        0     5820 2023-04-13 12:50:17.498262 router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/_trapper.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-04 18:59:52.839205 router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1582 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc
+-rw-r--r--   0        0        0     2062 2023-04-04 19:21:23.727171 router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc
+-rw-r--r--   0        0        0     2081 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/handler.py
+-rw-r--r--   0        0        0     2723 2023-04-04 19:21:22.431159 router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/server.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1049 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc
+-rw-r--r--   0        0        0      350 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/__pycache__/typing.cpython-38.pyc
+-rw-r--r--   0        0        0     1310 2023-04-04 18:59:52.915207 router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc
+-rw-r--r--   0        0        0     1680 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py
+-rw-r--r--   0        0        0      771 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/typing.py
+-rw-r--r--   0        0        0     2361 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/wlc.py
+-rw-r--r--   0        0        0     2327 2023-04-05 19:10:32.809547 router_log_preprocessor-0.1.5/router_log_preprocessor/settings.py
+-rw-r--r--   0        0        0      623 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/util/__init__.py
+-rw-r--r--   0        0        0      189 2023-04-04 18:59:52.907206 router_log_preprocessor-0.1.5/router_log_preprocessor/util/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1200 2023-04-04 18:59:52.911206 router_log_preprocessor-0.1.5/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc
+-rw-r--r--   0        0        0     3125 2023-04-17 19:09:25.191263 router_log_preprocessor-0.1.5/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc
+-rw-r--r--   0        0        0     2071 2023-04-04 18:58:31.002235 router_log_preprocessor-0.1.5/router_log_preprocessor/util/logging.py
+-rw-r--r--   0        0        0     3860 2023-04-17 19:18:08.344018 router_log_preprocessor-0.1.5/router_log_preprocessor/util/rfc3164_parser.py
+-rw-r--r--   0        0        0    10333 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.5/setup.py
+-rw-r--r--   0        0        0     9790 1970-01-01 00:00:00.000000 router_log_preprocessor-0.1.5/PKG-INFO
```

### Comparing `router_log_preprocessor-0.1.4/LICENSE` & `router_log_preprocessor-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/README.md` & `router_log_preprocessor-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/pyproject.toml` & `router_log_preprocessor-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "router-log-preprocessor"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 repository = "https://github.com/mastdi/router-log-preprocessor"
 authors = ["Martin Storgaard Dieu <martin@storgaarddieu.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "router_log_preprocessor"}]
```

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/__init__.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/__main__.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/__main__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__init__.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc` & `router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc` & `router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__pycache__/_dnsmasq_dhcp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc` & `router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__pycache__/_message.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc` & `router_log_preprocessor-0.1.5/router_log_preprocessor/domain/__pycache__/_wlc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/domain/_dnsmasq_dhcp.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/domain/_dnsmasq_dhcp.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/domain/_message.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/domain/_message.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/domain/_wlc.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/domain/_wlc.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/__init__.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc` & `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/__pycache__/abc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/abc.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/abc.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__init__.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc` & `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__pycache__/_known_clients.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc` & `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__pycache__/_mapper.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc` & `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/__pycache__/_trapper.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/_known_clients.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/_known_clients.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/_mapper.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/_mapper.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/hooks/zabbix/_trapper.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/hooks/zabbix/_trapper.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/__init__.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc` & `router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/__pycache__/handler.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc` & `router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/__pycache__/server.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/handler.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/handler.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/log_server/server.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/log_server/server.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/__init__.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc` & `router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/__pycache__/dnsmasq_dhcp.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc` & `router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/__pycache__/wlc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/dnsmasq_dhcp.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/typing.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/typing.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/preprocessors/wlc.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/preprocessors/wlc.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/settings.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/settings.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/util/__init__.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/util/__init__.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc` & `router_log_preprocessor-0.1.5/router_log_preprocessor/util/__pycache__/logging.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc` & `router_log_preprocessor-0.1.5/router_log_preprocessor/util/__pycache__/rfc3164_parser.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Apr  4 18:58:31 2023 UTC, .py size: 3588 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,190 +1,196 @@
-00000000: 550d 0d0a 0000 0000 5773 2c64 040e 0000  U.......Ws,d....
+00000000: 550d 0d0a 0000 0000 6399 3d64 6e0e 0000  U.......c.=dn...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 8e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6502 a005 6403 a101 5a06 6404 6405  ..e...d...Z.d.d.
 00000060: 6406 6407 6408 6409 640a 640b 640c 640d  d.d.d.d.d.d.d.d.
 00000070: 640e 640f 6410 9c0c 5a07 6500 6a08 4700  d.d.d...Z.e.j.G.
 00000080: 6411 6412 8400 6412 8302 8301 5a09 650a  d.d...d.....Z.e.
 00000090: 650a 650a 650a 650a 6501 6a01 6413 9c06  e.e.e.e.e.j.d...
 000000a0: 6414 6415 8404 5a0b 650a 6509 6416 9c02  d.d...Z.e.e.d...
 000000b0: 6417 6418 8404 5a0c 6401 5300 2919 e900  d.d...Z.d.S.)...
 000000c0: 0000 004e 2901 da08 4f70 7469 6f6e 616c  ...N)...Optional
-000000d0: 7a62 5e3c 285c 642b 293e 285b 612d 7a41  zb^<(\d+)>([a-zA
+000000d0: 7a6d 5e3c 285c 642b 293e 285b 612d 7a41  zm^<(\d+)>([a-zA
 000000e0: 2d5a 5d7b 337d 295c 737b 312c 327d 285c  -Z]{3})\s{1,2}(\
 000000f0: 647b 312c 327d 295c 7328 5c64 5c64 293a  d{1,2})\s(\d\d):
 00000100: 285c 645c 6429 3a28 5c64 5c64 295c 7328  (\d\d):(\d\d)\s(
-00000110: 5c53 2b29 5c73 285c 532b 3f29 283f 3a5c  \S+)\s(\S+?)(?:\
-00000120: 5b28 5b30 2d39 5d2b 295d 293f 3a5c 7328  [([0-9]+)])?:\s(
-00000130: 2e2a 2924 e901 0000 00e9 0200 0000 e903  .*)$............
-00000140: 0000 00e9 0400 0000 e905 0000 00e9 0600  ................
-00000150: 0000 e907 0000 00e9 0800 0000 e909 0000  ................
-00000160: 00e9 0a00 0000 e90b 0000 00e9 0c00 0000  ................
-00000170: 290c da03 4a61 6eda 0346 6562 da03 4d61  )...Jan..Feb..Ma
-00000180: 72da 0341 7072 da03 4d61 79da 034a 756e  r..Apr..May..Jun
-00000190: da03 4a75 6cda 0341 7567 da03 5365 70da  ..Jul..Aug..Sep.
-000001a0: 034f 6374 da03 4e6f 76da 0344 6563 6300  .Oct..Nov..Decc.
-000001b0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-000001c0: 0000 0040 0000 0073 5400 0000 6500 5a01  ...@...sT...e.Z.
-000001d0: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
-000001e0: 3c00 6504 6505 6403 3c00 6506 6a06 6505  <.e.e.d.<.e.j.e.
-000001f0: 6404 3c00 6507 6505 6405 3c00 6508 6507  d.<.e.e.d.<.e.e.
-00000200: 1900 6505 6406 3c00 6508 6504 1900 6505  ..e.d.<.e.e...e.
-00000210: 6407 3c00 6507 6505 6408 3c00 6409 5300  d.<.e.e.d.<.d.S.
-00000220: 290a da09 4c6f 6752 6563 6f72 647a 4854  )...LogRecordzHT
-00000230: 6865 2070 6172 7365 6420 6c6f 6720 7265  he parsed log re
-00000240: 636f 7264 2077 6974 6820 696e 666f 726d  cord with inform
-00000250: 6174 696f 6e20 636f 6e74 6169 6e65 6420  ation contained 
-00000260: 696e 2061 6e20 5246 4320 3331 3634 206c  in an RFC 3164 l
-00000270: 6f67 206c 696e 65da 0866 6163 696c 6974  og line..facilit
-00000280: 79da 0873 6576 6572 6974 79da 0974 696d  y..severity..tim
-00000290: 6573 7461 6d70 da08 686f 7374 6e61 6d65  estamp..hostname
-000002a0: da07 7072 6f63 6573 73da 0a70 726f 6365  ..process..proce
-000002b0: 7373 5f69 64da 076d 6573 7361 6765 4e29  ss_id..messageN)
-000002c0: 09da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-000002d0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000002e0: 616d 655f 5fda 075f 5f64 6f63 5f5f da03  ame__..__doc__..
-000002f0: 696e 74da 0f5f 5f61 6e6e 6f74 6174 696f  int..__annotatio
-00000300: 6e73 5f5f da08 6461 7465 7469 6d65 da03  ns__..datetime..
-00000310: 7374 7272 0200 0000 a900 722b 0000 0072  strr......r+...r
-00000320: 2b00 0000 fa68 2f68 6f6d 652f 6d79 732f  +....h/home/mys/
-00000330: 446f 6375 6d65 6e74 732f 4769 7448 7562  Documents/GitHub
-00000340: 2f6d 6173 7464 692f 726f 7574 6572 2d6c  /mastdi/router-l
-00000350: 6f67 2d70 7265 7072 6f63 6573 736f 722f  og-preprocessor/
-00000360: 726f 7574 6572 5f6c 6f67 5f70 7265 7072  router_log_prepr
-00000370: 6f63 6573 736f 722f 7574 696c 2f72 6663  ocessor/util/rfc
-00000380: 3331 3634 5f70 6172 7365 722e 7079 721b  3164_parser.pyr.
-00000390: 0000 0034 0000 0073 1000 0000 0a02 0402  ...4...s........
-000003a0: 0801 0801 0a01 0801 0c01 0c01 721b 0000  ............r...
-000003b0: 0029 06da 056d 6f6e 7468 da03 6461 79da  .)...month..day.
-000003c0: 0468 6f75 72da 066d 696e 7574 65da 0673  .hour..minute..s
-000003d0: 6563 6f6e 64da 0672 6574 7572 6e63 0500  econd..returnc..
-000003e0: 0000 0000 0000 0000 0000 0600 0000 0800  ................
-000003f0: 0000 4300 0000 7334 0000 0074 006a 00a0  ..C...s4...t.j..
-00000400: 01a1 007d 057c 056a 0274 037c 0019 0074  ...}.|.j.t.|...t
-00000410: 047c 0183 0174 047c 0283 0174 047c 0383  .|...t.|...t.|..
-00000420: 0174 047c 0483 0164 0164 028d 0653 0029  .t.|...d.d...S.)
-00000430: 0361 0803 0000 5468 6520 5449 4d45 5354  .a....The TIMEST
-00000440: 414d 5020 6669 656c 6420 6973 2074 6865  AMP field is the
-00000450: 206c 6f63 616c 2074 696d 652e 0a0a 2020   local time...  
-00000460: 2020 4974 2069 7320 6173 7375 6d65 6420    It is assumed 
-00000470: 7468 6174 2074 6865 206c 6f67 2065 6e74  that the log ent
-00000480: 7279 2074 696d 6573 7461 6d70 2069 7320  ry timestamp is 
-00000490: 7769 7468 696e 2074 6865 2073 616d 6520  within the same 
-000004a0: 7469 6d65 7a6f 6e65 2061 7320 7468 6973  timezone as this
-000004b0: 0a20 2020 2069 6e73 7461 6e63 6520 616e  .    instance an
-000004c0: 6420 7468 6174 2074 6865 206c 6f67 2065  d that the log e
-000004d0: 6e74 7279 2069 7320 6672 6f6d 2074 6865  ntry is from the
-000004e0: 2063 7572 7265 6e74 2079 6561 722e 0a0a   current year...
-000004f0: 2020 2020 3a70 6172 616d 206d 6f6e 7468      :param month
-00000500: 3a20 5468 6520 456e 676c 6973 6820 6c61  : The English la
-00000510: 6e67 7561 6765 2061 6262 7265 7669 6174  nguage abbreviat
-00000520: 696f 6e20 666f 7220 7468 6520 6d6f 6e74  ion for the mont
-00000530: 6820 6f66 2074 6865 2079 6561 7220 7769  h of the year wi
-00000540: 7468 2074 6865 0a20 2020 2020 2020 2020  th the.         
-00000550: 2020 2020 2020 2020 2066 6972 7374 2063           first c
-00000560: 6861 7261 6374 6572 2069 6e20 7570 7065  haracter in uppe
-00000570: 7263 6173 6520 616e 6420 7468 6520 6f74  rcase and the ot
-00000580: 6865 7220 7477 6f20 6368 6172 6163 7465  her two characte
-00000590: 7273 2069 6e0a 2020 2020 2020 2020 2020  rs in.          
-000005a0: 2020 2020 2020 2020 6c6f 7765 7263 6173          lowercas
-000005b0: 652e 0a20 2020 203a 7061 7261 6d20 6461  e..    :param da
-000005c0: 793a 2054 6865 2064 6179 206f 6620 7468  y: The day of th
-000005d0: 6520 6d6f 6e74 680a 2020 2020 3a70 6172  e month.    :par
-000005e0: 616d 2068 6f75 723a 2054 6865 2068 6f75  am hour: The hou
-000005f0: 7220 6973 2072 6570 7265 7365 6e74 6564  r is represented
-00000600: 2069 6e20 6120 3234 2d68 6f75 7220 666f   in a 24-hour fo
-00000610: 726d 6174 2069 6e20 6c6f 6361 6c20 7469  rmat in local ti
-00000620: 6d65 2e20 5661 6c69 640a 2020 2020 2020  me. Valid.      
-00000630: 2020 2020 2020 2020 2020 2065 6e74 7269             entri
-00000640: 6573 2061 7265 2062 6574 7765 656e 2030  es are between 0
-00000650: 3020 616e 6420 3233 2c20 696e 636c 7573  0 and 23, inclus
-00000660: 6976 652e 0a20 2020 203a 7061 7261 6d20  ive..    :param 
-00000670: 6d69 6e75 7465 3a20 5468 6520 6d69 6e75  minute: The minu
-00000680: 7465 2065 6e74 7279 2069 7320 6265 7477  te entry is betw
-00000690: 6565 6e20 3030 2061 6e64 2035 3920 696e  een 00 and 59 in
-000006a0: 636c 7573 6976 6520 696e 206c 6f63 616c  clusive in local
-000006b0: 2074 696d 652e 0a20 2020 203a 7061 7261   time..    :para
-000006c0: 6d20 7365 636f 6e64 3a20 5468 6520 7365  m second: The se
-000006d0: 636f 6e64 2065 6e74 7279 2069 7320 6265  cond entry is be
-000006e0: 7477 6565 6e20 3030 2061 6e64 2035 3920  tween 00 and 59 
-000006f0: 696e 636c 7573 6976 6520 696e 206c 6f63  inclusive in loc
-00000700: 616c 2074 696d 652e 0a20 2020 203a 7265  al time..    :re
-00000710: 7475 726e 3a20 5468 6520 6461 7465 2061  turn: The date a
-00000720: 6e64 2074 696d 6520 6f66 2074 6865 2074  nd time of the t
-00000730: 696d 6573 7461 6d70 2e0a 2020 2020 7201  imestamp..    r.
-00000740: 0000 0029 0672 2d00 0000 722e 0000 0072  ...).r-...r....r
-00000750: 2f00 0000 7230 0000 0072 3100 0000 da0b  /...r0...r1.....
-00000760: 6d69 6372 6f73 6563 6f6e 6429 0572 2900  microsecond).r).
-00000770: 0000 da03 6e6f 77da 0772 6570 6c61 6365  ....now..replace
-00000780: da06 5f4d 4f4e 5448 7227 0000 0029 0672  .._MONTHr'...).r
-00000790: 2d00 0000 722e 0000 0072 2f00 0000 7230  -...r....r/...r0
-000007a0: 0000 0072 3100 0000 7234 0000 0072 2b00  ...r1...r4...r+.
-000007b0: 0000 722b 0000 0072 2c00 0000 da15 7469  ..r+...r,.....ti
-000007c0: 6d65 7374 616d 705f 746f 5f64 6174 6574  mestamp_to_datet
-000007d0: 696d 6541 0000 0073 1200 0000 0012 0a01  imeA...s........
-000007e0: 0401 0601 0601 0601 0601 0601 02fa 7237  ..............r7
-000007f0: 0000 0029 02da 0672 6563 6f72 6472 3200  ...)...recordr2.
-00000800: 0000 6301 0000 0000 0000 0000 0000 0005  ..c.............
-00000810: 0000 0009 0000 0043 0000 0073 7e00 0000  .......C...s~...
-00000820: 7400 a001 7c00 a101 7d01 7c01 6401 6b08  t...|...}.|.d.k.
-00000830: 721a 7402 6402 8301 8201 7c01 a003 a100  r.t.d.....|.....
-00000840: 7d02 7404 7405 7c02 6403 1900 8301 6404  }.t.t.|.d.....d.
-00000850: 8302 5c02 7d03 7d04 7406 7c03 7c04 7407  ..\.}.}.t.|.|.t.
-00000860: 7c02 6405 6406 8502 1900 8e00 7c02 6406  |.d.d.......|.d.
-00000870: 1900 7c02 6407 1900 7c02 6404 1900 6401  ..|.d...|.d...d.
-00000880: 6b09 7270 7405 7c02 6404 1900 8301 6e02  k.rpt.|.d.....n.
-00000890: 6401 7c02 6408 1900 6409 8d07 5300 290a  d.|.d...d...S.).
-000008a0: 618c 0100 0050 6172 7365 2074 6865 2072  a....Parse the r
-000008b0: 6177 206c 6f67 2072 6563 6f72 6420 6163  aw log record ac
-000008c0: 636f 7264 696e 6720 746f 2054 6865 2042  cording to The B
-000008d0: 5344 2073 7973 6c6f 6720 5072 6f74 6f63  SD syslog Protoc
-000008e0: 6f6c 2028 5246 4320 3331 3634 292e 0a0a  ol (RFC 3164)...
-000008f0: 2020 2020 5468 6520 6d65 7373 6167 6520      The message 
-00000900: 7061 7274 2068 6173 2074 776f 2066 6965  part has two fie
-00000910: 6c64 7320 6b6e 6f77 6e20 6173 2074 6865  lds known as the
-00000920: 2054 4147 2066 6965 6c64 2061 6e64 2074   TAG field and t
-00000930: 6865 2043 4f4e 5445 4e54 2066 6965 6c64  he CONTENT field
-00000940: 2e20 5468 650a 2020 2020 7661 6c75 6520  . The.    value 
-00000950: 696e 2074 6865 2054 4147 2066 6965 6c64  in the TAG field
-00000960: 2077 696c 6c20 6265 2074 6865 206e 616d   will be the nam
-00000970: 6520 6f66 2074 6865 2070 726f 6772 616d  e of the program
-00000980: 206f 7220 7072 6f63 6573 7320 7468 6174   or process that
-00000990: 2067 656e 6572 6174 6564 0a20 2020 2074   generated.    t
-000009a0: 6865 206d 6573 7361 6765 2e20 5468 6520  he message. The 
-000009b0: 434f 4e54 454e 5420 636f 6e74 6169 6e73  CONTENT contains
-000009c0: 2074 6865 2064 6574 6169 6c73 206f 6620   the details of 
-000009d0: 7468 6520 6d65 7373 6167 652e 0a0a 2020  the message...  
-000009e0: 2020 3a70 6172 616d 2072 6563 6f72 643a    :param record:
-000009f0: 2041 2073 696e 676c 6520 7465 7874 206c   A single text l
-00000a00: 6f67 2072 6563 6f72 642e 0a20 2020 203a  og record..    :
-00000a10: 7265 7475 726e 3a20 4120 7061 7273 6564  return: A parsed
-00000a20: 206c 6f67 2072 6563 6f72 642e 0a20 2020   log record..   
-00000a30: 204e da00 7201 0000 0072 0a00 0000 7203   N..r....r....r.
-00000a40: 0000 0072 0800 0000 7209 0000 0072 0b00  ...r....r....r..
-00000a50: 0000 2907 721c 0000 0072 1d00 0000 721e  ..).r....r....r.
-00000a60: 0000 0072 1f00 0000 7220 0000 0072 2100  ...r....r ...r!.
-00000a70: 0000 7222 0000 0029 08da 105f 5246 4333  ..r"...)..._RFC3
-00000a80: 3136 345f 5041 5454 4552 4eda 056d 6174  164_PATTERN..mat
-00000a90: 6368 da0c 5275 6e74 696d 6545 7272 6f72  ch..RuntimeError
-00000aa0: da06 6772 6f75 7073 da06 6469 766d 6f64  ..groups..divmod
-00000ab0: 7227 0000 0072 1b00 0000 7237 0000 0029  r'...r....r7...)
-00000ac0: 0572 3800 0000 723b 0000 0072 3d00 0000  .r8...r;...r=...
-00000ad0: 721c 0000 0072 1d00 0000 722b 0000 0072  r....r....r+...r
-00000ae0: 2b00 0000 722c 0000 00da 0570 6172 7365  +...r,.....parse
-00000af0: 5e00 0000 731c 0000 0000 0a0a 0108 0108  ^...s...........
-00000b00: 0108 0216 0102 0102 0102 010e 0106 0106  ................
-00000b10: 011a 0106 f972 3f00 0000 290d da0b 6461  .....r?...)...da
-00000b20: 7461 636c 6173 7365 7372 2900 0000 da02  taclassesr).....
-00000b30: 7265 da06 7479 7069 6e67 7202 0000 00da  re..typingr.....
-00000b40: 0763 6f6d 7069 6c65 723a 0000 0072 3600  .compiler:...r6.
-00000b50: 0000 da09 6461 7461 636c 6173 7372 1b00  ....dataclassr..
-00000b60: 0000 722a 0000 0072 3700 0000 723f 0000  ..r*...r7...r?..
-00000b70: 0072 2b00 0000 722b 0000 0072 2b00 0000  .r+...r+...r+...
-00000b80: 722c 0000 00da 083c 6d6f 6475 6c65 3e0e  r,.....<module>.
-00000b90: 0000 0073 3a00 0000 0801 0801 0801 0c02  ...s:...........
-00000ba0: 0402 02fe 0412 0201 0201 0201 0201 0201  ................
-00000bb0: 0201 0201 0201 0201 0201 0201 02f4 0610  ................
-00000bc0: 0401 100d 0200 0200 0200 0200 0201 04fe  ................
-00000bd0: 0c1d                                     ..
+00000110: 5c53 2b29 285b 612d 7a41 2d5a 302d 395f  \S+)([a-zA-Z0-9_
+00000120: 5c2d 5c73 5d2a 2928 3f3a 5c5b 285b 302d  \-\s]*)(?:\[([0-
+00000130: 395d 2b29 5d29 3f3a 5c73 282e 2a29 24e9  9]+)])?:\s(.*)$.
+00000140: 0100 0000 e902 0000 00e9 0300 0000 e904  ................
+00000150: 0000 00e9 0500 0000 e906 0000 00e9 0700  ................
+00000160: 0000 e908 0000 00e9 0900 0000 e90a 0000  ................
+00000170: 00e9 0b00 0000 e90c 0000 0029 0cda 034a  ...........)...J
+00000180: 616e da03 4665 62da 034d 6172 da03 4170  an..Feb..Mar..Ap
+00000190: 72da 034d 6179 da03 4a75 6eda 034a 756c  r..May..Jun..Jul
+000001a0: da03 4175 67da 0353 6570 da03 4f63 74da  ..Aug..Sep..Oct.
+000001b0: 034e 6f76 da03 4465 6363 0000 0000 0000  .Nov..Decc......
+000001c0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
+000001d0: 0000 7354 0000 0065 005a 0164 005a 0255  ..sT...e.Z.d.Z.U
+000001e0: 0064 015a 0365 0465 0564 023c 0065 0465  .d.Z.e.e.d.<.e.e
+000001f0: 0564 033c 0065 066a 0665 0564 043c 0065  .d.<.e.j.e.d.<.e
+00000200: 0765 0564 053c 0065 0865 0719 0065 0564  .e.d.<.e.e...e.d
+00000210: 063c 0065 0865 0419 0065 0564 073c 0065  .<.e.e...e.d.<.e
+00000220: 0765 0564 083c 0064 0953 0029 0ada 094c  .e.d.<.d.S.)...L
+00000230: 6f67 5265 636f 7264 7a48 5468 6520 7061  ogRecordzHThe pa
+00000240: 7273 6564 206c 6f67 2072 6563 6f72 6420  rsed log record 
+00000250: 7769 7468 2069 6e66 6f72 6d61 7469 6f6e  with information
+00000260: 2063 6f6e 7461 696e 6564 2069 6e20 616e   contained in an
+00000270: 2052 4643 2033 3136 3420 6c6f 6720 6c69   RFC 3164 log li
+00000280: 6e65 da08 6661 6369 6c69 7479 da08 7365  ne..facility..se
+00000290: 7665 7269 7479 da09 7469 6d65 7374 616d  verity..timestam
+000002a0: 70da 0868 6f73 746e 616d 65da 0770 726f  p..hostname..pro
+000002b0: 6365 7373 da0a 7072 6f63 6573 735f 6964  cess..process_id
+000002c0: da07 6d65 7373 6167 654e 2909 da08 5f5f  ..messageN)...__
+000002d0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+000002e0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+000002f0: da07 5f5f 646f 635f 5fda 0369 6e74 da0f  ..__doc__..int..
+00000300: 5f5f 616e 6e6f 7461 7469 6f6e 735f 5fda  __annotations__.
+00000310: 0864 6174 6574 696d 65da 0373 7472 7202  .datetime..strr.
+00000320: 0000 00a9 0072 2b00 0000 722b 0000 00fa  .....r+...r+....
+00000330: 682f 686f 6d65 2f6d 7973 2f44 6f63 756d  h/home/mys/Docum
+00000340: 656e 7473 2f47 6974 4875 622f 6d61 7374  ents/GitHub/mast
+00000350: 6469 2f72 6f75 7465 722d 6c6f 672d 7072  di/router-log-pr
+00000360: 6570 726f 6365 7373 6f72 2f72 6f75 7465  eprocessor/route
+00000370: 725f 6c6f 675f 7072 6570 726f 6365 7373  r_log_preprocess
+00000380: 6f72 2f75 7469 6c2f 7266 6333 3136 345f  or/util/rfc3164_
+00000390: 7061 7273 6572 2e70 7972 1b00 0000 3400  parser.pyr....4.
+000003a0: 0000 7310 0000 000a 0204 0208 0108 010a  ..s.............
+000003b0: 0108 010c 010c 0172 1b00 0000 2906 da05  .......r....)...
+000003c0: 6d6f 6e74 68da 0364 6179 da04 686f 7572  month..day..hour
+000003d0: da06 6d69 6e75 7465 da06 7365 636f 6e64  ..minute..second
+000003e0: da06 7265 7475 726e 6305 0000 0000 0000  ..returnc.......
+000003f0: 0000 0000 0006 0000 0008 0000 0043 0000  .............C..
+00000400: 0073 3400 0000 7400 6a00 a001 a100 7d05  .s4...t.j.....}.
+00000410: 7c05 6a02 7403 7c00 1900 7404 7c01 8301  |.j.t.|...t.|...
+00000420: 7404 7c02 8301 7404 7c03 8301 7404 7c04  t.|...t.|...t.|.
+00000430: 8301 6401 6402 8d06 5300 2903 6108 0300  ..d.d...S.).a...
+00000440: 0054 6865 2054 494d 4553 5441 4d50 2066  .The TIMESTAMP f
+00000450: 6965 6c64 2069 7320 7468 6520 6c6f 6361  ield is the loca
+00000460: 6c20 7469 6d65 2e0a 0a20 2020 2049 7420  l time...    It 
+00000470: 6973 2061 7373 756d 6564 2074 6861 7420  is assumed that 
+00000480: 7468 6520 6c6f 6720 656e 7472 7920 7469  the log entry ti
+00000490: 6d65 7374 616d 7020 6973 2077 6974 6869  mestamp is withi
+000004a0: 6e20 7468 6520 7361 6d65 2074 696d 657a  n the same timez
+000004b0: 6f6e 6520 6173 2074 6869 730a 2020 2020  one as this.    
+000004c0: 696e 7374 616e 6365 2061 6e64 2074 6861  instance and tha
+000004d0: 7420 7468 6520 6c6f 6720 656e 7472 7920  t the log entry 
+000004e0: 6973 2066 726f 6d20 7468 6520 6375 7272  is from the curr
+000004f0: 656e 7420 7965 6172 2e0a 0a20 2020 203a  ent year...    :
+00000500: 7061 7261 6d20 6d6f 6e74 683a 2054 6865  param month: The
+00000510: 2045 6e67 6c69 7368 206c 616e 6775 6167   English languag
+00000520: 6520 6162 6272 6576 6961 7469 6f6e 2066  e abbreviation f
+00000530: 6f72 2074 6865 206d 6f6e 7468 206f 6620  or the month of 
+00000540: 7468 6520 7965 6172 2077 6974 6820 7468  the year with th
+00000550: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00000560: 2020 2020 6669 7273 7420 6368 6172 6163      first charac
+00000570: 7465 7220 696e 2075 7070 6572 6361 7365  ter in uppercase
+00000580: 2061 6e64 2074 6865 206f 7468 6572 2074   and the other t
+00000590: 776f 2063 6861 7261 6374 6572 7320 696e  wo characters in
+000005a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000005b0: 2020 206c 6f77 6572 6361 7365 2e0a 2020     lowercase..  
+000005c0: 2020 3a70 6172 616d 2064 6179 3a20 5468    :param day: Th
+000005d0: 6520 6461 7920 6f66 2074 6865 206d 6f6e  e day of the mon
+000005e0: 7468 0a20 2020 203a 7061 7261 6d20 686f  th.    :param ho
+000005f0: 7572 3a20 5468 6520 686f 7572 2069 7320  ur: The hour is 
+00000600: 7265 7072 6573 656e 7465 6420 696e 2061  represented in a
+00000610: 2032 342d 686f 7572 2066 6f72 6d61 7420   24-hour format 
+00000620: 696e 206c 6f63 616c 2074 696d 652e 2056  in local time. V
+00000630: 616c 6964 0a20 2020 2020 2020 2020 2020  alid.           
+00000640: 2020 2020 2020 656e 7472 6965 7320 6172        entries ar
+00000650: 6520 6265 7477 6565 6e20 3030 2061 6e64  e between 00 and
+00000660: 2032 332c 2069 6e63 6c75 7369 7665 2e0a   23, inclusive..
+00000670: 2020 2020 3a70 6172 616d 206d 696e 7574      :param minut
+00000680: 653a 2054 6865 206d 696e 7574 6520 656e  e: The minute en
+00000690: 7472 7920 6973 2062 6574 7765 656e 2030  try is between 0
+000006a0: 3020 616e 6420 3539 2069 6e63 6c75 7369  0 and 59 inclusi
+000006b0: 7665 2069 6e20 6c6f 6361 6c20 7469 6d65  ve in local time
+000006c0: 2e0a 2020 2020 3a70 6172 616d 2073 6563  ..    :param sec
+000006d0: 6f6e 643a 2054 6865 2073 6563 6f6e 6420  ond: The second 
+000006e0: 656e 7472 7920 6973 2062 6574 7765 656e  entry is between
+000006f0: 2030 3020 616e 6420 3539 2069 6e63 6c75   00 and 59 inclu
+00000700: 7369 7665 2069 6e20 6c6f 6361 6c20 7469  sive in local ti
+00000710: 6d65 2e0a 2020 2020 3a72 6574 7572 6e3a  me..    :return:
+00000720: 2054 6865 2064 6174 6520 616e 6420 7469   The date and ti
+00000730: 6d65 206f 6620 7468 6520 7469 6d65 7374  me of the timest
+00000740: 616d 702e 0a20 2020 2072 0100 0000 2906  amp..    r....).
+00000750: 722d 0000 0072 2e00 0000 722f 0000 0072  r-...r....r/...r
+00000760: 3000 0000 7231 0000 00da 0b6d 6963 726f  0...r1.....micro
+00000770: 7365 636f 6e64 2905 7229 0000 00da 036e  second).r).....n
+00000780: 6f77 da07 7265 706c 6163 65da 065f 4d4f  ow..replace.._MO
+00000790: 4e54 4872 2700 0000 2906 722d 0000 0072  NTHr'...).r-...r
+000007a0: 2e00 0000 722f 0000 0072 3000 0000 7231  ....r/...r0...r1
+000007b0: 0000 0072 3400 0000 722b 0000 0072 2b00  ...r4...r+...r+.
+000007c0: 0000 722c 0000 00da 1574 696d 6573 7461  ..r,.....timesta
+000007d0: 6d70 5f74 6f5f 6461 7465 7469 6d65 4100  mp_to_datetimeA.
+000007e0: 0000 7312 0000 0000 120a 0104 0106 0106  ..s.............
+000007f0: 0106 0106 0106 0102 fa72 3700 0000 2902  .........r7...).
+00000800: da06 7265 636f 7264 7232 0000 0063 0100  ..recordr2...c..
+00000810: 0000 0000 0000 0000 0000 0500 0000 0900  ................
+00000820: 0000 4300 0000 739c 0000 0074 00a0 017c  ..C...s....t...|
+00000830: 00a1 017d 017c 0164 016b 0872 2074 0264  ...}.|.d.k.r t.d
+00000840: 027c 009b 009d 0283 0182 017c 01a0 03a1  .|.........|....
+00000850: 007d 0274 0474 057c 0264 0319 0083 0164  .}.t.t.|.d.....d
+00000860: 0483 025c 027d 037d 0474 067c 037c 0474  ...\.}.}.t.|.|.t
+00000870: 077c 0264 0564 0685 0219 008e 007c 0264  .|.d.d.......|.d
+00000880: 0619 0074 087c 0264 0719 0083 0164 036b  ...t.|.d.....d.k
+00000890: 0472 747c 0264 0719 00a0 09a1 006e 0264  .rt|.d.......n.d
+000008a0: 017c 0264 0419 0064 016b 0972 8e74 057c  .|.d...d.k.r.t.|
+000008b0: 0264 0419 0083 016e 0264 017c 0264 0819  .d.....n.d.|.d..
+000008c0: 0064 098d 0753 0029 0a61 8c01 0000 5061  .d...S.).a....Pa
+000008d0: 7273 6520 7468 6520 7261 7720 6c6f 6720  rse the raw log 
+000008e0: 7265 636f 7264 2061 6363 6f72 6469 6e67  record according
+000008f0: 2074 6f20 5468 6520 4253 4420 7379 736c   to The BSD sysl
+00000900: 6f67 2050 726f 746f 636f 6c20 2852 4643  og Protocol (RFC
+00000910: 2033 3136 3429 2e0a 0a20 2020 2054 6865   3164)...    The
+00000920: 206d 6573 7361 6765 2070 6172 7420 6861   message part ha
+00000930: 7320 7477 6f20 6669 656c 6473 206b 6e6f  s two fields kno
+00000940: 776e 2061 7320 7468 6520 5441 4720 6669  wn as the TAG fi
+00000950: 656c 6420 616e 6420 7468 6520 434f 4e54  eld and the CONT
+00000960: 454e 5420 6669 656c 642e 2054 6865 0a20  ENT field. The. 
+00000970: 2020 2076 616c 7565 2069 6e20 7468 6520     value in the 
+00000980: 5441 4720 6669 656c 6420 7769 6c6c 2062  TAG field will b
+00000990: 6520 7468 6520 6e61 6d65 206f 6620 7468  e the name of th
+000009a0: 6520 7072 6f67 7261 6d20 6f72 2070 726f  e program or pro
+000009b0: 6365 7373 2074 6861 7420 6765 6e65 7261  cess that genera
+000009c0: 7465 640a 2020 2020 7468 6520 6d65 7373  ted.    the mess
+000009d0: 6167 652e 2054 6865 2043 4f4e 5445 4e54  age. The CONTENT
+000009e0: 2063 6f6e 7461 696e 7320 7468 6520 6465   contains the de
+000009f0: 7461 696c 7320 6f66 2074 6865 206d 6573  tails of the mes
+00000a00: 7361 6765 2e0a 0a20 2020 203a 7061 7261  sage...    :para
+00000a10: 6d20 7265 636f 7264 3a20 4120 7369 6e67  m record: A sing
+00000a20: 6c65 2074 6578 7420 6c6f 6720 7265 636f  le text log reco
+00000a30: 7264 2e0a 2020 2020 3a72 6574 7572 6e3a  rd..    :return:
+00000a40: 2041 2070 6172 7365 6420 6c6f 6720 7265   A parsed log re
+00000a50: 636f 7264 2e0a 2020 2020 4e7a 2d43 6f75  cord..    Nz-Cou
+00000a60: 6c64 206e 6f74 2070 6172 7365 2072 6563  ld not parse rec
+00000a70: 6f72 6420 6163 636f 7264 696e 6720 746f  ord according to
+00000a80: 2052 4643 3331 3634 3a20 7201 0000 0072   RFC3164: r....r
+00000a90: 0a00 0000 7203 0000 0072 0800 0000 7209  ....r....r....r.
+00000aa0: 0000 0072 0b00 0000 2907 721c 0000 0072  ...r....).r....r
+00000ab0: 1d00 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
+00000ac0: 0000 0072 2100 0000 7222 0000 0029 0ada  ...r!...r"...)..
+00000ad0: 105f 5246 4333 3136 345f 5041 5454 4552  ._RFC3164_PATTER
+00000ae0: 4eda 056d 6174 6368 da0c 5275 6e74 696d  N..match..Runtim
+00000af0: 6545 7272 6f72 da06 6772 6f75 7073 da06  eError..groups..
+00000b00: 6469 766d 6f64 7227 0000 0072 1b00 0000  divmodr'...r....
+00000b10: 7237 0000 00da 036c 656e da06 6c73 7472  r7.....len..lstr
+00000b20: 6970 2905 7238 0000 0072 3a00 0000 723c  ip).r8...r:...r<
+00000b30: 0000 0072 1c00 0000 721d 0000 0072 2b00  ...r....r....r+.
+00000b40: 0000 722b 0000 0072 2c00 0000 da05 7061  ..r+...r,.....pa
+00000b50: 7273 655e 0000 0073 1c00 0000 000a 0a01  rse^...s........
+00000b60: 0801 0e01 0802 1601 0201 0201 0201 0e01  ................
+00000b70: 0601 1e01 1a01 06f9 7240 0000 0029 0dda  ........r@...)..
+00000b80: 0b64 6174 6163 6c61 7373 6573 7229 0000  .dataclassesr)..
+00000b90: 00da 0272 65da 0674 7970 696e 6772 0200  ...re..typingr..
+00000ba0: 0000 da07 636f 6d70 696c 6572 3900 0000  ....compiler9...
+00000bb0: 7236 0000 00da 0964 6174 6163 6c61 7373  r6.....dataclass
+00000bc0: 721b 0000 0072 2a00 0000 7237 0000 0072  r....r*...r7...r
+00000bd0: 4000 0000 722b 0000 0072 2b00 0000 722b  @...r+...r+...r+
+00000be0: 0000 0072 2c00 0000 da08 3c6d 6f64 756c  ...r,.....<modul
+00000bf0: 653e 0e00 0000 733a 0000 0008 0108 0108  e>....s:........
+00000c00: 010c 0204 0202 fe04 1202 0102 0102 0102  ................
+00000c10: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000c20: f406 1004 0110 0d02 0002 0002 0002 0002  ................
+00000c30: 0104 fe0c 1d                             .....
```

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/util/logging.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/util/logging.py`

 * *Files identical despite different names*

### Comparing `router_log_preprocessor-0.1.4/router_log_preprocessor/util/rfc3164_parser.py` & `router_log_preprocessor-0.1.5/router_log_preprocessor/util/rfc3164_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     # Start of log
     r"^"
     # Pri
     r"<(\d+)>"
     # Timestamp
     r"([a-zA-Z]{3})\s{1,2}(\d{1,2})\s(\d\d):(\d\d):(\d\d)\s"
     # Hostname
-    r"(\S+)\s"
+    r"(\S+)"
     # Optional process information
-    r"(\S+?)(?:\[([0-9]+)])?:\s"
+    r"([a-zA-Z0-9_\-\s]*)(?:\[([0-9]+)])?:\s"
     # Message
     r"(.*)"
     # End of log
     r"$"
 )
 
 _MONTH = {
@@ -99,20 +99,22 @@
     the message. The CONTENT contains the details of the message.
 
     :param record: A single text log record.
     :return: A parsed log record.
     """
     match = _RFC3164_PATTERN.match(record)
     if match is None:
-        raise RuntimeError("")
+        raise RuntimeError(f"Could not parse record according to RFC3164: {record}")
     groups = match.groups()
     # Priority is facility * 8 + severity, so divmod is the inverse of that
     facility, severity = divmod(int(groups[0]), 8)
     return LogRecord(
         facility=facility,
         severity=severity,
         timestamp=timestamp_to_datetime(*groups[1:6]),
         hostname=groups[6],
-        process=groups[7],
+        # If the process name is given then there will be a leading space included
+        # from the space after the hostname. That space is removed using lstrip().
+        process=groups[7].lstrip() if len(groups[7]) > 0 else None,
         process_id=int(groups[8]) if groups[8] is not None else None,
         message=groups[9],
     )
```

### Comparing `router_log_preprocessor-0.1.4/setup.py` & `router_log_preprocessor-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 entry_points = \
 {'console_scripts': ['router-log-preprocessor = '
                      'router_log_preprocessor.__main__:main']}
 
 setup_kwargs = {
     'name': 'router-log-preprocessor',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': '',
     'long_description': '# Router Log Preprocessor\n![router-log-preprocessor](https://user-images.githubusercontent.com/105678820/228938795-66dbd955-813b-4fb3-a559-4f3a41f55bb9.png)\n\n> Garbage in, garbage out\n>\n> &mdash; <cite>George Fuechsel</cite>\n\nPreprocessors upcycle garbage input data into well-structured data to ensure reliable and accurate event handling in third-party systems such as Zabbix.\nBy parsing and filtering the input log data, the preprocessor helps to ensure that only high-quality data are sent for further analysis and alerting.\nThis helps to minimize false positives and ensure that network administrators receive reliable and actionable alerts about potential security threats or other issues.\n\n\nKey features:\n- **Wireless LAN Controller event** log entries are parsed to tangible enumerations\n- **DNSMASQ DHCP** log entries are parsed to catch which IP a given client is assigned to\n- **Zabbix** templates are included to ensure that the logs are can lead to actionable alerts\n- **Extendable** preprocessors and hooks to ensure future reliable information to network administrators\n\n## Installation\n```console\n$ pip install router-log-preprocessor\n```\n\nIf needed it can also be installed from sources.\nRequires [Poetry 1.3.2](https://python-poetry.org/).\n```console\n$ git pull https://github.com/mastdi/router-log-preprocessor.git\n$ cd router-log-preprocessor\n$ poetry install\n```\n\n## Usage\nInstalling the package using pip also creates the executable script named `router-log-preprocessor`.\nOn Linux systems the router log preprocessor can be run by\n\n```console\n./router-log-preprocessor\n```\n\nThe configuration solely happens through environment variables or a `.env` configuration file located in the current working directory.\nThe most important variables are documented below. \nA full sample can be found in [.env](https://raw.githubusercontent.com/mastdi/router-log-preprocessor/master/.env).\nThe application reads, in order of the least priority to the highest file:\n1. `.env`,\n2. `.env.dev`,\n3. `.env.test`,\n4. `.env.staging`,\n5. `.env.prod`,\n\nmeaning that values stored in `.env.prod` will overwrite any values from other dovenv files.\nParameters stored in environment variables will always take priority over values loaded from a dotenv file.\n\n```dotenv\n# Purpose: Specifies the IP address or hostname of the local interface to which the\n# logging system should bind.\n# Format: A string containing a valid IP address or hostname, such as "192.168.0.1" or\n# "example.com".\nLOG_SERVER_HOST="0.0.0.0"\n\n# Purpose: Specifies the port number of the server to which log data should be sent.\n# Format: An integer representing a valid port number, such as 514.\nLOG_SERVER_PORT=8514\n\n# Purpose: Specifies the hostname or IP address of the Zabbix server to which the\n# Zabbix Sender should send monitoring data.\n# Format: A string containing a valid hostname or IP address, such as "example.com" or\n# "192.168.0.1".\nZABBIX_HOST="example.com"\n\n# Purpose: Specifies the port number on which the Zabbix server is running and to\n# which the Zabbix Sender should send monitoring data.\n# Format: An integer representing a valid port number, such as 10051.\nZABBIX_PORT=10051\n```\n\n## As a service\n\nThis part will go through the steps to set up the Router Log Preprocessor as a service on Ubuntu.\nThe following steps will be explained in details below:\n\n- Create a service user\n- Create a virtual environment\n- Configure environment variables\n- Set up the logging directory\n- Create the service file\n- Start the service and check its status\n- Debugging the service using journalctl\n\n### Prerequisites\n\nTo install and set up the Router Log Preprocessor as a service on Ubuntu, you will need:\n\n- Python 3.8 installed or higher\n- `venv` package (can be installed via `apt-get install python3-venv` command)\n- `pip` package manager (should be included after activating the virtual environment)\n- Internet connection to download the Router Log Preprocessor package from PyPI and the `.env` file from the GitHub repository\n\nNote that some of these prerequisites may already be installed on your Ubuntu system.\nYou can check if Python and pip are installed by running the following commands:\n\n```console\npython3 --version\npip --version\n```\n\nIf both of these commands return the version number of Python and pip, respectively, you\'re good to go.\nOtherwise, you will need to install Python and pip on your Ubuntu system before proceeding.\n\n### Creating a service user\n\nFirst, we will create a service user to run the Router Log Preprocessor.\nThis is a good security practice as running the script as a root user is not needed.\n\nRun the following commands to create a new user called `rlp`:\n\n```console\nsudo adduser rlp --disabled-password --gecos ""\nsudo su rlp\ncd ~\n```\n\nThe first command creates a new user called `rlp` with a disabled password and no additional information. \nThe second command switches to the new user and moves to their home directory.\n\n### Creating a virtual environment\n\nNow that we have a service user set up, we can create a virtual environment to install the Router Log Preprocessor.\nThe following commands create a virtual environment using Python 3.8 and install the Router Log Preprocessor package:\n\n```console\npython3 -m venv venv\ncd venv\nsource bin/activate\npip install router-log-preprocessor\n```\n\nThese commands create a new virtual environment in the venv directory, activate the environment, and install the Router Log Preprocessor package.\n\n### Configuring the environment variables \nWe will create a .env file in the virtual environment directory to store these variables.\nYou can copy the default [.env](https://raw.githubusercontent.com/mastdi/router-log-preprocessor/master/.env) file from the Router Log Preprocessor repository and customize it according to your needs:\n```console\ncurl -o .env https://raw.githubusercontent.com/mastdi/router-log-preprocessor/master/.env\nnano .env\n```\nThis will download the .env file from the Router Log Preprocessor repository and open it in the Nano text editor. \nCustomize the file to set the environment variables you need.\n\nWe are done setting up the servie user:\n\n```console\nexit\n```\n\n### Setting up the logging directory\n\nIf you have set the `LOGGING_DIRECTORY` variable in the .env file to `/var/log/rlp`, you need to create the directory and set the ownership to the rlp user:\n\n```console\nsudo mkdir /var/log/rlp\nsudo chown rlp:rlp /var/log/rlp\n```\n\nThese commands will create the `/var/log/rlp` directory and set the ownership to the `rlp` user.\n\n### Creating the service file\n\nThe next step is to create a service file for the Router Log Preprocessor.\nThis file specifies how the service should be started and managed by the system.\nCreate a new file called rlp.service in the /etc/systemd/system/ directory using the following command:\n\n```console\nsudo nano /etc/systemd/system/rlp.service\n```\n\nThis will open the text editor with a new file.\nCopy the following text into the file:\n\n```ini\n[Unit]\nDescription=Router Log Preprocessor service\nAfter=network.target\n\n[Service]\nUser=rlp\nWorkingDirectory=/home/rlp/venv\nEnvironment="PATH=/home/rlp/venv/bin"\nEnvironmentFile=/home/rlp/venv/.env\nExecStart=/home/rlp/venv/bin/router-log-preprocessor\nRestart=on-failure\nRestartSec=5s\nStartLimitInterval=60s\nStartLimitBurst=3\n\n[Install]\nWantedBy=multi-user.target\n```\n\n\n### Starting the service\n\nThe service is now ready to be started.\nThe final step is to start the service, check if it is running, and ensuring that the service starts automatically on system boot.\nStart the service using the following command:\n```console\nsudo systemctl start rlp.service\n```\n\nThis starts the service based on the configuration we just provided.\nCheck that the service is started using the following command:\n\n```console\nsudo systemctl status rlp.service\n```\n\nThis should show `active (running)` in the console.\nTo make sure the service is started on system boot use the following command:\n\n```console\nsudo systemctl enable rlp.service \n```\n\n### Debugging the service creation\n\nTo debug any issues with the service, you can use the `journalctl` command.\nFor example, to view the logs of the `rlp` service, run the following command:\n\n```console\nsudo journalctl -u rlp.service -e\n```\n\nThis will show the logs of the `rlp` service and the `-e` flag will show the end of the logs.\nYou can use other flags like `-f` to follow the logs in real-time, `-n` to specify the number of lines to show, and `-r` to show the logs in reverse order (most recent first).\n\nIf the service crashes, you can also use the `--since` and `--until` flags to show the logs between a specific time range.\nFor example, to show the logs of the last 10 minutes, run the following command:\n\n```console\nsudo journalctl -u rlp.service --since "10 minutes ago"\n```\nThis will show the logs of the `rlp` service that were generated in the last 10 minutes.\nUse this command to debug any issues with the service.',
     'author': 'Martin Storgaard Dieu',
     'author_email': 'martin@storgaarddieu.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mastdi/router-log-preprocessor',
```

### Comparing `router_log_preprocessor-0.1.4/PKG-INFO` & `router_log_preprocessor-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: router-log-preprocessor
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Home-page: https://github.com/mastdi/router-log-preprocessor
 License: Apache-2.0
 Author: Martin Storgaard Dieu
 Author-email: martin@storgaarddieu.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

