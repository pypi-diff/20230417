# Comparing `tmp/cfn-lint-1.0.0a1.tar.gz` & `tmp/cfn-lint-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn-lint-1.0.0a1.tar", last modified: Tue Mar 14 14:51:30 2023, max compression
+gzip compressed data, was "cfn-lint-1.0.0a2.tar", last modified: Tue Mar 14 15:37:32 2023, max compression
```

## Comparing `cfn-lint-1.0.0a1.tar` & `cfn-lint-1.0.0a2.tar`

### file list

```diff
@@ -1,408 +1,2531 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.312049 cfn-lint-1.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-03-14 14:51:30.312049 cfn-lint-1.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-14 14:51:30.312049 cfn-lint-1.0.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.284049 cfn-lint-1.0.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.288049 cfn-lint-1.0.0a1/src/cfn_lint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-03-14 14:51:30.000000 cfn-lint-1.0.0a1/src/cfn_lint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-03-14 14:51:30.000000 cfn-lint-1.0.0a1/src/cfn_lint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 14:51:30.000000 cfn-lint-1.0.0a1/src/cfn_lint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-14 14:51:30.000000 cfn-lint-1.0.0a1/src/cfn_lint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 14:51:30.000000 cfn-lint-1.0.0a1/src/cfn_lint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-14 14:51:30.000000 cfn-lint-1.0.0a1/src/cfn_lint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-14 14:51:30.000000 cfn-lint-1.0.0a1/src/cfn_lint.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.288049 cfn-lint-1.0.0a1/src/cfnlint/
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27067 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.288049 cfn-lint-1.0.0a1/src/cfnlint/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.288049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.288049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-applicationautoscaling-scalingpolicy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-applicationautoscaling-scalingpolicy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.288049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-autoscaling-autoscalinggroup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-autoscaling-autoscalinggroup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.288049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-autoscaling-launchconfiguration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-autoscaling-launchconfiguration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.288049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-cloudfront-distribution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-cloudfront-distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.288049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-cloudwatch-alarm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-cloudwatch-alarm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.288049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-codepipeline-pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-codepipeline-pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.288049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-dynamodb-table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-dynamodb-table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.288049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-ec2-instance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-ec2-instance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.288049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-ec2-launchtemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-ec2-launchtemplate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-ec2-networkaclentry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-ec2-networkaclentry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroupingress/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroupingress/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-ec2-spotfleet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-ec2-spotfleet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-elasticloadbalancingv2-loadbalancer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-elasticloadbalancingv2-loadbalancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-events-rule/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-events-rule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-iam-policy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-iam-policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-lambda-eventsourcemapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-lambda-eventsourcemapping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-opsworks-instance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-opsworks-instance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-opsworks-stack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-opsworks-stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-rds-dbcluster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-rds-dbcluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-rds-dbinstance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-rds-dbinstance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-route53-healthcheck/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-route53-healthcheck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-route53-recordset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-route53-recordset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-route53-recordsetgroup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-route53-recordsetgroup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-s3-bucket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-s3-bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-servicediscovery-service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/aws-servicediscovery-service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/json-schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/json-schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSchemas/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSpecs/
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSpecs/BasedOnValue.json
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSpecs/LmbdRuntimeLifecycle.json
--rw-r--r--   0 runner    (1001) docker     (123)   531658 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSpecs/Policies.json
--rw-r--r--   0 runner    (1001) docker     (123)   429008 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSpecs/RdsProperties.json
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSpecs/StatefulResources.json
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSpecs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.284049 cfn-lint-1.0.0a1/src/cfnlint/data/CfnLintCli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/CfnLintCli/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/CfnLintCli/config/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/ExtendedProviderSchema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ExtendedProviderSchema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/ExtendedProviderSchema/all/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ExtendedProviderSchema/all/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/af-south-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/af-south-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-east-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-east-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-northeast-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-northeast-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-northeast-2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-northeast-2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-northeast-3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-northeast-3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-south-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-south-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-south-2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-south-2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-southeast-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-southeast-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-southeast-2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-southeast-2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.292049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-southeast-3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-southeast-3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-southeast-4/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ap-southeast-4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ca-central-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/ca-central-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/cn-north-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/cn-north-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/cn-northwest-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/cn-northwest-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/eu-central-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/eu-central-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/eu-central-2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/eu-central-2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/eu-north-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/eu-north-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/eu-south-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/eu-south-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/eu-south-2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/eu-south-2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/eu-west-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/eu-west-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/eu-west-2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/eu-west-2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/eu-west-3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/eu-west-3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/me-central-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/me-central-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/me-south-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/me-south-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/sa-east-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/sa-east-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/us-east-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/us-east-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/us-east-2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/us-east-2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/us-gov-east-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/us-gov-east-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/us-gov-west-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/us-gov-west-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/us-west-1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/us-west-1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/us-west-2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/ProviderSchemas/us-west-2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/data/Serverless/
--rw-r--r--   0 runner    (1001) docker     (123)   106855 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/Serverless/ManagedPolicies.json
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/Serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/decode/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/decode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/decode/cfn_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/decode/cfn_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/decode/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/decode/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/decode/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/decorators/refactored.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/formatters/
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    18274 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/jsonschema/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/jsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/jsonschema/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/jsonschema/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13184 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/jsonschema/_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/jsonschema/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/jsonschema/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/languageExtensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/maintenance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.296049 cfn-lint-1.0.0a1/src/cfnlint/rules/
--rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.300049 cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/And.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/Equals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/EqualsIsUseful.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/Exists.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/Not.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/Or.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/Used.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.300049 cfn-lint-1.0.0a1/src/cfnlint/rules/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/custom/Operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/custom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.300049 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Base64.py
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Cidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/DynamicReferenceSecureString.py
--rw-r--r--   0 runner    (1001) docker     (123)    11522 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/FindInMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/FindInMapKeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/GetAtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/GetAz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/If.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/ImportValue.py
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Join.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Length.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Not.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/RefExist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/RefInCondition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/RelationshipConditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Select.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Split.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/SubNeeded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/SubNotJoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/SubParametersUsed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/SubUnneeded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/ToJsonString.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.300049 cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/ApproachingLimitAttributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/ApproachingLimitName.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/ApproachingLimitNumber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/KeyName.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/LimitAttributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/LimitName.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/LimitNumber.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/Name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/Used.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.300049 cfn-lint-1.0.0a1/src/cfnlint/rules/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/metadata/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/metadata/InterfaceConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/metadata/InterfaceParameterExists.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.304049 cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/ApproachingLimitDescription.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/ApproachingLimitName.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/ApproachingLimitNumber.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/Description.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/ImportValue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/LimitDescription.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/LimitName.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/LimitNumber.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/Name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/Required.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/Value.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.304049 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/AllowedPattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/AllowedValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/ApproachingLimitName.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/ApproachingLimitNumber.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/ApproachingLimitValue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/Default.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/DefaultRef.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/LambdaMemorySize.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/LimitName.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/LimitNumber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/LimitValue.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/Name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/Types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/Used.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.308049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ApproachingLimitName.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ApproachingLimitNumber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/BothUpdateReplacePolicyDeletionPolicyNeeded.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/CircularDependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/DeletionPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/DependsOn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/DependsOnObsolete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/HardCodedArnProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/LimitName.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/LimitNumber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/Modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/Name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/NoEcho.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/PreviousGenerationInstanceType.py
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/RetentionPeriodOnResourceTypesWithAutoExpiringContent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ServerlessTransform.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/UniqueNames.py
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/UpdateReplacePolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/UpdateReplacePolicyDeletionPolicyOnStatefulResourceTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.308049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/backup/BackupPlanLifecycleRule.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/backup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.308049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/certificatemanager/
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/certificatemanager/DomainValidationOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/certificatemanager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.308049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/cloudformation/NestedStackParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/cloudformation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.308049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/cloudfront/
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/cloudfront/Aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/cloudfront/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.308049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/codepipeline/
--rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/codepipeline/CodepipelineStageActions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/codepipeline/CodepipelineStages.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/codepipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.308049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/dynamodb/AttributeMismatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/dynamodb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.308049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ecs/
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ecs/FargateDeploymentSchedulingStrategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ecs/TaskDefinitionEssentialContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ecs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.308049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ectwo/
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ectwo/Ebs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ectwo/RouteTableAssociation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ectwo/SecurityGroupIngress.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ectwo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.308049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/elasticache/CacheClusterFailover.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/elasticache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.308049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/elb/
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/elb/Elb.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/elb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.308049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/events/
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/events/RuleScheduleExpression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/events/RuleTargetsLimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.308049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/iam/
--rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/iam/Permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/iam/Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/iam/PolicyVersion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/iam/RefWithPath.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/iam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.308049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/lmbd/
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/lmbd/DeprecatedRuntime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/lmbd/DeprecatedRuntimeEnd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/lmbd/DeprecatedRuntimeEol.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/lmbd/EventsLogGroupName.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/lmbd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.312049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/AllowedPattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/AllowedValue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/AvailabilityZone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/AwsType.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/CfnSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/ImageId.py
--rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/JsonSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/ListDuplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/ListDuplicatesAllowed.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/ListSize.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/NumberSize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/OnlyOne.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/Password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/Properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/PropertiesTemplated.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/Required.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/StringSize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/ValuePrimitiveType.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.312049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/rds/
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/rds/InstanceSize.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/rds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.312049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/route53/
--rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/route53/RecordSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/route53/RecordSetName.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/route53/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.312049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/stepfunctions/StateMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/stepfunctions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.312049 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/updatepolicy/
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/updatepolicy/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/resources/updatepolicy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.312049 cfn-lint-1.0.0a1/src/cfnlint/rules/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/templates/ApproachingLimitDescription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/templates/ApproachingLimitSize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/templates/Base.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/templates/Description.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/templates/LimitDescription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/templates/LimitSize.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/rules/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.312049 cfn-lint-1.0.0a1/src/cfnlint/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/schema/_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/schema/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/schema/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/schema/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/schema/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 14:51:30.312049 cfn-lint-1.0.0a1/src/cfnlint/template/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/template/getatts.py
--rw-r--r--   0 runner    (1001) docker     (123)    46643 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/template/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-14 14:51:09.000000 cfn-lint-1.0.0a1/src/cfnlint/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.308994 cfn-lint-1.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-03-14 15:37:32.308994 cfn-lint-1.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-14 15:37:32.308994 cfn-lint-1.0.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.076990 cfn-lint-1.0.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.092990 cfn-lint-1.0.0a2/src/cfn_lint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-03-14 15:37:31.000000 cfn-lint-1.0.0a2/src/cfn_lint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   180013 2023-03-14 15:37:32.000000 cfn-lint-1.0.0a2/src/cfn_lint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 15:37:31.000000 cfn-lint-1.0.0a2/src/cfn_lint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-14 15:37:31.000000 cfn-lint-1.0.0a2/src/cfn_lint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 15:37:31.000000 cfn-lint-1.0.0a2/src/cfn_lint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-14 15:37:31.000000 cfn-lint-1.0.0a2/src/cfn_lint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-14 15:37:31.000000 cfn-lint-1.0.0a2/src/cfn_lint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.092990 cfn-lint-1.0.0a2/src/cfnlint/
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27067 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.092990 cfn-lint-1.0.0a2/src/cfnlint/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.092990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.092990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-applicationautoscaling-scalingpolicy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-applicationautoscaling-scalingpolicy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-applicationautoscaling-scalingpolicy/scalingpolicy.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.096990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-autoscaling-autoscalinggroup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-autoscaling-autoscalinggroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-autoscaling-autoscalinggroup/launchtemplatespecification-onlyone.json
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-autoscaling-autoscalinggroup/onlyone.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.096990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-autoscaling-launchconfiguration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-autoscaling-launchconfiguration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-autoscaling-launchconfiguration/blockdevicemapping-onlyone.json
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-autoscaling-launchconfiguration/blockdevicemapping-virtualname-exlusive.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.096990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-cloudfront-distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-cloudfront-distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-cloudfront-distribution/customerrorresponse-responsecode-inclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-cloudfront-distribution/origin-onlyone.json
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-cloudfront-distribution/viewercertificate-acmcertificatearn-inclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-cloudfront-distribution/viewercertificate-iamcertificateid-inclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-cloudfront-distribution/viewercertificate-onlyone.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.096990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-cloudwatch-alarm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-cloudwatch-alarm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-cloudwatch-alarm/metric-onlyone.json
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-cloudwatch-alarm/metrics-exclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-cloudwatch-alarm/statistic-exclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-cloudwatch-alarm/thresholdmetric-exclusive.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.096990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-codepipeline-pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-codepipeline-pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-codepipeline-pipeline/artifactstore-onlyone.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.096990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-dynamodb-table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-dynamodb-table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-dynamodb-table/billingmode-exclusive.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.096990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-instance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-instance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-instance/blockdevicemapping-onlyone.json
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-instance/blockdevicemapping-virtualname-exclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-instance/exclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-instance/required.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.096990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-launchtemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-launchtemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-launchtemplate/blockdevicemapping-virtualname.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.096990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-networkaclentry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-networkaclentry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-networkaclentry/required.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.096990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroup/egress-onlyone.json
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroup/ingress-cidrip-exclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroup/ingress-cidripv6-exclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroup/ingress-sourcesecuritygroupid-exclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroup/securitygroupegress-inclusive.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.096990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroupingress/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroupingress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroupingress/cidrip-exclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroupingress/cidripv6-exclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroupingress/groupid-exclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-securitygroupingress/sourcesecuritygroupid-exclusive.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.096990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-spotfleet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-spotfleet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-spotfleet/blockdevicemapping-onlyone.json
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-spotfleet/blockdevicemapping-virtualname.json
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-ec2-spotfleet/spotfleetrequestconfigdata-onlyone.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.096990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-elasticloadbalancingv2-loadbalancer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-elasticloadbalancingv2-loadbalancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-elasticloadbalancingv2-loadbalancer/subnets-onlyone.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.096990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-events-rule/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-events-rule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-events-rule/required.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.100990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-iam-policy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-iam-policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-iam-policy/required.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.100990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-lambda-eventsourcemapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-lambda-eventsourcemapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-lambda-eventsourcemapping/eventsourcearn-sqs-exclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-lambda-eventsourcemapping/eventsourcearn-stream-inclusive.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.100990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-opsworks-instance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-opsworks-instance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-opsworks-instance/blockdevicemapping-onlyone.json
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-opsworks-instance/blockdevicemapping-virtualname-exclusive.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.100990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-opsworks-stack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-opsworks-stack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-opsworks-stack/vpcid-inclusive.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.100990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-rds-dbcluster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-rds-dbcluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-rds-dbcluster/serverless-exclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-rds-dbcluster/snapshotidentifier-exclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-rds-dbcluster/sourcedbclusteridentifier-exclusive.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.100990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-rds-dbinstance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-rds-dbinstance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-rds-dbinstance/aurora-exclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-rds-dbinstance/sourcedbinstanceidentifier-exclusive.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.100990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-route53-healthcheck/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-route53-healthcheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-route53-healthcheck/healthcheckconfig-type-inclusive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-route53-healthcheck/healthcheckconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.100990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-route53-recordset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-route53-recordset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-route53-recordset/hostedzone-onlyone.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.100990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-route53-recordsetgroup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-route53-recordsetgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-route53-recordsetgroup/hostedzone-onlyone.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.100990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-s3-bucket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-s3-bucket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-s3-bucket/routingrulecondition-required.json
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-s3-bucket/websiteconfiguration-redirectallrequeststo-exclusive.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.100990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-servicediscovery-service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-servicediscovery-service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/aws-servicediscovery-service/healthcheckconfig-exclusive.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.100990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/json-schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/json-schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/json-schema/draft7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.100990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSchemas/resource/configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.104990 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSpecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSpecs/BasedOnValue.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSpecs/LmbdRuntimeLifecycle.json
+-rw-r--r--   0 runner    (1001) docker     (123)   531658 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSpecs/Policies.json
+-rw-r--r--   0 runner    (1001) docker     (123)   429008 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSpecs/RdsProperties.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSpecs/StatefulResources.json
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSpecs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.084990 cfn-lint-1.0.0a2/src/cfnlint/data/CfnLintCli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.104990 cfn-lint-1.0.0a2/src/cfnlint/data/CfnLintCli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/CfnLintCli/config/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.104990 cfn-lint-1.0.0a2/src/cfnlint/data/ExtendedProviderSchemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ExtendedProviderSchemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.104990 cfn-lint-1.0.0a2/src/cfnlint/data/ExtendedProviderSchemas/all/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ExtendedProviderSchemas/all/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.104990 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.108991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-amazonmq-configurationassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-apigatewayv2-vpclink.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-applicationautoscaling-scalingpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-athena-namedquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-autoscalingplans-scalingplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-cloudformation-waitcondition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-cloudfront-streamingdistribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-codepipeline-customactiontype.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-directoryservice-microsoftad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-ec2-clientvpnauthorizationrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13322 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-ec2-networkinsightsanalysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-ec2-networkinsightspath.json
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-ec2-networkinterfaceattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-ec2-networkinterfacepermission.json
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-ec2-subnetcidrblock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-ec2-transitgatewayroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-ec2-vpcendpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-ecs-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-emr-step.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-gamelift-alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-gamelift-build.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-gamelift-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-glue-datacatalogencryptionsettings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-guardduty-master.json
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-iam-accesskey.json
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-iam-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-iam-policy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-iot-certificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-iot-policy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-iot-policyprincipalattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-iot-thing.json
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-iot-thingprincipalattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-kinesis-streamconsumer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-lambda-layerversionpermission.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-opsworks-instance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-opsworks-layer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-opsworks-stack.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-route53-healthcheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-route53-hostedzone.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-route53resolver-resolverconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-secretsmanager-secrettargetattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-servicecatalog-acceptedportfolioshare.json
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-servicecatalog-portfolio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-servicecatalog-portfolioprincipalassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-servicecatalog-portfolioproductassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-servicecatalog-tagoptionassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-sns-topicpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-sqs-queue.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-transfer-workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-waf-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-waf-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-waf-sizeconstraintset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-waf-webacl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-waf-xssmatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-wafregional-geomatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-wafregional-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-wafregional-ratebasedrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-wafregional-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-wafregional-sizeconstraintset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-wafregional-webacl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-wafv2-loggingconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26773 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-wafv2-rulegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/af-south-1/aws-wafv2-webacl.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.112990 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-amazonmq-configurationassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-apigatewayv2-vpclink.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-athena-namedquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-autoscalingplans-scalingplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-cloudfront-streamingdistribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-cognito-userpool.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-cognito-userpoolclient.json
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-cognito-userpooldomain.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-cognito-userpoolriskconfigurationattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-cognito-userpooluicustomizationattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-cognito-userpoolusertogroupattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-ec2-clientvpnauthorizationrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13322 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-ec2-networkinsightsanalysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-ec2-networkinsightspath.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-ec2-trafficmirrorfilterrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-ec2-trafficmirrorsession.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-ec2-transitgatewayroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-eks-nodegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-gamelift-alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-gamelift-build.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-gamelift-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-glue-datacatalogencryptionsettings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-guardduty-master.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-kinesis-streamconsumer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-kinesisanalytics-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-kinesisanalytics-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-kinesisanalyticsv2-applicationcloudwatchloggingoption.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-kinesisanalyticsv2-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-lambda-layerversionpermission.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-neptune-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-neptune-dbinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-neptune-dbparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-route53resolver-resolverconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-secretsmanager-secrettargetattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-servicecatalog-acceptedportfolioshare.json
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-servicecatalog-portfolio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-servicecatalog-portfolioprincipalassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-servicecatalog-portfolioproductassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-servicecatalog-tagoptionassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-sqs-queue.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-transfer-workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-wafregional-geomatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-wafregional-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-wafregional-ratebasedrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-wafregional-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-wafregional-sizeconstraintset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-east-1/aws-wafregional-webacl.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.116991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30320 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-appflow-connectorprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35398 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-appflow-flow.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-ec2-vpnconnectionroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-location-tracker.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-managedblockchain-member.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-neptune-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-neptune-dbinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-neptune-dbparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-pinpoint-admchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-pinpoint-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-pinpoint-baiduchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-pinpoint-gcmchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-pinpoint-segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-refactorspaces-environment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-1/aws-route53resolver-resolverconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.116991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-config-aggregationauthorization.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-config-organizationconfigrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13322 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-ec2-networkinsightsanalysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-ec2-networkinsightspath.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-grafana-workspace.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-managedblockchain-member.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-neptune-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-neptune-dbinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-neptune-dbparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-pinpoint-admchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-pinpoint-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-pinpoint-baiduchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-pinpoint-gcmchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-pinpoint-segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-robomaker-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-robomaker-robot.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-robomaker-robotapplication.json
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-robomaker-robotapplicationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-robomaker-simulationapplication.json
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-robomaker-simulationapplicationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-route53resolver-resolverconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-sqs-queue.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-2/aws-transfer-workflow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.124991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-amazonmq-configurationassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-account.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-apikey.json
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-authorizer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-basepathmapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-clientcertificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-deployment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-documentationpart.json
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-documentationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-domainname.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-gatewayresponse.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-method.json
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-model.json
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-requestvalidator.json
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-resource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-restapi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-stage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-usageplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigateway-usageplankey.json
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-apigatewayv2-vpclink.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-athena-namedquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-autoscalingplans-scalingplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-cloudfront-streamingdistribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-codepipeline-customactiontype.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-ec2-transitgateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-ec2-transitgatewayattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-ec2-transitgatewayroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-gamelift-alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-gamelift-build.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-gamelift-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-glue-datacatalogencryptionsettings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-guardduty-master.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-iot-certificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-iot-policy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-iot-thing.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-lambda-layerversionpermission.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-route53resolver-resolverconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16473 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-sagemaker-domain.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-sagemaker-space.json
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-secretsmanager-secrettargetattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-servicecatalog-acceptedportfolioshare.json
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-servicecatalog-portfolio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-servicecatalog-portfolioprincipalassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-servicecatalog-portfolioproductassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-servicecatalog-tagoptionassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-servicecatalogappregistry-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-servicecatalogappregistry-attributegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-ssm-resourcedatasync.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-stepfunctions-activity.json
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-wafregional-geomatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-wafregional-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-wafregional-ratebasedrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-wafregional-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-wafregional-sizeconstraintset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-northeast-3/aws-wafregional-webacl.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.124991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-appstream-stackuserassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-appstream-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-cognito-userpoolusertogroupattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-config-organizationconfigrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-kinesisanalytics-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-kinesisanalytics-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-kinesisanalyticsv2-applicationcloudwatchloggingoption.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-kinesisanalyticsv2-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-location-tracker.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-neptune-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-neptune-dbinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-neptune-dbparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-robomaker-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-robomaker-robot.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-robomaker-robotapplication.json
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-robomaker-robotapplicationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-robomaker-simulationapplication.json
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-robomaker-simulationapplicationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-route53resolver-resolverconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-wafregional-geomatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-wafregional-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-wafregional-ratebasedrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-wafregional-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-wafregional-sizeconstraintset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-1/aws-wafregional-webacl.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.124991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-south-2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.128991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-cognito-userpoolusertogroupattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-docdb-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-grafana-workspace.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-managedblockchain-member.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-neptune-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-neptune-dbinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-neptune-dbparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-pinpoint-admchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-pinpoint-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-pinpoint-baiduchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-pinpoint-gcmchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-pinpoint-segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-1/aws-route53resolver-resolverconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.128991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/aws-ec2-trafficmirrorfilterrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/aws-ec2-trafficmirrorsession.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/aws-neptune-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/aws-neptune-dbinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/aws-neptune-dbparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/aws-networkfirewall-firewall.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13411 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/aws-networkfirewall-rulegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/aws-robomaker-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/aws-robomaker-robot.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/aws-robomaker-robotapplication.json
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/aws-robomaker-robotapplicationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/aws-robomaker-simulationapplication.json
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/aws-robomaker-simulationapplicationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-2/aws-route53resolver-resolverconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.136991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-amazonmq-configurationassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-account.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-apikey.json
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-authorizer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-basepathmapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-clientcertificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-deployment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-documentationpart.json
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-documentationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-domainname.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-gatewayresponse.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-method.json
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-model.json
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-requestvalidator.json
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-resource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-restapi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-stage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-usageplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-apigateway-usageplankey.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-applicationautoscaling-scalingpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-athena-namedquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-cloudformation-waitcondition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-cloudtrail-trail.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-codepipeline-customactiontype.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-directoryservice-microsoftad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-ec2-host.json
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-ec2-networkinterfaceattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-ec2-networkinterfacepermission.json
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-ec2-subnetcidrblock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-ec2-subnetnetworkaclassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-ec2-transitgateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-ec2-transitgatewayroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-ec2-vpcendpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-ecs-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-eks-nodegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-elasticbeanstalk-applicationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-elasticloadbalancingv2-listener.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-elasticloadbalancingv2-listenerrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-emr-step.json
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-events-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-gamelift-alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-gamelift-build.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-gamelift-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-iam-accesskey.json
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-iam-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-iam-policy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-iam-role.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-iot-certificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-iot-policy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-iot-policyprincipalattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-iot-thing.json
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-iot-thingprincipalattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-kinesis-stream.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-kms-alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-logs-subscriptionfilter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-opsworks-instance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-opsworks-layer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-opsworks-stack.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-redshift-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-redshift-clusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-redshift-clustersubnetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-route53-healthcheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-route53-hostedzone.json
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-secretsmanager-secrettargetattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-sns-topicpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-sqs-queue.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-ssm-resourcedatasync.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-transfer-workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-waf-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-waf-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-waf-sizeconstraintset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-waf-webacl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-waf-xssmatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26773 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-wafv2-rulegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-3/aws-wafv2-webacl.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.136991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ap-southeast-4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.140991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-appstream-imagebuilder.json
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-appstream-stackuserassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-appstream-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-cognito-userpoolusertogroupattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-config-organizationconfigrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-docdb-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-kinesisanalytics-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-kinesisanalytics-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-kinesisanalyticsv2-applicationcloudwatchloggingoption.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-kinesisanalyticsv2-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-location-tracker.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-pinpoint-admchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-pinpoint-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-pinpoint-baiduchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-pinpoint-gcmchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-pinpoint-segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-route53resolver-resolverconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-transfer-workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-wafregional-geomatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-wafregional-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-wafregional-ratebasedrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-wafregional-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-wafregional-sizeconstraintset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/ca-central-1/aws-wafregional-webacl.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.144991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-amazonmq-configurationassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-athena-namedquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-autoscalingplans-scalingplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-backup-backupselection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-backup-backupvault.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-cloudfront-streamingdistribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-config-aggregationauthorization.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-ec2-customergateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-ec2-trafficmirrorfilterrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-ec2-trafficmirrorsession.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-ec2-transitgateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-ec2-transitgatewayattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-ec2-transitgatewayroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-ec2-vpnconnection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-ecs-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-glue-datacatalogencryptionsettings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-guardduty-master.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-iotsitewise-assetmodel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-kinesisanalytics-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-kinesisanalytics-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-kinesisanalyticsv2-applicationcloudwatchloggingoption.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-kinesisanalyticsv2-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-redshift-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-redshift-clusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-redshift-clustersubnetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-route53-healthcheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-route53-hostedzone.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-route53resolver-resolverconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-secretsmanager-secrettargetattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-servicecatalog-acceptedportfolioshare.json
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-servicecatalog-portfolio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-servicecatalog-portfolioprincipalassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-servicecatalog-portfolioproductassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-servicecatalog-tagoptionassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-ssm-resourcedatasync.json
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-wafregional-geomatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-wafregional-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-wafregional-ratebasedrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-wafregional-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-wafregional-sizeconstraintset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-wafregional-webacl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-wafv2-loggingconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26773 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-wafv2-rulegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-north-1/aws-wafv2-webacl.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.148991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-amazonmq-configurationassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-apigateway-usageplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-appstream-directoryconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-appstream-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-appstream-imagebuilder.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-appstream-stack.json
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-appstream-stackuserassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-appstream-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-athena-preparedstatement.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-autoscalingplans-scalingplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-backup-backupselection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-backup-backupvault.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-cloudfront-streamingdistribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8875 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-codebuild-project.json
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-codedeploy-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-codedeploy-deploymentconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-config-aggregationauthorization.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-docdb-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-ec2-customergateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-ec2-eip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-ec2-trafficmirrorfilterrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-ec2-trafficmirrorsession.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-ec2-transitgateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-ec2-transitgatewayattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-ec2-transitgatewayroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-ec2-vpnconnection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-ec2-vpngateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-ecs-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-ecs-clustercapacityproviderassociations.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-gamelift-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-glue-datacatalogencryptionsettings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-guardduty-master.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-kinesis-stream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-kinesisanalytics-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-kinesisanalytics-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-kinesisanalyticsv2-applicationcloudwatchloggingoption.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-kinesisanalyticsv2-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-neptune-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-neptune-dbinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-neptune-dbparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-redshift-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-redshift-clusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-redshift-clustersubnetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-route53-healthcheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-route53-hostedzone.json
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-secretsmanager-secrettargetattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-servicecatalog-acceptedportfolioshare.json
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-servicecatalog-portfolio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-servicecatalog-portfolioprincipalassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-servicecatalog-portfolioproductassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-servicecatalog-tagoptionassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-sqs-queue.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-ssm-maintenancewindowtask.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-ssm-resourcedatasync.json
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-stepfunctions-activity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-transfer-workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-wafregional-geomatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-wafregional-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-wafregional-ratebasedrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-wafregional-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-wafregional-sizeconstraintset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-wafregional-webacl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-wafv2-loggingconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26773 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-wafv2-rulegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/cn-northwest-1/aws-wafv2-webacl.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.148991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/aws-config-organizationconfigrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/aws-ec2-transitgateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/aws-ec2-vpnconnectionroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/aws-kinesisanalytics-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/aws-kinesisanalytics-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/aws-location-tracker.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/aws-managedblockchain-member.json
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/aws-managedblockchain-node.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/aws-organizations-resourcepolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/aws-refactorspaces-environment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-1/aws-route53resolver-resolverconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.148991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-central-2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.152991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-amazonmq-configurationassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-athena-namedquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-autoscalingplans-scalingplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-cloudfront-streamingdistribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-cognito-userpoolriskconfigurationattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-cognito-userpooluicustomizationattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-cognito-userpoolusertogroupattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-ec2-transitgatewayroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-gamelift-alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-gamelift-build.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-gamelift-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-glue-datacatalogencryptionsettings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-guardduty-master.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-kinesisanalytics-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-kinesisanalytics-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-kinesisanalyticsv2-applicationcloudwatchloggingoption.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-kinesisanalyticsv2-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-lambda-layerversionpermission.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-medialive-inputsecuritygroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-neptune-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-neptune-dbinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-neptune-dbparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-route53resolver-resolverconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-secretsmanager-secrettargetattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-servicecatalog-acceptedportfolioshare.json
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-servicecatalog-portfolioproductassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-sqs-queue.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-north-1/aws-transfer-workflow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.160991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-amazonmq-configurationassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-apigatewayv2-vpclink.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-applicationautoscaling-scalingpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-athena-namedquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-autoscalingplans-scalingplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-cloudformation-waitcondition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-cloudfront-streamingdistribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-directoryservice-microsoftad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-ec2-clientvpnauthorizationrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13322 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-ec2-networkinsightsanalysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-ec2-networkinsightspath.json
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-ec2-networkinterfaceattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-ec2-networkinterfacepermission.json
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-ec2-subnetcidrblock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-ec2-transitgatewayroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-ec2-vpcendpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-ecs-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-elasticache-usergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-emr-step.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-gamelift-alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-gamelift-build.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-gamelift-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-glue-datacatalogencryptionsettings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-guardduty-master.json
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-iam-accesskey.json
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-iam-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-iam-policy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-iot-certificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-iot-policy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-iot-policyprincipalattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-iot-thing.json
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-iot-thingprincipalattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-kinesis-streamconsumer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-kinesisanalytics-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-kinesisanalytics-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-kinesisanalyticsv2-applicationcloudwatchloggingoption.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-kinesisanalyticsv2-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-lambda-layerversionpermission.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-opsworks-instance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-opsworks-layer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-opsworks-stack.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-rolesanywhere-profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-route53-healthcheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-route53-hostedzone.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-route53resolver-resolverconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-secretsmanager-secrettargetattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-servicecatalog-acceptedportfolioshare.json
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-servicecatalog-portfolio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-servicecatalog-portfolioprincipalassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-servicecatalog-portfolioproductassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-servicecatalog-tagoptionassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-sns-topicpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-sqs-queue.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-transfer-workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-waf-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-waf-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-waf-sizeconstraintset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-waf-webacl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-waf-xssmatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-wafregional-geomatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-wafregional-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-wafregional-ratebasedrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-wafregional-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-wafregional-sizeconstraintset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-1/aws-wafregional-webacl.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.160991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-south-2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.160991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-1/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-1/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-1/aws-managedblockchain-member.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-1/aws-route53resolver-resolverconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.160991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-amazonmq-configurationassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-appstream-imagebuilder.json
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-appstream-stackuserassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-appstream-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-grafana-workspace.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-location-tracker.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-managedblockchain-member.json
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-medialive-inputsecuritygroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-pinpoint-admchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-pinpoint-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-pinpoint-baiduchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-pinpoint-gcmchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-pinpoint-segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-2/aws-route53resolver-resolverconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.164991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-athena-namedquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-autoscalingplans-scalingplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-cognito-userpoolriskconfigurationattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-cognito-userpooluicustomizationattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-cognito-userpoolusertogroupattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-docdb-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-ec2-clientvpnauthorizationrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-gamelift-alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-gamelift-build.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-gamelift-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-guardduty-master.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-kinesisanalytics-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-kinesisanalytics-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-kinesisanalyticsv2-applicationcloudwatchloggingoption.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-kinesisanalyticsv2-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-medialive-inputsecuritygroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-neptune-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-neptune-dbinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-neptune-dbparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-route53resolver-resolverconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-sqs-queue.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-transfer-workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-wafregional-geomatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-wafregional-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-wafregional-ratebasedrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-wafregional-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-wafregional-sizeconstraintset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/eu-west-3/aws-wafregional-webacl.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.164991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-central-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-central-1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.168991 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-amazonmq-configurationassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-amplifyuibuilder-component.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-amplifyuibuilder-form.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-amplifyuibuilder-theme.json
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-apigatewayv2-vpclink.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-athena-namedquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-autoscalingplans-scalingplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-backup-backupselection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-backup-backupvault.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-backup-framework.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-backup-reportplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-cloudfront-streamingdistribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-codepipeline-customactiontype.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-cognito-userpoolriskconfigurationattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-cognito-userpooluicustomizationattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-cognito-userpoolusertogroupattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-ec2-clientvpnauthorizationrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13322 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-ec2-networkinsightsanalysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-ec2-networkinsightspath.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-ec2-trafficmirrorfilterrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-ec2-trafficmirrorsession.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-ec2-transitgateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-ec2-transitgatewayroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-ecs-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-events-archive.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-gamelift-alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-gamelift-build.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-gamelift-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-glue-datacatalogencryptionsettings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-guardduty-master.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-kinesis-streamconsumer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-kinesisanalytics-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-kinesisanalytics-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-kinesisanalyticsv2-applicationcloudwatchloggingoption.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-kinesisanalyticsv2-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-lambda-layerversionpermission.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-route53resolver-resolverconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-secretsmanager-secrettargetattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-servicecatalog-acceptedportfolioshare.json
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-servicecatalog-portfolio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-servicecatalog-portfolioprincipalassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-servicecatalog-portfolioproductassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-servicecatalog-tagoptionassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-sqs-queue.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-transfer-workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-wafregional-geomatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-wafregional-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-wafregional-ratebasedrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-wafregional-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-wafregional-sizeconstraintset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/me-south-1/aws-wafregional-webacl.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.172992 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-amazonmq-configurationassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-athena-namedquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-autoscalingplans-scalingplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-cognito-userpoolriskconfigurationattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-cognito-userpooluicustomizationattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-cognito-userpoolusertogroupattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-docdb-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-ec2-clientvpnauthorizationrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-glue-datacatalogencryptionsettings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-kinesisanalytics-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-kinesisanalytics-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-kinesisanalyticsv2-applicationcloudwatchloggingoption.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-kinesisanalyticsv2-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-location-tracker.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-neptune-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-neptune-dbinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-neptune-dbparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-networkmanager-connectattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-networkmanager-connectpeer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-networkmanager-corenetwork.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-networkmanager-sitetositevpnattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-networkmanager-vpcattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-route53resolver-resolverconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-wafregional-geomatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-wafregional-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-wafregional-ratebasedrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-wafregional-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-wafregional-sizeconstraintset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/sa-east-1/aws-wafregional-webacl.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.268993 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/alexa-ask-skill.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-accessanalyzer-analyzer.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-acmpca-certificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-acmpca-certificateauthority.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-acmpca-certificateauthorityactivation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-acmpca-permission.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-amazonmq-broker.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-amazonmq-configuration.json
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-amazonmq-configurationassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-amplify-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-amplify-branch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-amplify-domain.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10140 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-amplifyuibuilder-component.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-amplifyuibuilder-form.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-amplifyuibuilder-theme.json
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-account.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-apikey.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-authorizer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-basepathmapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-clientcertificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-deployment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-documentationpart.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-documentationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-domainname.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-gatewayresponse.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8902 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-method.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-requestvalidator.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-resource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-restapi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-stage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-usageplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-usageplankey.json
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigateway-vpclink.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigatewayv2-api.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigatewayv2-apigatewaymanagedoverrides.json
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigatewayv2-apimapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigatewayv2-authorizer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigatewayv2-deployment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigatewayv2-domainname.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigatewayv2-integration.json
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigatewayv2-integrationresponse.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigatewayv2-model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigatewayv2-route.json
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigatewayv2-routeresponse.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigatewayv2-stage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apigatewayv2-vpclink.json
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appconfig-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appconfig-configurationprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appconfig-deployment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appconfig-deploymentstrategy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appconfig-environment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appconfig-hostedconfigurationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appflow-connector.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32046 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appflow-connectorprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36123 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appflow-flow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appintegrations-dataintegration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appintegrations-eventintegration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-applicationautoscaling-scalabletarget.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-applicationautoscaling-scalingpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17950 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-applicationinsights-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appmesh-gatewayroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appmesh-mesh.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appmesh-route.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10724 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appmesh-virtualgateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14056 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appmesh-virtualnode.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appmesh-virtualrouter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appmesh-virtualservice.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apprunner-observabilityconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apprunner-service.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apprunner-vpcconnector.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-apprunner-vpcingressconnection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appstream-appblock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appstream-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appstream-applicationentitlementassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appstream-applicationfleetassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appstream-directoryconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appstream-entitlement.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appstream-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appstream-imagebuilder.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appstream-stack.json
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appstream-stackfleetassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appstream-stackuserassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appstream-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appsync-apicache.json
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appsync-apikey.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appsync-datasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appsync-domainname.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appsync-domainnameapiassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appsync-functionconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appsync-graphqlapi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appsync-graphqlschema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-appsync-resolver.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-aps-rulegroupsnamespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-aps-workspace.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-athena-datacatalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-athena-namedquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-athena-preparedstatement.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-athena-workgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-auditmanager-assessment.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10526 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-autoscaling-autoscalinggroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-autoscaling-launchconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-autoscaling-lifecyclehook.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-autoscaling-scalingpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-autoscaling-scheduledaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-autoscaling-warmpool.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-autoscalingplans-scalingplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-backup-backupplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-backup-backupselection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-backup-backupvault.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-backup-framework.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-backup-reportplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-batch-computeenvironment.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-batch-jobdefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-batch-jobqueue.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-batch-schedulingpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-billingconductor-billinggroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-billingconductor-customlineitem.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-billingconductor-pricingplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-billingconductor-pricingrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-budgets-budget.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-budgets-budgetsaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cassandra-keyspace.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cassandra-table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ce-anomalymonitor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ce-anomalysubscription.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ce-costcategory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-certificatemanager-account.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-certificatemanager-certificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-chatbot-slackchannelconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloud9-environmentec2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudformation-customresource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudformation-hookdefaultversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudformation-hooktypeconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudformation-hookversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudformation-macro.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudformation-moduledefaultversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudformation-moduleversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudformation-publictypeversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudformation-publisher.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudformation-resourcedefaultversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudformation-resourceversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudformation-stack.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudformation-stackset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudformation-typeactivation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudformation-waitcondition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudformation-waitconditionhandle.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudfront-cachepolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudfront-cloudfrontoriginaccessidentity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudfront-continuousdeploymentpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudfront-distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudfront-function.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudfront-keygroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudfront-monitoringsubscription.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudfront-originaccesscontrol.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudfront-originrequestpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudfront-publickey.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudfront-realtimelogconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudfront-responseheaderspolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudfront-streamingdistribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudtrail-channel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudtrail-eventdatastore.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudtrail-resourcepolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudtrail-trail.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudwatch-alarm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudwatch-anomalydetector.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudwatch-compositealarm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudwatch-dashboard.json
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudwatch-insightrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cloudwatch-metricstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codeartifact-domain.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codeartifact-repository.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codebuild-project.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codebuild-reportgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codebuild-sourcecredential.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codecommit-repository.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codedeploy-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codedeploy-deploymentconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codedeploy-deploymentgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codeguruprofiler-profilinggroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codegurureviewer-repositoryassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codepipeline-customactiontype.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codepipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codepipeline-webhook.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codestar-githubrepository.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codestarconnections-connection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-codestarnotifications-notificationrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cognito-identitypool.json
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cognito-identitypoolroleattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8309 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cognito-userpool.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cognito-userpoolclient.json
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cognito-userpooldomain.json
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cognito-userpoolgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cognito-userpoolidentityprovider.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cognito-userpoolresourceserver.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cognito-userpoolriskconfigurationattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cognito-userpooluicustomizationattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cognito-userpooluser.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cognito-userpoolusertogroupattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-config-aggregationauthorization.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-config-configrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-config-configurationaggregator.json
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-config-configurationrecorder.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-config-conformancepack.json
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-config-deliverychannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-config-organizationconfigrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-config-organizationconformancepack.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-config-remediationconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-config-storedquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-connect-approvedorigin.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-connect-contactflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-connect-contactflowmodule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-connect-hoursofoperation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-connect-instance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-connect-instancestorageconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-connect-integrationassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-connect-phonenumber.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-connect-quickconnect.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-connect-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-connect-securitykey.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7617 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-connect-tasktemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-connect-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-connect-userhierarchygroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-connectcampaigns-campaign.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-controltower-enabledcontrol.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-cur-reportdefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-customerprofiles-domain.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-customerprofiles-integration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-customerprofiles-objecttype.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-databrew-dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-databrew-job.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-databrew-project.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-databrew-recipe.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-databrew-ruleset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-databrew-schedule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-datasync-agent.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-datasync-locationefs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-datasync-locationfsxlustre.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-datasync-locationfsxontap.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-datasync-locationfsxopenzfs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-datasync-locationfsxwindows.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-datasync-locationhdfs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-datasync-locationnfs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-datasync-locationobjectstorage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-datasync-locations3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-datasync-locationsmb.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-datasync-task.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-dax-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-dax-parametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-dax-subnetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-detective-graph.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-detective-memberinvitation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-devopsguru-notificationchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-devopsguru-resourcecollection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-directoryservice-microsoftad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-dlm-lifecyclepolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-dms-certificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-dms-endpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-dms-eventsubscription.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-dms-replicationinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-dms-replicationsubnetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-dms-replicationtask.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-docdb-dbcluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-docdb-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-docdb-dbinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-docdb-dbsubnetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-docdbelastic-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12534 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-dynamodb-globaltable.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-dynamodb-table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-capacityreservation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-capacityreservationfleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-carriergateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-clientvpnauthorizationrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-clientvpnendpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-clientvpnroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-clientvpntargetnetworkassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-customergateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-dhcpoptions.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-ec2fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-egressonlyinternetgateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-eip.json
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-eipassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-enclavecertificateiamroleassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-flowlog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-gatewayroutetableassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-host.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-instance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-internetgateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-ipam.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-ipamallocation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-ipampool.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-ipampoolcidr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-ipamresourcediscovery.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-ipamresourcediscoveryassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-ipamscope.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-keypair.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15989 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-launchtemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-localgatewayroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-localgatewayroutetablevpcassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-natgateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-networkacl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-networkaclentry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-networkinsightsaccessscope.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-networkinsightsaccessscopeanalysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14613 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-networkinsightsanalysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-networkinsightspath.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-networkinterface.json
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-networkinterfaceattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-networkinterfacepermission.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-networkperformancemetricsubscription.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-placementgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-prefixlist.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-route.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-routetable.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-securitygroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-securitygroupegress.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-securitygroupingress.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19577 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-spotfleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-subnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-subnetcidrblock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-subnetnetworkaclassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-subnetroutetableassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-trafficmirrorfilter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-trafficmirrorfilterrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-trafficmirrorsession.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-trafficmirrortarget.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-transitgateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-transitgatewayattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-transitgatewayconnect.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-transitgatewaymulticastdomain.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-transitgatewaymulticastdomainassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-transitgatewaymulticastgroupmember.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-transitgatewaymulticastgroupsource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-transitgatewaypeeringattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-transitgatewayroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-transitgatewayroutetable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-transitgatewayroutetableassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-transitgatewayroutetablepropagation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-transitgatewayvpcattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-volume.json
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-volumeattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-vpc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-vpccidrblock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-vpcdhcpoptionsassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-vpcendpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-vpcendpointservice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-vpcendpointservicepermissions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-vpcgatewayattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-vpcpeeringconnection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-vpnconnection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-vpnconnectionroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-vpngateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ec2-vpngatewayroutepropagation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ecr-publicrepository.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ecr-pullthroughcacherule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ecr-registrypolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ecr-replicationconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ecr-repository.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ecs-capacityprovider.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ecs-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ecs-clustercapacityproviderassociations.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ecs-primarytaskset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ecs-service.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18556 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ecs-taskdefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9904 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ecs-taskset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-efs-accesspoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-efs-filesystem.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-efs-mounttarget.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-eks-addon.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-eks-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-eks-fargateprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-eks-identityproviderconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-eks-nodegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticache-cachecluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticache-globalreplicationgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticache-parametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticache-replicationgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticache-securitygroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticache-securitygroupingress.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticache-subnetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticache-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticache-usergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticbeanstalk-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticbeanstalk-applicationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticbeanstalk-configurationtemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticbeanstalk-environment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticloadbalancing-loadbalancer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticloadbalancingv2-listener.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticloadbalancingv2-listenercertificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticloadbalancingv2-listenerrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticloadbalancingv2-loadbalancer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticloadbalancingv2-targetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-elasticsearch-domain.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15486 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-emr-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-emr-instancefleetconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-emr-instancegroupconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-emr-securityconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-emr-step.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-emr-studio.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-emr-studiosessionmapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-emrcontainers-virtualcluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-emrserverless-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-events-apidestination.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-events-archive.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-events-connection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-events-endpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-events-eventbus.json
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-events-eventbuspolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-events-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-eventschemas-discoverer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-eventschemas-registry.json
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-eventschemas-registrypolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-eventschemas-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-evidently-experiment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-evidently-feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-evidently-launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-evidently-project.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-evidently-segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-finspace-environment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-fis-experimenttemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-fms-notificationchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-fms-policy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-forecast-dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-forecast-datasetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-frauddetector-detector.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-frauddetector-entitytype.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-frauddetector-eventtype.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-frauddetector-label.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-frauddetector-outcome.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-frauddetector-variable.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-fsx-datarepositoryassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-fsx-filesystem.json
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-fsx-snapshot.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-fsx-storagevirtualmachine.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-fsx-volume.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-gamelift-alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-gamelift-build.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20921 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-gamelift-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-gamelift-gameservergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-gamelift-gamesessionqueue.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-gamelift-location.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-gamelift-matchmakingconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-gamelift-matchmakingruleset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-gamelift-script.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-globalaccelerator-accelerator.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-globalaccelerator-endpointgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-globalaccelerator-listener.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-classifier.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-connection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-crawler.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-database.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-datacatalogencryptionsettings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-devendpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-job.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-mltransform.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-partition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-registry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-schemaversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-schemaversionmetadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-securityconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-trigger.json
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-glue-workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12575 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-grafana-workspace.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrass-connectordefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrass-connectordefinitionversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrass-coredefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrass-coredefinitionversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrass-devicedefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrass-devicedefinitionversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrass-functiondefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrass-functiondefinitionversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrass-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrass-groupversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrass-loggerdefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrass-loggerdefinitionversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrass-resourcedefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrass-resourcedefinitionversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrass-subscriptiondefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrass-subscriptiondefinitionversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrassv2-componentversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-greengrassv2-deployment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-groundstation-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-groundstation-dataflowendpointgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-groundstation-missionprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-guardduty-detector.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-guardduty-filter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-guardduty-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-guardduty-master.json
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-guardduty-member.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-guardduty-threatintelset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-healthlake-fhirdatastore.json
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iam-accesskey.json
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iam-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iam-instanceprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iam-managedpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iam-oidcprovider.json
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iam-policy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iam-role.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iam-samlprovider.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iam-servercertificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iam-servicelinkedrole.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iam-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iam-usertogroupaddition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iam-virtualmfadevice.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-identitystore-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-identitystore-groupmembership.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-imagebuilder-component.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-imagebuilder-containerrecipe.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-imagebuilder-distributionconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-imagebuilder-image.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-imagebuilder-imagepipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-imagebuilder-imagerecipe.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-imagebuilder-infrastructureconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-inspector-assessmenttarget.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-inspector-assessmenttemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-inspector-resourcegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-inspectorv2-filter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-accountauditconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-authorizer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-cacertificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-certificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-custommetric.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-dimension.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-domainconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-fleetmetric.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-jobtemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-logging.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-mitigationaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-policy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-policyprincipalattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-provisioningtemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-resourcespecificlogging.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-rolealias.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-scheduledaudit.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-securityprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-thing.json
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-thingprincipalattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16870 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot-topicruledestination.json
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot1click-device.json
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot1click-placement.json
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iot1click-project.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotanalytics-channel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotanalytics-dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotanalytics-datastore.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotanalytics-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotcoredeviceadvisor-suitedefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20938 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotevents-alarmmodel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25062 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotevents-detectormodel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotevents-input.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotfleethub-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotfleetwise-campaign.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotfleetwise-decodermanifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotfleetwise-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotfleetwise-modelmanifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotfleetwise-signalcatalog.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotfleetwise-vehicle.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotsitewise-accesspolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotsitewise-asset.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotsitewise-assetmodel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotsitewise-dashboard.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotsitewise-gateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotsitewise-portal.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotsitewise-project.json
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotthingsgraph-flowtemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iottwinmaker-componenttype.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iottwinmaker-entity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iottwinmaker-scene.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iottwinmaker-syncjob.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iottwinmaker-workspace.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotwireless-destination.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotwireless-deviceprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotwireless-fuotatask.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotwireless-multicastgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotwireless-networkanalyzerconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotwireless-partneraccount.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotwireless-serviceprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotwireless-taskdefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotwireless-wirelessdevice.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-iotwireless-wirelessgateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ivs-channel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ivs-playbackkeypair.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ivs-recordingconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ivs-streamkey.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13746 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kafkaconnect-connector.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38854 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kendra-datasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kendra-faq.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kendra-index.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kendraranking-executionplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kinesis-stream.json
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kinesis-streamconsumer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kinesisanalytics-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kinesisanalytics-applicationoutput.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kinesisanalytics-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36460 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kinesisanalyticsv2-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kinesisanalyticsv2-applicationcloudwatchloggingoption.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kinesisanalyticsv2-applicationoutput.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kinesisanalyticsv2-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24639 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kinesisfirehose-deliverystream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kinesisvideo-signalingchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kinesisvideo-stream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kms-alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kms-key.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-kms-replicakey.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lakeformation-datacellsfilter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lakeformation-datalakesettings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lakeformation-permissions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lakeformation-principalpermissions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lakeformation-resource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lakeformation-tag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lakeformation-tagassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lambda-alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lambda-codesigningconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lambda-eventinvokeconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lambda-eventsourcemapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lambda-function.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lambda-layerversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lambda-layerversionpermission.json
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lambda-permission.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lambda-url.json
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lambda-version.json
+-rw-r--r--   0 runner    (1001) docker     (123)    71849 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lex-bot.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lex-botalias.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lex-botversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lex-resourcepolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-licensemanager-grant.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-licensemanager-license.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lightsail-alarm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lightsail-bucket.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lightsail-certificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lightsail-container.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lightsail-database.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lightsail-disk.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10377 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lightsail-distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lightsail-instance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lightsail-loadbalancer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lightsail-loadbalancertlscertificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lightsail-staticip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-location-geofencecollection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-location-map.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-location-placeindex.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-location-routecalculator.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-location-tracker.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-location-trackerconsumer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-logs-destination.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-logs-loggroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-logs-metricfilter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-logs-querydefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-logs-resourcepolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-logs-subscriptionfilter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lookoutequipment-inferencescheduler.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lookoutmetrics-alert.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lookoutmetrics-anomalydetector.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-lookoutvision-project.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-m2-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-m2-environment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-macie-allowlist.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-macie-customdataidentifier.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-macie-findingsfilter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-macie-session.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-managedblockchain-member.json
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-managedblockchain-node.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-mediaconnect-flow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-mediaconnect-flowentitlement.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-mediaconnect-flowoutput.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-mediaconnect-flowsource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-mediaconnect-flowvpcinterface.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-mediaconvert-jobtemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-mediaconvert-preset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-mediaconvert-queue.json
+-rw-r--r--   0 runner    (1001) docker     (123)    58292 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-medialive-channel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-medialive-input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-medialive-inputsecuritygroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-mediapackage-asset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-mediapackage-channel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23952 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-mediapackage-originendpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15187 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-mediapackage-packagingconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-mediapackage-packaginggroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-mediastore-container.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-mediatailor-playbackconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-memorydb-acl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-memorydb-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-memorydb-parametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-memorydb-subnetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-memorydb-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-msk-batchscramsecret.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-msk-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-msk-configuration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-msk-serverlesscluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-mwaa-environment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-neptune-dbcluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-neptune-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-neptune-dbinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-neptune-dbparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-neptune-dbsubnetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkfirewall-firewall.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkfirewall-firewallpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkfirewall-loggingconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13427 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkfirewall-rulegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkmanager-connectattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkmanager-connectpeer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkmanager-corenetwork.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkmanager-customergatewayassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkmanager-device.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkmanager-globalnetwork.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkmanager-link.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkmanager-linkassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkmanager-site.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkmanager-sitetositevpnattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkmanager-transitgatewaypeering.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkmanager-transitgatewayregistration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-networkmanager-vpcattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-nimblestudio-launchprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-nimblestudio-streamingimage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-nimblestudio-studio.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-nimblestudio-studiocomponent.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-oam-link.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-oam-sink.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-omics-annotationstore.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-omics-referencestore.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-omics-rungroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-omics-sequencestore.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-omics-variantstore.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-omics-workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-opensearchserverless-accesspolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-opensearchserverless-collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-opensearchserverless-securityconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-opensearchserverless-securitypolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-opensearchserverless-vpcendpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-opensearchservice-domain.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-opsworks-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-opsworks-elasticloadbalancerattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-opsworks-instance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-opsworks-layer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-opsworks-stack.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-opsworks-userprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-opsworks-volume.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-opsworkscm-server.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-organizations-account.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-organizations-organizationalunit.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-organizations-policy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-panorama-applicationinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-panorama-package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-panorama-packageversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-personalize-dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-personalize-datasetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-personalize-schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9194 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-personalize-solution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-admchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-apnschannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-apnssandboxchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-apnsvoipchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-apnsvoipsandboxchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-applicationsettings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-baiduchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-campaign.json
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-emailchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-emailtemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-eventstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-gcmchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-inapptemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-pushtemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-smschannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-smstemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpoint-voicechannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpointemail-configurationset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpointemail-configurationseteventdestination.json
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpointemail-dedicatedippool.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pinpointemail-identity.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34847 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-pipes-pipe.json
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-qldb-ledger.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-qldb-stream.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-quicksight-analysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-quicksight-dashboard.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25067 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-quicksight-dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22702 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-quicksight-datasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-quicksight-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15703 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-quicksight-theme.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ram-resourceshare.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22982 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rds-dbcluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rds-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25005 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rds-dbinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rds-dbparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rds-dbproxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rds-dbproxyendpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rds-dbproxytargetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rds-dbsecuritygroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rds-dbsecuritygroupingress.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rds-dbsubnetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rds-eventsubscription.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rds-globalcluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rds-optiongroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-redshift-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-redshift-clusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-redshift-clustersecuritygroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-redshift-clustersecuritygroupingress.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-redshift-clustersubnetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-redshift-endpointaccess.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-redshift-endpointauthorization.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-redshift-eventsubscription.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-redshift-scheduledaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-redshiftserverless-namespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-redshiftserverless-workgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-refactorspaces-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-refactorspaces-environment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-refactorspaces-route.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-refactorspaces-service.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rekognition-collection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rekognition-project.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rekognition-streamprocessor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-resiliencehub-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-resiliencehub-resiliencypolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-resourceexplorer2-defaultviewassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-resourceexplorer2-index.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-resourceexplorer2-view.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-resourcegroups-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-robomaker-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-robomaker-robot.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-robomaker-robotapplication.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-robomaker-robotapplicationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-robomaker-simulationapplication.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-robomaker-simulationapplicationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rolesanywhere-crl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rolesanywhere-profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rolesanywhere-trustanchor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53-cidrcollection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53-dnssec.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53-healthcheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53-hostedzone.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53-keysigningkey.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53-recordset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53-recordsetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53recoverycontrol-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53recoverycontrol-controlpanel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53recoverycontrol-routingcontrol.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53recoverycontrol-safetyrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53recoveryreadiness-cell.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53recoveryreadiness-readinesscheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53recoveryreadiness-recoverygroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53recoveryreadiness-resourceset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53resolver-firewalldomainlist.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53resolver-firewallrulegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53resolver-firewallrulegroupassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53resolver-resolverconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53resolver-resolverdnssecconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53resolver-resolverendpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53resolver-resolverqueryloggingconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53resolver-resolverqueryloggingconfigassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53resolver-resolverrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-route53resolver-resolverruleassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15376 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-rum-appmonitor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-s3-accesspoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46511 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-s3-bucket.json
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-s3-bucketpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-s3-multiregionaccesspoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-s3-multiregionaccesspointpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-s3-storagelens.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-s3objectlambda-accesspoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-s3objectlambda-accesspointpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-s3outposts-accesspoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-s3outposts-bucket.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-s3outposts-bucketpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-s3outposts-endpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-appimageconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-coderepository.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17325 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-dataqualityjobdefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-device.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-devicefleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16481 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-domain.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-endpoint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-endpointconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-featuregroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-image.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-imageversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-model.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18274 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-modelbiasjobdefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18996 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-modelcard.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-modelexplainabilityjobdefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33168 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-modelpackage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-modelpackagegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19326 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-modelqualityjobdefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21189 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-monitoringschedule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-notebookinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-notebookinstancelifecycleconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-project.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-space.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-userprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sagemaker-workteam.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19806 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-scheduler-schedule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-scheduler-schedulegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sdb-domain.json
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-secretsmanager-resourcepolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-secretsmanager-rotationschedule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-secretsmanager-secret.json
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-secretsmanager-secrettargetattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-securityhub-hub.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalog-acceptedportfolioshare.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalog-cloudformationproduct.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalog-cloudformationprovisionedproduct.json
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalog-launchnotificationconstraint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalog-launchroleconstraint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalog-launchtemplateconstraint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalog-portfolio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalog-portfolioprincipalassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalog-portfolioproductassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalog-portfolioshare.json
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalog-resourceupdateconstraint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalog-serviceaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalog-serviceactionassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalog-stacksetconstraint.json
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalog-tagoption.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalog-tagoptionassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalogappregistry-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalogappregistry-attributegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalogappregistry-attributegroupassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicecatalogappregistry-resourceassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicediscovery-httpnamespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicediscovery-instance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicediscovery-privatednsnamespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicediscovery-publicdnsnamespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-servicediscovery-service.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ses-configurationset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ses-configurationseteventdestination.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ses-contactlist.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ses-dedicatedippool.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ses-emailidentity.json
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ses-receiptfilter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ses-receiptrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ses-receiptruleset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ses-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ses-vdmattributes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-signer-profilepermission.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-signer-signingprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-simspaceweaver-simulation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sns-subscription.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sns-topic.json
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sns-topicpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sqs-queue.json
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sqs-queuepolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ssm-association.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ssm-document.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ssm-maintenancewindow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ssm-maintenancewindowtarget.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ssm-maintenancewindowtask.json
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ssm-parameter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ssm-patchbaseline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ssm-resourcedatasync.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ssm-resourcepolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ssmcontacts-contact.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ssmcontacts-contactchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ssmincidents-replicationset.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-ssmincidents-responseplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sso-assignment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sso-instanceaccesscontrolattributeconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-sso-permissionset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-stepfunctions-activity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-stepfunctions-statemachine.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-supportapp-accountalias.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-supportapp-slackchannelconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-supportapp-slackworkspaceconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-synthetics-canary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-synthetics-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-timestream-database.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18873 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-timestream-scheduledquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-timestream-table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-transfer-agreement.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-transfer-certificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-transfer-connector.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-transfer-profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-transfer-server.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-transfer-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10456 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-transfer-workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-voiceid-domain.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-waf-bytematchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-waf-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-waf-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-waf-sizeconstraintset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-waf-sqlinjectionmatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-waf-webacl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-waf-xssmatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafregional-bytematchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafregional-geomatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafregional-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafregional-ratebasedrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafregional-regexpatternset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafregional-rule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafregional-sizeconstraintset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafregional-sqlinjectionmatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafregional-webacl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafregional-webaclassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafregional-xssmatchset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafv2-ipset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafv2-loggingconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafv2-regexpatternset.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27680 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafv2-rulegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32285 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafv2-webacl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wafv2-webaclassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wisdom-assistant.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wisdom-assistantassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-wisdom-knowledgebase.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-workspaces-connectionalias.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-workspaces-workspace.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-xray-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-xray-resourcepolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-1/aws-xray-samplingrule.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.268993 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-2/aws-appstream-stackuserassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-14 15:37:17.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-2/aws-appstream-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-2/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-2/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-2/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-2/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-2/aws-managedblockchain-member.json
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-2/aws-managedblockchain-node.json
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-2/aws-medialive-inputsecuritygroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-east-2/aws-route53resolver-resolverconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.276993 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-amazonmq-configurationassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigateway-account.json
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigateway-authorizer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigateway-basepathmapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigateway-clientcertificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigateway-deployment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigateway-documentationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigateway-gatewayresponse.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigateway-method.json
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigateway-model.json
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigateway-requestvalidator.json
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigateway-resource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigateway-restapi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigateway-stage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigatewayv2-api.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigatewayv2-authorizer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigatewayv2-deployment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigatewayv2-model.json
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-apigatewayv2-vpclink.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-autoscaling-launchconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-autoscaling-lifecyclehook.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-autoscaling-scalingpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-autoscaling-scheduledaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-codedeploy-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-codedeploy-deploymentconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-codepipeline-customactiontype.json
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-config-aggregationauthorization.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-clientvpnauthorizationrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-customergateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-eip.json
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-host.json
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-internetgateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-networkinterface.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-placementgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-routetable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-subnetnetworkaclassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-subnetroutetableassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-transitgateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-transitgatewayvpcattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-volume.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-vpc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-vpcpeeringconnection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-vpnconnection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ec2-vpngateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ecs-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-ecs-clustercapacityproviderassociations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-efs-mounttarget.json
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-elasticache-subnetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-elasticache-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-elasticbeanstalk-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-elasticbeanstalk-applicationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-elasticbeanstalk-configurationtemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-elasticbeanstalk-environment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-elasticloadbalancingv2-targetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-emr-securityconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-gamelift-alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-gamelift-build.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-gamelift-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-glue-datacatalogencryptionsettings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-greengrass-connectordefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-greengrass-coredefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-greengrass-devicedefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-greengrass-devicedefinitionversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-greengrass-functiondefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-greengrass-functiondefinitionversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-greengrass-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-greengrass-loggerdefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-greengrass-loggerdefinitionversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-greengrass-subscriptiondefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-greengrass-subscriptiondefinitionversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-guardduty-master.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-iam-instanceprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-iam-role.json
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-inspector-assessmenttarget.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-inspector-assessmenttemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-inspector-resourcegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-iot-scheduledaudit.json
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-iot-thing.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-kinesis-stream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-kinesisanalytics-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-kinesisanalytics-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-kinesisanalyticsv2-applicationcloudwatchloggingoption.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-kinesisanalyticsv2-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-neptune-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-neptune-dbinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-neptune-dbparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-route53-healthcheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-route53-hostedzone.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-route53resolver-resolverconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-route53resolver-resolverrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-route53resolver-resolverruleassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-secretsmanager-secrettargetattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-servicecatalog-acceptedportfolioshare.json
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-servicecatalog-portfolio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-servicecatalog-portfolioprincipalassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-servicecatalog-portfolioproductassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-servicecatalog-tagoptionassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-sns-topic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-sqs-queue.json
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-stepfunctions-activity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-transfer-connector.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-transfer-workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-wafv2-loggingconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26773 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-wafv2-rulegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-east-1/aws-wafv2-webacl.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.288994 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-amazonmq-configurationassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigateway-account.json
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigateway-authorizer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigateway-basepathmapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigateway-clientcertificate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigateway-deployment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigateway-documentationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigateway-gatewayresponse.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigateway-method.json
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigateway-model.json
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigateway-requestvalidator.json
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigateway-resource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigateway-restapi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigateway-stage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigateway-usageplan.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigatewayv2-api.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigatewayv2-authorizer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigatewayv2-deployment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigatewayv2-model.json
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-apigatewayv2-vpclink.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-appstream-imagebuilder.json
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-appstream-stackuserassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-appstream-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-autoscaling-launchconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-autoscaling-lifecyclehook.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-autoscaling-scalingpolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-autoscaling-scheduledaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-codedeploy-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-codedeploy-deploymentconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-codepipeline-customactiontype.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-cognito-userpoolriskconfigurationattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-cognito-userpooluicustomizationattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-cognito-userpoolusertogroupattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-config-aggregationauthorization.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-config-organizationconfigrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-docdb-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-clientvpnauthorizationrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-customergateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-eip.json
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-host.json
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-internetgateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-networkinterface.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-placementgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-routetable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-subnetnetworkaclassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-subnetroutetableassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-transitgateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-transitgatewayvpcattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-volume.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-vpc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-vpcpeeringconnection.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-vpnconnection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ec2-vpngateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ecs-cluster.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ecs-clustercapacityproviderassociations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-efs-mounttarget.json
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-elasticache-subnetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-elasticache-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-elasticbeanstalk-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-elasticbeanstalk-applicationversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-elasticbeanstalk-configurationtemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-elasticbeanstalk-environment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-elasticloadbalancingv2-targetgroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-emr-securityconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-gamelift-alias.json
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-gamelift-build.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-gamelift-fleet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-glue-datacatalogencryptionsettings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-guardduty-master.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-iam-instanceprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-iam-role.json
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-inspector-assessmenttarget.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-inspector-assessmenttemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-inspector-resourcegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-iot-scheduledaudit.json
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-iot-thing.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-iotsitewise-asset.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10149 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-iotsitewise-assetmodel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-kinesis-stream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-kinesisanalytics-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-kinesisanalytics-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-kinesisanalyticsv2-applicationcloudwatchloggingoption.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-kinesisanalyticsv2-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-neptune-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-neptune-dbinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-neptune-dbparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-pinpoint-admchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-pinpoint-app.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-pinpoint-baiduchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-pinpoint-gcmchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-pinpoint-segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-route53-healthcheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-route53-hostedzone.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-route53resolver-resolverrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-route53resolver-resolverruleassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-servicecatalog-acceptedportfolioshare.json
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-servicecatalog-portfolio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-servicecatalog-portfolioprincipalassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-servicecatalog-portfolioproductassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-servicecatalog-tagoptionassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-sns-topic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-sqs-queue.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-ssm-resourcedatasync.json
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-stepfunctions-activity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-transfer-connector.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-transfer-workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-wafv2-loggingconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26773 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-wafv2-rulegroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29871 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-gov-west-1/aws-wafv2-webacl.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.288994 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-appstream-directoryconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-appstream-stack.json
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-appstream-stackuserassociation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-appstream-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-athena-namedquery.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-cognito-userpoolriskconfigurationattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-cognito-userpooluicustomizationattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-cognito-userpoolusertogroupattachment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-datapipeline-pipeline.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-directoryservice-simplead.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-greengrass-coredefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-greengrass-devicedefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-greengrass-devicedefinitionversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-greengrass-functiondefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-greengrass-functiondefinitionversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-greengrass-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-greengrass-loggerdefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-greengrass-loggerdefinitionversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-greengrass-subscriptiondefinition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-greengrass-subscriptiondefinitionversion.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-iot-topicrule.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-kinesisanalytics-application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-kinesisanalytics-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-kinesisanalyticsv2-applicationcloudwatchloggingoption.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-kinesisanalyticsv2-applicationreferencedatasource.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-neptune-dbclusterparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-neptune-dbinstance.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-neptune-dbparametergroup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-1/aws-route53resolver-resolverconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.292994 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/aws-devicefarm-devicepool.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/aws-devicefarm-instanceprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/aws-devicefarm-networkprofile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/aws-devicefarm-project.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/aws-devicefarm-testgridproject.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/aws-devicefarm-vpceconfiguration.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/aws-ec2-vpcendpointconnectionnotification.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/aws-ec2-vpnconnectionroute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/aws-iot-mitigationaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/aws-logs-logstream.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/aws-managedblockchain-member.json
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/aws-managedblockchain-node.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/aws-organizations-resourcepolicy.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/aws-refactorspaces-environment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/ProviderSchemas/us-west-2/aws-route53resolver-resolverconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.292994 cfn-lint-1.0.0a2/src/cfnlint/data/Serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)   106855 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/Serverless/ManagedPolicies.json
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/Serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.292994 cfn-lint-1.0.0a2/src/cfnlint/decode/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/decode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/decode/cfn_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/decode/cfn_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/decode/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/decode/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/decode/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.292994 cfn-lint-1.0.0a2/src/cfnlint/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/decorators/refactored.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.292994 cfn-lint-1.0.0a2/src/cfnlint/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18274 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.292994 cfn-lint-1.0.0a2/src/cfnlint/jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/jsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/jsonschema/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/jsonschema/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13184 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/jsonschema/_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/jsonschema/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/jsonschema/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/languageExtensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/maintenance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.292994 cfn-lint-1.0.0a2/src/cfnlint/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.292994 cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/And.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/Equals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/EqualsIsUseful.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/Exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/Not.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/Or.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/Used.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.292994 cfn-lint-1.0.0a2/src/cfnlint/rules/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/custom/Operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/custom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.296994 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Cidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/DynamicReferenceSecureString.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11522 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/FindInMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/FindInMapKeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/GetAtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/GetAz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/If.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/ImportValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Not.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/RefExist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/RefInCondition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/RelationshipConditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/SubNeeded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/SubNotJoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/SubParametersUsed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/SubUnneeded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/ToJsonString.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.296994 cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/ApproachingLimitAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/ApproachingLimitName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/ApproachingLimitNumber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/KeyName.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/LimitAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/LimitName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/LimitNumber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/Name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/Used.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.296994 cfn-lint-1.0.0a2/src/cfnlint/rules/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/metadata/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/metadata/InterfaceConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/metadata/InterfaceParameterExists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.296994 cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/ApproachingLimitDescription.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/ApproachingLimitName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/ApproachingLimitNumber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/Description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/ImportValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/LimitDescription.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/LimitName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/LimitNumber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/Name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/Required.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/Value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.300994 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/AllowedPattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/AllowedValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/ApproachingLimitName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/ApproachingLimitNumber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/ApproachingLimitValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/Default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/DefaultRef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/LambdaMemorySize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/LimitName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/LimitNumber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/LimitValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/Name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/Types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/Used.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.300994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ApproachingLimitName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ApproachingLimitNumber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/BothUpdateReplacePolicyDeletionPolicyNeeded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/CircularDependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/DeletionPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/DependsOn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/DependsOnObsolete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/HardCodedArnProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/LimitName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/LimitNumber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/Modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/Name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/NoEcho.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/PreviousGenerationInstanceType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/RetentionPeriodOnResourceTypesWithAutoExpiringContent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ServerlessTransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/UniqueNames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/UpdateReplacePolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/UpdateReplacePolicyDeletionPolicyOnStatefulResourceTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.300994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/backup/BackupPlanLifecycleRule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/backup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.300994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/certificatemanager/
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/certificatemanager/DomainValidationOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/certificatemanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.300994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/cloudformation/NestedStackParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/cloudformation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.300994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/cloudfront/Aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/cloudfront/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.304994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/codepipeline/CodepipelineStageActions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/codepipeline/CodepipelineStages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/codepipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.304994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/dynamodb/AttributeMismatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/dynamodb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.304994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ecs/FargateDeploymentSchedulingStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ecs/TaskDefinitionEssentialContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ecs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.304994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ectwo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ectwo/Ebs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ectwo/RouteTableAssociation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ectwo/SecurityGroupIngress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ectwo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.304994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/elasticache/CacheClusterFailover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/elasticache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.304994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/elb/
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/elb/Elb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/elb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.304994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/events/RuleScheduleExpression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/events/RuleTargetsLimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.304994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/iam/
+-rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/iam/Permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/iam/Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/iam/PolicyVersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/iam/RefWithPath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/iam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.304994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/lmbd/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/lmbd/DeprecatedRuntime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/lmbd/DeprecatedRuntimeEnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/lmbd/DeprecatedRuntimeEol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/lmbd/EventsLogGroupName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/lmbd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.308994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/AllowedPattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/AllowedValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/AvailabilityZone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/AwsType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/CfnSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/ImageId.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/JsonSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/ListDuplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/ListDuplicatesAllowed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/ListSize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/NumberSize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/OnlyOne.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/Password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/Properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/PropertiesTemplated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/Required.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/StringSize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/ValuePrimitiveType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.308994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/rds/InstanceSize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/rds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.308994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/route53/
+-rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/route53/RecordSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/route53/RecordSetName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/route53/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.308994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/stepfunctions/StateMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/stepfunctions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.308994 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/updatepolicy/
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/updatepolicy/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/resources/updatepolicy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.308994 cfn-lint-1.0.0a2/src/cfnlint/rules/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/templates/ApproachingLimitDescription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/templates/ApproachingLimitSize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/templates/Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/templates/Description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/templates/LimitDescription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/templates/LimitSize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/rules/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.308994 cfn-lint-1.0.0a2/src/cfnlint/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/schema/_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/schema/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13570 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/schema/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/schema/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/schema/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 15:37:32.308994 cfn-lint-1.0.0a2/src/cfnlint/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/template/getatts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46643 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/template/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-14 15:37:18.000000 cfn-lint-1.0.0a2/src/cfnlint/version.py
```

### Comparing `cfn-lint-1.0.0a1/LICENSE` & `cfn-lint-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/PKG-INFO` & `cfn-lint-1.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-lint
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Checks CloudFormation templates for practices and behaviour that could potentially be improved
 Home-page: https://github.com/aws-cloudformation/cfn-python-lint
 Author: kddejong
 Author-email: kddejong@amazon.com
 License: MIT no attribution
 Keywords: aws,lint
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cfn-lint-1.0.0a1/README.md` & `cfn-lint-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/setup.py` & `cfn-lint-1.0.0a2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,18 +29,19 @@
     long_description_content_type="text/markdown",
     keywords='aws, lint',
     author='kddejong',
     author_email='kddejong@amazon.com',
     url='https://github.com/aws-cloudformation/cfn-python-lint',
     package_dir={'': 'src'},
     package_data={'cfnlint': [
-        'data/CloudSpecs/*.json',
+        'data/AdditionalSchemas/*/*.json',
+        'data/ProviderSchemas/*/*.json',
+        'data/ExtendendProviderSchemas/*/*.json',
         'data/AdditionalSpecs/*.json',
         'data/Serverless/*.json',
-        'data/ExtendedSpecs/*/*.json',
         'data/CfnLintCli/config/schema.json'
     ]},
     packages=find_packages('src'),
     zip_safe=False,
     install_requires=[
         'pyyaml>5.4',
         'aws-sam-translator>=1.60.1',
```

### Comparing `cfn-lint-1.0.0a1/src/cfn_lint.egg-info/PKG-INFO` & `cfn-lint-1.0.0a2/src/cfn_lint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-lint
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Checks CloudFormation templates for practices and behaviour that could potentially be improved
 Home-page: https://github.com/aws-cloudformation/cfn-python-lint
 Author: kddejong
 Author-email: kddejong@amazon.com
 License: MIT no attribution
 Keywords: aws,lint
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/__init__.py` & `cfn-lint-1.0.0a2/src/cfnlint/__init__.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/__main__.py` & `cfn-lint-1.0.0a2/src/cfnlint/__main__.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/api.py` & `cfn-lint-1.0.0a2/src/cfnlint/api.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/conditions.py` & `cfn-lint-1.0.0a2/src/cfnlint/conditions.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/config.py` & `cfn-lint-1.0.0a2/src/cfnlint/config.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/core.py` & `cfn-lint-1.0.0a2/src/cfnlint/core.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSpecs/BasedOnValue.json` & `cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSpecs/BasedOnValue.json`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSpecs/LmbdRuntimeLifecycle.json` & `cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSpecs/LmbdRuntimeLifecycle.json`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSpecs/Policies.json` & `cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSpecs/Policies.json`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSpecs/RdsProperties.json` & `cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSpecs/RdsProperties.json`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/data/AdditionalSpecs/StatefulResources.json` & `cfn-lint-1.0.0a2/src/cfnlint/data/AdditionalSpecs/StatefulResources.json`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/data/CfnLintCli/config/schema.json` & `cfn-lint-1.0.0a2/src/cfnlint/data/CfnLintCli/config/schema.json`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/data/Serverless/ManagedPolicies.json` & `cfn-lint-1.0.0a2/src/cfnlint/data/Serverless/ManagedPolicies.json`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/decode/cfn_json.py` & `cfn-lint-1.0.0a2/src/cfnlint/decode/cfn_json.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/decode/cfn_yaml.py` & `cfn-lint-1.0.0a2/src/cfnlint/decode/cfn_yaml.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/decode/decode.py` & `cfn-lint-1.0.0a2/src/cfnlint/decode/decode.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/decode/node.py` & `cfn-lint-1.0.0a2/src/cfnlint/decode/node.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/decorators/refactored.py` & `cfn-lint-1.0.0a2/src/cfnlint/decorators/refactored.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/exceptions.py` & `cfn-lint-1.0.0a2/src/cfnlint/exceptions.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/formatters/__init__.py` & `cfn-lint-1.0.0a2/src/cfnlint/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/graph.py` & `cfn-lint-1.0.0a2/src/cfnlint/graph.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/helpers.py` & `cfn-lint-1.0.0a2/src/cfnlint/helpers.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/jsonschema/_types.py` & `cfn-lint-1.0.0a2/src/cfnlint/jsonschema/_types.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/jsonschema/_utils.py` & `cfn-lint-1.0.0a2/src/cfnlint/jsonschema/_utils.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/jsonschema/_validators.py` & `cfn-lint-1.0.0a2/src/cfnlint/jsonschema/_validators.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/jsonschema/exceptions.py` & `cfn-lint-1.0.0a2/src/cfnlint/jsonschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/jsonschema/validator.py` & `cfn-lint-1.0.0a2/src/cfnlint/jsonschema/validator.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/languageExtensions.py` & `cfn-lint-1.0.0a2/src/cfnlint/languageExtensions.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/maintenance.py` & `cfn-lint-1.0.0a2/src/cfnlint/maintenance.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/__init__.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/common.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/common.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/And.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/And.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/Configuration.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/Configuration.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/Equals.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/Equals.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/EqualsIsUseful.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/EqualsIsUseful.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/Exists.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/Exists.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/Not.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/Not.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/Or.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/Or.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/Used.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/Used.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/conditions/common.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/conditions/common.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/custom/Operators.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/custom/Operators.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/custom/__init__.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Base64.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Base64.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Cidr.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Cidr.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/DynamicReferenceSecureString.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/DynamicReferenceSecureString.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/FindInMap.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/FindInMap.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/FindInMapKeys.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/FindInMapKeys.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/GetAtt.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/GetAtt.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/GetAz.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/GetAz.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/If.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/If.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/ImportValue.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/ImportValue.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Join.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Join.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Length.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Length.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Not.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Not.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Ref.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Ref.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/RefExist.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/RefExist.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/RefInCondition.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/RefInCondition.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/RelationshipConditions.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/RelationshipConditions.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Select.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Select.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Split.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Split.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/Sub.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/Sub.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/SubNeeded.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/SubNeeded.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/SubNotJoin.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/SubNotJoin.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/SubParametersUsed.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/SubParametersUsed.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/SubUnneeded.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/SubUnneeded.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/functions/ToJsonString.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/functions/ToJsonString.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/ApproachingLimitAttributes.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/ApproachingLimitAttributes.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/ApproachingLimitName.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/ApproachingLimitName.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/ApproachingLimitNumber.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/ApproachingLimitNumber.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/Configuration.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/Configuration.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/KeyName.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/KeyName.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/LimitAttributes.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/LimitAttributes.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/LimitName.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/LimitName.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/LimitNumber.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/LimitNumber.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/Name.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/Name.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/mappings/Used.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/mappings/Used.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/metadata/Config.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/metadata/Config.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/metadata/InterfaceConfiguration.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/metadata/InterfaceConfiguration.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/metadata/InterfaceParameterExists.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/metadata/InterfaceParameterExists.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/ApproachingLimitDescription.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/ApproachingLimitDescription.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/ApproachingLimitName.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/ApproachingLimitName.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/ApproachingLimitNumber.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/ApproachingLimitNumber.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/Configuration.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/Configuration.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/Description.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/Description.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/ImportValue.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/ImportValue.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/LimitDescription.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/LimitDescription.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/LimitName.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/LimitName.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/LimitNumber.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/LimitNumber.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/Name.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/Name.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/Required.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/Required.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/outputs/Value.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/outputs/Value.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/AllowedPattern.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/AllowedPattern.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/AllowedValue.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/AllowedValue.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/ApproachingLimitName.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/ApproachingLimitName.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/ApproachingLimitNumber.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/ApproachingLimitNumber.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/ApproachingLimitValue.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/ApproachingLimitValue.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/Configuration.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/Configuration.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/Default.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/Default.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/DefaultRef.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/DefaultRef.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/LambdaMemorySize.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/LambdaMemorySize.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/LimitName.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/LimitName.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/LimitNumber.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/LimitNumber.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/LimitValue.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/LimitValue.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/Name.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/Name.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/Types.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/Types.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/parameters/Used.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/parameters/Used.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ApproachingLimitName.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ApproachingLimitName.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ApproachingLimitNumber.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ApproachingLimitNumber.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/BothUpdateReplacePolicyDeletionPolicyNeeded.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/BothUpdateReplacePolicyDeletionPolicyNeeded.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/CircularDependency.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/CircularDependency.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/Configuration.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/Configuration.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/DeletionPolicy.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/DeletionPolicy.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/DependsOn.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/DependsOn.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/DependsOnObsolete.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/DependsOnObsolete.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/HardCodedArnProperties.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/HardCodedArnProperties.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/LimitName.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/LimitName.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/LimitNumber.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/LimitNumber.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/Modules.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/Modules.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/Name.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/Name.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/NoEcho.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/NoEcho.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/PreviousGenerationInstanceType.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/PreviousGenerationInstanceType.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/RetentionPeriodOnResourceTypesWithAutoExpiringContent.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/RetentionPeriodOnResourceTypesWithAutoExpiringContent.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ServerlessTransform.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ServerlessTransform.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/UniqueNames.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/UniqueNames.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/UpdateReplacePolicy.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/UpdateReplacePolicy.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/UpdateReplacePolicyDeletionPolicyOnStatefulResourceTypes.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/UpdateReplacePolicyDeletionPolicyOnStatefulResourceTypes.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/backup/BackupPlanLifecycleRule.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/backup/BackupPlanLifecycleRule.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/certificatemanager/DomainValidationOptions.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/certificatemanager/DomainValidationOptions.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/cloudformation/NestedStackParameters.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/cloudformation/NestedStackParameters.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/cloudfront/Aliases.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/cloudfront/Aliases.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/codepipeline/CodepipelineStageActions.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/codepipeline/CodepipelineStageActions.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/codepipeline/CodepipelineStages.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/codepipeline/CodepipelineStages.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/dynamodb/AttributeMismatch.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/dynamodb/AttributeMismatch.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ecs/FargateDeploymentSchedulingStrategy.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ecs/FargateDeploymentSchedulingStrategy.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ecs/TaskDefinitionEssentialContainer.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ecs/TaskDefinitionEssentialContainer.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ectwo/Ebs.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ectwo/Ebs.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ectwo/RouteTableAssociation.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ectwo/RouteTableAssociation.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/ectwo/SecurityGroupIngress.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/ectwo/SecurityGroupIngress.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/elasticache/CacheClusterFailover.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/elasticache/CacheClusterFailover.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/elb/Elb.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/elb/Elb.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/events/RuleScheduleExpression.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/events/RuleScheduleExpression.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/events/RuleTargetsLimit.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/events/RuleTargetsLimit.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/iam/Permissions.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/iam/Permissions.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/iam/Policy.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/iam/Policy.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/iam/PolicyVersion.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/iam/PolicyVersion.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/iam/RefWithPath.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/iam/RefWithPath.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/lmbd/DeprecatedRuntime.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/lmbd/DeprecatedRuntime.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/lmbd/DeprecatedRuntimeEnd.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/lmbd/DeprecatedRuntimeEnd.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/lmbd/DeprecatedRuntimeEol.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/lmbd/DeprecatedRuntimeEol.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/lmbd/EventsLogGroupName.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/lmbd/EventsLogGroupName.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/AllowedPattern.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/AllowedPattern.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/AllowedValue.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/AllowedValue.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/AvailabilityZone.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/AvailabilityZone.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/AwsType.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/AwsType.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/ImageId.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/ImageId.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/JsonSchema.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/JsonSchema.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/ListDuplicates.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/ListDuplicates.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/ListDuplicatesAllowed.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/ListDuplicatesAllowed.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/ListSize.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/ListSize.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/NumberSize.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/NumberSize.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/OnlyOne.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/OnlyOne.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/Password.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/Password.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/Properties.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/Properties.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/PropertiesTemplated.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/PropertiesTemplated.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/Required.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/Required.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/StringSize.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/StringSize.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/properties/ValuePrimitiveType.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/properties/ValuePrimitiveType.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/rds/InstanceSize.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/rds/InstanceSize.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/route53/RecordSet.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/route53/RecordSet.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/route53/RecordSetName.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/route53/RecordSetName.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/stepfunctions/StateMachine.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/stepfunctions/StateMachine.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/resources/updatepolicy/Configuration.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/resources/updatepolicy/Configuration.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/templates/ApproachingLimitDescription.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/templates/ApproachingLimitDescription.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/templates/ApproachingLimitSize.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/templates/ApproachingLimitSize.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/templates/Base.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/templates/Base.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/templates/Description.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/templates/Description.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/templates/LimitDescription.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/templates/LimitDescription.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/rules/templates/LimitSize.py` & `cfn-lint-1.0.0a2/src/cfnlint/rules/templates/LimitSize.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/runner.py` & `cfn-lint-1.0.0a2/src/cfnlint/runner.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/schema/_pointer.py` & `cfn-lint-1.0.0a2/src/cfnlint/schema/_pointer.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/schema/manager.py` & `cfn-lint-1.0.0a2/src/cfnlint/schema/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     _cache: Dict[str, Union[Sequence, str]] = {}
 
     def __init__(self) -> None:
         self._patch_path = os.path.join(
             os.path.dirname(__file__),
             "..",
             "data",
-            "ExtendedProviderSchema",
+            "ExtendedProviderSchemas",
         )
         self._root_path = os.path.join(
             os.path.dirname(__file__),
             "..",
             "data",
             "ProviderSchemas",
         )
@@ -239,15 +239,15 @@
                     file_path = os.path.basename(filename)
                     module = dirpath.replace(f"{append_dir}", f"{region}").replace(
                         os.path.sep, "."
                     )
                     LOGGER.info("Processing patch in %s.%s", module, file_path)
                     jsonpatch.JsonPatch(
                         load_resource(
-                            f"cfnlint.data.ExtendedProviderSchema.{module}", file_path
+                            f"cfnlint.data.ExtendedProviderSchemas.{module}", file_path
                         )
                     ).apply(content, in_place=True)
 
         return content
 
     def patch(self, filename: str, regions: Sequence[str]):
         try:
```

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/schema/patch.py` & `cfn-lint-1.0.0a2/src/cfnlint/schema/patch.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/schema/schema.py` & `cfn-lint-1.0.0a2/src/cfnlint/schema/schema.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/template/getatts.py` & `cfn-lint-1.0.0a2/src/cfnlint/template/getatts.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/template/template.py` & `cfn-lint-1.0.0a2/src/cfnlint/template/template.py`

 * *Files identical despite different names*

### Comparing `cfn-lint-1.0.0a1/src/cfnlint/transform.py` & `cfn-lint-1.0.0a2/src/cfnlint/transform.py`

 * *Files identical despite different names*

