# Comparing `tmp/rucio-webui-1.9.5.tar.gz` & `tmp/rucio-webui-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rucio-webui-1.9.5.tar", last modified: Tue Jan 24 09:14:11 2017, max compression
+gzip compressed data, was "dist/rucio-webui-1.9.6.tar", last modified: Tue Feb  7 09:03:55 2017, max compression
```

## Comparing `rucio-webui-1.9.5.tar` & `rucio-webui-1.9.6.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:14:11.000000 rucio-webui-1.9.5/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:14:11.000000 rucio-webui-1.9.5/lib/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:14:11.000000 rucio-webui-1.9.5/lib/rucio/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:14:11.000000 rucio-webui-1.9.5/lib/rucio/web/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:14:11.000000 rucio-webui-1.9.5/lib/rucio/web/ui/
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:14:11.000000 rucio-webui-1.9.5/lib/rucio/web/ui/common/
--rwxr-xr-x   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/common/__init__.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     6732 2016-11-28 16:40:28.000000 rucio-webui-1.9.5/lib/rucio/web/ui/common/utils.py
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:14:11.000000 rucio-webui-1.9.5/lib/rucio/web/ui/media/
--rw-r--r--   0 barisits (51071) zp        (1307)    84798 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/media/error.jpg
--rw-r--r--   0 barisits (51071) zp        (1307)     1150 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/media/favicon.ico
--rw-r--r--   0 barisits (51071) zp        (1307)      753 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/media/get_info.png
--rw-r--r--   0 barisits (51071) zp        (1307)    19563 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/media/rucio_logo.png
--rw-r--r--   0 barisits (51071) zp        (1307)    32246 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/media/spinner.gif
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:14:11.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/
--rw-r--r--   0 barisits (51071) zp        (1307)     3731 2016-11-25 16:30:17.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/account_rse_usage.js
--rw-r--r--   0 barisits (51071) zp        (1307)    10930 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/account_usage.js
--rw-r--r--   0 barisits (51071) zp        (1307)     4998 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/accounting.js
--rw-r--r--   0 barisits (51071) zp        (1307)    11474 2016-11-28 16:40:28.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/approve_rules.js
--rw-r--r--   0 barisits (51071) zp        (1307)    15087 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/backlog_mon.js
--rw-r--r--   0 barisits (51071) zp        (1307)     1054 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/bad_replicas.js
--rw-r--r--   0 barisits (51071) zp        (1307)    10664 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/bad_replicas_summary.js
--rw-r--r--   0 barisits (51071) zp        (1307)     6117 2016-11-28 16:40:28.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/base.js
--rw-r--r--   0 barisits (51071) zp        (1307)    28400 2016-11-25 16:30:17.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/chosen.jquery.min.js
--rw-r--r--   0 barisits (51071) zp        (1307)    11060 2016-11-25 16:30:17.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/chosen.min.css
--rw-r--r--   0 barisits (51071) zp        (1307)     5653 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/cond.js
--rw-r--r--   0 barisits (51071) zp        (1307)     5770 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/dbrelease.js
--rw-r--r--   0 barisits (51071) zp        (1307)    17161 2016-11-28 16:40:28.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/did.js
--rw-r--r--   0 barisits (51071) zp        (1307)     1395 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/filesize.min.js
--rw-r--r--   0 barisits (51071) zp        (1307)    19508 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/foundation-icons.css
--rw-r--r--   0 barisits (51071) zp        (1307)    54568 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/foundation-icons.eot
--rw-r--r--   0 barisits (51071) zp        (1307)   150535 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/foundation-icons.svg
--rw-r--r--   0 barisits (51071) zp        (1307)    56976 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/foundation-icons.ttf
--rw-r--r--   0 barisits (51071) zp        (1307)    32020 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/foundation-icons.woff
--rw-r--r--   0 barisits (51071) zp        (1307)     1359 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/heartbeats.js
--rw-r--r--   0 barisits (51071) zp        (1307)     1138 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/http_api_usage.js
--rw-r--r--   0 barisits (51071) zp        (1307)      859 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring.css
--rw-r--r--   0 barisits (51071) zp        (1307)    12429 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_account_details.js
--rw-r--r--   0 barisits (51071) zp        (1307)     3537 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_accounts.js
--rw-r--r--   0 barisits (51071) zp        (1307)     5317 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js
--rw-r--r--   0 barisits (51071) zp        (1307)     3801 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_apiclasses.js
--rw-r--r--   0 barisits (51071) zp        (1307)     3555 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_index.js
--rw-r--r--   0 barisits (51071) zp        (1307)     3051 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_resources.js
--rw-r--r--   0 barisits (51071) zp        (1307)     8904 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js
--rw-r--r--   0 barisits (51071) zp        (1307)     3061 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_scriptids.js
--rw-r--r--   0 barisits (51071) zp        (1307)    10043 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_utils.js
--rw-r--r--   0 barisits (51071) zp        (1307)     2279 2016-11-25 16:30:17.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/index.js
--rw-r--r--   0 barisits (51071) zp        (1307)    23108 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/jquery.multiple.select.js
--rw-r--r--   0 barisits (51071) zp        (1307)     6966 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/jquery.storageapi.min.js
--rw-r--r--   0 barisits (51071) zp        (1307)    12443 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/list_rules.js
--rw-r--r--   0 barisits (51071) zp        (1307)     4282 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/multiple-select.css
--rw-r--r--   0 barisits (51071) zp        (1307)     3342 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/multiple-select.png
--rw-r--r--   0 barisits (51071) zp        (1307)    50060 2016-11-28 16:40:29.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/request_rule.js
--rw-r--r--   0 barisits (51071) zp        (1307)    21828 2016-11-28 16:40:29.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/rse_account_usage.js
--rw-r--r--   0 barisits (51071) zp        (1307)     6559 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/rse_locks.js
--rw-r--r--   0 barisits (51071) zp        (1307)    10434 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/rse_usage.js
--rw-r--r--   0 barisits (51071) zp        (1307)     2194 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/rucio.css
--rw-r--r--   0 barisits (51071) zp        (1307)    45503 2016-11-28 16:40:29.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/rucio.js
--rw-r--r--   0 barisits (51071) zp        (1307)    21237 2016-11-28 16:40:29.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/rule.js
--rw-r--r--   0 barisits (51071) zp        (1307)     1341 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/rules.js
--rw-r--r--   0 barisits (51071) zp        (1307)     6323 2016-11-25 16:30:17.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/search.js
--rw-r--r--   0 barisits (51071) zp        (1307)     7256 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/subscription.js
--rw-r--r--   0 barisits (51071) zp        (1307)     2994 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/subscriptionrules.js
--rw-r--r--   0 barisits (51071) zp        (1307)     5046 2016-11-28 16:40:29.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/subscriptions.js
--rw-r--r--   0 barisits (51071) zp        (1307)     1095 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/suspicious_replicas.js
--rw-r--r--   0 barisits (51071) zp        (1307)      599 2016-11-25 16:30:17.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/version.js
--rw-r--r--   0 barisits (51071) zp        (1307)        5 2017-01-24 09:14:09.000000 rucio-webui-1.9.5/lib/rucio/web/ui/static/webui_version
-drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-01-24 09:14:11.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/
--rw-r--r--   0 barisits (51071) zp        (1307)      885 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/account_rse_usage.html
--rw-r--r--   0 barisits (51071) zp        (1307)     1726 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/account_usage.html
--rw-r--r--   0 barisits (51071) zp        (1307)      749 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/accounting.html
--rw-r--r--   0 barisits (51071) zp        (1307)     3441 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/approve_rules.html
--rw-r--r--   0 barisits (51071) zp        (1307)     2786 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/backlog_mon.html
--rw-r--r--   0 barisits (51071) zp        (1307)     1053 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/bad_replicas.html
--rw-r--r--   0 barisits (51071) zp        (1307)     2187 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/bad_replicas_summary.html
--rw-r--r--   0 barisits (51071) zp        (1307)     8123 2016-11-25 16:30:17.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/base.html
--rw-r--r--   0 barisits (51071) zp        (1307)     2552 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/cond.html
--rw-r--r--   0 barisits (51071) zp        (1307)     2575 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/dbrelease.html
--rw-r--r--   0 barisits (51071) zp        (1307)     1162 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/did.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4050 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/dumps.html
--rw-r--r--   0 barisits (51071) zp        (1307)     1120 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/heartbeats.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5788 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_api_usage.html
--rw-r--r--   0 barisits (51071) zp        (1307)    10884 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_monitoring_account_details.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4121 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_monitoring_accounts.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4466 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_monitoring_apiclass_details.html
--rw-r--r--   0 barisits (51071) zp        (1307)     3483 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_monitoring_apiclasses.html
--rw-r--r--   0 barisits (51071) zp        (1307)     5181 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_monitoring_index.html
--rw-r--r--   0 barisits (51071) zp        (1307)     3461 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_monitoring_resources.html
--rw-r--r--   0 barisits (51071) zp        (1307)     7382 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_monitoring_scriptid_details.html
--rw-r--r--   0 barisits (51071) zp        (1307)     3453 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_monitoring_scriptids.html
--rw-r--r--   0 barisits (51071) zp        (1307)      509 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/index.html
--rw-r--r--   0 barisits (51071) zp        (1307)     1692 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/infrastructure.html
--rw-r--r--   0 barisits (51071) zp        (1307)     4042 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/list_rules.html
--rw-r--r--   0 barisits (51071) zp        (1307)      756 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/problem.html
--rw-r--r--   0 barisits (51071) zp        (1307)    15598 2016-11-25 16:30:17.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/request_rule.html
--rw-r--r--   0 barisits (51071) zp        (1307)     2284 2016-11-25 16:30:17.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/rse_account_usage.html
--rw-r--r--   0 barisits (51071) zp        (1307)     1436 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/rse_locks.html
--rw-r--r--   0 barisits (51071) zp        (1307)     1257 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/rse_usage.html
--rw-r--r--   0 barisits (51071) zp        (1307)     1237 2016-11-28 16:40:29.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/rule.html
--rw-r--r--   0 barisits (51071) zp        (1307)     1919 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/rules.html
--rw-r--r--   0 barisits (51071) zp        (1307)     2050 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/search.html
--rw-r--r--   0 barisits (51071) zp        (1307)      755 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/subscription.html
--rw-r--r--   0 barisits (51071) zp        (1307)      863 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/subscriptionrules.html
--rw-r--r--   0 barisits (51071) zp        (1307)     1462 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/subscriptions.html
--rw-r--r--   0 barisits (51071) zp        (1307)     1068 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/templates/suspicious_replicas.html
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/__init__.py
--rwxr-xr-x   0 barisits (51071) zp        (1307)     8920 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/ui/main.py
--rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/web/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)      337 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/__init__.py
--rw-r--r--   0 barisits (51071) zp        (1307)      249 2017-01-24 09:14:09.000000 rucio-webui-1.9.5/lib/rucio/vcsversion.py
--rw-r--r--   0 barisits (51071) zp        (1307)     1127 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/lib/rucio/version.py
--rw-r--r--   0 barisits (51071) zp        (1307)      541 2016-11-25 15:17:13.000000 rucio-webui-1.9.5/AUTHORS
--rw-r--r--   0 barisits (51071) zp        (1307)      273 2016-11-25 15:17:13.000000 rucio-webui-1.9.5/ChangeLog
--rw-r--r--   0 barisits (51071) zp        (1307)      274 2016-11-25 15:17:13.000000 rucio-webui-1.9.5/LICENSE
--rw-r--r--   0 barisits (51071) zp        (1307)      432 2017-01-24 09:14:08.000000 rucio-webui-1.9.5/MANIFEST.in
--rw-r--r--   0 barisits (51071) zp        (1307)      286 2017-01-24 09:14:08.000000 rucio-webui-1.9.5/README.rst
--rw-r--r--   0 barisits (51071) zp        (1307)     7396 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/pylintrc
--rw-r--r--   0 barisits (51071) zp        (1307)     1014 2016-11-25 15:17:14.000000 rucio-webui-1.9.5/setup.cfg
--rw-r--r--   0 barisits (51071) zp        (1307)     4124 2017-01-24 09:14:08.000000 rucio-webui-1.9.5/setup.py
--rw-r--r--   0 barisits (51071) zp        (1307)      751 2017-01-24 09:14:11.000000 rucio-webui-1.9.5/PKG-INFO
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:55.000000 rucio-webui-1.9.6/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:55.000000 rucio-webui-1.9.6/lib/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:55.000000 rucio-webui-1.9.6/lib/rucio/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:55.000000 rucio-webui-1.9.6/lib/rucio/web/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:55.000000 rucio-webui-1.9.6/lib/rucio/web/ui/
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:55.000000 rucio-webui-1.9.6/lib/rucio/web/ui/common/
+-rwxr-xr-x   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/common/__init__.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     6732 2016-11-28 16:40:28.000000 rucio-webui-1.9.6/lib/rucio/web/ui/common/utils.py
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:55.000000 rucio-webui-1.9.6/lib/rucio/web/ui/media/
+-rw-r--r--   0 barisits (51071) zp        (1307)    84798 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/media/error.jpg
+-rw-r--r--   0 barisits (51071) zp        (1307)     1150 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/media/favicon.ico
+-rw-r--r--   0 barisits (51071) zp        (1307)      753 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/media/get_info.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    19563 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/media/rucio_logo.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    32246 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/media/spinner.gif
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:55.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/
+-rw-r--r--   0 barisits (51071) zp        (1307)     3731 2016-11-25 16:30:17.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/account_rse_usage.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    10930 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/account_usage.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     4998 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/accounting.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    11474 2016-11-28 16:40:28.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/approve_rules.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    15087 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/backlog_mon.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     1054 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/bad_replicas.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    10664 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/bad_replicas_summary.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     6117 2016-11-28 16:40:28.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/base.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    28400 2016-11-25 16:30:17.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/chosen.jquery.min.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    11060 2016-11-25 16:30:17.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/chosen.min.css
+-rw-r--r--   0 barisits (51071) zp        (1307)     5653 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/cond.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     5770 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/dbrelease.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    17161 2016-11-28 16:40:28.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/did.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     1395 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/filesize.min.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    19508 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/foundation-icons.css
+-rw-r--r--   0 barisits (51071) zp        (1307)    54568 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/foundation-icons.eot
+-rw-r--r--   0 barisits (51071) zp        (1307)   150535 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/foundation-icons.svg
+-rw-r--r--   0 barisits (51071) zp        (1307)    56976 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/foundation-icons.ttf
+-rw-r--r--   0 barisits (51071) zp        (1307)    32020 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/foundation-icons.woff
+-rw-r--r--   0 barisits (51071) zp        (1307)     1359 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/heartbeats.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     1138 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/http_api_usage.js
+-rw-r--r--   0 barisits (51071) zp        (1307)      859 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring.css
+-rw-r--r--   0 barisits (51071) zp        (1307)    12429 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_account_details.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     3537 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_accounts.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     5317 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     3801 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_apiclasses.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     3555 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_index.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     3051 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_resources.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     8904 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     3061 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_scriptids.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    10043 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_utils.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     2279 2016-11-25 16:30:17.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/index.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    23108 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/jquery.multiple.select.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     6966 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/jquery.storageapi.min.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    12443 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/list_rules.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     4282 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/multiple-select.css
+-rw-r--r--   0 barisits (51071) zp        (1307)     3342 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/multiple-select.png
+-rw-r--r--   0 barisits (51071) zp        (1307)    50060 2016-11-28 16:40:29.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/request_rule.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    21828 2016-11-28 16:40:29.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/rse_account_usage.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     6559 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/rse_locks.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    10434 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/rse_usage.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     2194 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/rucio.css
+-rw-r--r--   0 barisits (51071) zp        (1307)    45503 2016-11-28 16:40:29.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/rucio.js
+-rw-r--r--   0 barisits (51071) zp        (1307)    21237 2016-11-28 16:40:29.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/rule.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     1341 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/rules.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     6323 2016-11-25 16:30:17.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/search.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     7256 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/subscription.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     2994 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/subscriptionrules.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     5046 2016-11-28 16:40:29.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/subscriptions.js
+-rw-r--r--   0 barisits (51071) zp        (1307)     1095 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/suspicious_replicas.js
+-rw-r--r--   0 barisits (51071) zp        (1307)      599 2016-11-25 16:30:17.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/version.js
+-rw-r--r--   0 barisits (51071) zp        (1307)        5 2017-02-07 09:03:52.000000 rucio-webui-1.9.6/lib/rucio/web/ui/static/webui_version
+drwxr-xr-x   0 barisits (51071) zp        (1307)        0 2017-02-07 09:03:55.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/
+-rw-r--r--   0 barisits (51071) zp        (1307)      885 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/account_rse_usage.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     1726 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/account_usage.html
+-rw-r--r--   0 barisits (51071) zp        (1307)      749 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/accounting.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     3441 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/approve_rules.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     2786 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/backlog_mon.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     1053 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/bad_replicas.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     2187 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/bad_replicas_summary.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     8123 2016-11-25 16:30:17.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/base.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     2552 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/cond.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     2575 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/dbrelease.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     1162 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/did.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4050 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/dumps.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     1120 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/heartbeats.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5788 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_api_usage.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    10884 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_monitoring_account_details.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4121 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_monitoring_accounts.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4466 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_monitoring_apiclass_details.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     3483 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_monitoring_apiclasses.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     5181 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_monitoring_index.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     3461 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_monitoring_resources.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     7382 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_monitoring_scriptid_details.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     3453 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_monitoring_scriptids.html
+-rw-r--r--   0 barisits (51071) zp        (1307)      509 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/index.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     1692 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/infrastructure.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     4042 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/list_rules.html
+-rw-r--r--   0 barisits (51071) zp        (1307)      756 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/problem.html
+-rw-r--r--   0 barisits (51071) zp        (1307)    15598 2016-11-25 16:30:17.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/request_rule.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     2284 2016-11-25 16:30:17.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/rse_account_usage.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     1436 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/rse_locks.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     1257 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/rse_usage.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     1237 2016-11-28 16:40:29.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/rule.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     1919 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/rules.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     2050 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/search.html
+-rw-r--r--   0 barisits (51071) zp        (1307)      755 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/subscription.html
+-rw-r--r--   0 barisits (51071) zp        (1307)      863 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/subscriptionrules.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     1462 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/subscriptions.html
+-rw-r--r--   0 barisits (51071) zp        (1307)     1068 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/templates/suspicious_replicas.html
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/__init__.py
+-rwxr-xr-x   0 barisits (51071) zp        (1307)     8920 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/ui/main.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      282 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/web/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      337 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/__init__.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      249 2017-02-07 09:03:52.000000 rucio-webui-1.9.6/lib/rucio/vcsversion.py
+-rw-r--r--   0 barisits (51071) zp        (1307)     1127 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/lib/rucio/version.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      541 2016-11-25 15:17:13.000000 rucio-webui-1.9.6/AUTHORS
+-rw-r--r--   0 barisits (51071) zp        (1307)      273 2016-11-25 15:17:13.000000 rucio-webui-1.9.6/ChangeLog
+-rw-r--r--   0 barisits (51071) zp        (1307)      274 2016-11-25 15:17:13.000000 rucio-webui-1.9.6/LICENSE
+-rw-r--r--   0 barisits (51071) zp        (1307)      432 2017-02-07 09:03:52.000000 rucio-webui-1.9.6/MANIFEST.in
+-rw-r--r--   0 barisits (51071) zp        (1307)      286 2017-02-07 09:03:52.000000 rucio-webui-1.9.6/README.rst
+-rw-r--r--   0 barisits (51071) zp        (1307)     7396 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/pylintrc
+-rw-r--r--   0 barisits (51071) zp        (1307)     1014 2016-11-25 15:17:14.000000 rucio-webui-1.9.6/setup.cfg
+-rw-r--r--   0 barisits (51071) zp        (1307)     4124 2017-02-07 09:03:52.000000 rucio-webui-1.9.6/setup.py
+-rw-r--r--   0 barisits (51071) zp        (1307)      751 2017-02-07 09:03:55.000000 rucio-webui-1.9.6/PKG-INFO
```

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/common/utils.py` & `rucio-webui-1.9.6/lib/rucio/web/ui/common/utils.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/media/error.jpg` & `rucio-webui-1.9.6/lib/rucio/web/ui/media/error.jpg`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/media/favicon.ico` & `rucio-webui-1.9.6/lib/rucio/web/ui/media/favicon.ico`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/media/get_info.png` & `rucio-webui-1.9.6/lib/rucio/web/ui/media/get_info.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/media/rucio_logo.png` & `rucio-webui-1.9.6/lib/rucio/web/ui/media/rucio_logo.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/media/spinner.gif` & `rucio-webui-1.9.6/lib/rucio/web/ui/media/spinner.gif`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/account_rse_usage.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/account_rse_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/account_usage.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/account_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/accounting.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/accounting.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/approve_rules.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/approve_rules.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/backlog_mon.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/backlog_mon.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/bad_replicas.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/bad_replicas.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/bad_replicas_summary.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/bad_replicas_summary.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/base.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/base.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/chosen.jquery.min.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/chosen.jquery.min.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/chosen.min.css` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/chosen.min.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/cond.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/cond.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/dbrelease.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/dbrelease.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/did.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/did.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/filesize.min.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/filesize.min.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/foundation-icons.css` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/foundation-icons.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/foundation-icons.eot` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/foundation-icons.eot`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/foundation-icons.svg` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/foundation-icons.svg`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/foundation-icons.ttf` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/foundation-icons.ttf`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/foundation-icons.woff` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/foundation-icons.woff`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/heartbeats.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/heartbeats.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/http_api_usage.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/http_api_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring.css` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_account_details.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_account_details.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_accounts.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_accounts.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_apiclass_details.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_apiclasses.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_apiclasses.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_index.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_index.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_resources.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_resources.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_scriptid_details.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_scriptids.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_scriptids.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/http_monitoring_utils.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/http_monitoring_utils.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/index.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/index.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/jquery.multiple.select.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/jquery.multiple.select.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/jquery.storageapi.min.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/jquery.storageapi.min.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/list_rules.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/list_rules.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/multiple-select.css` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/multiple-select.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/multiple-select.png` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/multiple-select.png`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/request_rule.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/request_rule.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/rse_account_usage.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/rse_account_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/rse_locks.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/rse_locks.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/rse_usage.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/rse_usage.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/rucio.css` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/rucio.css`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/rucio.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/rucio.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/rule.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/rule.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/rules.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/rules.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/search.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/search.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/subscription.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/subscription.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/subscriptionrules.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/subscriptionrules.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/subscriptions.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/subscriptions.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/suspicious_replicas.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/suspicious_replicas.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/static/version.js` & `rucio-webui-1.9.6/lib/rucio/web/ui/static/version.js`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/account_rse_usage.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/account_rse_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/account_usage.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/account_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/accounting.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/accounting.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/approve_rules.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/approve_rules.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/backlog_mon.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/backlog_mon.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/bad_replicas.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/bad_replicas.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/bad_replicas_summary.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/bad_replicas_summary.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/base.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/base.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/cond.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/cond.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/dbrelease.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/dbrelease.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/did.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/did.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/dumps.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/dumps.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/heartbeats.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/heartbeats.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_api_usage.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_api_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_monitoring_account_details.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_monitoring_account_details.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_monitoring_accounts.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_monitoring_accounts.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_monitoring_apiclass_details.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_monitoring_apiclass_details.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_monitoring_apiclasses.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_monitoring_apiclasses.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_monitoring_index.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_monitoring_index.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_monitoring_resources.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_monitoring_resources.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_monitoring_scriptid_details.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_monitoring_scriptid_details.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/http_monitoring_scriptids.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/http_monitoring_scriptids.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/infrastructure.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/infrastructure.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/list_rules.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/list_rules.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/problem.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/problem.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/request_rule.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/request_rule.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/rse_account_usage.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/rse_account_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/rse_locks.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/rse_locks.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/rse_usage.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/rse_usage.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/rule.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/rule.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/rules.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/rules.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/search.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/search.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/subscription.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/subscription.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/subscriptionrules.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/subscriptionrules.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/subscriptions.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/subscriptions.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/templates/suspicious_replicas.html` & `rucio-webui-1.9.6/lib/rucio/web/ui/templates/suspicious_replicas.html`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/web/ui/main.py` & `rucio-webui-1.9.6/lib/rucio/web/ui/main.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/lib/rucio/version.py` & `rucio-webui-1.9.6/lib/rucio/version.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/AUTHORS` & `rucio-webui-1.9.6/AUTHORS`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/pylintrc` & `rucio-webui-1.9.6/pylintrc`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/setup.cfg` & `rucio-webui-1.9.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/setup.py` & `rucio-webui-1.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `rucio-webui-1.9.5/PKG-INFO` & `rucio-webui-1.9.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rucio-webui
-Version: 1.9.5
+Version: 1.9.6
 Summary: Rucio WebUI Package
 Home-page: http://rucio.cern.ch/
 Author: Rucio
 Author-email: rucio-dev@cern.ch
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

