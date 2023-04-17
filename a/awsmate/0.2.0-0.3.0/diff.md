# Comparing `tmp/awsmate-0.2.0.tar.gz` & `tmp/awsmate-0.3.0.tar.gz`

## Comparing `awsmate-0.2.0.tar` & `awsmate-0.3.0.tar`

### file list

```diff
@@ -1,63 +1,65 @@
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 awsmate-0.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 awsmate-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 awsmate-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 awsmate-0.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 awsmate-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 awsmate-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 awsmate-0.2.0/.github/workflows/tests.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/requirements.txt
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/apigateway.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/awsmate.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/changelog.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/code_of_conduct.rst
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/conf.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/contributing.rst
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/eventbridge.rst
--rw-r--r--   0        0        0    12065 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/example_application.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/genindex.rst
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/index.rst
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/lambdafunction.rst
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/logger.rst
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/readme.rst
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/release_process.rst
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/s3.rst
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/testing.rst
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/_static/flyout.js
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/_static/theme.css
--rwxr-xr-x   0        0        0     1607 2020-02-02 00:00:00.000000 awsmate-0.2.0/docs/source/_templates/layout.html
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/check_terraform
--rwxr-xr-x   0        0        0      181 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/deploy.sh
--rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/undeploy.sh
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/variables.tfvars
--rwxr-xr-x   0        0        0     1102 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/src/lambda_apigateway_returns_403.py
--rwxr-xr-x   0        0        0     1790 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/src/lambda_apigateway_returns_500.py
--rwxr-xr-x   0        0        0     3702 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/src/lambda_apigateway_returns_okay.py
--rwxr-xr-x   0        0        0      465 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/src/lambda_eventbridge_scheduler.py
--rwxr-xr-x   0        0        0      661 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/src/lambda_s3_notification.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/tf/00-provider.tf
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/tf/00-variables.tf
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/tf/01-lambda-iam-role.tf
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/tf/02-awsmate-lambda-layer.tf
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/tf/03-apigateway-lambda-functions.tf
--rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/tf/04-apigateway.tf
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/tf/05-eventbridge-lambda-functions.tf
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/tf/06-eventbridge-iam-role.tf
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/tf/07-eventbridge-scheduler.tf
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/tf/08-s3-bucket.tf
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 awsmate-0.2.0/example/tf/09-s3-lambda-functions.tf
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 awsmate-0.2.0/src/awsmate/__init__.py
--rw-r--r--   0        0        0    45535 2020-02-02 00:00:00.000000 awsmate-0.2.0/src/awsmate/apigateway.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 awsmate-0.2.0/src/awsmate/eventbridge.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 awsmate-0.2.0/src/awsmate/lambdafunction.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 awsmate-0.2.0/src/awsmate/logger.py
--rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 awsmate-0.2.0/src/awsmate/s3.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 awsmate-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0    33111 2020-02-02 00:00:00.000000 awsmate-0.2.0/tests/unit/test_apigateway.py
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 awsmate-0.2.0/tests/unit/test_eventbridge.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 awsmate-0.2.0/tests/unit/test_lambdafunction.py
--rw-r--r--   0        0        0    14666 2020-02-02 00:00:00.000000 awsmate-0.2.0/tests/unit/test_s3.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 awsmate-0.2.0/.gitignore
--rw-r--r--   0        0        0    13827 2020-02-02 00:00:00.000000 awsmate-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 awsmate-0.2.0/README.md
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 awsmate-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 awsmate-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 awsmate-0.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 awsmate-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 awsmate-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 awsmate-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 awsmate-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 awsmate-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 awsmate-0.3.0/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/requirements.txt
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/apigateway.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/awsmate.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/changelog.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/code_of_conduct.rst
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/conf.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/contributing.rst
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/eventbridge.rst
+-rw-r--r--   0        0        0    12601 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/example_application.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/genindex.rst
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/index.rst
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/lambdafunction.rst
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/logger.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/readme.rst
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/release_process.rst
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/s3.rst
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/testing.rst
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/_static/flyout.js
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/_static/theme.css
+-rwxr-xr-x   0        0        0     1607 2020-02-02 00:00:00.000000 awsmate-0.3.0/docs/source/_templates/layout.html
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/check_terraform
+-rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/deploy.sh
+-rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/undeploy.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/variables.tfvars
+-rwxr-xr-x   0        0        0     1102 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/src/lambda_apigateway_returns_403.py
+-rwxr-xr-x   0        0        0     1808 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/src/lambda_apigateway_returns_500.py
+-rwxr-xr-x   0        0        0     3738 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/src/lambda_apigateway_returns_okay.py
+-rwxr-xr-x   0        0        0      465 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/src/lambda_eventbridge_scheduler.py
+-rwxr-xr-x   0        0        0      394 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/src/lambda_logger.py
+-rwxr-xr-x   0        0        0      742 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/src/lambda_s3_notification.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/00-provider.tf
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/00-variables.tf
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/01-lambda-iam-role.tf
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/02-awsmate-lambda-layer.tf
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/03-apigateway-lambda-functions.tf
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/04-apigateway.tf
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/05-eventbridge-lambda-functions.tf
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/06-eventbridge-iam-role.tf
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/07-eventbridge-scheduler.tf
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/08-s3-bucket.tf
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/09-s3-lambda-functions.tf
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 awsmate-0.3.0/example/tf/10-logger-lambda-functions.tf
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 awsmate-0.3.0/src/awsmate/__init__.py
+-rw-r--r--   0        0        0    52826 2020-02-02 00:00:00.000000 awsmate-0.3.0/src/awsmate/apigateway.py
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 awsmate-0.3.0/src/awsmate/eventbridge.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 awsmate-0.3.0/src/awsmate/lambdafunction.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 awsmate-0.3.0/src/awsmate/logger.py
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 awsmate-0.3.0/src/awsmate/s3.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 awsmate-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0    34262 2020-02-02 00:00:00.000000 awsmate-0.3.0/tests/unit/test_apigateway.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 awsmate-0.3.0/tests/unit/test_eventbridge.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 awsmate-0.3.0/tests/unit/test_lambdafunction.py
+-rw-r--r--   0        0        0    15684 2020-02-02 00:00:00.000000 awsmate-0.3.0/tests/unit/test_s3.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 awsmate-0.3.0/.gitignore
+-rw-r--r--   0        0        0    13827 2020-02-02 00:00:00.000000 awsmate-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 awsmate-0.3.0/README.md
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 awsmate-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 awsmate-0.3.0/PKG-INFO
```

### Comparing `awsmate-0.2.0/CHANGELOG.md` & `awsmate-0.3.0/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,57 @@
 All notable changes to this project are documented in this file.
 
+## [0.3.0] - 2023-04-17
+
+### Added
+
+- Code
+    - added class ``awsmate.apigateway.HttpServerError``
+    - added class ``awsmate.apigateway.HttpError``, which is the base class of ``awsmate.apigateway.HttpClientError`` and ``awsmate.apigateway.HttpServerError``
+    - added class ``awsmate.apigateway.HttpServerError`` hierarchy
+    - added method ``awsmate.s3.LambdaNotificationEvent.object_url()`` 
+
+- Example application
+    - added a Lambda function specific to ``awsmate.logger``
+
+### Changed
+
+- Code
+    - ``awsmate.logger.log_internal_error()``: explanatory message has been made optional
+    - ``awsmate.apigateway.HttpClientError`` doesn't log an error anymore at construction time
+    - ``awsmate.apigateway.build_http_server_error_response()`` has a new signature and logs a critical error and a stack trace by default
+    - ``awsmate.apigateway.build_http_client_error_response()`` now logs an error by default
+    - ``awsmate.s3.LambdaNotificationEvent.object_key()`` performs URL decoding on the returned value
+
+- Documentation
+    - example application: rewording
+
+- Example application
+    - made the AWS region used for deployment configurable through an environment variable, without editing any file  
+
+### Deprecated
+
+*nothing*
+
+### Removed
+
+*nothing*
+
+### Fixed
+
+- Code
+    - ``awsmate.apigateway``: corrected type hints for ``**kwargs``
+- Example application
+    - deployment scripts: ``.`` was mistakenly assumed to be in the ``PATH``.
+    - API Gateway: fixed the redeployment issue
+
+### Security
+
+*nothing*
+
 ## [0.2.0] - 2023-04-05
 
 ### Added
 
 - Code
     - added `awsmate.apigateway.LambdaProxyEvent.source_ip()`
     - added all missing ``awsmate.apigateway.HttpClientError`` subclasses
```

### Comparing `awsmate-0.2.0/CODE_OF_CONDUCT.md` & `awsmate-0.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/CONTRIBUTING.md` & `awsmate-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `awsmate-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/.github/workflows/tests.yaml` & `awsmate-0.3.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/docs/source/conf.py` & `awsmate-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/docs/source/example_application.rst` & `awsmate-0.3.0/docs/source/example_application.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Example application
 ===================
 
-An example application is provided in the Github repository of this library to show how to implement its features.
+An example application is provided in the Github repository of this library.
+To deploy it or to modify it for experimentation, you can download the repository in one of the following ways:
 
-To deploy this example application, modify it for experimentation, etc, you can download the repository in one of the following ways:
-
-* ``git clone https://github.com/shlublu/awsmate.git``
-* download a ``zip`` or ``tar.gz`` archive from the `awsmate release page on Github <https://github.com/shlublu/awsmate/releases>`_
+* using git: ``git clone https://github.com/shlublu/awsmate.git``
+* manually: ``zip`` and ``tar.gz`` archives are available on the `release page of the repository <https://github.com/shlublu/awsmate/releases>`_
 
 Prerequisites
 -------------
 
 To deploy and run this application, you will need:
 
 * an AWS account with valid credentials to create, modify and destroy AWS resources
@@ -34,47 +33,48 @@
                 |
                 |___tf/ (Terraform sources of this example application)
 
 
 Instructions for deployment
 ---------------------------
 
-Credentials
-~~~~~~~~~~~
+AWS settings
+~~~~~~~~~~~~
 
 * Using configuration and credentials files:
-    *   Define a default profile in ``~/.aws/``, or use the AWS CLI ``aws configure`` command
-    *   Please see the `AWS documentation of these configuration files <https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html>`_  for further details
+    *   define a default profile in ``~/.aws/``, or use the AWS CLI ``aws configure`` command
+    *   please see the `AWS documentation of these configuration files <https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html>`_  for further details
 * Using environment variables: 
-    *   Define the environment variables ``AWS_ACCESS_KEY_ID``, ``AWS_SECRET_ACCESS_KEY``, (...) with the parameters corresponding to your AWS IAM credentials 
-    *   Export them all using the shell ``export`` command
-    *   Please see the `AWS documentation of these environment variables <https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-envvars.html>`_  for further details
+    *   define your AWS IAM credential using the environment variables ``AWS_ACCESS_KEY_ID``, ``AWS_SECRET_ACCESS_KEY``, (...)  
+    *   define the AWS region you wish to deploy in using the environment variable ``AWS_REGION``
+    *   export all these environment variables using the shell ``export`` command
+    *   please see the `AWS documentation of these environment variables <https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-envvars.html>`_  for further details
 
-Depending on your AWS IAM setup, you may have to use the AWS CLI to execute commands such as ``aws sts assume-role`` or ``aws sso login`` on top of the above.
+In some companies and organizations you may have to use the AWS CLI to execute commands such as ``aws sts assume-role`` or ``aws sso login`` on top of or instead of the above. Should you have issues defining your AWS settings, please check with your AWS administrator.
 
 .. _Deployment:
 
 Deployment
 ~~~~~~~~~~
 
 From the ``example`` directory seen above:
 
 * run ``./deploy.sh``: this will deploy all AWS resources described in the ``tf/`` directory. This may take some time, and this produces a pretty verbose log.
-* then take note of the final log message ``endpoint_url = "https://<deployment id>.execute-api.<region>.amazonaws.com/v0"``: this is the URL of the newly deployed example API.
+* then take note of the final log message ``endpoint_url = "https://<deployment id>.execute-api.<region>.amazonaws.com/v0"``: this is the base URL of the newly deployed example API. 
 
 The :ref:`section "Application users's guide" <UsersGuide>` below explains how to use this example application.
 
-**Caveat**: 
+**Caveats** 
 
-Should you redeploy the example application after having modified the API Gateway routes or parameters defined in ``tf/03-apigateway.tf`` to experiment on your own, the 
-API Gateway resources will be modified ib AWS but the API will not be actually redeployed. You will need to redeploy it using the AWS console or the AWS CLI 
-before continuing to use the example application, otherwise unexpected behaviour may occur such as unexpected messages ``{"message":"Missing Authentication Token"}`` when
-querying the example API. 
+**Security**: The example API is accessible from the whole internet to anyone who would find its URL. We recommend undeploying the example application after 
+use (see :ref:`section "Undeployment" <Undeployment>` below) to avoid any unexpected use or hack attempt. 
+The URL of the API is generated by AWS at creation time, which makes it change each time you undeploy/redeploy the example application.
 
-You can also undeploy the application (see :ref:`section "Undeployment" <Undeployment>`) below before deploying it again. This would work but this would change the ``endpoint_url``. 
+**awsmate upgrades**: Terraform version and example application structure may change from an ``awsmate`` version to another. We recommend undeploying 
+the example application before upgrading it in order to avoid any compatibility issue.
 
 .. _Undeployment:
 
 Undeployment
 ~~~~~~~~~~~~
 
 From the ``example`` directory above, run:
@@ -109,53 +109,54 @@
 
 * Use
 
     The ``<endpoint_url>`` placeholder below need replacing by the actual value returned by ``./deploy.sh``, as seen in :ref:`section "Deployment" <Deployment>` above.
 
     * Route "okay": ``lambda_apigateway_returns_okay.py``
         * Command-line with ``curl`` 
-            * ``curl -X https://<endpoint_url>/okay/<any path>?<any url parameter>=<any value> --data '<any JSON payload>' --header '<any name>: <any value>'`` 
-            * Example: ``curl -X POST https://<endpoint_url>/okay/lets/go?someParam=someValue --data '{ "someKey": 42 }' --header 'X-example: 42'``
+            * ``curl -v -X <method> https://<endpoint_url>/okay/<any path>?<any url parameter>=<any value> --data '<any JSON payload>' --header '<any name>: <any value>'`` 
+            * Example: ``curl -v -X POST https://<endpoint_url>/okay/lets/go?someParam=someValue --data '{ "someKey": 42 }' --header 'X-example: 42'``
             * Returns 200 with a JSON payload that contains the result of all methods of ``awsmate.apigateway.LambdaProxyEvent`` plus the raw event received from AWS API Gateway.
             * Demonstrates
-                * the use of all methods of ``awsmate.apigateway.LambdaProxyEvent``,
-                * the use of the HTTP response builder ``awsmate.apigateway.build_http_response()``
+                * the use of all methods of :class:`awsmate.apigateway.LambdaProxyEvent`,
+                * the use of the HTTP response builder :func:`awsmate.apigateway.build_http_response`
             * Tip: play with the ``Accept`` and ``Accept-Encoding`` headers, play with the routes, play with the URL parameters
         * With a web browser
             * ``https://<endpoint_url>/okay/<any path>?<any url parameter>=<any value>``
             * Example: ``https://<endpoint_url>/okay/lets/go?someParam=someValue``
             * Returns an HTML page that is an HTML transformation of the JSON payload described in the command-line example just above.
             * Demonstrates 
                 * the same of the above, plus
                 * the use of the ``custom_transformers`` (here: HTML transformation of the API response) described in :doc:`the apigateway module documentation <apigateway>`,
-                * the use of ``extra_headers`` (here: to handle CORS) with ``awsmate.apigateway.build_http_response()``,
-                * the ``gzip`` built-in functionality of ``awsmate.apigateway.build_http_response()`` based on the ``Accept-Encoding`` header (unless your browser does not accept gzip!),
+                * the use of ``extra_headers`` (here: to handle CORS) with :func:`awsmate.apigateway.build_http_response`,
+                * the ``gzip`` built-in functionality of :func:`awsmate.apigateway.build_http_response` based on the ``Accept-Encoding`` header (unless your browser does not accept gzip!),
                 * the handling of preferences submitted through ``Accept*`` headers in `weighted quality value syntax <https://developer.mozilla.org/en-US/docs/Web/HTTP/Content_negotiation>`_.
             * Tip: think of how you could localize the returned content depending on the ``Accept-Language`` header submitted by the browser
     * Route "forbidden": ``lambda_apigateway_returns_403.py``
         * Command-line with ``curl`` 
-            * ``curl -X GET https://<endpoint_url>/forbidden' --header '<any name>: <any value>'`` 
-            * Example: ``curl -X GET https://<endpoint_url>/forbidden``
-            * Returns 403 with a JSON payload that explains access is forbidden
+            * ``curl -v -X GET https://<endpoint_url>/forbidden' --header '<any name>: <any value>'`` 
+            * Example: ``curl -v -X GET https://<endpoint_url>/forbidden``
+            * Returns 403 with a JSON payload that explains the access is forbidden
+            * Logs an error message in AWS Cloudwatch. See :ref:`section "Logger features" <LoggerFeatures>` below for further details.
             * Demonstrates
-                * the use of the HTTP response builder ``awsmate.apigateway.build_http_client_error_response()``
+                * the use of the HTTP response builder :func:`awsmate.apigateway.build_http_client_error_response`
         * With a web browser
             * ``https://<endpoint_url>/forbidden``
             * Example: ``https://<endpoint_url>/forbidden``
             * Returns an HTML page that is an HTML transformation of the JSON payload described in the command-line example just above.
             * Demonstrates 
                 * the same of the above plus the same extras seen with the "okay" route above
     * Route "crash": ``lambda_apigateway_returns_500.py``
         * Command-line with ``curl`` 
-            * ``curl -X GET https://<endpoint_url>/crash' --header '<any name>: <any value>'`` 
-            * Example: ``curl -X GET https://<endpoint_url>/crash``
-            * Returns 500 with a JSON payload that explains an internal error occurred
-            * Logs a complete stack trace in AWS Cloudwatch. See :ref:`section "Logger features" <LoggerFeatures>` below for further details.
+            * ``curl -v -X GET https://<endpoint_url>/crash' --header '<any name>: <any value>'`` 
+            * Example: ``curl -v -X GET https://<endpoint_url>/crash``
+            * Returns 500 with a JSON payload explaining that an internal error occurred
+            * Logs a complete stack trace of this crash in AWS Cloudwatch. See :ref:`section "Logger features" <LoggerFeatures>` below for further details.
             * Demonstrates
-                * the use of the HTTP response builder ``awsmate.apigateway.build_http_server_error_response()`` 
+                * the use of the HTTP response builder :func:`awsmate.apigateway.build_http_server_error_response` 
                 * how not to reveal the cause of the crash to the end user (which would be a security breach) while logging it for debugging purposes
         * With a web browser
             * ``https://<endpoint_url>/crash``
             * Example: ``https://<endpoint_url>/crash``
             * Returns an HTML page that is an HTML transformation of the JSON payload described in the command-line example just above.
             * Demonstrates 
                 * the same of the above plus the same extras seen with the "okay" route above                
@@ -174,21 +175,21 @@
                 |___src
                      |
                      |___lambda_eventbridge_scheduler.py
 
 
 * Use
     * Step by step instructions
-        * Go to the Cloudwatch service page
+        * Go to the Cloudwatch service page of the AWS Console
         * Follow the "Logs/Log group" link of the left navigation panel
         * Search for the ``/aws/lambda/awsmate_eventbridge_scheduler`` log group and open it
         * Open the most recent log stream (the scheduler triggers an event every 5 minutes)
-        * This show a log that contains the result of all methods of ``awsmate.eventbridge.LambdaBridgePutEvent`` plus the raw event received from the AWS EventBridge service.
+        * This show a log that contains the result of all methods of :class:`awsmate.eventbridge.LambdaBridgePutEvent` plus the raw event received from the AWS EventBridge service.
     * This demonstrates
-        * the use of all methods of ``awsmate.eventbridge.LambdaBridgePutEvent``
+        * the use of all methods of :class:`awsmate.eventbridge.LambdaBridgePutEvent`
     
 Lambda Function features: :doc:`lambdafunction <lambdafunction>` module
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 *Nothing for now*
 
 S3 features: :doc:`s3 <s3>` module
@@ -207,47 +208,48 @@
 
 
 * Use
     * Step by step instructions
         * Go to the S3 service page
         * Open the page of the S3 bucket ``awsmate-drop-files-here-<your AWS account number>``
         * Upload a file into this bucket
-        * Go to the Cloudwatch service page
+        * Go to the Cloudwatch service page of the AWS Console
         * Follow the "Logs/Log group" link of the left navigation panel
         * Search for the ``/aws/lambda/awsmate_s3_notification`` log group and open it
         * Open the most recent log stream
-        * This show a log that contains the result of all methods of ``awsmate.s3.LambdaNotificationEvent`` plus the raw event received from the AWS S3 service.
+        * This show a log that contains the result of all methods of :class:`awsmate.s3.LambdaNotificationEvent` plus the raw event received from the AWS S3 service.
     * This demonstrates
-        * the use of all methods of ``awsmate.s3.LambdaNotificationEvent``
+        * the use of all methods of :class:`awsmate.s3.LambdaNotificationEvent`
     * Tip: try to delete a file from the S3 bucket and see the corresponding log, try to drop or delete several files in a single action
 
 
 .. _LoggerFeatures:
 
 Logger features: :doc:`logger <logger>` module
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * Relevant source files
 
-All files are relevant but we recommand the following one:
-
 ::
 
     awsmate
         |___example
                 |
                 |___src
                      |
-                     |___lambda_apigateway_returns_500.py 
+                     |___lambda_logger.py 
 
 
 * Use
     * Step by step instructions
-        * Open the URL ``https://<endpoint_url>/crash`` with your web browser
-        * Go to the Cloudwatch service page
+        * Go to the Lambda service page of the AWS Console
+        * Follow the "Functions" link of the left navigation panel
+        * Search for the ``awsmate_logger`` function and open it
+        * Use the "Test" button to run it once. This will lead you to create a test event if not done already: any payload can be used as the event is not used by this function.
+        * Go to the Cloudwatch service page of the AWS Console
         * Follow the "Logs/Log group" link of the left navigation panel
-        * Search for the ``/aws/lambda/awsmate_apigateway_returns_500`` log group and open it
+        * Search for the ``/aws/lambda/awsmate_logger`` log group and open it
         * Open the most recent log stream
-        * This shows a log containing a critical error message followed by a stack trace showing the details of this crash simulation, and then an informational message showing the returned payload
+        * This shows a log containing a series of messages of progressive log levels from INFO to CRITICAL, followed by a stack trace showing the details of a crash simulation.
     * This demonstrates
-        * the use of the ``log_internal_error`` function of ``awsmate.logger``
-        * the use of the ``logger`` object of ``awsmate.logger``, which is a `standard Python logger <https://docs.python.org/3/library/logging.html>`_
+        * the use of the :data:`awsmate.logger.logger` object, which is a `standard Python logger <https://docs.python.org/3/library/logging.html>`_
+        * the use of :func:`awsmate.logger.log_internal_error`
```

### Comparing `awsmate-0.2.0/docs/source/release_process.rst` & `awsmate-0.3.0/docs/source/release_process.rst`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/docs/source/_static/flyout.js` & `awsmate-0.3.0/docs/source/_static/flyout.js`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/docs/source/_templates/layout.html` & `awsmate-0.3.0/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/example/check_terraform` & `awsmate-0.3.0/example/check_terraform`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/example/src/lambda_apigateway_returns_403.py` & `awsmate-0.3.0/example/src/lambda_apigateway_returns_403.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/example/src/lambda_apigateway_returns_500.py` & `awsmate-0.3.0/example/src/lambda_apigateway_returns_500.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,36 +22,35 @@
     }
 
     # Deals with CORS provided HTTP OPTIONS is dealt with on API Gateway side.
     extra_headers = {
         'Access-Control-Allow-Origin': '*'
     }
 
+    event = ag.LambdaProxyEvent(raw_event)
+
     try:
-        event = ag.LambdaProxyEvent(raw_event)
-        
         ag.determine_content_type(event, custom_transformers=html_transformers)
 
         #############################
         # Specific work starts here
 
-        raise RuntimeError("Let's simulate some crash")
+        raise RuntimeError("Let's simulate some crash caused by a programmatic error")
     
         # Specific work finishes here
         #############################    
 
     except ag.HttpClientError as err:
         logger.error(f'Client made a mistake: {repr(err)}')
         response = ag.build_http_client_error_response(err, event=event, extra_headers=extra_headers, custom_transformers=html_transformers)
 
     except Exception as err:
-        log_internal_error('Well, we expected that one')
-
         response = ag.build_http_server_error_response(
-            'Something wrong happened, and this is on our end!', 
+            ag.HttpInternalServerError(),
+            client_message='Something wrong happened, and this is on our end!', 
             event=event, 
             extra_headers=extra_headers, 
             custom_transformers=html_transformers
         )
 
     logger.info(f'Returned payload:\n{json.dumps(response)}')
```

### Comparing `awsmate-0.2.0/example/src/lambda_apigateway_returns_okay.py` & `awsmate-0.3.0/example/src/lambda_apigateway_returns_okay.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,17 +45,17 @@
         'text/html': dict_to_html_regular  
     }
 
     custom_transformers_error = { 
         'text/html': dict_to_html_error
     }
 
-    try:
-        event = ag.LambdaProxyEvent(raw_event)
+    event = ag.LambdaProxyEvent(raw_event)
 
+    try:
         ag.determine_content_type(event, custom_transformers=custom_transformers_regular)
 
         #############################
         # Specific work starts here
 
         payload = {
             'event.source_ip()' : str(event.source_ip()),    
@@ -77,21 +77,22 @@
 
         # Specific work finishes here
         #############################
 
         response = ag.build_http_response(200, payload, event=event, extra_headers=extra_headers, custom_transformers=custom_transformers_regular)
 
     except ag.HttpClientError as err:
-        logger.error(f'Client made a mistake: {repr(err)}')
+        logger.error(f'Client made a mistake')
         response = ag.build_http_client_error_response(err, event=event, extra_headers=extra_headers, custom_transformers=custom_transformers_error)
 
     except Exception as err:
-        log_internal_error('This is actually unexpected.')
+        logger.critical('This is actually unexpected')
         response = ag.build_http_server_error_response(
-            'Something wrong happened, and this is on our end!',
+            ag.HttpInternalServerError(),
+            client_message='Something wrong happened, and this is on our end!',
             event=event, 
             extra_headers=extra_headers, 
             custom_transformers=custom_transformers_error
         )
 
     logger.info(f'Returned payload:\n{json.dumps(response)}')
```

### Comparing `awsmate-0.2.0/example/src/lambda_s3_notification.py` & `awsmate-0.3.0/example/src/lambda_s3_notification.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import site
 site.addsitedir('/opt')
 
 import json 
 
-from awsmate.logger import logger
+from awsmate.logger import logger, log_internal_error
 from awsmate.s3 import LambdaNotificationEvent
 
 
 def lambda_handler(raw_event, context):
     event = LambdaNotificationEvent(raw_event)
 
     logger.info(f'event.event_name(): {event.event_name()}')
     logger.info(f'event.bucket_arn(): {event.bucket_arn()}')
     logger.info(f'event.bucket_name(): {event.bucket_name()}')
     logger.info(f'event.object_key(): {event.object_key()}')
     logger.info(f'event.object_size(): {event.object_size()}')
     logger.info(f'event.object_etag(): {event.object_etag()}')
+    logger.info(f'event.object_url(): {event.object_url()}')
 
     logger.info(f'Raw event:\n{json.dumps(raw_event, indent=2)}')
```

### Comparing `awsmate-0.2.0/example/tf/01-lambda-iam-role.tf` & `awsmate-0.3.0/example/tf/01-lambda-iam-role.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/example/tf/03-apigateway-lambda-functions.tf` & `awsmate-0.3.0/example/tf/03-apigateway-lambda-functions.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/example/tf/04-apigateway.tf` & `awsmate-0.3.0/example/tf/04-apigateway.tf`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,20 @@
         aws_api_gateway_integration.get_error500,
 
         aws_api_gateway_gateway_response.generic_4XX,
         aws_api_gateway_gateway_response.generic_5XX
     ]
 
     rest_api_id = aws_api_gateway_rest_api.demonstrator.id
+
+    stage_description = "${timestamp()}"  
+
+    lifecycle {
+        create_before_destroy = true
+    }    
 }
 
 resource "aws_api_gateway_stage" "demonstrator" {
     stage_name = "v0"
     rest_api_id   = aws_api_gateway_rest_api.demonstrator.id
     deployment_id = aws_api_gateway_deployment.demonstrator.id
 }
```

### Comparing `awsmate-0.2.0/example/tf/05-eventbridge-lambda-functions.tf` & `awsmate-0.3.0/example/tf/05-eventbridge-lambda-functions.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/example/tf/06-eventbridge-iam-role.tf` & `awsmate-0.3.0/example/tf/06-eventbridge-iam-role.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/example/tf/08-s3-bucket.tf` & `awsmate-0.3.0/example/tf/08-s3-bucket.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/example/tf/09-s3-lambda-functions.tf` & `awsmate-0.3.0/example/tf/09-s3-lambda-functions.tf`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/src/awsmate/apigateway.py` & `awsmate-0.3.0/src/awsmate/apigateway.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import ipaddress
 import json
 import re
 import typing
 
 from http import HTTPStatus
 
-from awsmate.logger import logger
+from awsmate.logger import logger, log_internal_error
 from awsmate.lambdafunction import LambdaEvent, AwsEventSpecificationError
 
 
 class MalformedPayloadError(RuntimeError):
     """
     Error raised by :class:`~LambdaProxyEvent` in case of malformed input payload.
     """
@@ -25,15 +25,16 @@
         """
         
         super().__init__(msg)
         
 
 class LambdaProxyEvent(LambdaEvent):
     """
-    Mapping of the input event received by an AWS Lambda function triggered by AWS API Gateway during a client API call.
+    Mapping of the input event received by an AWS Lambda function triggered by AWS API Gateway and integrated 
+    in `AWS_PROXY <https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-set-up-simple-proxy.html>`_ mode.
     """
 
     def __init__(self, event_object: dict):
         """
         Parameters
         ----------
         event_object : dict
@@ -441,62 +442,76 @@
 
         if claims and not isinstance(claims, dict):
             raise AwsEventSpecificationError(f"Claims should be a dict, not a {type(claims)}.")
 
         return claims
     
 
-class HttpClientError(RuntimeError):
+class HttpError(RuntimeError):
     """
-    Error that represents a HTTP response status code that comes with a message.
+    HTTP error response: status code and message.
+
+    Examples
+    --------
+    >>> raise HttpError(404, 'Not Found')    
     """
 
     def __init__(self, status: int, msg: str) -> None:
         """
         Parameters
         ----------
         status : int
             The HTTP response status code. This value is taken as-is, there is no validation routine.
         msg : str
             The explanatory message.
-
-        Examples
-        --------
-        >>> raise HttpClientError(404, 'Not sure where it is!')
         """
 
         super().__init__(msg)
 
         self._status = status
-        matched = re.match(r".*'.*\.(.*)'.*", str(self.__class__))
-
-        logger.error(f'{"" if matched is None else matched.group(1)}: {str(status)} - {str(msg)}')
 
 
     @property
     def status(self) -> int:
         """
-        Returns the HTTP response status code. 
-
-        Returns
-        -------
-        int
-            The HTTP response status code. 
+        int : HTTP response status code. 
 
         Examples
         --------
-        Given ``e = HttpClientError(403, 'Forbidden')``
+        Given ``e = HttpError(403, 'Forbidden')``
 
         >>> e.status
         403
         """
         
         return self._status
 
 
+class HttpClientError(HttpError):
+    """
+    Client HTTP error response.
+
+    Examples
+    --------
+    >>> raise HttpClientError(404, 'Not Found')    
+    """
+    pass
+
+
+class HttpServerError(HttpError):
+    """
+    Server-side HTTP error response.
+
+    Examples
+    --------
+    >>> raise HttpServerError(503, 'Service Unavailable')    
+    """
+    pass
+
+
 class HttpBadRequestError(HttpClientError):
     """
     Error that represents a HTTP response status 400 "Bad request".
     """
     
     def __init__(self, msg: typing.Optional[str] = None):
         """
@@ -1033,14 +1048,245 @@
         Examples
         --------
         >>> raise HttpRequestHeaderFieldsTooLargeError()               
         """
         
         httpStatus = HTTPStatus.REQUEST_HEADER_FIELDS_TOO_LARGE
         super().__init__(httpStatus.value, msg if msg else httpStatus.phrase)           
+
+
+class HttpInternalServerError(HttpServerError):
+    """
+    Error that represents a HTTP response status 500 "Internal server error".
+    """
+    
+    def __init__(self, msg: typing.Optional[str] = None):
+        """
+        Parameters
+        ----------
+        msg : str
+            Explanatory message. A default message is used if omitted.
+
+        Examples
+        --------
+        >>> raise HttpInternalServerError()               
+        """
+        
+        httpStatus = HTTPStatus.INTERNAL_SERVER_ERROR
+        super().__init__(httpStatus.value, msg if msg else httpStatus.phrase)       
+
+
+class HttpNotImplementedError(HttpServerError):
+    """
+    Error that represents a HTTP response status 501 "Not implemented".
+    """
+    
+    def __init__(self, msg: typing.Optional[str] = None):
+        """
+        Parameters
+        ----------
+        msg : str
+            Explanatory message. A default message is used if omitted.
+
+        Examples
+        --------
+        >>> raise HttpNotImplementedError()               
+        """
+        
+        httpStatus = HTTPStatus.NOT_IMPLEMENTED
+        super().__init__(httpStatus.value, msg if msg else httpStatus.phrase)  
+
+
+class HttpBadGatewayError(HttpServerError):
+    """
+    Error that represents a HTTP response status 502 "Bad gateway".
+    """
+    
+    def __init__(self, msg: typing.Optional[str] = None):
+        """
+        Parameters
+        ----------
+        msg : str
+            Explanatory message. A default message is used if omitted.
+
+        Examples
+        --------
+        >>> raise HttpBadGatewayError()               
+        """
+        
+        httpStatus = HTTPStatus.BAD_GATEWAY
+        super().__init__(httpStatus.value, msg if msg else httpStatus.phrase)  
+
+
+class HttpRServiceUnavailableError(HttpServerError):
+    """
+    Error that represents a HTTP response status 503 "Service unavailable".
+    """
+    
+    def __init__(self, msg: typing.Optional[str] = None):
+        """
+        Parameters
+        ----------
+        msg : str
+            Explanatory message. A default message is used if omitted.
+
+        Examples
+        --------
+        >>> raise HttpRServiceUnavailableError()               
+        """
+        
+        httpStatus = HTTPStatus.SERVICE_UNAVAILABLE
+        super().__init__(httpStatus.value, msg if msg else httpStatus.phrase)  
+
+
+class HttpGatewayTimeoutError(HttpServerError):
+    """
+    Error that represents a HTTP response status 504 "GatewayTimeout".
+    """
+    
+    def __init__(self, msg: typing.Optional[str] = None):
+        """
+        Parameters
+        ----------
+        msg : str
+            Explanatory message. A default message is used if omitted.
+
+        Examples
+        --------
+        >>> raise HttpGatewayTimeoutError()               
+        """
+        
+        httpStatus = HTTPStatus.GATEWAY_TIMEOUT
+        super().__init__(httpStatus.value, msg if msg else httpStatus.phrase)  
+
+
+class HttpVersionNotSupportedError(HttpServerError):
+    """
+    Error that represents a HTTP response status 505 "HTTP version not supported".
+    """
+    
+    def __init__(self, msg: typing.Optional[str] = None):
+        """
+        Parameters
+        ----------
+        msg : str
+            Explanatory message. A default message is used if omitted.
+
+        Examples
+        --------
+        >>> raise HttpVersionNotSupportedError()               
+        """
+        
+        httpStatus = HTTPStatus.HTTP_VERSION_NOT_SUPPORTED
+        super().__init__(httpStatus.value, msg if msg else httpStatus.phrase)  
+
+
+class HttpVarianteAlsoNegociatesError(HttpServerError):
+    """
+    Error that represents a HTTP response status 506 "Variant also negociates".
+    """
+    
+    def __init__(self, msg: typing.Optional[str] = None):
+        """
+        Parameters
+        ----------
+        msg : str
+            Explanatory message. A default message is used if omitted.
+
+        Examples
+        --------
+        >>> raise HttpVarianteAlsoNegociatesError()               
+        """
+        
+        httpStatus = HTTPStatus.VARIANT_ALSO_NEGOTIATES
+        super().__init__(httpStatus.value, msg if msg else httpStatus.phrase)  
+
+
+class HttpInsufficientStorageError(HttpServerError):
+    """
+    Error that represents a HTTP response status 507 "Insufficient storage".
+    """
+    
+    def __init__(self, msg: typing.Optional[str] = None):
+        """
+        Parameters
+        ----------
+        msg : str
+            Explanatory message. A default message is used if omitted.
+
+        Examples
+        --------
+        >>> raise HttpInsufficientStorageError()               
+        """
+        
+        httpStatus = HTTPStatus.INSUFFICIENT_STORAGE
+        super().__init__(httpStatus.value, msg if msg else httpStatus.phrase)  
+
+
+class HttpLoopDetectedError(HttpServerError):
+    """
+    Error that represents a HTTP response status 508 "Loop detected"".
+    """
+    
+    def __init__(self, msg: typing.Optional[str] = None):
+        """
+        Parameters
+        ----------
+        msg : str
+            Explanatory message. A default message is used if omitted.
+
+        Examples
+        --------
+        >>> raise HttpLoopDetectedError()               
+        """
+        
+        httpStatus = HTTPStatus.LOOP_DETECTED
+        super().__init__(httpStatus.value, msg if msg else httpStatus.phrase)  
+
+
+class HttpNotExtendedError(HttpServerError):
+    """
+    Error that represents a HTTP response status 510 "Not extended".
+    """
+    
+    def __init__(self, msg: typing.Optional[str] = None):
+        """
+        Parameters
+        ----------
+        msg : str
+            Explanatory message. A default message is used if omitted.
+
+        Examples
+        --------
+        >>> raise HttpNotExtendedError()               
+        """
+        
+        httpStatus = HTTPStatus.NOT_EXTENDED
+        super().__init__(httpStatus.value, msg if msg else httpStatus.phrase)  
+
+
+class HttpNetworkAuthenticationRequiredError(HttpServerError):
+    """
+    Error that represents a HTTP response status 511 "Network authentication required".
+    """
+    
+    def __init__(self, msg: typing.Optional[str] = None):
+        """
+        Parameters
+        ----------
+        msg : str
+            Explanatory message. A default message is used if omitted.
+
+        Examples
+        --------
+        >>> raise HttpNetworkAuthenticationRequiredError()               
+        """
+        
+        httpStatus = HTTPStatus.NETWORK_AUTHENTICATION_REQUIRED
+        super().__init__(httpStatus.value, msg if msg else httpStatus.phrase)         
         
 
 def simple_message(message: str) -> typing.Dict[str, str]:
     """
     Turns a ``str`` into a ``dict`` payload having "Message" as a key and the passed string as a value.
 
     :func:`build_http_response` uses this function to build response payloads from strings. 
@@ -1069,15 +1315,15 @@
 
 
 def determine_content_type(event: LambdaProxyEvent, *, custom_transformers: typing.Optional[typing.Dict[str, typing.Callable[[dict], typing.Tuple[str, str]]]] = None) -> str:
     """
     Determines the ``Content-Type`` of the response to be sent based on the ``Accept`` header of the request.
 
     ``application/json`` is the only ``Content-Type`` transformer available by default. It is mapped to the ``Accept`` values
-    ``*/*``, ``application/*`` and ``application/json``. Any other ``Accept`` value leads to a :class:`HttpNotAcceptableError` unless
+    ``*/*``, ``application/*`` and ``application/json``. Any other ``Accept`` value leads to a :exc:`HttpNotAcceptableError` unless
     ``custom_transformers`` map this ``Accept`` value to an appropriate transformer.
 
     Preferences are handled by :func:`LambdaProxyEvent.header_sorted_preferences`. Should no ``Accept`` header be given, ``*/*`` is assumed.
 
     Parameters
     ----------
     event : LambdaProxyEvent
@@ -1120,34 +1366,35 @@
     >>>
     >>> determine_content_type(event, custom_transformers=custom_transformers)
     'text/csv'
 
     Notes
     -----
     It is a good idea to call this function at the very beginning of your Lambda handler. This way you can make sure that
-    the accepted ``Content-Type`` matches what your API is capable of returning, and return an :class:`~HttpNotAcceptableError` 
+    the accepted ``Content-Type`` matches what your API is capable of returning, and return an :exc:`~HttpNotAcceptableError` 
     response without doing any unnecessary processing otherwise.
 
     The example below only accepts ``*/*``, ``application/*`` and ``application/json``, all mapped to ``application/json`` by default. 
 
     >>> def lambda_handler(raw_event, context):
     >>>     import awsmate.apigateway as amag
     >>>
+    >>>     event = amag.LambdaProxyEvent(raw_event) 
+    >>>
     >>>     try:
-    >>>         event = amag.LambdaProxyEvent(raw_event) 
     >>>         amag.determine_content_type(event)
     >>>
     >>>         # Everything you need to do
     >>>
     >>>         return amag.build_http_response(200, "OK", event=event)
     >>>
     >>>     except amag.HttpClientError as err:
-    >>>         return amag.build_http_client_error_response(err) # We will end up here should HttpNotAcceptableError be raised by determine_content_type()
+    >>>         return amag.build_http_client_error_response(err, event=event) # We will end up here should HttpNotAcceptableError be raised by determine_content_type()
     >>>     except Exception:
-    >>>         return amag.build_http_server_error_response()
+    >>>         return amag.build_http_server_error_response(amag.HttpInternalServerError(), event=event)
     """
 
     acceptedMimeTypes = event.header_sorted_preferences('Accept')
 
     if len(acceptedMimeTypes) == 0:
         acceptedMimeTypes = ( '*/*', None )
 
@@ -1249,15 +1496,15 @@
         event: typing.Optional[LambdaProxyEvent] = None, 
         custom_transformers: typing.Optional[typing.Dict[str, typing.Callable[[dict], typing.Tuple[str, str]]]] = None,
         extra_headers: typing.Optional[typing.Dict[str, str]] = None
     ) -> dict:
     """
     Builds the HTTP response the Lambda handler has to return to API Gateway.
 
-    Should the ``Accept`` header of the API call lead to a :class:`HttpNotAcceptableError`, an error message is returned instead
+    Should the ``Accept`` header of the API call lead to a :exc:`HttpNotAcceptableError`, an error message is returned instead
     of the passed payload and the status code is set accordingly. 
     
     This function handles the ``Accept-Encoding: gzip`` header of the API call for you. It also sets the base-64 flag of the response to ``True`` if
     the returned ``Content-Type`` is binary.
 
     Parameters
     ----------
@@ -1347,89 +1594,98 @@
     if useGzip:
         ret['headers']['Content-Encoding'] = 'gzip'
 
     return ret
 
 
 def build_http_server_error_response(
-        message: typing.Optional[str] = None, 
-        **kwargs: typing.Dict[str, typing.Any]
+        error: HttpServerError, *,
+        client_message: typing.Optional[str] = None,
+        log: bool = True,
+        **kwargs: typing.Any
     ) -> dict:
     """
-    Convenience function that builds an HTTP error 500 response to be returned to API Gateway by the Lambda handler.
+    Convenience function that builds an HTTP error 5XX response to be returned to API Gateway by the Lambda handler.
 
-    Warnings
-    --------
-    .. deprecated:: 0.2.0
-          `build_http_server_error_response` will change in version 0.3.0: the `message` positional parameter will be replaced by an
-          `error` parameter of type `HttpServerError` to be introduced in the same version.
+    Unless specified otherwise, calling this function logs a stack trace of the error showing the status and the actual error message. 
+    This message is replaced by a client-oriented message in the HTTP response.
 
     Parameters
     ----------
-    message : str
-        Optional error message. If omitted, the default message is "Sorry, an error occured. Please contact the API administrator to have this sorted out."
-    **kwarg : dict
+    error : HttpServerError
+        Object representing the error. 
+    client_message : str
+        Optional client-oriented message. An english canned message is used if omitted.
+    log : bool
+        Optional flag that defines whether a stack trace should be logged. ``True`` if omitted.
+    **kwarg : any
         Optional arguments to pass to :func:`build_http_response`
 
     Returns
     -------
     dict
-        The HTTP error 500 response to return to API Gateway.      
+        The HTTP error 5XX response to return to API Gateway.        
       
     Examples
     --------
-    >>> build_http_server_error_response('Oops, our bad...')
-    {'isBase64Encoded': False, 'statusCode': 500, 'body': '{\\n  "Message": "Oops, our bad..."\\n}', 'headers': {'Content-Type': 'application/json; charset=utf-8'}}
+    >>> build_http_server_error_response(HttpInsufficientStorageError(), client_message='Sorry, we have an issue.')
+    {'isBase64Encoded': False, 'statusCode': 507, 'body': '{\\n  "Message": "Sorry, we have an issue."\\n}', 'headers': {'Content-Type': 'application/json; charset=utf-8'}}
 
     Notes
     -----
-    This function simply calls:
-
-    >>> build_http_response(500, message, **kwargs)
-
-    It is a good idea to make your Lambda handler to catch all unexpected errors to return a proper error message should anything go wrong.
+    This function simply calls 
+    
+    >>> build_http_response(error.status, client_message, **kwargs)
+        
+    It is a good idea to make your Lambda handler to catch all unexpected errors to return a clean user-oriented error message should anything go wrong.
 
     >>> def lambda_handler(raw_event, context):
     >>>     import awsmate.apigateway as amag
-    >>>     from awsmate.logger import log_internal_error
     >>>
-    >>>     try:
-    >>>         event = amag.LambdaProxyEvent(raw_event) 
+    >>>     event = amag.LambdaProxyEvent(raw_event) 
     >>>
+    >>>     try:
     >>>         # Everything you need to do
     >>>
     >>>         return amag.build_http_response(200, "OK", event=event)
     >>>
     >>>     except amag.HttpClientError as err:
     >>>         return amag.build_http_client_error_response(err, event=event) 
     >>>     except Exception:
     >>>         # We will end up here should any unexpected error occur
-    >>>         log_internal_error("Logs everything you need in CloudWatch")
-    >>>         return amag.build_http_server_error_response(event=event) 
+    >>>         return amag.build_http_server_error_response(amag.HttpInternalServerError(), event=event) 
     """
     
+    if log:
+        log_internal_error(f'{error.status} - {error}')
+
     return build_http_response(
-        500, 
-        message if message else "Sorry, an error occured. Please contact the API administrator to have this sorted out.",
+        error.status, 
+        client_message if client_message else 'Sorry, an error occured. Please contact the API administrator to have this sorted out.',
         **kwargs
     )
 
 
 def build_http_client_error_response(
-        error: HttpClientError, 
-        **kwargs: typing.Dict[str, typing.Any]
+        error: HttpClientError, *,
+        log: bool = True,
+        **kwargs: typing.Any
     ) -> dict:
     """
     Convenience function that builds an HTTP error 4XX response to be returned to API Gateway by the Lambda handler.
 
+    Unless specified otherwise, calling this function logs an error showing the status and message. 
+
     Parameters
     ----------
     error : HttpClientError
         Object representing the error. 
-    **kwarg : dict
+    log : bool
+        Optional flag that defines whether a stack trace should be logged. ``True`` if omitted.
+    **kwarg : any
         Optional arguments to pass to :func:`build_http_response`
 
     Returns
     -------
     dict
         The HTTP error 4XX response to return to API Gateway.      
 
@@ -1440,30 +1696,33 @@
     
     Notes
     -----
     This function simply calls 
     
     >>> build_http_response(error.status, str(error), **kwargs)
 
-    It is a good idea to make your Lambda handler to catch all HttpClientError to return a proper error message should there be any problem with the request.
+    It is a good idea to make your Lambda handler to catch all HttpClientError to return a clean error message should there be any problem with the request.
 
     >>> def lambda_handler(raw_event, context):
     >>>     import awsmate.apigateway as amag
     >>>
-    >>>     try:
-    >>>         event = amag.LambdaProxyEvent(raw_event) 
+    >>>     event = amag.LambdaProxyEvent(raw_event) 
     >>>
+    >>>     try:
     >>>         # Everything you need to do
     >>>
     >>>         return amag.build_http_response(200, "OK", event=event)
     >>>
     >>>     except amag.HttpClientError as err:
     >>>         return amag.build_http_client_error_response(err, event=event) # We will end up here should anything be wrong in the client's request
     >>>     except Exception:
-    >>>         return amag.build_http_server_error_response(event=event) 
+    >>>         return amag.build_http_server_error_response(amag.HttpInternalServerError(), event=event) 
     """
 
+    if log:
+        logger.error(f'{error.status} - {error}')
+
     return build_http_response(
         error.status, 
         str(error),
         **kwargs
     )
```

### Comparing `awsmate-0.2.0/src/awsmate/eventbridge.py` & `awsmate-0.3.0/src/awsmate/eventbridge.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/src/awsmate/lambdafunction.py` & `awsmate-0.3.0/src/awsmate/lambdafunction.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         super().__init__(msg)
 
 
 class LambdaEvent():
     """
     Superclass of input events received by AWS Lambda functions triggered by the various AWS services. 
 
-    Without being abstract, this class has no other public method than :func:`LambdaEvent.__init__`.
+    Without being abstract, this class has no other public method than :meth:`LambdaEvent.__init__`.
     """
     
     @staticmethod
     def _raiseEventStructureError(msg: str) -> None:
         raise AwsEventSpecificationError(f"Event structure is not as expected: {msg}.")
```

### Comparing `awsmate-0.2.0/src/awsmate/logger.py` & `awsmate-0.3.0/src/awsmate/logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 import logging
 import traceback
-
+import typing
 
 defaultLevel = logging.INFO
 
 logging.basicConfig(format = '%(message)s', level = defaultLevel)
 
 logger = logging.getLogger()
 """
-Object used for logging.
-
-This object is a standard logger from the Python module ``logging``.
+logging.Logger : Standard logger from the Python module ``logging``.
 
 Examples
 --------
 >>> logger.warning('No configuration properties found. Used default values.')
 """
 
 logger.setLevel(defaultLevel)
 
 
-def log_internal_error(msg: str) -> None:
+def log_internal_error(msg: typing.Optional[str] = None) -> None:
     """
-    Logs an internal error with an explanatory message followed by a stack trace. 
+    Logs an error explanatory message followed by a stack trace. 
     
     This function is very useful if you redirect your Lambda function outputs to AWS Cloudwatch, which is recommended. Logs issued by 
     this function appear as ``CRITICAL``. 
 
     Parameters
     ----------
     msg : str
-        Explanatory message. 
+        Optional explanatory message. 
 
     Examples
     --------
     >>> try:
     >>>   raise RuntimeError('WOW!')
     >>> except Exception:
-    >>>   log_internal_error("Something wrong happened")
-    INTERNAL ERROR: Something wrong happened.
+    >>>   log_internal_error("This one is expected")
+    INTERNAL ERROR: This one is expected.
     Traceback (most recent call last):
     File "<stdin>", line 2, in <module>
     RuntimeError: WOW!
     """
     
     logger.critical(f"INTERNAL ERROR: {msg}.")
     logger.critical(traceback.format_exc())
```

### Comparing `awsmate-0.2.0/src/awsmate/s3.py` & `awsmate-0.3.0/src/awsmate/s3.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,246 +1,274 @@
-import typing
-        
-from awsmate.lambdafunction import LambdaEvent
-
-
-class LambdaNotificationEvent(LambdaEvent):
-    """
-    Mapping of the input event received by an AWS Lambda function triggered by AWS S3 Notification.
-    """
-
-    def __init__(self, event_object: dict):
-        """
-        Parameters
-        ----------
-        event_object : dict
-            The parameter ``event`` received by the AWS Lambda function handler.
-
-        Raises
-        ------
-        TypeError
-            If ``event_object`` is not a ``dict``.  
-                    
-        Examples
-        --------
-        >>> def lambda_handler(raw_event, context):
-        >>>     from awsmate.s3 import LambdaNotificationEvent
-        >>>     event = LambdaNotificationEvent(raw_event)                
-        """
-
-        super().__init__(event_object)
-
-
-    def _records_structure(self) -> dict:
-        KEY_RECORDS = "Records"
-
-        try:
-            ret = self._event[KEY_RECORDS][0]
-
-        except KeyError as err:
-            LambdaEvent._raiseCannotReachError(str(err))
-        
-        except IndexError:
-            LambdaEvent._raiseEventStructureError(f"'{KEY_RECORDS}' is empty")
-
-        if len(self._event[KEY_RECORDS]) != 1:
-            LambdaEvent._raiseEventStructureError(
-                f"event contains {str(len(self._event[KEY_RECORDS]))} {KEY_RECORDS} where 1 is expected"
-            )
-        
-        return ret
-        
-        
-    def _s3_structure(self) -> dict:
-        try:
-            ret = self._records_structure()["s3"]
-
-        except KeyError as err:
-            LambdaEvent._raiseCannotReachError(str(err))
-        
-        return ret
-    
-
-    def _object_structure(self) -> dict:
-        try:
-            ret = self._s3_structure()["object"]
-    
-        except KeyError as err:
-            LambdaEvent._raiseCannotReachError(str(err))
-
-        return ret         
-    
-
-    def _bucket_structure(self) -> dict:
-        try:
-            ret = self._s3_structure()["bucket"]
-    
-        except KeyError as err:
-            LambdaEvent._raiseCannotReachError(str(err))
-
-        return ret  
-    
-
-    def object_key(self) -> str:
-        """
-        Returns the key of the S3 object that is the subject of this notification.
-
-        Returns
-        -------
-        str
-            The key of the S3 object.
-
-        Raises
-        ------
-        awsmate.lambdafunction.AwsEventSpecificationError
-            If the event structure does not allow retrieving this key.         
-
-        Examples
-        --------
-        >>> event.objet_key()
-        'path/to/some/object'
-        """
-        
-        try:
-            ret = self._object_structure()["key"]
-    
-        except KeyError as err:
-            LambdaEvent._raiseCannotReachError(str(err))
-
-        return ret 
-
-
-    def object_size(self) -> typing.Optional[int]:
-        """
-        Returns the size of the S3 object that is the subject of this notification.
-
-        The size is only defined for object creation events, not for deletions.
-
-        Returns
-        -------
-        int
-            The size of the S3 object in bytes or ``None`` if not defined
-
-        Raises
-        ------
-        awsmate.lambdafunction.AwsEventSpecificationError
-            If the event structure is invalid.         
-
-        Examples
-        --------
-        >>> event.objet_size()
-        43168
-        """
-        
-        return self._object_structure().get('size', None)
-
-
-    def object_etag(self) -> typing.Optional[str]:
-        """
-        Returns the eTag of the S3 object that is the subject of this notification.
-
-        The eTag is only defined for object creation events, not for deletions.
-
-        Returns
-        -------
-        str
-            The eTag of the S3 object or ``None`` if not defined.
-
-        Raises
-        ------
-        awsmate.lambdafunction.AwsEventSpecificationError
-            If the event structure is invalid.         
-
-        Examples
-        --------
-        >>> event.objet_etag()
-        '8b38dac3b5c48c44704ec934eabae5a2'
-        """
-        
-        return self._object_structure().get('eTag', None)
-
-
-    def bucket_name(self) -> str:
-        """
-        Returns the name of the S3 bucket that is the subject of this notification.
-
-        Returns
-        -------
-        str
-            The name of the S3 bucket.
-
-        Raises
-        ------
-        awsmate.lambdafunction.AwsEventSpecificationError
-            If the event structure does not allow retrieving this bucket name.         
-
-        Examples
-        --------
-        >>> event.bucket_name()
-        'my-example-s3-bucket'
-        """
-        
-        try:
-            ret = self._bucket_structure()["name"]
-    
-        except KeyError as err:
-            LambdaEvent._raiseCannotReachError(str(err))
-
-        return ret     
-
-
-    def bucket_arn(self) -> str:
-        """
-        Returns the arn of the S3 bucket that is the subject of this notification.
-
-        Returns
-        -------
-        str
-            The arn of the S3 bucket.
-
-        Raises
-        ------
-        awsmate.lambdafunction.AwsEventSpecificationError
-            If the event structure does not allow retrieving this bucket arn.         
-
-        Examples
-        --------
-        >>> event.bucket_arn()
-        'arn:aws:s3:::my-example-s3-bucket'
-        """
-        
-        try:
-            ret = self._bucket_structure()["arn"]
-    
-        except KeyError as err:
-            LambdaEvent._raiseCannotReachError(str(err))
-
-        return ret  
-
-
-    def event_name(self) -> str:
-        """
-        Returns the name of the S3 event that triggered this notification.
-
-        Returns
-        -------
-        str
-            The S3 event name.
-
-        Raises
-        ------
-        awsmate.lambdafunction.AwsEventSpecificationError
-            If the event structure does not allow retrieving this event name.         
-
-        Examples
-        --------
-        >>> event.event_name()
-        'ObjectCreated:Put'
-        """
-        
-        try:
-            ret = self._records_structure()["eventName"]
-    
-        except KeyError as err:
-            LambdaEvent._raiseCannotReachError(str(err))
-
-        return ret          
+import typing
+        
+from urllib.parse import unquote_plus        
+from awsmate.lambdafunction import LambdaEvent
+
+
+class LambdaNotificationEvent(LambdaEvent):
+    """
+    Mapping of the input event received by an AWS Lambda function triggered by AWS S3 Notification.
+    """
+
+    def __init__(self, event_object: dict):
+        """
+        Parameters
+        ----------
+        event_object : dict
+            The parameter ``event`` received by the AWS Lambda function handler.
+
+        Raises
+        ------
+        TypeError
+            If ``event_object`` is not a ``dict``.  
+                    
+        Examples
+        --------
+        >>> def lambda_handler(raw_event, context):
+        >>>     from awsmate.s3 import LambdaNotificationEvent
+        >>>     event = LambdaNotificationEvent(raw_event)                
+        """
+
+        super().__init__(event_object)
+
+
+    def _records_structure(self) -> dict:
+        KEY_RECORDS = "Records"
+
+        try:
+            ret = self._event[KEY_RECORDS][0]
+
+        except KeyError as err:
+            LambdaEvent._raiseCannotReachError(str(err))
+        
+        except IndexError:
+            LambdaEvent._raiseEventStructureError(f"'{KEY_RECORDS}' is empty")
+
+        if len(self._event[KEY_RECORDS]) != 1:
+            LambdaEvent._raiseEventStructureError(
+                f"event contains {str(len(self._event[KEY_RECORDS]))} {KEY_RECORDS} where 1 is expected"
+            )
+        
+        return ret
+        
+        
+    def _s3_structure(self) -> dict:
+        try:
+            ret = self._records_structure()["s3"]
+
+        except KeyError as err:
+            LambdaEvent._raiseCannotReachError(str(err))
+        
+        return ret
+    
+
+    def _object_structure(self) -> dict:
+        try:
+            ret = self._s3_structure()["object"]
+    
+        except KeyError as err:
+            LambdaEvent._raiseCannotReachError(str(err))
+
+        return ret         
+    
+
+    def _bucket_structure(self) -> dict:
+        try:
+            ret = self._s3_structure()["bucket"]
+    
+        except KeyError as err:
+            LambdaEvent._raiseCannotReachError(str(err))
+
+        return ret  
+    
+
+    def object_key(self) -> str:
+        """
+        Returns the key of the S3 object that is the subject of this notification.
+
+        The returned value is URL decoded.
+
+        Returns
+        -------
+        str
+            The key of the S3 object.
+
+        Raises
+        ------
+        awsmate.lambdafunction.AwsEventSpecificationError
+            If the event structure does not allow retrieving this key.         
+
+        Examples
+        --------
+        >>> event.objet_key()
+        'path/to/object'
+        """
+        
+        try:
+            ret = unquote_plus(self._object_structure()["key"])
+    
+        except KeyError as err:
+            LambdaEvent._raiseCannotReachError(str(err))
+
+        return ret 
+
+
+    def object_size(self) -> typing.Optional[int]:
+        """
+        Returns the size of the S3 object that is the subject of this notification.
+
+        The size is only defined for object creation events, not for deletions.
+
+        Returns
+        -------
+        int
+            The size of the S3 object in bytes or ``None`` if not defined
+
+        Raises
+        ------
+        awsmate.lambdafunction.AwsEventSpecificationError
+            If the event structure is invalid.         
+
+        Examples
+        --------
+        >>> event.objet_size()
+        43168
+        """
+        
+        return self._object_structure().get('size', None)
+
+
+    def object_etag(self) -> typing.Optional[str]:
+        """
+        Returns the eTag of the S3 object that is the subject of this notification.
+
+        The eTag is only defined for object creation events, not for deletions.
+
+        Returns
+        -------
+        str
+            The eTag of the S3 object or ``None`` if not defined.
+
+        Raises
+        ------
+        awsmate.lambdafunction.AwsEventSpecificationError
+            If the event structure is invalid.         
+
+        Examples
+        --------
+        >>> event.objet_etag()
+        '8b38dac3b5c48c44704ec934eabae5a2'
+        """
+        
+        return self._object_structure().get('eTag', None)
+    
+
+    def object_url(self):
+        """
+        Returns the complete URL of the S3 object that is the subject of this notification.
+
+        The returned value is URL decoded.
+
+        Returns
+        -------
+        str
+            The URL of the S3 object.
+
+        Raises
+        ------
+        awsmate.lambdafunction.AwsEventSpecificationError
+            If the event structure is invalid.         
+
+        Examples
+        --------
+        >>> event.object_url()
+        's3://my-example-s3-bucket/path/to/object'
+        """
+ 
+        return f's3://{self.bucket_name()}/{self.object_key()}'
+
+
+    def bucket_name(self) -> str:
+        """
+        Returns the name of the S3 bucket that is the subject of this notification.
+
+        Returns
+        -------
+        str
+            The name of the S3 bucket.
+
+        Raises
+        ------
+        awsmate.lambdafunction.AwsEventSpecificationError
+            If the event structure does not allow retrieving this bucket name.         
+
+        Examples
+        --------
+        >>> event.bucket_name()
+        'my-example-s3-bucket'
+        """
+        
+        try:
+            ret = self._bucket_structure()["name"]
+    
+        except KeyError as err:
+            LambdaEvent._raiseCannotReachError(str(err))
+
+        return ret     
+
+
+    def bucket_arn(self) -> str:
+        """
+        Returns the arn of the S3 bucket that is the subject of this notification.
+
+        Returns
+        -------
+        str
+            The arn of the S3 bucket.
+
+        Raises
+        ------
+        awsmate.lambdafunction.AwsEventSpecificationError
+            If the event structure does not allow retrieving this bucket arn.         
+
+        Examples
+        --------
+        >>> event.bucket_arn()
+        'arn:aws:s3:::my-example-s3-bucket'
+        """
+        
+        try:
+            ret = self._bucket_structure()["arn"]
+    
+        except KeyError as err:
+            LambdaEvent._raiseCannotReachError(str(err))
+
+        return ret  
+
+
+    def event_name(self) -> str:
+        """
+        Returns the name of the S3 event that triggered this notification.
+
+        Returns
+        -------
+        str
+            The S3 event name.
+
+        Raises
+        ------
+        awsmate.lambdafunction.AwsEventSpecificationError
+            If the event structure does not allow retrieving this event name.         
+
+        Examples
+        --------
+        >>> event.event_name()
+        'ObjectCreated:Put'
+        """
+        
+        try:
+            ret = self._records_structure()["eventName"]
+    
+        except KeyError as err:
+            LambdaEvent._raiseCannotReachError(str(err))
+
+        return ret
```

### Comparing `awsmate-0.2.0/tests/unit/test_apigateway.py` & `awsmate-0.3.0/tests/unit/test_apigateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -787,25 +787,14 @@
     message = f'{random.randint(1000, 9999)} some text'
 
     test = ag.HttpClientError(status, message)
 
     assert str(test) == message
 
 
-def test_HttpClientError_init_logsProperly(caplog):
-    import re
-
-    status = random.randint(200, 599)
-    message = f'{random.randint(1000, 9999)} some text'
-
-    ag.HttpClientError(status, message)
-
-    assert re.match(f'ERROR    root:apigateway.py:[0-9]{{3}} HttpClientError: {str(status)} - {message}\n', caplog.text)
-
-
 def test_simple_message_returnsProperPayload():
     message = f'{random.randint(0, 9999)} with some blablah'
 
     payload = ag.simple_message(message)
 
     assert payload == { "Message": message }
 
@@ -1129,41 +1118,62 @@
 
     response = ag.build_http_response(status, payload, extra_headers = extra_headers)
 
     assert response == expectedResponse    
 
 
 def test_build_http_server_error_response_passeAllParameters():
-    message = 'some msg'
+    error = ag.HttpInsufficientStorageError()
+    msg = 'client message'
     event = ag.LambdaProxyEvent({})
     transformers = { 'text/*': lambda x : (x, 'text/strange') }
     extra_headers={ 'someKey': 'someValue' }
 
     with patch('awsmate.apigateway.build_http_response') as mbhser:
-        ag.build_http_server_error_response(message, event=event, custom_transformers=transformers, extra_headers=extra_headers)
+        ag.build_http_server_error_response(error, client_message=msg, event=event, custom_transformers=transformers, extra_headers=extra_headers)
 
     mbhser.assert_called_once_with(
-        500, 
-        message, 
+        507, 
+        msg, 
         event=event,
         custom_transformers=transformers,
         extra_headers=extra_headers
     )
     
 
 def test_build_http_server_error_response_usesDefaultMessageIfUnspecified():
     with patch('awsmate.apigateway.build_http_response') as mbhser:
-        ag.build_http_server_error_response()
+        ag.build_http_server_error_response(ag.HttpRServiceUnavailableError())
 
     mbhser.assert_called_once_with(
-        500, 
+        503, 
         "Sorry, an error occured. Please contact the API administrator to have this sorted out.", 
     )
 
 
+def test_build_http_server_error_response_callsLoggerByDefault():
+    error = ag.HttpRServiceUnavailableError()
+
+    with patch('awsmate.apigateway.build_http_response'):
+        with patch('awsmate.apigateway.log_internal_error') as mlie:
+            ag.build_http_server_error_response(error)
+
+    mlie.assert_called_once_with(f'{error.status} - {str(error)}')    
+
+
+def test_build_http_server_error_response_doesNotCallsLoggerIfSpecified():
+    error = ag.HttpRServiceUnavailableError()
+
+    with patch('awsmate.apigateway.build_http_response'):
+        with patch('awsmate.apigateway.log_internal_error') as mlie:
+            ag.build_http_server_error_response(error, log=False)
+
+    mlie.assert_not_called()
+
+
 def test_build_http_client_error_response_passeAllParameters():
     exception = ag.HttpBadRequestError("some message")
     event = ag.LambdaProxyEvent({})
     transformers = { 'text/*': lambda x : (x, 'text/strange') }
     extra_headers={ 'someKey': 'someValue' }
 
     with patch('awsmate.apigateway.build_http_response') as mbhser:
@@ -1172,7 +1182,28 @@
     mbhser.assert_called_once_with(
         exception.status, 
         str(exception), 
         event=event,
         custom_transformers=transformers,
         extra_headers=extra_headers
     )
+
+
+def test_build_http_client_error_response_callsLoggerByDefault():
+    error = ag.HttpNotFoundError()
+
+    with patch('awsmate.apigateway.build_http_response'):
+        with patch.object(ag.logger, 'error') as mle:
+            ag.build_http_client_error_response(error)
+
+    mle.assert_called_once_with(f'{error.status} - {str(error)}')  
+
+
+def test_build_http_client_error_response_doesNotCallsLoggerIfSpecified():
+    error = ag.HttpNotFoundError()
+
+    with patch('awsmate.apigateway.build_http_response'):
+        with patch.object(ag.logger, 'error') as mle:
+            ag.build_http_client_error_response(error, log=False)
+
+    mle.assert_not_called()  
+
```

### Comparing `awsmate-0.2.0/tests/unit/test_eventbridge.py` & `awsmate-0.3.0/tests/unit/test_eventbridge.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/tests/unit/test_lambdafunction.py` & `awsmate-0.3.0/tests/unit/test_lambdafunction.py`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/tests/unit/test_s3.py` & `awsmate-0.3.0/tests/unit/test_s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,14 +245,32 @@
     }    
 
     test = s3.LambdaNotificationEvent(event)
 
     assert test.object_key() == "stuff" 
 
 
+def test_LambdaNotificationEvent_object_key_performsUrlDecoding():
+    event = {
+        "Records": [
+            {
+                "s3": {
+                    "object": {
+                        "key": "stuff+stuff%20and+more%20stuff%21+Et%20voil%C3%A0."
+                    }
+                }
+            }
+        ]
+    }    
+
+    test = s3.LambdaNotificationEvent(event)
+
+    assert test.object_key() == "stuff stuff and more stuff! Et voilà."     
+
+
 def test_LambdaNotificationEvent_object_key_raisesIfEventDoesNotHaveAKeyUnderObject():
     event = {
         "Records": [
             {
                 "s3": {
                     "object": {}
                 }
@@ -396,14 +414,35 @@
 
     with patch.object(s3.LambdaNotificationEvent, '_object_structure') as ms3n:
         test.object_etag()
 
     ms3n.assert_called_once_with()
 
 
+def test_LambdaNotificationEvent_object_url_returnsTheExpectedValue():
+    event = {
+        "Records": [
+            {
+                "s3": {
+                    "bucket": {
+                        "name": "my-example-bucket"
+                    },
+                    "object": {
+                        "key": "some/stuff"
+                    }
+                }
+            }
+        ]
+    }    
+
+    test = s3.LambdaNotificationEvent(event)
+
+    assert test.object_url() == "s3://my-example-bucket/some/stuff"
+    
+
 def test_LambdaNotificationEvent_bucket_name_returnsTheExpectedValue():
     event = {
         "Records": [
             {
                 "s3": {
                     "bucket": {
                         "name": "my-example-bucket"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `awsmate-0.2.0/LICENSE.txt` & `awsmate-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/README.md` & `awsmate-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `awsmate-0.2.0/pyproject.toml` & `awsmate-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build" 
 
 [project]
 name = "awsmate"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
     { name="Vincent Poulain (Shlublu)", email="shlublu@yahoo.fr" },
 ]
-description = "A companion for your AWS Python developments. It provides you with helper code that facilitates the use of various AWS services."
+description = "A companion for your AWS Python developments."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Intended Audience :: Developers",
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.9",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)"
 ]
-keywords = ["python", "aws", "aws-apigateway", "aws-lambda", "aws-s3"]
+keywords = ["python", "aws", "aws-apigateway", "aws-eventbridge", "aws-lambda", "aws-s3"]
 
 [project.urls]
 "Repository" = "https://github.com/shlublu/awsmate"
 "Documentation" = "https://awsmate.readthedocs.io/"
 "Bug Tracker" = "https://github.com/shlublu/awsmate/issues"
 "Changelog" = "https://github.com/shlublu/awsmate/blob/master/CHANGELOG.md"
```

### Comparing `awsmate-0.2.0/PKG-INFO` & `awsmate-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: awsmate
-Version: 0.2.0
-Summary: A companion for your AWS Python developments. It provides you with helper code that facilitates the use of various AWS services.
+Version: 0.3.0
+Summary: A companion for your AWS Python developments.
 Project-URL: Repository, https://github.com/shlublu/awsmate
 Project-URL: Documentation, https://awsmate.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/shlublu/awsmate/issues
 Project-URL: Changelog, https://github.com/shlublu/awsmate/blob/master/CHANGELOG.md
 Author-email: "Vincent Poulain (Shlublu)" <shlublu@yahoo.fr>
 License-File: LICENSE.txt
-Keywords: aws,aws-apigateway,aws-lambda,aws-s3,python
+Keywords: aws,aws-apigateway,aws-eventbridge,aws-lambda,aws-s3,python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
```

