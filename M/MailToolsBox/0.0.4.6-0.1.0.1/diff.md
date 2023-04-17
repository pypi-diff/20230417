# Comparing `tmp/MailToolsBox-0.0.4.6.tar.gz` & `tmp/MailToolsBox-0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MailToolsBox-0.0.4.6.tar", last modified: Fri Sep 20 19:51:06 2019, max compression
+gzip compressed data, was "MailToolsBox-0.1.0.1.tar", last modified: Mon Apr 17 11:40:50 2023, max compression
```

## Comparing `MailToolsBox-0.0.4.6.tar` & `MailToolsBox-0.1.0.1.tar`

### file list

```diff
@@ -1,8 +1,16 @@
-drwxrwxr-x   0 rambod    (1000) rambod    (1000)        0 2019-09-20 19:51:06.000000 MailToolsBox-0.0.4.6/
-drwxrwxr-x   0 rambod    (1000) rambod    (1000)        0 2019-09-20 19:51:06.000000 MailToolsBox-0.0.4.6/MailToolsBox/
--rw-rw-r--   0 rambod    (1000) rambod    (1000)       92 2019-09-20 18:37:19.000000 MailToolsBox-0.0.4.6/MailToolsBox/__init__.py
--rw-rw-r--   0 rambod    (1000) rambod    (1000)     5263 2019-09-20 19:14:57.000000 MailToolsBox-0.0.4.6/MailToolsBox/imapClient.py
--rw-r--r--   0 rambod    (1000) rambod    (1000)      979 2019-09-09 20:10:57.000000 MailToolsBox-0.0.4.6/MailToolsBox/mailSender.py
--rw-rw-r--   0 rambod    (1000) rambod    (1000)     2685 2019-09-20 19:51:06.000000 MailToolsBox-0.0.4.6/PKG-INFO
--rw-rw-r--   0 rambod    (1000) rambod    (1000)     1625 2019-09-20 19:43:10.000000 MailToolsBox-0.0.4.6/README.rst
--rw-rw-r--   0 rambod    (1000) rambod    (1000)     1314 2019-09-20 19:50:13.000000 MailToolsBox-0.0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:40:50.966057 MailToolsBox-0.1.0.1/
+-rw-rw-rw-   0        0        0     1084 2023-04-16 11:08:50.000000 MailToolsBox-0.1.0.1/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 11:40:50.954059 MailToolsBox-0.1.0.1/MailToolsBox/
+-rw-rw-rw-   0        0        0       94 2023-04-16 11:08:50.000000 MailToolsBox-0.1.0.1/MailToolsBox/__init__.py
+-rw-rw-rw-   0        0        0     5190 2023-04-17 09:46:20.000000 MailToolsBox-0.1.0.1/MailToolsBox/imapClient.py
+-rw-rw-rw-   0        0        0     3853 2023-04-17 09:46:24.000000 MailToolsBox-0.1.0.1/MailToolsBox/mailSender.py
+drwxrwxrwx   0        0        0        0 2023-04-17 11:40:50.964056 MailToolsBox-0.1.0.1/MailToolsBox.egg-info/
+-rw-rw-rw-   0        0        0     3489 2023-04-17 11:40:50.000000 MailToolsBox-0.1.0.1/MailToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-04-17 11:40:50.000000 MailToolsBox-0.1.0.1/MailToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 11:40:50.000000 MailToolsBox-0.1.0.1/MailToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-17 11:40:50.000000 MailToolsBox-0.1.0.1/MailToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-17 11:40:50.000000 MailToolsBox-0.1.0.1/MailToolsBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3489 2023-04-17 11:40:50.966057 MailToolsBox-0.1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2723 2023-04-17 11:23:42.000000 MailToolsBox-0.1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-17 11:40:50.967055 MailToolsBox-0.1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1381 2023-04-17 11:32:27.000000 MailToolsBox-0.1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

