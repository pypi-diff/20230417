# Comparing `tmp/watchtower_browser_testing-0.3.8.tar.gz` & `tmp/watchtower_browser_testing-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.3.8.tar", last modified: Thu Apr 13 19:27:57 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.3.9.tar", last modified: Thu Apr 13 19:32:15 2023, max compression
```

## Comparing `watchtower_browser_testing-0.3.8.tar` & `watchtower_browser_testing-0.3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 19:27:57.394562 watchtower_browser_testing-0.3.8/
--rw-rw-rw-   0        0        0      310 2023-04-13 19:27:57.394562 watchtower_browser_testing-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.3.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 19:27:57.394562 watchtower_browser_testing-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1106 2023-04-13 18:41:33.000000 watchtower_browser_testing-0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:27:57.378186 watchtower_browser_testing-0.3.8/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-13 18:26:41.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:27:57.394562 watchtower_browser_testing-0.3.8/watchtower_browser_testing/templates/
--rw-rw-rw-   0        0        0     2613 2023-04-13 19:27:41.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing/templates/measurement_plan.html
--rw-rw-rw-   0        0        0    14236 2023-04-13 19:16:36.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-13 19:27:48.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:27:57.394562 watchtower_browser_testing-0.3.8/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-13 19:27:57.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-04-13 19:27:57.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 19:27:57.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-13 19:27:57.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-13 19:27:57.000000 watchtower_browser_testing-0.3.8/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 19:32:15.220158 watchtower_browser_testing-0.3.9/
+-rw-rw-rw-   0        0        0      310 2023-04-13 19:32:15.220158 watchtower_browser_testing-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.3.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 19:32:15.220158 watchtower_browser_testing-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2023-04-13 18:41:33.000000 watchtower_browser_testing-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:32:15.220158 watchtower_browser_testing-0.3.9/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-13 18:26:41.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:32:15.220158 watchtower_browser_testing-0.3.9/watchtower_browser_testing/templates/
+-rw-rw-rw-   0        0        0     3255 2023-04-13 19:32:04.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing/templates/measurement_plan.html
+-rw-rw-rw-   0        0        0    14236 2023-04-13 19:16:36.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-13 19:32:04.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-13 19:32:15.220158 watchtower_browser_testing-0.3.9/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-13 19:32:15.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-04-13 19:32:15.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 19:32:15.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-13 19:32:15.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-13 19:32:15.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.3.8/setup.py` & `watchtower_browser_testing-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.8/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.3.9/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.8/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.3.9/watchtower_browser_testing/helpers.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.8/watchtower_browser_testing/templates/measurement_plan.html` & `watchtower_browser_testing-0.3.9/watchtower_browser_testing/templates/measurement_plan.html`

 * *Files 16% similar despite different names*

```diff
@@ -16,30 +16,39 @@
     padding-top: 1rem;
 }
 
 .alert_exclamation {
     vertical-align: text-bottom;
     margin-right: 0.5rem;
 }
+
+.message_check {
+    vertical-align: text-bottom;
+    margin-right: 0.5rem;
+}
 </style>
 </head>
 <body>
     <div class="container">
         <div class="{{ content.type }}" id="container_{{ content.id }}" >
             {% if test_results %}
             {% if test_results.errors %}
                 <div class="alert alert-danger" role="alert" style="margin-top:1rem;">
-                    <svg xmlns="http://www.w3.org/2000/svg" width="1.2rem" height="1.2rem" fill="currentColor" class="bi bi-exclamation-triangle" viewBox="0 0 16 16">
+                    <svg xmlns="http://www.w3.org/2000/svg" width="1.2rem" height="1.2rem" fill="currentColor" class="bi bi-exclamation-triangle alert_exclamation" viewBox="0 0 16 16">
                         <path d="M7.938 2.016A.13.13 0 0 1 8.002 2a.13.13 0 0 1 .063.016.146.146 0 0 1 .054.057l6.857 11.667c.036.06.035.124.002.183a.163.163 0 0 1-.054.06.116.116 0 0 1-.066.017H1.146a.115.115 0 0 1-.066-.017.163.163 0 0 1-.054-.06.176.176 0 0 1 .002-.183L7.884 2.073a.147.147 0 0 1 .054-.057zm1.044-.45a1.13 1.13 0 0 0-1.96 0L.165 13.233c-.457.778.091 1.767.98 1.767h13.713c.889 0 1.438-.99.98-1.767L8.982 1.566z"/>
                         <path d="M7.002 12a1 1 0 1 1 2 0 1 1 0 0 1-2 0zM7.1 5.995a.905.905 0 1 1 1.8 0l-.35 3.507a.552.552 0 0 1-1.1 0L7.1 5.995z"/>
                     </svg>
-                    A test ran at {{ test_results.time }} and there were {{ test_results.errors.total }} errors in total
+                    A test ran at {{ test_results.time }} and there were <strong>{{ test_results.errors.total }} errors</strong> in total
                 </div>
             {% else %}
-                <div class="alert alert-success" role="alert">
+                <div class="alert alert-success" role="alert" style="margin-top:1rem;">
+                    <svg xmlns="http://www.w3.org/2000/svg" width="1.2rem" height="1.2rem" fill="currentColor" class="bi bi-check-circle message_check" viewBox="0 0 16 16">
+                        <path d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"/>
+                        <path d="M10.97 4.97a.235.235 0 0 0-.02.022L7.477 9.417 5.384 7.323a.75.75 0 0 0-1.06 1.06L6.97 11.03a.75.75 0 0 0 1.079-.02l3.992-4.99a.75.75 0 0 0-1.071-1.05z"/>
+                    </svg>
                     A test ran at {{ test_results.time }} and there were no errors
                 </div>
             {% endif %}
             {% endif %}
             {{ content.description }}
             {% for test in content.children %}
                 <div class="{{ test.type }}" id="container_{{ test.id }}">
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% if test_results %} {% if test_results.errors %}
     A test ran at {{ test_results.time }} and there were {
 { test_results.errors.total }} errors in total
 {% else %}
-A test ran at {{ test_results.time }} and there were no errors
+    A test ran at {{ test_results.time }} and there were no errors
 {% endif %} {% endif %} {{ content.description }} {% for test in
 content.children %}
 {{ test.description }} {% for scenario in test.children %}
 {{ scenario.description }}
 {% endfor %}
 {% endfor %}
```

### Comparing `watchtower_browser_testing-0.3.8/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.3.9/watchtower_browser_testing/testsuite.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.8/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.3.9/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.8/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.3.9/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

