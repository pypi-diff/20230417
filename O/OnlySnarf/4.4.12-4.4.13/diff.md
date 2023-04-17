# Comparing `tmp/OnlySnarf-4.4.12.tar.gz` & `tmp/OnlySnarf-4.4.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OnlySnarf-4.4.12.tar", last modified: Fri Mar 24 19:03:56 2023, max compression
+gzip compressed data, was "OnlySnarf-4.4.13.tar", last modified: Mon Apr 17 17:48:33 2023, max compression
```

## Comparing `OnlySnarf-4.4.12.tar` & `OnlySnarf-4.4.13.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-03-24 19:03:56.382163 OnlySnarf-4.4.12/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    29932 2023-03-24 19:03:20.000000 OnlySnarf-4.4.12/CHANGELOG.md
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1064 2023-03-17 21:48:54.000000 OnlySnarf-4.4.12/LICENSE.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      141 2023-03-17 21:48:54.000000 OnlySnarf-4.4.12/MANIFEST.in
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-03-24 19:03:56.378163 OnlySnarf-4.4.12/OnlySnarf/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-03-17 21:48:54.000000 OnlySnarf-4.4.12/OnlySnarf/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      387 2023-03-23 21:28:52.000000 OnlySnarf-4.4.12/OnlySnarf/__main__.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-03-24 19:03:56.378163 OnlySnarf-4.4.12/OnlySnarf/classes/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-03-17 21:48:54.000000 OnlySnarf-4.4.12/OnlySnarf/classes/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4388 2023-03-23 21:28:52.000000 OnlySnarf-4.4.12/OnlySnarf/classes/discount.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1892 2023-03-17 21:48:54.000000 OnlySnarf-4.4.12/OnlySnarf/classes/element.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15697 2023-03-22 19:25:25.000000 OnlySnarf-4.4.12/OnlySnarf/classes/file.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12176 2023-03-23 21:28:52.000000 OnlySnarf-4.4.12/OnlySnarf/classes/message.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1974 2023-03-18 05:22:21.000000 OnlySnarf-4.4.12/OnlySnarf/classes/poll.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    13655 2023-03-23 21:28:52.000000 OnlySnarf-4.4.12/OnlySnarf/classes/profile.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    10171 2023-03-23 21:28:52.000000 OnlySnarf-4.4.12/OnlySnarf/classes/promotion.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4922 2023-03-23 21:28:52.000000 OnlySnarf-4.4.12/OnlySnarf/classes/schedule.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    18008 2023-03-23 19:53:10.000000 OnlySnarf-4.4.12/OnlySnarf/classes/user.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-03-24 19:03:56.378163 OnlySnarf-4.4.12/OnlySnarf/conf/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2240 2023-03-23 21:28:52.000000 OnlySnarf-4.4.12/OnlySnarf/conf/config.conf
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2262 2023-03-23 21:28:52.000000 OnlySnarf-4.4.12/OnlySnarf/conf/test-config.conf
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-03-24 19:03:56.378163 OnlySnarf-4.4.12/OnlySnarf/elements/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-03-17 21:48:54.000000 OnlySnarf-4.4.12/OnlySnarf/elements/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15689 2023-03-17 21:48:54.000000 OnlySnarf-4.4.12/OnlySnarf/elements/driver.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1401 2023-03-17 21:48:54.000000 OnlySnarf-4.4.12/OnlySnarf/elements/login.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    11335 2023-03-17 21:48:54.000000 OnlySnarf-4.4.12/OnlySnarf/elements/profile.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-03-24 19:03:56.378163 OnlySnarf-4.4.12/OnlySnarf/lib/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-03-17 21:48:54.000000 OnlySnarf-4.4.12/OnlySnarf/lib/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)   163102 2023-03-24 19:03:16.000000 OnlySnarf-4.4.12/OnlySnarf/lib/driver.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     9500 2023-03-17 21:48:54.000000 OnlySnarf-4.4.12/OnlySnarf/lib/ffmpeg.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5069 2023-03-24 18:59:04.000000 OnlySnarf-4.4.12/OnlySnarf/snarf.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-03-24 19:03:56.382163 OnlySnarf-4.4.12/OnlySnarf/util/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-03-17 21:48:54.000000 OnlySnarf-4.4.12/OnlySnarf/util/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1321 2023-03-24 17:52:07.000000 OnlySnarf-4.4.12/OnlySnarf/util/args.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1062 2023-03-17 21:48:54.000000 OnlySnarf-4.4.12/OnlySnarf/util/colorize.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1440 2023-03-23 21:28:52.000000 OnlySnarf-4.4.12/OnlySnarf/util/config.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2954 2023-03-23 21:28:52.000000 OnlySnarf-4.4.12/OnlySnarf/util/defaults.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2025 2023-03-17 21:48:54.000000 OnlySnarf-4.4.12/OnlySnarf/util/logger.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12085 2023-03-24 17:52:07.000000 OnlySnarf-4.4.12/OnlySnarf/util/optional_args.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    19010 2023-03-24 19:03:17.000000 OnlySnarf-4.4.12/OnlySnarf/util/settings.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3725 2023-03-23 21:28:52.000000 OnlySnarf-4.4.12/OnlySnarf/util/validators.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-03-24 19:03:56.378163 OnlySnarf-4.4.12/OnlySnarf.egg-info/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3266 2023-03-24 19:03:56.000000 OnlySnarf-4.4.12/OnlySnarf.egg-info/PKG-INFO
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1153 2023-03-24 19:03:56.000000 OnlySnarf-4.4.12/OnlySnarf.egg-info/SOURCES.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        1 2023-03-24 19:03:56.000000 OnlySnarf-4.4.12/OnlySnarf.egg-info/dependency_links.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       47 2023-03-24 19:03:56.000000 OnlySnarf-4.4.12/OnlySnarf.egg-info/entry_points.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       53 2023-03-24 19:03:56.000000 OnlySnarf-4.4.12/OnlySnarf.egg-info/requires.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       91 2023-03-24 19:03:56.000000 OnlySnarf-4.4.12/OnlySnarf.egg-info/top_level.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3266 2023-03-24 19:03:56.382163 OnlySnarf-4.4.12/PKG-INFO
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2636 2023-03-23 23:07:26.000000 OnlySnarf-4.4.12/README.md
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-03-24 19:03:56.382163 OnlySnarf-4.4.12/setup.cfg
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1285 2023-03-24 18:48:31.000000 OnlySnarf-4.4.12/setup.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-03-24 19:03:56.382163 OnlySnarf-4.4.12/tests/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1209 2023-03-17 21:48:54.000000 OnlySnarf-4.4.12/tests/test_profile.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1451 2023-03-17 21:48:54.000000 OnlySnarf-4.4.12/tests/test_promotion.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    30127 2023-04-17 17:48:00.000000 OnlySnarf-4.4.13/CHANGELOG.md
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1064 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/LICENSE.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      141 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/MANIFEST.in
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.716371 OnlySnarf-4.4.13/OnlySnarf/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      387 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/__main__.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/OnlySnarf/classes/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4388 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/discount.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1892 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/element.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15697 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/file.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12176 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/message.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1974 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/poll.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    13655 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/profile.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    10171 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/promotion.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4922 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/schedule.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    18008 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/classes/user.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/OnlySnarf/conf/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2240 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/conf/config.conf
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2262 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/conf/test-config.conf
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/OnlySnarf/elements/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/elements/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15689 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/elements/driver.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1401 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/elements/login.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    11335 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/elements/profile.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/OnlySnarf/lib/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/lib/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)   163434 2023-04-17 17:48:00.000000 OnlySnarf-4.4.13/OnlySnarf/lib/driver.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     9500 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/lib/ffmpeg.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5069 2023-04-17 17:48:00.000000 OnlySnarf-4.4.13/OnlySnarf/snarf.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/OnlySnarf/util/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/util/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1321 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/util/args.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1062 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/util/colorize.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1482 2023-04-17 17:48:00.000000 OnlySnarf-4.4.13/OnlySnarf/util/config.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3114 2023-04-17 17:48:00.000000 OnlySnarf-4.4.13/OnlySnarf/util/defaults.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2025 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/util/logger.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12152 2023-04-17 17:48:00.000000 OnlySnarf-4.4.13/OnlySnarf/util/optional_args.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    19125 2023-04-17 17:48:00.000000 OnlySnarf-4.4.13/OnlySnarf/util/settings.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3725 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/OnlySnarf/util/validators.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.716371 OnlySnarf-4.4.13/OnlySnarf.egg-info/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3266 2023-04-17 17:48:33.000000 OnlySnarf-4.4.13/OnlySnarf.egg-info/PKG-INFO
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1153 2023-04-17 17:48:33.000000 OnlySnarf-4.4.13/OnlySnarf.egg-info/SOURCES.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        1 2023-04-17 17:48:33.000000 OnlySnarf-4.4.13/OnlySnarf.egg-info/dependency_links.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       47 2023-04-17 17:48:33.000000 OnlySnarf-4.4.13/OnlySnarf.egg-info/entry_points.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       53 2023-04-17 17:48:33.000000 OnlySnarf-4.4.13/OnlySnarf.egg-info/requires.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       91 2023-04-17 17:48:33.000000 OnlySnarf-4.4.13/OnlySnarf.egg-info/top_level.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3266 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/PKG-INFO
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2636 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/README.md
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/setup.cfg
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1285 2023-04-17 17:48:00.000000 OnlySnarf-4.4.13/setup.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-17 17:48:33.720371 OnlySnarf-4.4.13/tests/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1209 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/tests/test_profile.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1451 2023-04-16 06:45:34.000000 OnlySnarf-4.4.13/tests/test_promotion.py
```

### Comparing `OnlySnarf-4.4.12/CHANGELOG.md` & `OnlySnarf-4.4.13/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -673,15 +673,21 @@
   - removed nonworking browser references in optional args
   - fixed discount bug
 **4.4.12: 3/24/2023**
   - RPi4 debugging
   - fixed element bug when posting
   - fixed users
   - fixed error message on close
-  
+  **4/15/2023**
+  - cleaned up git repo size / long clone time
+**4.4.13: 4/17/2023**
+  - Windows compatability testing
+  - updated pathings for Windows
+  - retested google login (remains disabled)
+
 ------------------------------------------------------------------------------------
 
 ## TODO
 
 - add bypass for 2fa
 https://www.geeksforgeeks.org/two-factor-authentication-using-google-authenticator-in-python/
 https://stackoverflow.com/questions/55870489/how-to-handle-google-authenticator-with-selenium
```

### Comparing `OnlySnarf-4.4.12/LICENSE.txt` & `OnlySnarf-4.4.13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/classes/discount.py` & `OnlySnarf-4.4.13/OnlySnarf/classes/discount.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/classes/element.py` & `OnlySnarf-4.4.13/OnlySnarf/classes/element.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/classes/file.py` & `OnlySnarf-4.4.13/OnlySnarf/classes/file.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/classes/message.py` & `OnlySnarf-4.4.13/OnlySnarf/classes/message.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/classes/poll.py` & `OnlySnarf-4.4.13/OnlySnarf/classes/poll.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/classes/profile.py` & `OnlySnarf-4.4.13/OnlySnarf/classes/profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/classes/promotion.py` & `OnlySnarf-4.4.13/OnlySnarf/classes/promotion.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/classes/schedule.py` & `OnlySnarf-4.4.13/OnlySnarf/classes/schedule.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/classes/user.py` & `OnlySnarf-4.4.13/OnlySnarf/classes/user.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/conf/config.conf` & `OnlySnarf-4.4.13/OnlySnarf/conf/config.conf`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/conf/test-config.conf` & `OnlySnarf-4.4.13/OnlySnarf/conf/test-config.conf`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/elements/driver.py` & `OnlySnarf-4.4.13/OnlySnarf/elements/driver.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/elements/login.py` & `OnlySnarf-4.4.13/OnlySnarf/elements/login.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/elements/profile.py` & `OnlySnarf-4.4.13/OnlySnarf/elements/profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/lib/driver.py` & `OnlySnarf-4.4.13/OnlySnarf/lib/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -2824,15 +2824,21 @@
         def add_options(options):
             if str(Settings.is_show_window()) == "False":
                 options.add_argument('--headless')
             options.add_argument("--no-sandbox") # Bypass OS security model
             options.add_argument("--disable-gpu")
             options.add_argument("--disable-extensions")
             options.add_argument("--disable-dev-shm-usage")
-            options.add_argument("user-data-dir=/tmp/selenium") # do not disable, required for cookies to work 
+
+            # if os.name == 'nt':
+                # options.add_argument(r"--user-data-dir=C:\Users\brain\AppData\Local\Google\Chrome\User Data")
+            # else:
+                # options.add_argument("--user-data-dir="+os.path.join(Settings.get_base_directory(),"tmp","selenium")) # do not disable, required for cookies to work 
+            options.add_argument(r'--profile-directory=Alex D') #e.g. Profile 3
+            
             # options.add_argument("--allow-insecure-localhost")            
             # possibly linux only
             # options.add_argument('disable-notifications')
             # https://stackoverflow.com/questions/50642308/webdriverexception-unknown-error-devtoolsactiveport-file-doesnt-exist-while-t
             # options.add_arguments("start-maximized"); // open Browser in maximized mode
             # options.add_argument("--window-size=1920,1080")
             # options.add_argument("--disable-crash-reporter")
@@ -3061,17 +3067,17 @@
             if os.environ.get("ENV") and str(os.environ.get("ENV")) == "test": return False
             os._exit(1)
 
         browser.implicitly_wait(30) # seconds
         browser.set_page_load_timeout(1200)
         browser.file_detector = LocalFileDetector() # for uploading via remote sessions
         if str(Settings.is_show_window()) == "False":
-            Settings.print("browser created - {} (headless)".format(browserType))
+            Settings.print("browser spawned successfully (headless)".format(browserType))
         else:
-            Settings.print("browser created - {}".format(browserType))
+            Settings.print("browser spawned successfully".format(browserType))
         return browser
 
     ## possibly move these functions elsewhere (again)
     def read_session_data(self):
         Settings.maybe_print("reading local session")
         path_ = os.path.join(Settings.get_base_directory(), "session.json")
         Settings.dev_print("local session path: "+str(path_))
```

### Comparing `OnlySnarf-4.4.12/OnlySnarf/lib/ffmpeg.py` & `OnlySnarf-4.4.13/OnlySnarf/lib/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/snarf.py` & `OnlySnarf-4.4.13/OnlySnarf/snarf.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/util/args.py` & `OnlySnarf-4.4.13/OnlySnarf/util/args.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/util/colorize.py` & `OnlySnarf-4.4.13/OnlySnarf/util/colorize.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/util/config.py` & `OnlySnarf-4.4.13/OnlySnarf/util/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # parse config file while maintaining default values from args
 
 import configparser
 import os
 
 ## SAME as Settings.get_base_directory ##
-USER = os.getenv('USER')
+import getpass
+USER = getpass.getuser()
+# USER = os.getenv('USER')
 if str(os.getenv('SUDO_USER')) != "root" and str(os.getenv('SUDO_USER')) != "None":
     USER = os.getenv('SUDO_USER')
 configFile = "config.conf"
 if os.environ.get('ENV') == "test":
   configFile = os.path.join(os.getcwd(), "OnlySnarf/conf", "test-config.conf")
 elif os.path.isfile(os.path.join("/home/{}/.onlysnarf/conf".format(USER), "config.conf")):
   configFile = os.path.join("/home/{}/.onlysnarf/conf".format(USER), "config.conf")
```

### Comparing `OnlySnarf-4.4.12/OnlySnarf/util/defaults.py` & `OnlySnarf-4.4.13/OnlySnarf/util/defaults.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,30 +66,38 @@
 
 USER_LIMIT = 10
 
 #########
 # Paths #
 #########
 
-USER = os.getenv('USER')
+import getpass
+USER = getpass.getuser()
+# USER = os.getenv('USER')
 if str(os.getenv('SUDO_USER')) != "root" and str(os.getenv('SUDO_USER')) != "None":
     USER = os.getenv('SUDO_USER')
 
-ROOT_PATH = "/home/{}/.onlysnarf".format(USER)
+# linux default
+HOME_DIR = "/home"
+# check for Windows
+if os.name == 'nt':
+    HOME_DIR = "C:\\Users"
+ROOT_PATH = os.path.join(HOME_DIR, USER, ".onlysnarf")
+    
 DOWNLOAD_PATH = os.path.join(ROOT_PATH, "downloads")
 UPLOAD_PATH = os.path.join(ROOT_PATH, "uploads")
 LOG_PATH = os.path.join(ROOT_PATH, "snarf.log")
 REMOTE_PATH = ROOT_PATH
 CONFIGS_PATH = os.path.join(ROOT_PATH, "conf")
 USERS_PATH = os.path.join(CONFIGS_PATH, "users.json")
 PROFILE_PATH = os.path.join(CONFIGS_PATH, "profile.json")
 CONFIG_PATH = os.path.join(CONFIGS_PATH, "config.conf")
 if os.environ.get('ENV') == "test":
     # CONFIG_PATH = os.path.join(CONFIGS_PATH, "test-config.conf")
-    CONFIG_PATH = os.path.join(os.getcwd(), "OnlySnarf/conf", "test-config.conf")
+    CONFIG_PATH = os.path.join(os.getcwd(), "OnlySnarf", "conf", "test-config.conf")
 PROFILES_PATH = os.path.join(CONFIGS_PATH, "users")
 
 if os.environ.get('ENV') == "test":
     print("Paths:")
     print("root: "+ROOT_PATH)
     print("configs: "+CONFIGS_PATH)
     print("config: "+CONFIG_PATH)
```

### Comparing `OnlySnarf-4.4.12/OnlySnarf/util/logger.py` & `OnlySnarf-4.4.13/OnlySnarf/util/logger.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf/util/optional_args.py` & `OnlySnarf-4.4.13/OnlySnarf/util/optional_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
   ##
   # -browser
   parser.add_argument('-browser', '-B', type=str, default="auto", choices=["auto","brave","chrome","chromium","firefox","remote"], dest='browser', help='web browser to use')
   # parser.add_argument('-browser', '-B', type=str, default="auto", choices=["auto","brave","chrome","chromium","firefox","ie","edge","opera","remote"], dest='browser', help='web browser to use')
   ##
   # -login
   # method to prefer when logging in
+  # note: "google" is disabled due to updates&testing requirements
   parser.add_argument('-login', '-L', dest='login', default="auto", choices=["auto","onlyfans","twitter"], help='method of user login to prefer')
   ##
   # -reduce
   # enables file reduction
   parser.add_argument('-reduce', action='store_true', dest='reduce', help='enable reducing files over 50 MB')
   ##
   # --save
```

### Comparing `OnlySnarf-4.4.12/OnlySnarf/util/settings.py` & `OnlySnarf-4.4.13/OnlySnarf/util/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,43 +399,45 @@
 
     def get_user_config(username="default"):
         import configparser
         config_file = configparser.ConfigParser()
         # strip email
         if "@" in username: username = username[0 : username.index("@")]
         Settings.dev_print("retrieving user config: {}".format(username))
+        Settings.dev_print(os.path.join(Settings.get_base_directory(), "conf", "users", username+".conf"))
         config_file.read(os.path.join(Settings.get_base_directory(), "conf", "users", username+".conf"))
         userConfig = {}
         for section in config_file.sections():
-            # print(section)
+            # Settings.dev_print(section)
             for key in config_file[section]:
-                # print(section, key, config_file[section][key].strip("\""))
+                # Settings.dev_print(section, key, config_file[section][key].strip("\""))
                 userConfig[section.lower()+"_"+key.lower()] = config_file[section][key].strip("\"")
+        # Settings.dev_print(userConfig)
         return userConfig
 
     def get_username():
         return config["username"] or "default"
 
     def get_username_onlyfans():
         try:
             return Settings.get_user_config(Settings.get_username())["onlyfans_username"]
         except Exception as e:
             Settings.err_print(e)
         return ""
 
     def get_username_google():
         try:
-            return config["google_username"] or Settings.get_user_config(Settings.get_username())["google_username"]
+            return Settings.get_user_config(Settings.get_username())["google_username"]
         except Exception as e:
             Settings.err_print(e)
         return ""            
 
     def get_username_twitter():
         try:
-            return config["twitter_username"] or Settings.get_user_config(Settings.get_username())["twitter_username"]
+            return Settings.get_user_config(Settings.get_username())["twitter_username"]
         except Exception as e:
             Settings.err_print(e)
         return ""
 
     def get_remote_browser_host():
         return config["remote_browser_host"]
```

### Comparing `OnlySnarf-4.4.12/OnlySnarf/util/validators.py` & `OnlySnarf-4.4.13/OnlySnarf/util/validators.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/OnlySnarf.egg-info/PKG-INFO` & `OnlySnarf-4.4.13/OnlySnarf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OnlySnarf
-Version: 4.4.12
+Version: 4.4.13
 Summary: OnlyFans Content Distribution Tool
 Home-page: https://github.com/skeetzo/onlysnarf
 Author: Skeetzo
 Author-email: WebmasterSkeetzo@gmail.com
 Keywords: OnlyFans,OnlySnarf,selenium,snarf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OnlySnarf Version: 4.4.12 Summary: OnlyFans Content
+Metadata-Version: 2.1 Name: OnlySnarf Version: 4.4.13 Summary: OnlyFans Content
 Distribution Tool Home-page: https://github.com/skeetzo/onlysnarf Author:
 Skeetzo Author-email: WebmasterSkeetzo@gmail.com Keywords:
 OnlyFans,OnlySnarf,selenium,snarf Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: System :: Emulators Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `OnlySnarf-4.4.12/OnlySnarf.egg-info/SOURCES.txt` & `OnlySnarf-4.4.13/OnlySnarf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/PKG-INFO` & `OnlySnarf-4.4.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OnlySnarf
-Version: 4.4.12
+Version: 4.4.13
 Summary: OnlyFans Content Distribution Tool
 Home-page: https://github.com/skeetzo/onlysnarf
 Author: Skeetzo
 Author-email: WebmasterSkeetzo@gmail.com
 Keywords: OnlyFans,OnlySnarf,selenium,snarf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OnlySnarf Version: 4.4.12 Summary: OnlyFans Content
+Metadata-Version: 2.1 Name: OnlySnarf Version: 4.4.13 Summary: OnlyFans Content
 Distribution Tool Home-page: https://github.com/skeetzo/onlysnarf Author:
 Skeetzo Author-email: WebmasterSkeetzo@gmail.com Keywords:
 OnlyFans,OnlySnarf,selenium,snarf Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: System :: Emulators Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `OnlySnarf-4.4.12/README.md` & `OnlySnarf-4.4.13/README.md`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/setup.py` & `OnlySnarf-4.4.13/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="OnlySnarf",
-    version="4.4.12",
+    version="4.4.13",
     author="Skeetzo",
     author_email="WebmasterSkeetzo@gmail.com",
     url = 'https://github.com/skeetzo/onlysnarf',
     keywords = ['OnlyFans', 'OnlySnarf', 'selenium', 'snarf'],
     description="OnlyFans Content Distribution Tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `OnlySnarf-4.4.12/tests/test_profile.py` & `OnlySnarf-4.4.13/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.4.12/tests/test_promotion.py` & `OnlySnarf-4.4.13/tests/test_promotion.py`

 * *Files identical despite different names*

