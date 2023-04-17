# Comparing `tmp/django-forbid-0.0.5.tar.gz` & `tmp/django-forbid-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-forbid-0.0.5.tar", last modified: Fri Apr 14 15:00:56 2023, max compression
+gzip compressed data, was "django-forbid-0.0.6.tar", last modified: Mon Apr 17 15:36:39 2023, max compression
```

## Comparing `django-forbid-0.0.5.tar` & `django-forbid-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:56.387156 django-forbid-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-14 15:00:45.000000 django-forbid-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-14 15:00:56.387156 django-forbid-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-14 15:00:45.000000 django-forbid-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-14 15:00:45.000000 django-forbid-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-14 15:00:56.387156 django-forbid-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 15:00:45.000000 django-forbid-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:56.383156 django-forbid-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:56.387156 django-forbid-0.0.5/src/django_forbid/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 15:00:45.000000 django-forbid-0.0.5/src/django_forbid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-14 15:00:45.000000 django-forbid-0.0.5/src/django_forbid/access.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-14 15:00:45.000000 django-forbid-0.0.5/src/django_forbid/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-14 15:00:45.000000 django-forbid-0.0.5/src/django_forbid/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-14 15:00:45.000000 django-forbid-0.0.5/src/django_forbid/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-14 15:00:45.000000 django-forbid-0.0.5/src/django_forbid/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:00:56.387156 django-forbid-0.0.5/src/django_forbid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-14 15:00:56.000000 django-forbid-0.0.5/src/django_forbid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-14 15:00:56.000000 django-forbid-0.0.5/src/django_forbid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:00:56.000000 django-forbid-0.0.5/src/django_forbid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:00:56.000000 django-forbid-0.0.5/src/django_forbid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 15:00:56.000000 django-forbid-0.0.5/src/django_forbid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 15:00:56.000000 django-forbid-0.0.5/src/django_forbid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:36:39.547046 django-forbid-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-17 15:36:29.000000 django-forbid-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-04-17 15:36:39.547046 django-forbid-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-04-17 15:36:29.000000 django-forbid-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-17 15:36:29.000000 django-forbid-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-17 15:36:39.547046 django-forbid-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 15:36:29.000000 django-forbid-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:36:39.543046 django-forbid-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:36:39.543046 django-forbid-0.0.6/src/django_forbid/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 15:36:29.000000 django-forbid-0.0.6/src/django_forbid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-17 15:36:29.000000 django-forbid-0.0.6/src/django_forbid/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-17 15:36:29.000000 django-forbid-0.0.6/src/django_forbid/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-17 15:36:29.000000 django-forbid-0.0.6/src/django_forbid/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-17 15:36:29.000000 django-forbid-0.0.6/src/django_forbid/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-17 15:36:29.000000 django-forbid-0.0.6/src/django_forbid/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-17 15:36:29.000000 django-forbid-0.0.6/src/django_forbid/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:36:39.543046 django-forbid-0.0.6/src/django_forbid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-04-17 15:36:39.000000 django-forbid-0.0.6/src/django_forbid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-17 15:36:39.000000 django-forbid-0.0.6/src/django_forbid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:36:39.000000 django-forbid-0.0.6/src/django_forbid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:36:39.000000 django-forbid-0.0.6/src/django_forbid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-17 15:36:39.000000 django-forbid-0.0.6/src/django_forbid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 15:36:39.000000 django-forbid-0.0.6/src/django_forbid.egg-info/top_level.txt
```

### Comparing `django-forbid-0.0.5/LICENSE` & `django-forbid-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-forbid-0.0.5/PKG-INFO` & `django-forbid-0.0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,11 @@
-Metadata-Version: 2.1
-Name: django-forbid
-Version: 0.0.5
-Summary: Django app for forbidding access to some countries
-Home-page: https://github.com/pysnippet/django-forbid
-Author: Artyom Vancyan
-Author-email: artyom@pysnippet.org
-License: MIT
-Keywords: python,django,forbid,django-forbid
-Platform: unix
-Platform: linux
-Platform: osx
-Platform: win32
-Classifier: Operating System :: OS Independent
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.1
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Django :: 4.1
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Django Forbid <img src="https://github.com/pysnippet.png" align="right" height="64" />
 
-Django app for forbidding access to some countries.
+Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN
+detection.
 
 [![PyPI](https://img.shields.io/pypi/v/django-forbid.svg)](https://pypi.org/project/django-forbid/)
 [![Python](https://img.shields.io/pypi/pyversions/django-forbid.svg?logoColor=white)](https://pypi.org/project/django-forbid/)
 [![Django](https://img.shields.io/pypi/djversions/django-forbid.svg?color=0C4B33&label=django)](https://pypi.org/project/django-forbid/)
 [![License](https://img.shields.io/pypi/l/django-forbid.svg)](https://github.com/pysnippet/django-forbid/blob/master/LICENSE)
 [![Tests](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml/badge.svg)](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml)
 
@@ -74,43 +42,65 @@
 
 ## Usage
 
 After connecting the Django Forbid to your project, you can define the set of desired zones to be forbidden or allowed.
 All you need is to set the `DJANGO_FORBID` variable in your project's settings. It should be a dictionary with the
 following keys:
 
+- `DEVICES` - list of devices to permit or forbid access to
 - `COUNTRIES` - list of countries to permit or forbid access to
 - `TERRITORIES` - list of territories to permit or forbid access to
 - `OPTIONS` - a dictionary for additional settings
-  - `ACTION` - whether to `PERMIT` or `FORBID` access to the listed zones (default is `FORBID`)
-  - `PERIOD` - time in seconds to check for access again, 0 means on each request
-  - `VPN` - use VPN detection and forbid access to VPN users
-  - `URL` - set of URLs to redirect to when the user is located in a forbidden country or using a VPN
-      - `FORBIDDEN_LOC` - the URL to redirect to when the user is located in a forbidden country
-      - `FORBIDDEN_VPN` - the URL to redirect to when the user is using a VPN
+    - `ACTION` - whether to `PERMIT` or `FORBID` access to the listed zones (default is `FORBID`)
+    - `PERIOD` - time in seconds to check for access again, 0 means on each request
+    - `VPN` - use VPN detection and forbid access to VPN users
+    - `URL` - set of URLs to redirect to when the user is located in a forbidden country or using a VPN
+        - `FORBIDDEN_LOC` - the URL to redirect to when the user is located in a forbidden country
+        - `FORBIDDEN_VPN` - the URL to redirect to when the user is using a VPN
+        - `FORBIDDEN_KIT` - the URL to redirect to when the user is using a forbidden device
+
+Unlike the `COUNTRIES` and `TERRITORIES`, where the middleware decides whether to permit or forbid access based on the
+given `ACTION` value, the `DEVICES` list accepts device types where the names starting with `!` are forbidden. This is
+done to make it possible to make them all mix together.
+
+```python
+# Forbid access to all devices that have a small screen.
+'DEVICES': ['!car', '!player', '!peripheral', '!camera']
+
+# Allow access to all devices having regular or large screens.
+'DEVICES': ['desktop', 'smartphone', 'console', 'tablet', 'tv']
+```
+
+The available device types are: `smartphone`, `peripheral` - refers to all hardware components that are attached to a
+computer, `wearable` - common types of wearable technology include smartwatches and smartglasses, `phablet` - a
+smartphone having a larger screen, `console` - PlayStation, Xbox, etc., `display`, `speaker` - Google Assistant, Siri,
+Alexa, etc., `desktop`, `tablet`, `camera`, `player` - iPod, Sony Walkman, Creative Zen, etc., `phone`, `car` - refers
+to a car browser and `tv` - refers to TVs having internet access.
 
 ```python
 DJANGO_FORBID = {
+    'DEVICES': ['desktop', 'smartphone', 'console', 'tablet', 'tv'],
     'COUNTRIES': ['US', 'GB'],
     'TERRITORIES': ['EU'],
     'OPTIONS': {
         'ACTION': 'PERMIT',
         'PERIOD': 300,
         'VPN': True,
         'URL': {
-            'FORBIDDEN_LOC': 'forbidden_country',
+            'FORBIDDEN_LOC': 'forbidden_location',
             'FORBIDDEN_VPN': 'forbidden_network',
+            'FORBIDDEN_KIT': 'forbidden_device',
         },
     },
 }
 ```
 
-The available ISO 3166 alpha-2 country codes are listed in [here](https://www.iban.com/country-codes). And the available
-ISO continent codes are: `AF` - Africa, `AN` - Antarctica, `AS` - Asia, `EU` - Europe, `NA` - North America, `OC` -
-Oceania and `SA` - South America.
+The available country codes in the required ISO 3166 alpha-2 format are
+listed [here](https://www.iban.com/country-codes). And the available continent codes (territories) are: `AF` -
+Africa, `AN` - Antarctica, `AS` - Asia, `EU` - Europe, `NA` - North America, `OC` - Oceania and `SA` - South America.
 
 _None of the settings are required. If you don't specify any settings, the middleware will not do anything._
 
 ## Contribute
 
 Any contribution is welcome. If you have any ideas or suggestions, feel free to open an issue or a pull request. And
 don't forget to add tests for your changes.
```

### Comparing `django-forbid-0.0.5/setup.cfg` & `django-forbid-0.0.6/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 [metadata]
 name = django-forbid
 version = attr: django_forbid.__version__
 author = Artyom Vancyan
 author_email = artyom@pysnippet.org
-description = Django app for forbidding access to some countries
+description = Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN detection.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pysnippet/django-forbid
 keywords = 
 	python
 	django
+	permit
 	forbid
+	access
+	device
+	secure
+	country
+	control
+	security
+	location
+	territory
+	vpn
+	detection
 	django-forbid
 license = MIT
 license_file = LICENSE
 platforms = unix, linux, osx, win32
 classifiers = 
 	Operating System :: OS Independent
 	Framework :: Django
@@ -35,14 +46,15 @@
 
 [options]
 packages = 
 	django_forbid
 install_requires = 
 	Django>=2.1
 	geoip2
+	device_detector
 include_package_data = yes
 python_requires = >=3.6
 package_dir = 
 	=src
 zip_safe = no
 
 [egg_info]
```

### Comparing `django-forbid-0.0.5/src/django_forbid/access.py` & `django-forbid-0.0.6/src/django_forbid/access.py`

 * *Files identical despite different names*

### Comparing `django-forbid-0.0.5/src/django_forbid/config.py` & `django-forbid-0.0.6/src/django_forbid/config.py`

 * *Files identical despite different names*

### Comparing `django-forbid-0.0.5/src/django_forbid/detect.py` & `django-forbid-0.0.6/src/django_forbid/detect.py`

 * *Files identical despite different names*

### Comparing `django-forbid-0.0.5/src/django_forbid/middleware.py` & `django-forbid-0.0.6/src/django_forbid/middleware.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,38 @@
 from django.http import HttpResponseForbidden
 from django.shortcuts import redirect
 from django.utils.timezone import utc
 
 from .access import grants_access
 from .config import Settings
 from .detect import detect_vpn
+from .device import detect_device
+from .device import device_forbidden
 
 
 class ForbidMiddleware:
     """Middleware to forbid access to the site."""
 
     def __init__(self, get_response):
         self.get_response = get_response
 
     def __call__(self, request):
         address = request.META.get("REMOTE_ADDR")
         address = request.META.get("HTTP_X_FORWARDED_FOR", address)
 
+        # Detects the user's device and saves it in the session.
+        if not request.session.get("DEVICE"):
+            http_ua = request.META.get("HTTP_USER_AGENT")
+            request.session["DEVICE"] = detect_device(http_ua)
+
+        if device_forbidden(request.session.get("DEVICE")):
+            if Settings.has("OPTIONS.URL.FORBIDDEN_KIT"):
+                return redirect(Settings.get("OPTIONS.URL.FORBIDDEN_KIT"))
+            return HttpResponseForbidden()
+
         # Checks if the PERIOD attr is set and the user has been granted access.
         if Settings.has("OPTIONS.PERIOD") and request.session.has_key("ACCESS"):
             acss = datetime.utcnow().replace(tzinfo=utc).timestamp()
 
             # Checks if access is not timed out yet.
             if acss - request.session.get("ACCESS") < Settings.get("OPTIONS.PERIOD"):
                 return detect_vpn(self.get_response, request)
```

### Comparing `django-forbid-0.0.5/src/django_forbid.egg-info/PKG-INFO` & `django-forbid-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-forbid
-Version: 0.0.5
-Summary: Django app for forbidding access to some countries
+Version: 0.0.6
+Summary: Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN detection.
 Home-page: https://github.com/pysnippet/django-forbid
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
-Keywords: python,django,forbid,django-forbid
+Keywords: python,django,permit,forbid,access,device,secure,country,control,security,location,territory,vpn,detection,django-forbid
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: win32
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.1
@@ -29,15 +29,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Forbid <img src="https://github.com/pysnippet.png" align="right" height="64" />
 
-Django app for forbidding access to some countries.
+Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN
+detection.
 
 [![PyPI](https://img.shields.io/pypi/v/django-forbid.svg)](https://pypi.org/project/django-forbid/)
 [![Python](https://img.shields.io/pypi/pyversions/django-forbid.svg?logoColor=white)](https://pypi.org/project/django-forbid/)
 [![Django](https://img.shields.io/pypi/djversions/django-forbid.svg?color=0C4B33&label=django)](https://pypi.org/project/django-forbid/)
 [![License](https://img.shields.io/pypi/l/django-forbid.svg)](https://github.com/pysnippet/django-forbid/blob/master/LICENSE)
 [![Tests](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml/badge.svg)](https://github.com/pysnippet/django-forbid/actions/workflows/tests.yml)
 
@@ -74,43 +75,65 @@
 
 ## Usage
 
 After connecting the Django Forbid to your project, you can define the set of desired zones to be forbidden or allowed.
 All you need is to set the `DJANGO_FORBID` variable in your project's settings. It should be a dictionary with the
 following keys:
 
+- `DEVICES` - list of devices to permit or forbid access to
 - `COUNTRIES` - list of countries to permit or forbid access to
 - `TERRITORIES` - list of territories to permit or forbid access to
 - `OPTIONS` - a dictionary for additional settings
-  - `ACTION` - whether to `PERMIT` or `FORBID` access to the listed zones (default is `FORBID`)
-  - `PERIOD` - time in seconds to check for access again, 0 means on each request
-  - `VPN` - use VPN detection and forbid access to VPN users
-  - `URL` - set of URLs to redirect to when the user is located in a forbidden country or using a VPN
-      - `FORBIDDEN_LOC` - the URL to redirect to when the user is located in a forbidden country
-      - `FORBIDDEN_VPN` - the URL to redirect to when the user is using a VPN
+    - `ACTION` - whether to `PERMIT` or `FORBID` access to the listed zones (default is `FORBID`)
+    - `PERIOD` - time in seconds to check for access again, 0 means on each request
+    - `VPN` - use VPN detection and forbid access to VPN users
+    - `URL` - set of URLs to redirect to when the user is located in a forbidden country or using a VPN
+        - `FORBIDDEN_LOC` - the URL to redirect to when the user is located in a forbidden country
+        - `FORBIDDEN_VPN` - the URL to redirect to when the user is using a VPN
+        - `FORBIDDEN_KIT` - the URL to redirect to when the user is using a forbidden device
+
+Unlike the `COUNTRIES` and `TERRITORIES`, where the middleware decides whether to permit or forbid access based on the
+given `ACTION` value, the `DEVICES` list accepts device types where the names starting with `!` are forbidden. This is
+done to make it possible to make them all mix together.
+
+```python
+# Forbid access to all devices that have a small screen.
+'DEVICES': ['!car', '!player', '!peripheral', '!camera']
+
+# Allow access to all devices having regular or large screens.
+'DEVICES': ['desktop', 'smartphone', 'console', 'tablet', 'tv']
+```
+
+The available device types are: `smartphone`, `peripheral` - refers to all hardware components that are attached to a
+computer, `wearable` - common types of wearable technology include smartwatches and smartglasses, `phablet` - a
+smartphone having a larger screen, `console` - PlayStation, Xbox, etc., `display`, `speaker` - Google Assistant, Siri,
+Alexa, etc., `desktop`, `tablet`, `camera`, `player` - iPod, Sony Walkman, Creative Zen, etc., `phone`, `car` - refers
+to a car browser and `tv` - refers to TVs having internet access.
 
 ```python
 DJANGO_FORBID = {
+    'DEVICES': ['desktop', 'smartphone', 'console', 'tablet', 'tv'],
     'COUNTRIES': ['US', 'GB'],
     'TERRITORIES': ['EU'],
     'OPTIONS': {
         'ACTION': 'PERMIT',
         'PERIOD': 300,
         'VPN': True,
         'URL': {
-            'FORBIDDEN_LOC': 'forbidden_country',
+            'FORBIDDEN_LOC': 'forbidden_location',
             'FORBIDDEN_VPN': 'forbidden_network',
+            'FORBIDDEN_KIT': 'forbidden_device',
         },
     },
 }
 ```
 
-The available ISO 3166 alpha-2 country codes are listed in [here](https://www.iban.com/country-codes). And the available
-ISO continent codes are: `AF` - Africa, `AN` - Antarctica, `AS` - Asia, `EU` - Europe, `NA` - North America, `OC` -
-Oceania and `SA` - South America.
+The available country codes in the required ISO 3166 alpha-2 format are
+listed [here](https://www.iban.com/country-codes). And the available continent codes (territories) are: `AF` -
+Africa, `AN` - Antarctica, `AS` - Asia, `EU` - Europe, `NA` - North America, `OC` - Oceania and `SA` - South America.
 
 _None of the settings are required. If you don't specify any settings, the middleware will not do anything._
 
 ## Contribute
 
 Any contribution is welcome. If you have any ideas or suggestions, feel free to open an issue or a pull request. And
 don't forget to add tests for your changes.
```

