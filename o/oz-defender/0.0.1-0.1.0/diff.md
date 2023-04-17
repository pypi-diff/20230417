# Comparing `tmp/oz_defender-0.0.1.tar.gz` & `tmp/oz_defender-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oz_defender-0.0.1.tar", max compression
+gzip compressed data, was "oz_defender-0.1.0.tar", max compression
```

## Comparing `oz_defender-0.0.1.tar` & `oz_defender-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,6 @@
--rw-r--r--   0        0        0     1063 2023-04-17 14:22:35.535570 oz_defender-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-16 23:14:31.460410 oz_defender-0.0.1/oz_defender/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 23:14:31.460579 oz_defender-0.0.1/oz_defender/relay/__init__.py
--rw-r--r--   0        0        0     2764 2023-04-17 15:14:00.184602 oz_defender-0.0.1/oz_defender/relay/client.py
--rw-r--r--   0        0        0      167 2023-04-17 15:14:00.184950 oz_defender-0.0.1/oz_defender/relay/exceptions.py
--rw-r--r--   0        0        0      710 2023-04-17 15:15:10.842644 oz_defender-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 oz_defender-0.0.1/setup.py
--rw-r--r--   0        0        0     1679 1970-01-01 00:00:00.000000 oz_defender-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      161 2023-01-27 00:46:21.077437 oz_defender-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 23:14:31.460410 oz_defender-0.1.0/oz_defender/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 23:14:31.460579 oz_defender-0.1.0/oz_defender/relay/__init__.py
+-rw-r--r--   0        0        0      323 2023-04-17 10:25:27.073309 oz_defender-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 oz_defender-0.1.0/setup.py
+-rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 oz_defender-0.1.0/PKG-INFO
```

