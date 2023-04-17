# Comparing `tmp/cloudsnorkel.cdk-github-runners-0.9.4.tar.gz` & `tmp/cloudsnorkel.cdk-github-runners-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudsnorkel.cdk-github-runners-0.9.4.tar", last modified: Wed Apr 12 00:08:28 2023, max compression
+gzip compressed data, was "cloudsnorkel.cdk-github-runners-0.9.5.tar", last modified: Mon Apr 17 04:11:37 2023, max compression
```

## Comparing `cloudsnorkel.cdk-github-runners-0.9.4.tar` & `cloudsnorkel.cdk-github-runners-0.9.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:08:28.739040 cloudsnorkel.cdk-github-runners-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-04-12 00:08:28.739040 cloudsnorkel.cdk-github-runners-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 00:08:28.739040 cloudsnorkel.cdk-github-runners-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:08:28.731040 cloudsnorkel.cdk-github-runners-0.9.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:08:28.731040 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:08:28.735040 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel/cdk_github_runners/
--rw-r--r--   0 runner    (1001) docker     (123)   555013 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel/cdk_github_runners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:08:28.735040 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel/cdk_github_runners/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel/cdk_github_runners/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1986936 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel/cdk_github_runners/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:08:28.735040 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel.cdk_github_runners.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-04-12 00:08:28.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-12 00:08:28.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 00:08:28.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel.cdk_github_runners.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 00:08:28.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel.cdk_github_runners.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 00:08:28.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel.cdk_github_runners.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:11:37.405109 cloudsnorkel.cdk-github-runners-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-04-17 04:11:37.405109 cloudsnorkel.cdk-github-runners-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 04:11:37.405109 cloudsnorkel.cdk-github-runners-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:11:37.401109 cloudsnorkel.cdk-github-runners-0.9.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:11:37.401109 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:11:37.401109 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel/cdk_github_runners/
+-rw-r--r--   0 runner    (1001) docker     (123)   560908 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel/cdk_github_runners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:11:37.401109 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel/cdk_github_runners/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel/cdk_github_runners/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1988051 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 04:11:25.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel/cdk_github_runners/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 04:11:37.401109 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel.cdk_github_runners.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-04-17 04:11:37.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-17 04:11:37.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 04:11:37.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel.cdk_github_runners.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 04:11:37.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel.cdk_github_runners.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 04:11:37.000000 cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel.cdk_github_runners.egg-info/top_level.txt
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.4/LICENSE` & `cloudsnorkel.cdk-github-runners-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudsnorkel.cdk-github-runners-0.9.4/PKG-INFO` & `cloudsnorkel.cdk-github-runners-0.9.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudsnorkel.cdk-github-runners
-Version: 0.9.4
+Version: 0.9.5
 Summary: CDK construct to create GitHub Actions self-hosted runners. A webhook listens to events and creates ephemeral runners on the fly.
 Home-page: https://github.com/CloudSnorkel/cdk-github-runners.git
 Author: Amir Szekely<amir@cloudsnorkel.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/CloudSnorkel/cdk-github-runners.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GitHub Self-Hosted Runners CDK Constructs
 
 [![NPM](https://img.shields.io/npm/v/@cloudsnorkel/cdk-github-runners?label=npm&logo=npm)](https://www.npmjs.com/package/@cloudsnorkel/cdk-github-runners)
 [![PyPI](https://img.shields.io/pypi/v/cloudsnorkel.cdk-github-runners?label=pypi&logo=pypi)](https://pypi.org/project/cloudsnorkel.cdk-github-runners)
-[![Maven Central](https://img.shields.io/maven-central/v/com.cloudsnorkel/cdk.github.runners.svg?label=Maven%20Central&logo=java)](https://search.maven.org/search?q=g:%22com.cloudsnorkel%22%20AND%20a:%22cdk.github.runners%22)
+[![Maven Central](https://img.shields.io/maven-central/v/com.cloudsnorkel/cdk.github.runners.svg?label=Maven%20Central&logo=apachemaven)](https://search.maven.org/search?q=g:%22com.cloudsnorkel%22%20AND%20a:%22cdk.github.runners%22)
 [![Go](https://img.shields.io/github/v/tag/CloudSnorkel/cdk-github-runners?color=red&label=go&logo=go)](https://pkg.go.dev/github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners)
 [![Nuget](https://img.shields.io/nuget/v/CloudSnorkel.Cdk.Github.Runners?color=red&&logo=nuget)](https://www.nuget.org/packages/CloudSnorkel.Cdk.Github.Runners/)
 [![Release](https://github.com/CloudSnorkel/cdk-github-runners/actions/workflows/release.yml/badge.svg)](https://github.com/CloudSnorkel/cdk-github-runners/actions/workflows/release.yml)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/CloudSnorkel/cdk-github-runners/blob/main/LICENSE)
 
 Use this CDK construct to create ephemeral [self-hosted GitHub runners](https://docs.github.com/en/actions/hosting-your-own-runners/about-self-hosted-runners) on-demand inside your AWS account.
 
@@ -41,14 +41,15 @@
 * Automatically updated build environment with latest runner version
 
 Self-hosted runners in AWS are useful when:
 
 * You need easy access to internal resources in your actions
 * You want to pre-install some software for your actions
 * You want to provide some basic AWS API access (but [aws-actions/configure-aws-credentials](https://github.com/marketplace/actions/configure-aws-credentials-action-for-github-actions) has more security controls)
+* You are using GitHub Enterprise Server
 
 Ephemeral (or on-demand) runners are the [recommended way by GitHub](https://docs.github.com/en/actions/hosting-your-own-runners/autoscaling-with-self-hosted-runners#using-ephemeral-runners-for-autoscaling) for auto-scaling, and they make sure all jobs run with a clean image. Runners are started on-demand. You don't pay unless a job is running.
 
 ## API
 
 The best way to browse API documentation is on [Constructs Hub](https://constructs.dev/packages/@cloudsnorkel/cdk-github-runners/). It is available in all supported programming languages.
 
@@ -239,22 +240,34 @@
 
 ## Troubleshooting
 
 1. Always start with the status function, make sure no errors are reported, and confirm all status codes are OK
 2. If jobs are stuck on pending:
 
    1. Make sure `runs-on` in the workflow matches the expected labels set in the runner provider
-   2. If it happens every time, cancel the job and start it again
+   2. If jobs get stuck often and take a long time to start, cancel the pending jobs and start them again
 3. Confirm the webhook Lambda was called by visiting the URL in `troubleshooting.webhookHandlerUrl` from `status.json`
 
    1. If it's not called or logs errors, confirm the webhook settings on the GitHub side
    2. If you see too many errors, make sure you're only sending `workflow_job` events
 4. When using GitHub app, make sure there are active installation in `github.auth.app.installations`
 5. Check execution details of the orchestrator step function by visiting the URL in `troubleshooting.stepFunctionUrl` from `status.json`
 
    1. Use the details tab to find the specific execution of the provider (Lambda, CodeBuild, Fargate, etc.)
    2. Every step function execution should be successful, even if the runner action inside it failed
 
+## Monitoring
+
+There are two important ways to monitor your runners:
+
+1. Make sure runners don't fail to start. When that happens, jobs may sit and wait. Use `GitHubRunners.metricFailed()` to get a metric for the number of failed runner starts. You should use this metric to trigger an alarm.
+2. Make sure runner images don't fail to build. Failed runner image builds mean you will get stuck with out-of-date software on your runners. It may lead to security vulnerabilities, or it may lead to slower runner start-ups as the runner software itself needs to be updated. Use `GitHubRunners.failedImageBuildsTopic()` to get SNS topic that gets notified of failed runner image builds. You should subscribe to this topic.
+
+Other useful metrics to track:
+
+1. Use `GitHubRunners.metricJobCompleted()` to get a metric for the number of completed jobs broken down by labels and job success.
+2. Use `GitHubRunners.metricTime()` to get a metric for the total time a runner is running. This includes the overhead of starting the runner.
+
 ## Other Options
 
 1. [philips-labs/terraform-aws-github-runner](https://github.com/philips-labs/terraform-aws-github-runner) if you're using Terraform
 2. [actions/actions-runner-controller](https://github.com/actions/actions-runner-controller) if you're using Kubernetes
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.4/README.md` & `cloudsnorkel.cdk-github-runners-0.9.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # GitHub Self-Hosted Runners CDK Constructs
 
 [![NPM](https://img.shields.io/npm/v/@cloudsnorkel/cdk-github-runners?label=npm&logo=npm)](https://www.npmjs.com/package/@cloudsnorkel/cdk-github-runners)
 [![PyPI](https://img.shields.io/pypi/v/cloudsnorkel.cdk-github-runners?label=pypi&logo=pypi)](https://pypi.org/project/cloudsnorkel.cdk-github-runners)
-[![Maven Central](https://img.shields.io/maven-central/v/com.cloudsnorkel/cdk.github.runners.svg?label=Maven%20Central&logo=java)](https://search.maven.org/search?q=g:%22com.cloudsnorkel%22%20AND%20a:%22cdk.github.runners%22)
+[![Maven Central](https://img.shields.io/maven-central/v/com.cloudsnorkel/cdk.github.runners.svg?label=Maven%20Central&logo=apachemaven)](https://search.maven.org/search?q=g:%22com.cloudsnorkel%22%20AND%20a:%22cdk.github.runners%22)
 [![Go](https://img.shields.io/github/v/tag/CloudSnorkel/cdk-github-runners?color=red&label=go&logo=go)](https://pkg.go.dev/github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners)
 [![Nuget](https://img.shields.io/nuget/v/CloudSnorkel.Cdk.Github.Runners?color=red&&logo=nuget)](https://www.nuget.org/packages/CloudSnorkel.Cdk.Github.Runners/)
 [![Release](https://github.com/CloudSnorkel/cdk-github-runners/actions/workflows/release.yml/badge.svg)](https://github.com/CloudSnorkel/cdk-github-runners/actions/workflows/release.yml)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/CloudSnorkel/cdk-github-runners/blob/main/LICENSE)
 
 Use this CDK construct to create ephemeral [self-hosted GitHub runners](https://docs.github.com/en/actions/hosting-your-own-runners/about-self-hosted-runners) on-demand inside your AWS account.
 
@@ -17,14 +17,15 @@
 * Automatically updated build environment with latest runner version
 
 Self-hosted runners in AWS are useful when:
 
 * You need easy access to internal resources in your actions
 * You want to pre-install some software for your actions
 * You want to provide some basic AWS API access (but [aws-actions/configure-aws-credentials](https://github.com/marketplace/actions/configure-aws-credentials-action-for-github-actions) has more security controls)
+* You are using GitHub Enterprise Server
 
 Ephemeral (or on-demand) runners are the [recommended way by GitHub](https://docs.github.com/en/actions/hosting-your-own-runners/autoscaling-with-self-hosted-runners#using-ephemeral-runners-for-autoscaling) for auto-scaling, and they make sure all jobs run with a clean image. Runners are started on-demand. You don't pay unless a job is running.
 
 ## API
 
 The best way to browse API documentation is on [Constructs Hub](https://constructs.dev/packages/@cloudsnorkel/cdk-github-runners/). It is available in all supported programming languages.
 
@@ -215,22 +216,34 @@
 
 ## Troubleshooting
 
 1. Always start with the status function, make sure no errors are reported, and confirm all status codes are OK
 2. If jobs are stuck on pending:
 
    1. Make sure `runs-on` in the workflow matches the expected labels set in the runner provider
-   2. If it happens every time, cancel the job and start it again
+   2. If jobs get stuck often and take a long time to start, cancel the pending jobs and start them again
 3. Confirm the webhook Lambda was called by visiting the URL in `troubleshooting.webhookHandlerUrl` from `status.json`
 
    1. If it's not called or logs errors, confirm the webhook settings on the GitHub side
    2. If you see too many errors, make sure you're only sending `workflow_job` events
 4. When using GitHub app, make sure there are active installation in `github.auth.app.installations`
 5. Check execution details of the orchestrator step function by visiting the URL in `troubleshooting.stepFunctionUrl` from `status.json`
 
    1. Use the details tab to find the specific execution of the provider (Lambda, CodeBuild, Fargate, etc.)
    2. Every step function execution should be successful, even if the runner action inside it failed
 
+## Monitoring
+
+There are two important ways to monitor your runners:
+
+1. Make sure runners don't fail to start. When that happens, jobs may sit and wait. Use `GitHubRunners.metricFailed()` to get a metric for the number of failed runner starts. You should use this metric to trigger an alarm.
+2. Make sure runner images don't fail to build. Failed runner image builds mean you will get stuck with out-of-date software on your runners. It may lead to security vulnerabilities, or it may lead to slower runner start-ups as the runner software itself needs to be updated. Use `GitHubRunners.failedImageBuildsTopic()` to get SNS topic that gets notified of failed runner image builds. You should subscribe to this topic.
+
+Other useful metrics to track:
+
+1. Use `GitHubRunners.metricJobCompleted()` to get a metric for the number of completed jobs broken down by labels and job success.
+2. Use `GitHubRunners.metricTime()` to get a metric for the total time a runner is running. This includes the overhead of starting the runner.
+
 ## Other Options
 
 1. [philips-labs/terraform-aws-github-runner](https://github.com/philips-labs/terraform-aws-github-runner) if you're using Terraform
 2. [actions/actions-runner-controller](https://github.com/actions/actions-runner-controller) if you're using Kubernetes
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.4/setup.py` & `cloudsnorkel.cdk-github-runners-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudsnorkel.cdk-github-runners",
-    "version": "0.9.4",
+    "version": "0.9.5",
     "description": "CDK construct to create GitHub Actions self-hosted runners. A webhook listens to events and creates ephemeral runners on the fly.",
     "license": "Apache-2.0",
     "url": "https://github.com/CloudSnorkel/cdk-github-runners.git",
     "long_description_content_type": "text/markdown",
     "author": "Amir Szekely<amir@cloudsnorkel.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudsnorkel.cdk_github_runners",
         "cloudsnorkel.cdk_github_runners._jsii"
     ],
     "package_data": {
         "cloudsnorkel.cdk_github_runners._jsii": [
-            "cdk-github-runners@0.9.4.jsii.tgz"
+            "cdk-github-runners@0.9.5.jsii.tgz"
         ],
         "cloudsnorkel.cdk_github_runners": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel/cdk_github_runners/__init__.py` & `cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel/cdk_github_runners/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 # GitHub Self-Hosted Runners CDK Constructs
 
 [![NPM](https://img.shields.io/npm/v/@cloudsnorkel/cdk-github-runners?label=npm&logo=npm)](https://www.npmjs.com/package/@cloudsnorkel/cdk-github-runners)
 [![PyPI](https://img.shields.io/pypi/v/cloudsnorkel.cdk-github-runners?label=pypi&logo=pypi)](https://pypi.org/project/cloudsnorkel.cdk-github-runners)
-[![Maven Central](https://img.shields.io/maven-central/v/com.cloudsnorkel/cdk.github.runners.svg?label=Maven%20Central&logo=java)](https://search.maven.org/search?q=g:%22com.cloudsnorkel%22%20AND%20a:%22cdk.github.runners%22)
+[![Maven Central](https://img.shields.io/maven-central/v/com.cloudsnorkel/cdk.github.runners.svg?label=Maven%20Central&logo=apachemaven)](https://search.maven.org/search?q=g:%22com.cloudsnorkel%22%20AND%20a:%22cdk.github.runners%22)
 [![Go](https://img.shields.io/github/v/tag/CloudSnorkel/cdk-github-runners?color=red&label=go&logo=go)](https://pkg.go.dev/github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners)
 [![Nuget](https://img.shields.io/nuget/v/CloudSnorkel.Cdk.Github.Runners?color=red&&logo=nuget)](https://www.nuget.org/packages/CloudSnorkel.Cdk.Github.Runners/)
 [![Release](https://github.com/CloudSnorkel/cdk-github-runners/actions/workflows/release.yml/badge.svg)](https://github.com/CloudSnorkel/cdk-github-runners/actions/workflows/release.yml)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/CloudSnorkel/cdk-github-runners/blob/main/LICENSE)
 
 Use this CDK construct to create ephemeral [self-hosted GitHub runners](https://docs.github.com/en/actions/hosting-your-own-runners/about-self-hosted-runners) on-demand inside your AWS account.
 
@@ -18,14 +18,15 @@
 * Automatically updated build environment with latest runner version
 
 Self-hosted runners in AWS are useful when:
 
 * You need easy access to internal resources in your actions
 * You want to pre-install some software for your actions
 * You want to provide some basic AWS API access (but [aws-actions/configure-aws-credentials](https://github.com/marketplace/actions/configure-aws-credentials-action-for-github-actions) has more security controls)
+* You are using GitHub Enterprise Server
 
 Ephemeral (or on-demand) runners are the [recommended way by GitHub](https://docs.github.com/en/actions/hosting-your-own-runners/autoscaling-with-self-hosted-runners#using-ephemeral-runners-for-autoscaling) for auto-scaling, and they make sure all jobs run with a clean image. Runners are started on-demand. You don't pay unless a job is running.
 
 ## API
 
 The best way to browse API documentation is on [Constructs Hub](https://constructs.dev/packages/@cloudsnorkel/cdk-github-runners/). It is available in all supported programming languages.
 
@@ -216,25 +217,37 @@
 
 ## Troubleshooting
 
 1. Always start with the status function, make sure no errors are reported, and confirm all status codes are OK
 2. If jobs are stuck on pending:
 
    1. Make sure `runs-on` in the workflow matches the expected labels set in the runner provider
-   2. If it happens every time, cancel the job and start it again
+   2. If jobs get stuck often and take a long time to start, cancel the pending jobs and start them again
 3. Confirm the webhook Lambda was called by visiting the URL in `troubleshooting.webhookHandlerUrl` from `status.json`
 
    1. If it's not called or logs errors, confirm the webhook settings on the GitHub side
    2. If you see too many errors, make sure you're only sending `workflow_job` events
 4. When using GitHub app, make sure there are active installation in `github.auth.app.installations`
 5. Check execution details of the orchestrator step function by visiting the URL in `troubleshooting.stepFunctionUrl` from `status.json`
 
    1. Use the details tab to find the specific execution of the provider (Lambda, CodeBuild, Fargate, etc.)
    2. Every step function execution should be successful, even if the runner action inside it failed
 
+## Monitoring
+
+There are two important ways to monitor your runners:
+
+1. Make sure runners don't fail to start. When that happens, jobs may sit and wait. Use `GitHubRunners.metricFailed()` to get a metric for the number of failed runner starts. You should use this metric to trigger an alarm.
+2. Make sure runner images don't fail to build. Failed runner image builds mean you will get stuck with out-of-date software on your runners. It may lead to security vulnerabilities, or it may lead to slower runner start-ups as the runner software itself needs to be updated. Use `GitHubRunners.failedImageBuildsTopic()` to get SNS topic that gets notified of failed runner image builds. You should subscribe to this topic.
+
+Other useful metrics to track:
+
+1. Use `GitHubRunners.metricJobCompleted()` to get a metric for the number of completed jobs broken down by labels and job success.
+2. Use `GitHubRunners.metricTime()` to get a metric for the total time a runner is running. This includes the overhead of starting the runner.
+
 ## Other Options
 
 1. [philips-labs/terraform-aws-github-runner](https://github.com/philips-labs/terraform-aws-github-runner) if you're using Terraform
 2. [actions/actions-runner-controller](https://github.com/actions/actions-runner-controller) if you're using Kubernetes
 '''
 import abc
 import builtins
@@ -301,15 +314,15 @@
         security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
         subnet_selection: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
         vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''(experimental) Properties for {@link AmiBuilder} construct.
 
         :param architecture: (experimental) Image architecture. Default: Architecture.X86_64
-        :param install_docker: (experimental) Install Docker inside the image, so it can be used by the runner. You may want to disable this if you are building a Windows image and don't have a Docker Desktop license. Default: true
+        :param install_docker: (experimental) Install Docker inside the image, so it can be used by the runner. Default: true
         :param instance_type: (experimental) The instance type used to build the image. Default: m5.large
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
         :param os: (experimental) Image OS. Default: OS.LINUX
         :param rebuild_interval: (experimental) Schedule the AMI to be rebuilt every given interval. Useful for keeping the AMI up-do-date with the latest GitHub runner version and latest OS updates. Set to zero to disable. Default: Duration.days(7)
         :param runner_version: (experimental) Version of GitHub Runners to install. Default: latest version available
         :param security_group: (deprecated) Security group to assign to launched builder instances. Default: new security group
@@ -372,16 +385,14 @@
         result = self._values.get("architecture")
         return typing.cast(typing.Optional["Architecture"], result)
 
     @builtins.property
     def install_docker(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Install Docker inside the image, so it can be used by the runner.
 
-        You may want to disable this if you are building a Windows image and don't have a Docker Desktop license.
-
         :default: true
 
         :stability: experimental
         '''
         result = self._values.get("install_docker")
         return typing.cast(typing.Optional[builtins.bool], result)
 
@@ -776,15 +787,15 @@
         timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''(experimental) Properties for CodeBuildImageBuilder construct.
 
         :param dockerfile_path: (experimental) Path to Dockerfile to be built. It can be a path to a Dockerfile, a folder containing a Dockerfile, or a zip file containing a Dockerfile.
         :param architecture: (experimental) Image architecture. Default: Architecture.X86_64
-        :param build_image: (experimental) Build image to use in CodeBuild. This is the image that's going to run the code that builds the runner image. The only action taken in CodeBuild is running ``docker build``. You would therefore not need to change this setting often. Default: Ubuntu 20.04 for x64 and Amazon Linux 2 for ARM64
+        :param build_image: (experimental) Build image to use in CodeBuild. This is the image that's going to run the code that builds the runner image. The only action taken in CodeBuild is running ``docker build``. You would therefore not need to change this setting often. Default: Ubuntu 22.04 for x64 and Amazon Linux 2 for ARM64
         :param compute_type: (experimental) The type of compute to use for this build. See the {@link ComputeType} enum for the possible values. Default: {@link ComputeType#SMALL }
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
         :param os: (experimental) Image OS. Default: OS.LINUX
         :param rebuild_interval: (experimental) Schedule the image to be rebuilt every given interval. Useful for keeping the image up-do-date with the latest GitHub runner version and latest OS updates. Set to zero to disable. Default: Duration.days(7)
         :param runner_version: (experimental) Version of GitHub Runners to install. Default: latest version available
         :param security_group: (experimental) Security Group to assign to this instance. Default: public project with no security group
@@ -868,15 +879,15 @@
     ) -> typing.Optional[_aws_cdk_aws_codebuild_ceddda9d.IBuildImage]:
         '''(experimental) Build image to use in CodeBuild.
 
         This is the image that's going to run the code that builds the runner image.
 
         The only action taken in CodeBuild is running ``docker build``. You would therefore not need to change this setting often.
 
-        :default: Ubuntu 20.04 for x64 and Amazon Linux 2 for ARM64
+        :default: Ubuntu 22.04 for x64 and Amazon Linux 2 for ARM64
 
         :stability: experimental
         '''
         result = self._values.get("build_image")
         return typing.cast(typing.Optional[_aws_cdk_aws_codebuild_ceddda9d.IBuildImage], result)
 
     @builtins.property
@@ -1040,15 +1051,15 @@
         self,
         *,
         build_image: typing.Optional[_aws_cdk_aws_codebuild_ceddda9d.IBuildImage] = None,
         compute_type: typing.Optional[_aws_cdk_aws_codebuild_ceddda9d.ComputeType] = None,
         timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     ) -> None:
         '''
-        :param build_image: (experimental) Build image to use in CodeBuild. This is the image that's going to run the code that builds the runner image. The only action taken in CodeBuild is running ``docker build``. You would therefore not need to change this setting often. Default: Ubuntu 20.04 for x64 and Amazon Linux 2 for ARM64
+        :param build_image: (experimental) Build image to use in CodeBuild. This is the image that's going to run the code that builds the runner image. The only action taken in CodeBuild is running ``docker build``. You would therefore not need to change this setting often. Default: Ubuntu 22.04 for x64 and Amazon Linux 2 for ARM64
         :param compute_type: (experimental) The type of compute to use for this build. See the {@link ComputeType} enum for the possible values. Default: {@link ComputeType#SMALL }
         :param timeout: (experimental) The number of minutes after which AWS CodeBuild stops the build if it's not complete. For valid values, see the timeoutInMinutes field in the AWS CodeBuild User Guide. Default: Duration.hours(1)
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__57eba0e804792fea32cbb8b094226d90afd105dd84432bb9e2d32380259a548f)
@@ -1069,15 +1080,15 @@
     ) -> typing.Optional[_aws_cdk_aws_codebuild_ceddda9d.IBuildImage]:
         '''(experimental) Build image to use in CodeBuild.
 
         This is the image that's going to run the code that builds the runner image.
 
         The only action taken in CodeBuild is running ``docker build``. You would therefore not need to change this setting often.
 
-        :default: Ubuntu 20.04 for x64 and Amazon Linux 2 for ARM64
+        :default: Ubuntu 22.04 for x64 and Amazon Linux 2 for ARM64
 
         :stability: experimental
         '''
         result = self._values.get("build_image")
         return typing.cast(typing.Optional[_aws_cdk_aws_codebuild_ceddda9d.IBuildImage], result)
 
     @builtins.property
@@ -2617,15 +2628,16 @@
     Example::
 
        new ImageBuilderComponent(this, 'AWS CLI', {
          platform: 'Windows',
          displayName: 'AWS CLI',
          description: 'Install latest version of AWS CLI',
          commands: [
-           'Start-Process msiexec.exe -Wait -ArgumentList \\'/i https://awscli.amazonaws.com/AWSCLIV2.msi /qn\\'',
+           '$p = Start-Process msiexec.exe -PassThru -Wait -ArgumentList \\'/i https://awscli.amazonaws.com/AWSCLIV2.msi /qn\\'',
+           'if ($p.ExitCode -ne 0) { throw "Exit code is $p.ExitCode" }',
          ],
        }
 
     :deprecated: Use ``RunnerImageComponent`` instead as this be internal soon.
 
     :stability: deprecated
     '''
@@ -2636,36 +2648,39 @@
         id: builtins.str,
         *,
         commands: typing.Sequence[builtins.str],
         description: builtins.str,
         display_name: builtins.str,
         platform: builtins.str,
         assets: typing.Optional[typing.Sequence[typing.Union[ImageBuilderAsset, typing.Dict[builtins.str, typing.Any]]]] = None,
+        reboot: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param commands: (experimental) Shell commands to run when adding this component to the image. On Linux, these are bash commands. On Windows, there are PowerShell commands.
         :param description: (experimental) Component description.
         :param display_name: (experimental) Component display name.
         :param platform: (experimental) Component platform. Must match the builder platform.
         :param assets: (experimental) Optional assets to add to the built image.
+        :param reboot: (experimental) Require a reboot after installing this component. Default: false
 
         :stability: deprecated
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__363ebaab8a0bcbaea3d32a9c7e3cb241f08cf49d6eea02ba40eaaef9af89f266)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = ImageBuilderComponentProperties(
             commands=commands,
             description=description,
             display_name=display_name,
             platform=platform,
             assets=assets,
+            reboot=reboot,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @jsii.member(jsii_name="grantAssetsRead")
     def grant_assets_read(self, grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable) -> None:
         '''(deprecated) Grants read permissions to the principal on the assets buckets.
@@ -2742,51 +2757,57 @@
     jsii_struct_bases=[],
     name_mapping={
         "commands": "commands",
         "description": "description",
         "display_name": "displayName",
         "platform": "platform",
         "assets": "assets",
+        "reboot": "reboot",
     },
 )
 class ImageBuilderComponentProperties:
     def __init__(
         self,
         *,
         commands: typing.Sequence[builtins.str],
         description: builtins.str,
         display_name: builtins.str,
         platform: builtins.str,
         assets: typing.Optional[typing.Sequence[typing.Union[ImageBuilderAsset, typing.Dict[builtins.str, typing.Any]]]] = None,
+        reboot: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''(experimental) Properties for ImageBuilderComponent construct.
 
         :param commands: (experimental) Shell commands to run when adding this component to the image. On Linux, these are bash commands. On Windows, there are PowerShell commands.
         :param description: (experimental) Component description.
         :param display_name: (experimental) Component display name.
         :param platform: (experimental) Component platform. Must match the builder platform.
         :param assets: (experimental) Optional assets to add to the built image.
+        :param reboot: (experimental) Require a reboot after installing this component. Default: false
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b86439e194b36e470271c572c251444f98c4b86a68fa7e63cf41ae1fa9628d4a)
             check_type(argname="argument commands", value=commands, expected_type=type_hints["commands"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument display_name", value=display_name, expected_type=type_hints["display_name"])
             check_type(argname="argument platform", value=platform, expected_type=type_hints["platform"])
             check_type(argname="argument assets", value=assets, expected_type=type_hints["assets"])
+            check_type(argname="argument reboot", value=reboot, expected_type=type_hints["reboot"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "commands": commands,
             "description": description,
             "display_name": display_name,
             "platform": platform,
         }
         if assets is not None:
             self._values["assets"] = assets
+        if reboot is not None:
+            self._values["reboot"] = reboot
 
     @builtins.property
     def commands(self) -> typing.List[builtins.str]:
         '''(experimental) Shell commands to run when adding this component to the image.
 
         On Linux, these are bash commands. On Windows, there are PowerShell commands.
 
@@ -2833,14 +2854,25 @@
         '''(experimental) Optional assets to add to the built image.
 
         :stability: experimental
         '''
         result = self._values.get("assets")
         return typing.cast(typing.Optional[typing.List[ImageBuilderAsset]], result)
 
+    @builtins.property
+    def reboot(self) -> typing.Optional[builtins.bool]:
+        '''(experimental) Require a reboot after installing this component.
+
+        :default: false
+
+        :stability: experimental
+        '''
+        result = self._values.get("reboot")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -3053,15 +3085,15 @@
 
         Base Docker image: ``public.ecr.aws/lambda/nodejs:14-x86_64`` or ``public.ecr.aws/lambda/nodejs:14-arm64``
 
         :param scope: -
         :param id: -
         :param architecture: (experimental) Image architecture. Default: Architecture.X86_64
         :param aws_image_builder_options: (experimental) Options specific to AWS Image Builder. Only used when builderType is RunnerImageBuilderType.AWS_IMAGE_BUILDER.
-        :param base_ami: (experimental) Base AMI from which runner AMIs will be built. Default: latest Ubuntu 20.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
+        :param base_ami: (experimental) Base AMI from which runner AMIs will be built. This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version. Default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
         :param base_docker_image: (experimental) Base image from which Docker runner images will be built. Default: public.ecr.aws/lts/ubuntu:22.04 for Os.LINUX_UBUNTU, public.ecr.aws/amazonlinux/amazonlinux:2 for Os.LINUX_AMAZON_2, mcr.microsoft.com/windows/servercore:ltsc2019-amd64 for Os.WINDOWS
         :param builder_type: Default: CodeBuild for Linux Docker image, AWS Image Builder for Windows Docker image and any AMI
         :param code_build_options: (experimental) Options specific to CodeBuild image builder. Only used when builderType is RunnerImageBuilderType.CODE_BUILD.
         :param components: (experimental) Components to install on the image. Default: none
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
         :param os: (experimental) Image OS. Default: OS.LINUX
@@ -4114,15 +4146,15 @@
         vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param architecture: (experimental) Image architecture. Default: Architecture.X86_64
         :param aws_image_builder_options: (experimental) Options specific to AWS Image Builder. Only used when builderType is RunnerImageBuilderType.AWS_IMAGE_BUILDER.
-        :param base_ami: (experimental) Base AMI from which runner AMIs will be built. Default: latest Ubuntu 20.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
+        :param base_ami: (experimental) Base AMI from which runner AMIs will be built. This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version. Default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
         :param base_docker_image: (experimental) Base image from which Docker runner images will be built. Default: public.ecr.aws/lts/ubuntu:22.04 for Os.LINUX_UBUNTU, public.ecr.aws/amazonlinux/amazonlinux:2 for Os.LINUX_AMAZON_2, mcr.microsoft.com/windows/servercore:ltsc2019-amd64 for Os.WINDOWS
         :param builder_type: Default: CodeBuild for Linux Docker image, AWS Image Builder for Windows Docker image and any AMI
         :param code_build_options: (experimental) Options specific to CodeBuild image builder. Only used when builderType is RunnerImageBuilderType.CODE_BUILD.
         :param components: (experimental) Components to install on the image. Default: none
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
         :param os: (experimental) Image OS. Default: OS.LINUX
@@ -4185,15 +4217,15 @@
 
         The implementation will differ based on the OS, architecture, and requested builder type.
 
         :param scope: -
         :param id: -
         :param architecture: (experimental) Image architecture. Default: Architecture.X86_64
         :param aws_image_builder_options: (experimental) Options specific to AWS Image Builder. Only used when builderType is RunnerImageBuilderType.AWS_IMAGE_BUILDER.
-        :param base_ami: (experimental) Base AMI from which runner AMIs will be built. Default: latest Ubuntu 20.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
+        :param base_ami: (experimental) Base AMI from which runner AMIs will be built. This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version. Default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
         :param base_docker_image: (experimental) Base image from which Docker runner images will be built. Default: public.ecr.aws/lts/ubuntu:22.04 for Os.LINUX_UBUNTU, public.ecr.aws/amazonlinux/amazonlinux:2 for Os.LINUX_AMAZON_2, mcr.microsoft.com/windows/servercore:ltsc2019-amd64 for Os.WINDOWS
         :param builder_type: Default: CodeBuild for Linux Docker image, AWS Image Builder for Windows Docker image and any AMI
         :param code_build_options: (experimental) Options specific to CodeBuild image builder. Only used when builderType is RunnerImageBuilderType.CODE_BUILD.
         :param components: (experimental) Components to install on the image. Default: none
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
         :param os: (experimental) Image OS. Default: OS.LINUX
@@ -4412,15 +4444,15 @@
         security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
         subnet_selection: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
         vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''
         :param architecture: (experimental) Image architecture. Default: Architecture.X86_64
         :param aws_image_builder_options: (experimental) Options specific to AWS Image Builder. Only used when builderType is RunnerImageBuilderType.AWS_IMAGE_BUILDER.
-        :param base_ami: (experimental) Base AMI from which runner AMIs will be built. Default: latest Ubuntu 20.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
+        :param base_ami: (experimental) Base AMI from which runner AMIs will be built. This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version. Default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
         :param base_docker_image: (experimental) Base image from which Docker runner images will be built. Default: public.ecr.aws/lts/ubuntu:22.04 for Os.LINUX_UBUNTU, public.ecr.aws/amazonlinux/amazonlinux:2 for Os.LINUX_AMAZON_2, mcr.microsoft.com/windows/servercore:ltsc2019-amd64 for Os.WINDOWS
         :param builder_type: Default: CodeBuild for Linux Docker image, AWS Image Builder for Windows Docker image and any AMI
         :param code_build_options: (experimental) Options specific to CodeBuild image builder. Only used when builderType is RunnerImageBuilderType.CODE_BUILD.
         :param components: (experimental) Components to install on the image. Default: none
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
         :param os: (experimental) Image OS. Default: OS.LINUX
@@ -4511,15 +4543,17 @@
         result = self._values.get("aws_image_builder_options")
         return typing.cast(typing.Optional[AwsImageBuilderRunnerImageBuilderProps], result)
 
     @builtins.property
     def base_ami(self) -> typing.Optional[builtins.str]:
         '''(experimental) Base AMI from which runner AMIs will be built.
 
-        :default: latest Ubuntu 20.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
+        This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version.
+
+        :default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
 
         :stability: experimental
         '''
         result = self._values.get("base_ami")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
@@ -4764,15 +4798,15 @@
         return typing.cast("RunnerImageComponent", jsii.sinvoke(cls, "custom", [props]))
 
     @jsii.member(jsii_name="docker")
     @builtins.classmethod
     def docker(cls) -> "RunnerImageComponent":
         '''(experimental) A component to install Docker.
 
-        On Windows this installs Docker Desktop.
+        On Windows this sets up dockerd for Windows containers without Docker Desktop. If you need Linux containers on Windows, you'll need to install Docker Desktop which doesn't seem to play well with servers (PRs welcome).
 
         :stability: experimental
         '''
         return typing.cast("RunnerImageComponent", jsii.sinvoke(cls, "docker", []))
 
     @jsii.member(jsii_name="dockerInDocker")
     @builtins.classmethod
@@ -4924,14 +4958,29 @@
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7ff728adc7084e50163879cf938d15b8d276df893b0a66f820410e736e6b8246)
             check_type(argname="argument _os", value=_os, expected_type=type_hints["_os"])
             check_type(argname="argument _architecture", value=_architecture, expected_type=type_hints["_architecture"])
         return typing.cast(typing.List[builtins.str], jsii.invoke(self, "getDockerCommands", [_os, _architecture]))
 
+    @jsii.member(jsii_name="shouldReboot")
+    def should_reboot(self, _os: Os, _architecture: Architecture) -> builtins.bool:
+        '''(experimental) Returns true if the image builder should be rebooted after this component is installed.
+
+        :param _os: -
+        :param _architecture: -
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__4df207340fa2acd15c1f7ba9d50447510dbe0aea58f11301ec935f4fbd00947f)
+            check_type(argname="argument _os", value=_os, expected_type=type_hints["_os"])
+            check_type(argname="argument _architecture", value=_architecture, expected_type=type_hints["_architecture"])
+        return typing.cast(builtins.bool, jsii.invoke(self, "shouldReboot", [_os, _architecture]))
+
     @builtins.property
     @jsii.member(jsii_name="name")
     @abc.abstractmethod
     def name(self) -> builtins.str:
         '''(experimental) Component name.
 
         Used to identify component in image build logs, and for {@link RunnerImageBuilder.removeComponent }
@@ -5691,15 +5740,15 @@
         subnet_selection: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
         vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param architecture: (experimental) Image architecture. Default: Architecture.X86_64
-        :param install_docker: (experimental) Install Docker inside the image, so it can be used by the runner. You may want to disable this if you are building a Windows image and don't have a Docker Desktop license. Default: true
+        :param install_docker: (experimental) Install Docker inside the image, so it can be used by the runner. Default: true
         :param instance_type: (experimental) The instance type used to build the image. Default: m5.large
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
         :param os: (experimental) Image OS. Default: OS.LINUX
         :param rebuild_interval: (experimental) Schedule the AMI to be rebuilt every given interval. Useful for keeping the AMI up-do-date with the latest GitHub runner version and latest OS updates. Set to zero to disable. Default: Duration.days(7)
         :param runner_version: (experimental) Version of GitHub Runners to install. Default: latest version available
         :param security_group: (deprecated) Security group to assign to launched builder instances. Default: new security group
@@ -5996,15 +6045,15 @@
         vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param dockerfile_path: (experimental) Path to Dockerfile to be built. It can be a path to a Dockerfile, a folder containing a Dockerfile, or a zip file containing a Dockerfile.
         :param architecture: (experimental) Image architecture. Default: Architecture.X86_64
-        :param build_image: (experimental) Build image to use in CodeBuild. This is the image that's going to run the code that builds the runner image. The only action taken in CodeBuild is running ``docker build``. You would therefore not need to change this setting often. Default: Ubuntu 20.04 for x64 and Amazon Linux 2 for ARM64
+        :param build_image: (experimental) Build image to use in CodeBuild. This is the image that's going to run the code that builds the runner image. The only action taken in CodeBuild is running ``docker build``. You would therefore not need to change this setting often. Default: Ubuntu 22.04 for x64 and Amazon Linux 2 for ARM64
         :param compute_type: (experimental) The type of compute to use for this build. See the {@link ComputeType} enum for the possible values. Default: {@link ComputeType#SMALL }
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
         :param os: (experimental) Image OS. Default: OS.LINUX
         :param rebuild_interval: (experimental) Schedule the image to be rebuilt every given interval. Useful for keeping the image up-do-date with the latest GitHub runner version and latest OS updates. Set to zero to disable. Default: Duration.days(7)
         :param runner_version: (experimental) Version of GitHub Runners to install. Default: latest version available
         :param security_group: (experimental) Security Group to assign to this instance. Default: public project with no security group
@@ -6269,15 +6318,15 @@
         - ``RunnerImageComponent.dockerInDocker()``
         - ``RunnerImageComponent.githubRunner()``
 
         :param scope: -
         :param id: -
         :param architecture: (experimental) Image architecture. Default: Architecture.X86_64
         :param aws_image_builder_options: (experimental) Options specific to AWS Image Builder. Only used when builderType is RunnerImageBuilderType.AWS_IMAGE_BUILDER.
-        :param base_ami: (experimental) Base AMI from which runner AMIs will be built. Default: latest Ubuntu 20.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
+        :param base_ami: (experimental) Base AMI from which runner AMIs will be built. This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version. Default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
         :param base_docker_image: (experimental) Base image from which Docker runner images will be built. Default: public.ecr.aws/lts/ubuntu:22.04 for Os.LINUX_UBUNTU, public.ecr.aws/amazonlinux/amazonlinux:2 for Os.LINUX_AMAZON_2, mcr.microsoft.com/windows/servercore:ltsc2019-amd64 for Os.WINDOWS
         :param builder_type: Default: CodeBuild for Linux Docker image, AWS Image Builder for Windows Docker image and any AMI
         :param code_build_options: (experimental) Options specific to CodeBuild image builder. Only used when builderType is RunnerImageBuilderType.CODE_BUILD.
         :param components: (experimental) Components to install on the image. Default: none
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
         :param os: (experimental) Image OS. Default: OS.LINUX
@@ -7214,15 +7263,15 @@
         - ``RunnerImageComponent.docker()``
         - ``RunnerImageComponent.githubRunner()``
 
         :param scope: -
         :param id: -
         :param architecture: (experimental) Image architecture. Default: Architecture.X86_64
         :param aws_image_builder_options: (experimental) Options specific to AWS Image Builder. Only used when builderType is RunnerImageBuilderType.AWS_IMAGE_BUILDER.
-        :param base_ami: (experimental) Base AMI from which runner AMIs will be built. Default: latest Ubuntu 20.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
+        :param base_ami: (experimental) Base AMI from which runner AMIs will be built. This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version. Default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
         :param base_docker_image: (experimental) Base image from which Docker runner images will be built. Default: public.ecr.aws/lts/ubuntu:22.04 for Os.LINUX_UBUNTU, public.ecr.aws/amazonlinux/amazonlinux:2 for Os.LINUX_AMAZON_2, mcr.microsoft.com/windows/servercore:ltsc2019-amd64 for Os.WINDOWS
         :param builder_type: Default: CodeBuild for Linux Docker image, AWS Image Builder for Windows Docker image and any AMI
         :param code_build_options: (experimental) Options specific to CodeBuild image builder. Only used when builderType is RunnerImageBuilderType.CODE_BUILD.
         :param components: (experimental) Components to install on the image. Default: none
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
         :param os: (experimental) Image OS. Default: OS.LINUX
@@ -7833,15 +7882,15 @@
         - ``RunnerImageComponent.dockerInDocker()``
         - ``RunnerImageComponent.githubRunner()``
 
         :param scope: -
         :param id: -
         :param architecture: (experimental) Image architecture. Default: Architecture.X86_64
         :param aws_image_builder_options: (experimental) Options specific to AWS Image Builder. Only used when builderType is RunnerImageBuilderType.AWS_IMAGE_BUILDER.
-        :param base_ami: (experimental) Base AMI from which runner AMIs will be built. Default: latest Ubuntu 20.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
+        :param base_ami: (experimental) Base AMI from which runner AMIs will be built. This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version. Default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
         :param base_docker_image: (experimental) Base image from which Docker runner images will be built. Default: public.ecr.aws/lts/ubuntu:22.04 for Os.LINUX_UBUNTU, public.ecr.aws/amazonlinux/amazonlinux:2 for Os.LINUX_AMAZON_2, mcr.microsoft.com/windows/servercore:ltsc2019-amd64 for Os.WINDOWS
         :param builder_type: Default: CodeBuild for Linux Docker image, AWS Image Builder for Windows Docker image and any AMI
         :param code_build_options: (experimental) Options specific to CodeBuild image builder. Only used when builderType is RunnerImageBuilderType.CODE_BUILD.
         :param components: (experimental) Components to install on the image. Default: none
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
         :param os: (experimental) Image OS. Default: OS.LINUX
@@ -8513,15 +8562,15 @@
         - ``RunnerImageComponent.awsCli()``
         - ``RunnerImageComponent.githubRunner()``
 
         :param scope: -
         :param id: -
         :param architecture: (experimental) Image architecture. Default: Architecture.X86_64
         :param aws_image_builder_options: (experimental) Options specific to AWS Image Builder. Only used when builderType is RunnerImageBuilderType.AWS_IMAGE_BUILDER.
-        :param base_ami: (experimental) Base AMI from which runner AMIs will be built. Default: latest Ubuntu 20.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
+        :param base_ami: (experimental) Base AMI from which runner AMIs will be built. This can be an actual AMI or an AWS Image Builder ARN that points to the latest AMI. For example ``arn:aws:imagebuilder:us-east-1:aws:image/ubuntu-server-22-lts-x86/x.x.x`` would always use the latest version of Ubuntu 22.04 in each build. If you want a specific version, you can replace ``x.x.x`` with that version. Default: latest Ubuntu 22.04 AMI for Os.LINUX_UBUNTU, latest Amazon Linux 2 AMI for Os.LINUX_AMAZON_2, latest Windows Server 2022 AMI for Os.WINDOWS
         :param base_docker_image: (experimental) Base image from which Docker runner images will be built. Default: public.ecr.aws/lts/ubuntu:22.04 for Os.LINUX_UBUNTU, public.ecr.aws/amazonlinux/amazonlinux:2 for Os.LINUX_AMAZON_2, mcr.microsoft.com/windows/servercore:ltsc2019-amd64 for Os.WINDOWS
         :param builder_type: Default: CodeBuild for Linux Docker image, AWS Image Builder for Windows Docker image and any AMI
         :param code_build_options: (experimental) Options specific to CodeBuild image builder. Only used when builderType is RunnerImageBuilderType.CODE_BUILD.
         :param components: (experimental) Components to install on the image. Default: none
         :param log_removal_policy: (experimental) Removal policy for logs of image builds. If deployment fails on the custom resource, try setting this to ``RemovalPolicy.RETAIN``. This way the CodeBuild logs can still be viewed, and you can see why the build failed. We try to not leave anything behind when removed. But sometimes a log staying behind is useful. Default: RemovalPolicy.DESTROY
         :param log_retention: (experimental) The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.ONE_MONTH
         :param os: (experimental) Image OS. Default: OS.LINUX
@@ -9940,14 +9989,15 @@
     id: builtins.str,
     *,
     commands: typing.Sequence[builtins.str],
     description: builtins.str,
     display_name: builtins.str,
     platform: builtins.str,
     assets: typing.Optional[typing.Sequence[typing.Union[ImageBuilderAsset, typing.Dict[builtins.str, typing.Any]]]] = None,
+    reboot: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__a450535474a302df6d17ac0b627edd05f72f54c900f36380517d39fc0a3b15e4(
     grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
 ) -> None:
@@ -9972,14 +10022,15 @@
 def _typecheckingstub__b86439e194b36e470271c572c251444f98c4b86a68fa7e63cf41ae1fa9628d4a(
     *,
     commands: typing.Sequence[builtins.str],
     description: builtins.str,
     display_name: builtins.str,
     platform: builtins.str,
     assets: typing.Optional[typing.Sequence[typing.Union[ImageBuilderAsset, typing.Dict[builtins.str, typing.Any]]]] = None,
+    reboot: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__637ac3a7237f114ea2a9842f95653a0d13444cd4da7a4dfe9330fdb98204e19b(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
@@ -10286,14 +10337,21 @@
 def _typecheckingstub__7ff728adc7084e50163879cf938d15b8d276df893b0a66f820410e736e6b8246(
     _os: Os,
     _architecture: Architecture,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__4df207340fa2acd15c1f7ba9d50447510dbe0aea58f11301ec935f4fbd00947f(
+    _os: Os,
+    _architecture: Architecture,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__4ee6536536b6c0e4ddbbb0d090a8deb491f5ecb4e1271d4525e6ea2835a39ef2(
     _os: Os,
     _architecture: Architecture,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO` & `cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudsnorkel.cdk-github-runners
-Version: 0.9.4
+Version: 0.9.5
 Summary: CDK construct to create GitHub Actions self-hosted runners. A webhook listens to events and creates ephemeral runners on the fly.
 Home-page: https://github.com/CloudSnorkel/cdk-github-runners.git
 Author: Amir Szekely<amir@cloudsnorkel.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/CloudSnorkel/cdk-github-runners.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GitHub Self-Hosted Runners CDK Constructs
 
 [![NPM](https://img.shields.io/npm/v/@cloudsnorkel/cdk-github-runners?label=npm&logo=npm)](https://www.npmjs.com/package/@cloudsnorkel/cdk-github-runners)
 [![PyPI](https://img.shields.io/pypi/v/cloudsnorkel.cdk-github-runners?label=pypi&logo=pypi)](https://pypi.org/project/cloudsnorkel.cdk-github-runners)
-[![Maven Central](https://img.shields.io/maven-central/v/com.cloudsnorkel/cdk.github.runners.svg?label=Maven%20Central&logo=java)](https://search.maven.org/search?q=g:%22com.cloudsnorkel%22%20AND%20a:%22cdk.github.runners%22)
+[![Maven Central](https://img.shields.io/maven-central/v/com.cloudsnorkel/cdk.github.runners.svg?label=Maven%20Central&logo=apachemaven)](https://search.maven.org/search?q=g:%22com.cloudsnorkel%22%20AND%20a:%22cdk.github.runners%22)
 [![Go](https://img.shields.io/github/v/tag/CloudSnorkel/cdk-github-runners?color=red&label=go&logo=go)](https://pkg.go.dev/github.com/CloudSnorkel/cdk-github-runners-go/cloudsnorkelcdkgithubrunners)
 [![Nuget](https://img.shields.io/nuget/v/CloudSnorkel.Cdk.Github.Runners?color=red&&logo=nuget)](https://www.nuget.org/packages/CloudSnorkel.Cdk.Github.Runners/)
 [![Release](https://github.com/CloudSnorkel/cdk-github-runners/actions/workflows/release.yml/badge.svg)](https://github.com/CloudSnorkel/cdk-github-runners/actions/workflows/release.yml)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/CloudSnorkel/cdk-github-runners/blob/main/LICENSE)
 
 Use this CDK construct to create ephemeral [self-hosted GitHub runners](https://docs.github.com/en/actions/hosting-your-own-runners/about-self-hosted-runners) on-demand inside your AWS account.
 
@@ -41,14 +41,15 @@
 * Automatically updated build environment with latest runner version
 
 Self-hosted runners in AWS are useful when:
 
 * You need easy access to internal resources in your actions
 * You want to pre-install some software for your actions
 * You want to provide some basic AWS API access (but [aws-actions/configure-aws-credentials](https://github.com/marketplace/actions/configure-aws-credentials-action-for-github-actions) has more security controls)
+* You are using GitHub Enterprise Server
 
 Ephemeral (or on-demand) runners are the [recommended way by GitHub](https://docs.github.com/en/actions/hosting-your-own-runners/autoscaling-with-self-hosted-runners#using-ephemeral-runners-for-autoscaling) for auto-scaling, and they make sure all jobs run with a clean image. Runners are started on-demand. You don't pay unless a job is running.
 
 ## API
 
 The best way to browse API documentation is on [Constructs Hub](https://constructs.dev/packages/@cloudsnorkel/cdk-github-runners/). It is available in all supported programming languages.
 
@@ -239,22 +240,34 @@
 
 ## Troubleshooting
 
 1. Always start with the status function, make sure no errors are reported, and confirm all status codes are OK
 2. If jobs are stuck on pending:
 
    1. Make sure `runs-on` in the workflow matches the expected labels set in the runner provider
-   2. If it happens every time, cancel the job and start it again
+   2. If jobs get stuck often and take a long time to start, cancel the pending jobs and start them again
 3. Confirm the webhook Lambda was called by visiting the URL in `troubleshooting.webhookHandlerUrl` from `status.json`
 
    1. If it's not called or logs errors, confirm the webhook settings on the GitHub side
    2. If you see too many errors, make sure you're only sending `workflow_job` events
 4. When using GitHub app, make sure there are active installation in `github.auth.app.installations`
 5. Check execution details of the orchestrator step function by visiting the URL in `troubleshooting.stepFunctionUrl` from `status.json`
 
    1. Use the details tab to find the specific execution of the provider (Lambda, CodeBuild, Fargate, etc.)
    2. Every step function execution should be successful, even if the runner action inside it failed
 
+## Monitoring
+
+There are two important ways to monitor your runners:
+
+1. Make sure runners don't fail to start. When that happens, jobs may sit and wait. Use `GitHubRunners.metricFailed()` to get a metric for the number of failed runner starts. You should use this metric to trigger an alarm.
+2. Make sure runner images don't fail to build. Failed runner image builds mean you will get stuck with out-of-date software on your runners. It may lead to security vulnerabilities, or it may lead to slower runner start-ups as the runner software itself needs to be updated. Use `GitHubRunners.failedImageBuildsTopic()` to get SNS topic that gets notified of failed runner image builds. You should subscribe to this topic.
+
+Other useful metrics to track:
+
+1. Use `GitHubRunners.metricJobCompleted()` to get a metric for the number of completed jobs broken down by labels and job success.
+2. Use `GitHubRunners.metricTime()` to get a metric for the total time a runner is running. This includes the overhead of starting the runner.
+
 ## Other Options
 
 1. [philips-labs/terraform-aws-github-runner](https://github.com/philips-labs/terraform-aws-github-runner) if you're using Terraform
 2. [actions/actions-runner-controller](https://github.com/actions/actions-runner-controller) if you're using Kubernetes
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt` & `cloudsnorkel.cdk-github-runners-0.9.5/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt
 src/cloudsnorkel.cdk_github_runners.egg-info/dependency_links.txt
 src/cloudsnorkel.cdk_github_runners.egg-info/requires.txt
 src/cloudsnorkel.cdk_github_runners.egg-info/top_level.txt
 src/cloudsnorkel/cdk_github_runners/__init__.py
 src/cloudsnorkel/cdk_github_runners/py.typed
 src/cloudsnorkel/cdk_github_runners/_jsii/__init__.py
-src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.4.jsii.tgz
+src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.5.jsii.tgz
```

