# Comparing `tmp/onvif-zeep-async-1.2.9.tar.gz` & `tmp/onvif-zeep-async-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-1.2.9.tar", last modified: Sat Apr 15 22:40:29 2023, max compression
+gzip compressed data, was "onvif-zeep-async-1.3.0.tar", last modified: Mon Apr 17 19:15:14 2023, max compression
```

## Comparing `onvif-zeep-async-1.2.9.tar` & `onvif-zeep-async-1.3.0.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 22:40:29.727860 onvif-zeep-async-1.2.9/
--rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/.pre-commit-config.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-1.2.9/CHANGES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-1.2.9/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-04-15 22:40:29.727908 onvif-zeep-async-1.2.9/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/bandit.yaml
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 22:40:29.719304 onvif-zeep-async-1.2.9/examples/
--rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/examples/events.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/examples/rotate_image.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/examples/streaming.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 22:40:29.719973 onvif-zeep-async-1.2.9/onvif/
--rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    20526 2023-04-15 22:40:06.000000 onvif-zeep-async-1.2.9/onvif/client.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/definition.py
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-04-15 22:40:10.000000 onvif-zeep-async-1.2.9/onvif/version.txt
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 22:40:29.726644 onvif-zeep-async-1.2.9/onvif/wsdl/
--rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/addressing
--rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/b-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/display.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/envelope
--rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/events.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/include
--rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/media.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/onvif.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/r-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/recording.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/replay.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/search.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/t-1.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/types.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/xml.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/onvif/wsdl/xmlmime
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 22:40:29.727602 onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-04-15 22:40:29.000000 onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1417 2023-04-15 22:40:29.000000 onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-04-15 22:40:29.000000 onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-04-15 22:40:29.000000 onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/entry_points.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-04-15 22:40:29.000000 onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-04-15 22:40:29.000000 onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/pyproject.toml
--rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-04-15 22:40:29.728137 onvif-zeep-async-1.2.9/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1801 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-15 22:40:29.727731 onvif-zeep-async-1.2.9/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-09 20:17:08.000000 onvif-zeep-async-1.2.9/tests/test.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-17 19:15:14.950480 onvif-zeep-async-1.3.0/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-1.3.0/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-1.3.0/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-04-17 19:15:14.950532 onvif-zeep-async-1.3.0/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-17 19:15:14.940950 onvif-zeep-async-1.3.0/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-17 19:15:14.941547 onvif-zeep-async-1.3.0/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    23183 2023-04-17 19:14:33.000000 onvif-zeep-async-1.3.0/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-04-17 19:14:58.000000 onvif-zeep-async-1.3.0/onvif/version.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-17 19:15:14.949080 onvif-zeep-async-1.3.0/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)    16384 2023-04-16 04:45:10.000000 onvif-zeep-async-1.3.0/onvif/wsdl/.events.wsdl.swn
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-17 19:15:14.950207 onvif-zeep-async-1.3.0/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-04-17 19:15:14.000000 onvif-zeep-async-1.3.0/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1445 2023-04-17 19:15:14.000000 onvif-zeep-async-1.3.0/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-04-17 19:15:14.000000 onvif-zeep-async-1.3.0/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-04-17 19:15:14.000000 onvif-zeep-async-1.3.0/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-1.3.0/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-04-17 19:15:14.000000 onvif-zeep-async-1.3.0/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-04-17 19:15:14.000000 onvif-zeep-async-1.3.0/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-04-17 19:15:14.950779 onvif-zeep-async-1.3.0/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1801 2023-04-16 08:49:32.000000 onvif-zeep-async-1.3.0/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-04-17 19:15:14.950316 onvif-zeep-async-1.3.0/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-09 20:17:08.000000 onvif-zeep-async-1.3.0/tests/test.py
```

### Comparing `onvif-zeep-async-1.2.9/.gitignore` & `onvif-zeep-async-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/.pre-commit-config.yaml` & `onvif-zeep-async-1.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/LICENSE` & `onvif-zeep-async-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/Makefile` & `onvif-zeep-async-1.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/PKG-INFO` & `onvif-zeep-async-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 1.2.9
+Version: 1.3.0
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-1.2.9/README.rst` & `onvif-zeep-async-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/examples/events.py` & `onvif-zeep-async-1.3.0/examples/events.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/examples/rotate_image.py` & `onvif-zeep-async-1.3.0/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/examples/streaming.py` & `onvif-zeep-async-1.3.0/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/__init__.py` & `onvif-zeep-async-1.3.0/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/client.py` & `onvif-zeep-async-1.3.0/onvif/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 import asyncio
 import contextlib
 import datetime as dt
 from functools import lru_cache
 import logging
 import os.path
 import ssl
-from typing import IO, Any, Dict, Optional, Tuple, Union
+from typing import Any, Dict, Optional, Tuple
 
 import httpx
-from httpx import AsyncClient, BasicAuth, DigestAuth
+from httpx import AsyncClient, BasicAuth, DigestAuth, TransportError
 from zeep.cache import SqliteCache
 from zeep.client import AsyncClient as BaseZeepAsyncClient, Settings
-from zeep.exceptions import Fault
+from zeep.exceptions import Fault, XMLSyntaxError
 import zeep.helpers
 from zeep.loader import parse_xml
 from zeep.proxy import AsyncServiceProxy
-from zeep.transports import AsyncTransport
+from zeep.transports import AsyncTransport, Transport
 from zeep.wsa import WsAddressingPlugin
 from zeep.wsdl import Document
+from zeep.wsdl.bindings.soap import SoapOperation
 from zeep.wsse.username import UsernameToken
 
 from onvif.definition import SERVICES
 from onvif.exceptions import ONVIFAuthError, ONVIFError, ONVIFTimeoutError
 
 logger = logging.getLogger("onvif")
 logging.basicConfig(level=logging.INFO)
@@ -87,47 +88,38 @@
         if self.dt_diff is not None:
             self.created += self.dt_diff
         result = super().apply(envelope, headers)
         self.created = old_created
         return result
 
 
-class AsyncSafeTransport:
-    """A transport that blocks all I/O for zeep."""
+class AsyncSafeTransport(Transport):
+    """A transport that blocks all remote I/O for zeep."""
 
-    def load(self, *args: Any, **kwargs: Any) -> None:
-        """Load the given XML document.
-
-        This should never be called, but we want to raise
-        an error if it is so we know we're doing something wrong
-        and do not accidentally block the event loop.
-        """
-        raise RuntimeError("Loading is not supported in async mode")
+    def load(self, url: str) -> None:
+        """Load the given XML document."""
+        if not _path_isfile(url):
+            raise RuntimeError(f"Loading {url} is not supported in async mode")
+        # Ideally this would happen in the executor but the library
+        # does not call this from a coroutine so the best we can do
+        # without a major refactor is to cache this so it only happens
+        # once per process at startup. Previously it would happen once
+        # per service per camera per setup which is a lot of blocking
+        # I/O in the event loop so this is a major improvement.
+        with open(os.path.expanduser(url), "rb") as fh:
+            return fh.read()
 
 
 _ASYNC_TRANSPORT = AsyncSafeTransport()
 
 
 @lru_cache(maxsize=128)
-def _cached_parse_xml(path: str) -> Any:
+def _cached_document(url: str) -> Document:
     """Load external XML document from disk."""
-    with open(os.path.expanduser(path), "rb") as fh:
-        return parse_xml(fh.read(), _ASYNC_TRANSPORT, settings=_DEFAULT_SETTINGS)
-
-
-class DocumentWithCache(Document):
-    """A WSDL document that supports caching."""
-
-    def _get_xml_document(self, url: Union[IO, str]) -> Any:
-        """Load external XML document from a file-like object or URL."""
-        if _path_isfile(url):
-            return _cached_parse_xml(url)
-        raise RuntimeError(
-            f"Cannot fetch {url} in async mode because it would block the event loop"
-        )
+    return Document(url, _ASYNC_TRANSPORT, settings=_DEFAULT_SETTINGS)
 
 
 class ZeepAsyncClient(BaseZeepAsyncClient):
     """Overwrite create_service method to be async."""
 
     def create_service(self, binding_name, address):
         """Create a new ServiceProxy for the given binding name and address.
@@ -212,25 +204,27 @@
             AsyncTransport(client=client, wsdl_client=wsdl_client)
             if no_cache
             else AsyncTransport(
                 client=client, wsdl_client=wsdl_client, cache=SqliteCache()
             )
         )
         settings = _DEFAULT_SETTINGS
+        self.document = _cached_document(url)
+        self.binding_name = binding_name
         self.zeep_client_authless = ZeepAsyncClient(
-            wsdl=DocumentWithCache(url, self.transport, settings=settings),
+            wsdl=self.document,
             transport=self.transport,
             settings=settings,
             plugins=[WsAddressingPlugin()],
         )
         self.ws_client_authless = self.zeep_client_authless.create_service(
             binding_name, self.xaddr
         )
         self.zeep_client = ZeepAsyncClient(
-            wsdl=DocumentWithCache(url, self.transport, settings=settings),
+            wsdl=self.document,
             wsse=wsse,
             transport=self.transport,
             settings=settings,
             plugins=[WsAddressingPlugin()],
         )
         self.ws_client = self.zeep_client.create_service(binding_name, self.xaddr)
 
@@ -292,17 +286,76 @@
         if builtin:
             return self.__dict__[name]
         if name.startswith("authless_"):
             return service_wrapper(getattr(self.ws_client_authless, name.split("_")[1]))
         return service_wrapper(getattr(self.ws_client, name))
 
 
+class NotificationManager:
+    """Manager to process notifications."""
+
+    def __init__(self, device: "ONVIFCamera", config: Dict[str, Any]) -> None:
+        """Initialize the notification processor."""
+        self._service: Optional[ONVIFService] = None
+        self._operation: Optional[SoapOperation] = None
+        self._device = device
+        self._config = config
+
+    async def setup(self) -> ONVIFService:
+        """Setup the notification processor."""
+        notify_service = self._device.create_notification_service()
+        notify_subscribe = await notify_service.Subscribe(self._config)
+        # pylint: disable=protected-access
+        self._device.xaddrs[
+            "http://www.onvif.org/ver10/events/wsdl/NotificationConsumer"
+        ] = notify_subscribe.SubscriptionReference.Address._value_1
+        # Create subscription manager
+        # 5.2.3 BASIC NOTIFICATION INTERFACE - NOTIFY
+        # Call SetSynchronizationPoint to generate a notification message
+        # to ensure the webhooks are working.
+        #
+        # If this fails this is OK as it just means we will switch
+        # to webhook later when the first notification is received.
+        service = self._device.create_onvif_service(
+            "pullpoint", port_type="NotificationConsumer"
+        )
+        self._operation = service.document.bindings[service.binding_name].get(
+            "PullMessages"
+        )
+        self._service = service
+        return self._device.create_subscription_service("NotificationConsumer")
+
+    async def start(self) -> None:
+        """Start the notification processor."""
+        assert self._service, "Call setup first"
+        try:
+            await self._service.SetSynchronizationPoint()
+        except (Fault, asyncio.TimeoutError, TransportError, TypeError):
+            logger.debug("%s: SetSynchronizationPoint failed", self._service.url)
+
+    def process(self, content: bytes) -> Optional[Any]:
+        """Process a notification message."""
+        if not self._operation:
+            logger.debug("%s: Notifications not setup", self._device.host)
+            return
+        try:
+            envelope = parse_xml(
+                content,  # type: ignore[arg-type]
+                _ASYNC_TRANSPORT,
+                settings=_DEFAULT_SETTINGS,
+            )
+        except XMLSyntaxError as exc:
+            logger.error("Received invalid XML: %s", exc)
+            return None
+        return self._operation.process_reply(envelope)
+
+
 class ONVIFCamera:
     """
-    Python Implemention ONVIF compliant device
+    Python Implementation ONVIF compliant device
     This class integrates onvif services
 
     adjust_time parameter allows authentication on cameras without being time synchronized.
     Please note that using NTP on both end is the recommended solution,
     this should only be used in "safe" environments.
     Also, this cannot be used on AXIS camera, as every request is authenticated, contrary to ONVIF standard
 
@@ -397,14 +450,20 @@
             self.xaddrs[
                 "http://www.onvif.org/ver10/events/wsdl/PullPointSubscription"
             ] = pullpoint.SubscriptionReference.Address._value_1
         except Fault:
             return False
         return True
 
+    def create_notification_manager(
+        self, config: Optional[Dict[str, Any]] = None
+    ) -> NotificationManager:
+        """Create a notification manager."""
+        return NotificationManager(self, config)
+
     async def close(self):
         """Close all transports."""
         await self._snapshot_client.aclose()
         for service in self.services.values():
             await service.close()
 
     async def get_snapshot_uri(self, profile_token):
```

### Comparing `onvif-zeep-async-1.2.9/onvif/definition.py` & `onvif-zeep-async-1.3.0/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/exceptions.py` & `onvif-zeep-async-1.3.0/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/addressing` & `onvif-zeep-async-1.3.0/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-1.3.0/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-1.3.0/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/display.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/envelope` & `onvif-zeep-async-1.3.0/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/events.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/media.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-1.3.0/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-1.3.0/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/search.wsdl` & `onvif-zeep-async-1.3.0/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-1.3.0/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/types.xsd` & `onvif-zeep-async-1.3.0/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-1.3.0/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-1.3.0/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/xml.xsd` & `onvif-zeep-async-1.3.0/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif/wsdl/xmlmime` & `onvif-zeep-async-1.3.0/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-1.3.0/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 1.2.9
+Version: 1.3.0
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-1.2.9/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-1.3.0/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 examples/rotate_image.py
 examples/streaming.py
 onvif/__init__.py
 onvif/client.py
 onvif/definition.py
 onvif/exceptions.py
 onvif/version.txt
+onvif/wsdl/.events.wsdl.swn
 onvif/wsdl/__init__.py
 onvif/wsdl/accesscontrol.wsdl
 onvif/wsdl/actionengine.wsdl
 onvif/wsdl/addressing
 onvif/wsdl/advancedsecurity.wsdl
 onvif/wsdl/analytics.wsdl
 onvif/wsdl/analyticsdevice.wsdl
```

### Comparing `onvif-zeep-async-1.2.9/pylintrc` & `onvif-zeep-async-1.3.0/pylintrc`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-1.2.9/setup.py` & `onvif-zeep-async-1.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages, setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 version_path = os.path.join(here, "onvif/version.txt")
 version = open(version_path).read().strip()
 
-requires = ["httpx>=0.19.0,<1.0.0", "zeep[async]>=4.1.0,<5.0.0"]
+requires = ["httpx>=0.19.0,<1.0.0", "zeep[async]>=4.2.1,<5.0.0"]
 
 CLASSIFIERS = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Customer Service",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
```

### Comparing `onvif-zeep-async-1.2.9/tests/test.py` & `onvif-zeep-async-1.3.0/tests/test.py`

 * *Files identical despite different names*

