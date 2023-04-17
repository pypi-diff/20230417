# Comparing `tmp/ethereal-0.1.0.tar.gz` & `tmp/ethereal-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethereal-0.1.0.tar", max compression
+gzip compressed data, was "ethereal-0.1.1.tar", max compression
```

## Comparing `ethereal-0.1.0.tar` & `ethereal-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-04-02 19:03:02.167776 ethereal-0.1.0/LICENSE
--rw-r--r--   0        0        0       11 2023-04-02 19:07:10.971245 ethereal-0.1.0/ethereal/__init__.py
--rw-r--r--   0        0        0      301 2023-04-02 19:04:50.462088 ethereal-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      497 2023-04-02 19:07:23.901137 ethereal-0.1.0/setup.py
--rw-r--r--   0        0        0      309 2023-04-02 19:07:23.901255 ethereal-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-02 19:03:02.167776 ethereal-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1308 2023-04-16 07:11:11.928618 ethereal-0.1.1/ethereal/__init__.py
+-rw-r--r--   0        0        0     1402 2023-04-14 14:08:02.175740 ethereal-0.1.1/ethereal/app.py
+-rw-r--r--   0        0        0      288 2023-04-14 18:53:08.549415 ethereal-0.1.1/ethereal/base.py
+-rw-r--r--   0        0        0     6978 2023-04-16 06:36:31.316428 ethereal-0.1.1/ethereal/cache.py
+-rw-r--r--   0        0        0      971 2023-04-14 18:52:21.303480 ethereal-0.1.1/ethereal/containers.py
+-rw-r--r--   0        0        0     8806 2023-04-17 07:14:39.659777 ethereal-0.1.1/ethereal/contracts.py
+-rw-r--r--   0        0        0     4652 2023-04-14 18:47:51.186401 ethereal-0.1.1/ethereal/etherscan.py
+-rw-r--r--   0        0        0     3175 2023-04-14 14:31:35.858070 ethereal-0.1.1/ethereal/facade.py
+-rw-r--r--   0        0        0     1439 2023-04-14 18:59:17.941096 ethereal-0.1.1/ethereal/networks.py
+-rw-r--r--   0        0        0      532 2023-04-17 07:22:56.553897 ethereal-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      702 2023-04-17 18:04:11.416973 ethereal-0.1.1/setup.py
+-rw-r--r--   0        0        0      520 2023-04-17 18:04:11.417119 ethereal-0.1.1/PKG-INFO
```

### Comparing `ethereal-0.1.0/LICENSE` & `ethereal-0.1.1/LICENSE`

 * *Files identical despite different names*

