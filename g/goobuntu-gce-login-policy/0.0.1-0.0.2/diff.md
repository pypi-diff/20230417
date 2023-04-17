# Comparing `tmp/goobuntu-gce-login-policy-0.0.1.tar.gz` & `tmp/goobuntu-gce-login-policy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goobuntu-gce-login-policy-0.0.1.tar", last modified: Mon Apr 17 00:31:10 2023, max compression
+gzip compressed data, was "goobuntu-gce-login-policy-0.0.2.tar", last modified: Mon Apr 17 01:46:00 2023, max compression
```

## Comparing `goobuntu-gce-login-policy-0.0.1.tar` & `goobuntu-gce-login-policy-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
-drwxrwxr-x   0 jarrah    (1000) jarrah    (1000)        0 2023-04-17 00:31:10.246321 goobuntu-gce-login-policy-0.0.1/
--rw-rw-r--   0 jarrah    (1000) jarrah    (1000)      752 2023-04-17 00:31:10.246321 goobuntu-gce-login-policy-0.0.1/PKG-INFO
--rw-rw-r--   0 jarrah    (1000) jarrah    (1000)       63 2023-04-17 00:20:24.973022 goobuntu-gce-login-policy-0.0.1/setup.cfg
--rw-rw-r--   0 jarrah    (1000) jarrah    (1000)     1590 2023-04-17 00:31:05.410251 goobuntu-gce-login-policy-0.0.1/setup.py
+drwxrwxr-x   0 jarrah    (1000) jarrah    (1000)        0 2023-04-17 01:46:00.255133 goobuntu-gce-login-policy-0.0.2/
+-rw-rw-r--   0 jarrah    (1000) jarrah    (1000)      534 2023-04-17 01:46:00.255133 goobuntu-gce-login-policy-0.0.2/PKG-INFO
+-rw-rw-r--   0 jarrah    (1000) jarrah    (1000)       33 2023-04-17 01:41:00.442723 goobuntu-gce-login-policy-0.0.2/setup.cfg
+-rw-rw-r--   0 jarrah    (1000) jarrah    (1000)     1105 2023-04-17 01:45:56.343076 goobuntu-gce-login-policy-0.0.2/setup.py
```

