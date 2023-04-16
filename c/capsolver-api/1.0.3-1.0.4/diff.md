# Comparing `tmp/capsolver_api-1.0.3.tar.gz` & `tmp/capsolver_api-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsolver_api-1.0.3.tar", last modified: Sun Apr 16 15:28:50 2023, max compression
+gzip compressed data, was "capsolver_api-1.0.4.tar", last modified: Sun Apr 16 22:07:41 2023, max compression
```

## Comparing `capsolver_api-1.0.3.tar` & `capsolver_api-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 15:28:50.647375 capsolver_api-1.0.3/
--rw-rw-rw-   0        0        0      501 2023-04-16 15:28:50.646863 capsolver_api-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 15:28:50.618523 capsolver_api-1.0.3/capsolver_api/
--rw-rw-rw-   0        0        0      736 2023-04-07 21:00:53.000000 capsolver_api-1.0.3/capsolver_api/__init__.py
--rw-rw-rw-   0        0        0     3853 2023-04-08 10:03:50.000000 capsolver_api-1.0.3/capsolver_api/capsolver_py.py
--rw-rw-rw-   0        0        0      205 2023-04-08 08:44:48.000000 capsolver_api-1.0.3/capsolver_api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:28:50.632427 capsolver_api-1.0.3/capsolver_api/recognitions/
--rw-rw-rw-   0        0        0     1054 2023-04-08 09:37:26.000000 capsolver_api-1.0.3/capsolver_api/recognitions/aws_waf.py
--rw-rw-rw-   0        0        0     1062 2023-04-08 09:37:26.000000 capsolver_api-1.0.3/capsolver_api/recognitions/funcaptcha.py
--rw-rw-rw-   0        0        0     1062 2023-04-08 09:37:26.000000 capsolver_api-1.0.3/capsolver_api/recognitions/hcaptcha.py
--rw-rw-rw-   0        0        0     1301 2023-04-07 20:39:29.000000 capsolver_api-1.0.3/capsolver_api/recognitions/image_to_task.py
--rw-rw-rw-   0        0        0     1007 2023-04-08 09:37:59.000000 capsolver_api-1.0.3/capsolver_api/recognitions/recaptcha.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:28:50.645835 capsolver_api-1.0.3/capsolver_api/tasks/
--rw-rw-rw-   0        0        0     1279 2023-04-08 09:34:47.000000 capsolver_api-1.0.3/capsolver_api/tasks/cloudflare_challenge.py
--rw-rw-rw-   0        0        0     1280 2023-04-08 09:33:49.000000 capsolver_api-1.0.3/capsolver_api/tasks/cloudflare_turnstile.py
--rw-rw-rw-   0        0        0     1302 2023-04-08 09:34:38.000000 capsolver_api-1.0.3/capsolver_api/tasks/datadome.py
--rw-rw-rw-   0        0        0     1544 2023-04-08 09:34:31.000000 capsolver_api-1.0.3/capsolver_api/tasks/funcaptcha.py
--rw-rw-rw-   0        0        0     1874 2023-04-08 09:34:23.000000 capsolver_api-1.0.3/capsolver_api/tasks/geetest.py
--rw-rw-rw-   0        0        0     2047 2023-04-08 09:34:15.000000 capsolver_api-1.0.3/capsolver_api/tasks/hcaptcha.py
--rw-rw-rw-   0        0        0     1250 2023-04-08 09:34:09.000000 capsolver_api-1.0.3/capsolver_api/tasks/mtcaptcha.py
--rw-rw-rw-   0        0        0     2056 2023-04-08 09:34:03.000000 capsolver_api-1.0.3/capsolver_api/tasks/recaptchav2.py
--rw-rw-rw-   0        0        0     2146 2023-04-08 09:33:58.000000 capsolver_api-1.0.3/capsolver_api/tasks/recaptchav3.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:28:50.625218 capsolver_api-1.0.3/capsolver_api.egg-info/
--rw-rw-rw-   0        0        0      501 2023-04-16 15:28:50.000000 capsolver_api-1.0.3/capsolver_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      798 2023-04-16 15:28:50.000000 capsolver_api-1.0.3/capsolver_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 15:28:50.000000 capsolver_api-1.0.3/capsolver_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-16 15:28:50.000000 capsolver_api-1.0.3/capsolver_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 15:28:50.000000 capsolver_api-1.0.3/capsolver_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 15:28:50.647895 capsolver_api-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      872 2023-04-16 15:28:43.000000 capsolver_api-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 22:07:41.636023 capsolver_api-1.0.4/
+-rw-rw-rw-   0        0        0     1083 2023-04-11 20:44:23.000000 capsolver_api-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2708 2023-04-16 22:07:41.636023 capsolver_api-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1993 2023-04-16 21:57:47.000000 capsolver_api-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 22:07:41.603962 capsolver_api-1.0.4/capsolver_api/
+-rw-rw-rw-   0        0        0      736 2023-04-07 21:00:53.000000 capsolver_api-1.0.4/capsolver_api/__init__.py
+-rw-rw-rw-   0        0        0     3853 2023-04-08 10:03:50.000000 capsolver_api-1.0.4/capsolver_api/capsolver_api.py
+-rw-rw-rw-   0        0        0      205 2023-04-08 08:44:48.000000 capsolver_api-1.0.4/capsolver_api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-16 22:07:41.619413 capsolver_api-1.0.4/capsolver_api/recognitions/
+-rw-rw-rw-   0        0        0     1054 2023-04-08 09:37:26.000000 capsolver_api-1.0.4/capsolver_api/recognitions/aws_waf.py
+-rw-rw-rw-   0        0        0     1062 2023-04-08 09:37:26.000000 capsolver_api-1.0.4/capsolver_api/recognitions/funcaptcha.py
+-rw-rw-rw-   0        0        0     1062 2023-04-08 09:37:26.000000 capsolver_api-1.0.4/capsolver_api/recognitions/hcaptcha.py
+-rw-rw-rw-   0        0        0     1301 2023-04-07 20:39:29.000000 capsolver_api-1.0.4/capsolver_api/recognitions/image_to_task.py
+-rw-rw-rw-   0        0        0     1007 2023-04-08 09:37:59.000000 capsolver_api-1.0.4/capsolver_api/recognitions/recaptcha.py
+drwxrwxrwx   0        0        0        0 2023-04-16 22:07:41.634023 capsolver_api-1.0.4/capsolver_api/tasks/
+-rw-rw-rw-   0        0        0     1279 2023-04-08 09:34:47.000000 capsolver_api-1.0.4/capsolver_api/tasks/cloudflare_challenge.py
+-rw-rw-rw-   0        0        0     1280 2023-04-08 09:33:49.000000 capsolver_api-1.0.4/capsolver_api/tasks/cloudflare_turnstile.py
+-rw-rw-rw-   0        0        0     1302 2023-04-08 09:34:38.000000 capsolver_api-1.0.4/capsolver_api/tasks/datadome.py
+-rw-rw-rw-   0        0        0     1544 2023-04-08 09:34:31.000000 capsolver_api-1.0.4/capsolver_api/tasks/funcaptcha.py
+-rw-rw-rw-   0        0        0     1874 2023-04-08 09:34:23.000000 capsolver_api-1.0.4/capsolver_api/tasks/geetest.py
+-rw-rw-rw-   0        0        0     2047 2023-04-08 09:34:15.000000 capsolver_api-1.0.4/capsolver_api/tasks/hcaptcha.py
+-rw-rw-rw-   0        0        0     1250 2023-04-08 09:34:09.000000 capsolver_api-1.0.4/capsolver_api/tasks/mtcaptcha.py
+-rw-rw-rw-   0        0        0     2056 2023-04-08 09:34:03.000000 capsolver_api-1.0.4/capsolver_api/tasks/recaptchav2.py
+-rw-rw-rw-   0        0        0     2146 2023-04-08 09:33:58.000000 capsolver_api-1.0.4/capsolver_api/tasks/recaptchav3.py
+drwxrwxrwx   0        0        0        0 2023-04-16 22:07:41.610409 capsolver_api-1.0.4/capsolver_api.egg-info/
+-rw-rw-rw-   0        0        0     2708 2023-04-16 22:07:41.000000 capsolver_api-1.0.4/capsolver_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      817 2023-04-16 22:07:41.000000 capsolver_api-1.0.4/capsolver_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 22:07:41.000000 capsolver_api-1.0.4/capsolver_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 22:07:41.000000 capsolver_api-1.0.4/capsolver_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-16 22:07:41.000000 capsolver_api-1.0.4/capsolver_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 22:07:41.636023 capsolver_api-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2023-04-16 22:06:09.000000 capsolver_api-1.0.4/setup.py
```

### Comparing `capsolver_api-1.0.3/capsolver_api/__init__.py` & `capsolver_api-1.0.4/capsolver_api/__init__.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.3/capsolver_api/capsolver_py.py` & `capsolver_api-1.0.4/capsolver_api/capsolver_api.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.3/capsolver_api/recognitions/aws_waf.py` & `capsolver_api-1.0.4/capsolver_api/recognitions/aws_waf.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.3/capsolver_api/recognitions/funcaptcha.py` & `capsolver_api-1.0.4/capsolver_api/recognitions/funcaptcha.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.3/capsolver_api/recognitions/hcaptcha.py` & `capsolver_api-1.0.4/capsolver_api/recognitions/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.3/capsolver_api/recognitions/image_to_task.py` & `capsolver_api-1.0.4/capsolver_api/recognitions/image_to_task.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.3/capsolver_api/recognitions/recaptcha.py` & `capsolver_api-1.0.4/capsolver_api/recognitions/recaptcha.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.3/capsolver_api/tasks/cloudflare_challenge.py` & `capsolver_api-1.0.4/capsolver_api/tasks/cloudflare_challenge.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.3/capsolver_api/tasks/cloudflare_turnstile.py` & `capsolver_api-1.0.4/capsolver_api/tasks/cloudflare_turnstile.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.3/capsolver_api/tasks/datadome.py` & `capsolver_api-1.0.4/capsolver_api/tasks/datadome.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.3/capsolver_api/tasks/funcaptcha.py` & `capsolver_api-1.0.4/capsolver_api/tasks/funcaptcha.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.3/capsolver_api/tasks/geetest.py` & `capsolver_api-1.0.4/capsolver_api/tasks/geetest.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.3/capsolver_api/tasks/hcaptcha.py` & `capsolver_api-1.0.4/capsolver_api/tasks/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.3/capsolver_api/tasks/mtcaptcha.py` & `capsolver_api-1.0.4/capsolver_api/tasks/mtcaptcha.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.3/capsolver_api/tasks/recaptchav2.py` & `capsolver_api-1.0.4/capsolver_api/tasks/recaptchav2.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.3/capsolver_api/tasks/recaptchav3.py` & `capsolver_api-1.0.4/capsolver_api/tasks/recaptchav3.py`

 * *Files identical despite different names*

### Comparing `capsolver_api-1.0.3/capsolver_api.egg-info/SOURCES.txt` & `capsolver_api-1.0.4/capsolver_api.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+LICENSE
+README.md
 setup.py
 capsolver_api/__init__.py
-capsolver_api/capsolver_py.py
+capsolver_api/capsolver_api.py
 capsolver_api/exceptions.py
 capsolver_api.egg-info/PKG-INFO
 capsolver_api.egg-info/SOURCES.txt
 capsolver_api.egg-info/dependency_links.txt
 capsolver_api.egg-info/requires.txt
 capsolver_api.egg-info/top_level.txt
 capsolver_api/recognitions/aws_waf.py
```

