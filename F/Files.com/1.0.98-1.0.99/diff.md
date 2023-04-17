# Comparing `tmp/Files.com-1.0.98.tar.gz` & `tmp/Files.com-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Files.com-1.0.98.tar", last modified: Tue Mar  2 21:50:07 2021, max compression
+gzip compressed data, was "dist/Files.com-1.0.99.tar", last modified: Tue Mar  2 22:59:24 2021, max compression
```

## Comparing `Files.com-1.0.98.tar` & `Files.com-1.0.99.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-02 21:50:07.000000 Files.com-1.0.98/
--rw-r--r--   0 root         (0) root         (0)     4430 2021-03-02 21:49:53.000000 Files.com-1.0.98/README.md
--rw-r--r--   0 root         (0) root         (0)      233 2021-03-02 21:50:07.000000 Files.com-1.0.98/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      474 2021-03-02 21:49:53.000000 Files.com-1.0.98/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-02 21:50:07.000000 Files.com-1.0.98/Files.com.egg-info/
--rw-r--r--   0 root         (0) root         (0)       10 2021-03-02 21:50:07.000000 Files.com-1.0.98/Files.com.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       43 2021-03-02 21:50:07.000000 Files.com-1.0.98/Files.com.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      233 2021-03-02 21:50:07.000000 Files.com-1.0.98/Files.com.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2021-03-02 21:50:07.000000 Files.com-1.0.98/Files.com.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     2358 2021-03-02 21:50:07.000000 Files.com-1.0.98/Files.com.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-03-02 21:50:07.000000 Files.com-1.0.98/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-02 21:50:07.000000 Files.com-1.0.98/files_sdk/
--rw-r--r--   0 root         (0) root         (0)     7398 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1482 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/api.py
--rw-r--r--   0 root         (0) root         (0)     9286 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/api_client.py
--rw-r--r--   0 root         (0) root         (0)     1136 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/list_obj.py
--rw-r--r--   0 root         (0) root         (0)      957 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/util.py
--rw-r--r--   0 root         (0) root         (0)     1409 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-02 21:50:07.000000 Files.com-1.0.98/files_sdk/models/
--rw-r--r--   0 root         (0) root         (0)     9685 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/message.py
--rw-r--r--   0 root         (0) root         (0)     3300 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1854 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/action.py
--rw-r--r--   0 root         (0) root         (0)     6957 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/project.py
--rw-r--r--   0 root         (0) root         (0)     5740 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/folder.py
--rw-r--r--   0 root         (0) root         (0)     2343 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/file_upload_part.py
--rw-r--r--   0 root         (0) root         (0)     1007 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/errors.py
--rw-r--r--   0 root         (0) root         (0)     1481 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/bundle_registration.py
--rw-r--r--   0 root         (0) root         (0)     3086 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/ip_address.py
--rw-r--r--   0 root         (0) root         (0)    14374 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/history.py
--rw-r--r--   0 root         (0) root         (0)     5597 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/user_request.py
--rw-r--r--   0 root         (0) root         (0)     1288 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/preview.py
--rw-r--r--   0 root         (0) root         (0)    36698 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/remote_server.py
--rw-r--r--   0 root         (0) root         (0)     5877 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/message_reaction.py
--rw-r--r--   0 root         (0) root         (0)     1244 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/payment_line_item.py
--rw-r--r--   0 root         (0) root         (0)      898 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/auto.py
--rw-r--r--   0 root         (0) root         (0)     2104 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/dns_record.py
--rw-r--r--   0 root         (0) root         (0)    42376 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/user.py
--rw-r--r--   0 root         (0) root         (0)    13193 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     1359 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/inbox_registration.py
--rw-r--r--   0 root         (0) root         (0)    10978 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/group.py
--rw-r--r--   0 root         (0) root         (0)     8701 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/permission.py
--rw-r--r--   0 root         (0) root         (0)     5123 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/app.py
--rw-r--r--   0 root         (0) root         (0)    19449 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/file.py
--rw-r--r--   0 root         (0) root         (0)     1269 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/status.py
--rw-r--r--   0 root         (0) root         (0)     2641 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/bundle_download.py
--rw-r--r--   0 root         (0) root         (0)     7427 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/bundle_recipient.py
--rw-r--r--   0 root         (0) root         (0)     7716 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/message_comment.py
--rw-r--r--   0 root         (0) root         (0)      958 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/image.py
--rw-r--r--   0 root         (0) root         (0)    21873 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/automation.py
--rw-r--r--   0 root         (0) root         (0)     1047 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/public_ip_address.py
--rw-r--r--   0 root         (0) root         (0)     5554 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/history_export_result.py
--rw-r--r--   0 root         (0) root         (0)     2985 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/usage_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     3557 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/invoice.py
--rw-r--r--   0 root         (0) root         (0)    20360 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/bundle.py
--rw-r--r--   0 root         (0) root         (0)     1882 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/account_line_item.py
--rw-r--r--   0 root         (0) root         (0)     3557 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/payment.py
--rw-r--r--   0 root         (0) root         (0)     8158 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/request.py
--rw-r--r--   0 root         (0) root         (0)     6611 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/sso_strategy.py
--rw-r--r--   0 root         (0) root         (0)    13384 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/history_export.py
--rw-r--r--   0 root         (0) root         (0)     7736 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/form_field_set.py
--rw-r--r--   0 root         (0) root         (0)    30227 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/site.py
--rw-r--r--   0 root         (0) root         (0)     7399 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/inbox_recipient.py
--rw-r--r--   0 root         (0) root         (0)     4329 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/settings_change.py
--rw-r--r--   0 root         (0) root         (0)     4670 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/external_event.py
--rw-r--r--   0 root         (0) root         (0)     4449 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/usage_daily_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4911 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/bandwidth_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     5786 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/lock.py
--rw-r--r--   0 root         (0) root         (0)    10487 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/clickwrap.py
--rw-r--r--   0 root         (0) root         (0)     5771 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/session.py
--rw-r--r--   0 root         (0) root         (0)     4131 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/file_comment_reaction.py
--rw-r--r--   0 root         (0) root         (0)    15591 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/api_key.py
--rw-r--r--   0 root         (0) root         (0)     2657 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/user_cipher_use.py
--rw-r--r--   0 root         (0) root         (0)    16874 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/behavior.py
--rw-r--r--   0 root         (0) root         (0)     8059 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/group_user.py
--rw-r--r--   0 root         (0) root         (0)     7832 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/public_key.py
--rw-r--r--   0 root         (0) root         (0)     6037 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/message_comment_reaction.py
--rw-r--r--   0 root         (0) root         (0)     8052 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/as2_key.py
--rw-r--r--   0 root         (0) root         (0)     1547 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/invoice_line_item.py
--rw-r--r--   0 root         (0) root         (0)     6648 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/file_comment.py
--rw-r--r--   0 root         (0) root         (0)     1426 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/form_field.py
--rw-r--r--   0 root         (0) root         (0)     2525 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/inbox_upload.py
--rw-r--r--   0 root         (0) root         (0)     4971 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/style.py
--rw-r--r--   0 root         (0) root         (0)     8649 2021-03-02 21:49:53.000000 Files.com-1.0.98/files_sdk/models/file_action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-02 22:59:24.000000 Files.com-1.0.99/
+-rw-r--r--   0 root         (0) root         (0)     4430 2021-03-02 22:59:09.000000 Files.com-1.0.99/README.md
+-rw-r--r--   0 root         (0) root         (0)      233 2021-03-02 22:59:24.000000 Files.com-1.0.99/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      474 2021-03-02 22:59:09.000000 Files.com-1.0.99/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-02 22:59:24.000000 Files.com-1.0.99/Files.com.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       10 2021-03-02 22:59:24.000000 Files.com-1.0.99/Files.com.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2021-03-02 22:59:24.000000 Files.com-1.0.99/Files.com.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      233 2021-03-02 22:59:24.000000 Files.com-1.0.99/Files.com.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2021-03-02 22:59:24.000000 Files.com-1.0.99/Files.com.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     2358 2021-03-02 22:59:24.000000 Files.com-1.0.99/Files.com.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-03-02 22:59:24.000000 Files.com-1.0.99/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-02 22:59:24.000000 Files.com-1.0.99/files_sdk/
+-rw-r--r--   0 root         (0) root         (0)     7398 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/api.py
+-rw-r--r--   0 root         (0) root         (0)     9286 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/api_client.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/list_obj.py
+-rw-r--r--   0 root         (0) root         (0)      957 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/util.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-03-02 22:59:24.000000 Files.com-1.0.99/files_sdk/models/
+-rw-r--r--   0 root         (0) root         (0)     9685 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/message.py
+-rw-r--r--   0 root         (0) root         (0)     3300 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/action.py
+-rw-r--r--   0 root         (0) root         (0)     6957 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/project.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/folder.py
+-rw-r--r--   0 root         (0) root         (0)     2343 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/file_upload_part.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1481 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/bundle_registration.py
+-rw-r--r--   0 root         (0) root         (0)     3086 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/ip_address.py
+-rw-r--r--   0 root         (0) root         (0)    14374 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/history.py
+-rw-r--r--   0 root         (0) root         (0)     5597 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1288 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/preview.py
+-rw-r--r--   0 root         (0) root         (0)    36698 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/remote_server.py
+-rw-r--r--   0 root         (0) root         (0)     5877 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/message_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     1244 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/payment_line_item.py
+-rw-r--r--   0 root         (0) root         (0)      898 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/auto.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/dns_record.py
+-rw-r--r--   0 root         (0) root         (0)    42376 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/user.py
+-rw-r--r--   0 root         (0) root         (0)    13193 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/inbox_registration.py
+-rw-r--r--   0 root         (0) root         (0)    10978 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/group.py
+-rw-r--r--   0 root         (0) root         (0)     8701 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/permission.py
+-rw-r--r--   0 root         (0) root         (0)     5123 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/app.py
+-rw-r--r--   0 root         (0) root         (0)    19449 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/file.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/status.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/bundle_download.py
+-rw-r--r--   0 root         (0) root         (0)     7427 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/bundle_recipient.py
+-rw-r--r--   0 root         (0) root         (0)     7716 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/message_comment.py
+-rw-r--r--   0 root         (0) root         (0)      958 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/image.py
+-rw-r--r--   0 root         (0) root         (0)    21873 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/automation.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/public_ip_address.py
+-rw-r--r--   0 root         (0) root         (0)     5554 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/history_export_result.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/usage_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     3557 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/invoice.py
+-rw-r--r--   0 root         (0) root         (0)    20360 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/bundle.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/account_line_item.py
+-rw-r--r--   0 root         (0) root         (0)     3557 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/payment.py
+-rw-r--r--   0 root         (0) root         (0)     8158 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/request.py
+-rw-r--r--   0 root         (0) root         (0)     6611 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/sso_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    13384 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/history_export.py
+-rw-r--r--   0 root         (0) root         (0)     7736 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/form_field_set.py
+-rw-r--r--   0 root         (0) root         (0)    30227 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/site.py
+-rw-r--r--   0 root         (0) root         (0)     7399 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/inbox_recipient.py
+-rw-r--r--   0 root         (0) root         (0)     4329 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/settings_change.py
+-rw-r--r--   0 root         (0) root         (0)     4670 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/external_event.py
+-rw-r--r--   0 root         (0) root         (0)     4449 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/usage_daily_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4911 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/bandwidth_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     5786 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/lock.py
+-rw-r--r--   0 root         (0) root         (0)    10487 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/clickwrap.py
+-rw-r--r--   0 root         (0) root         (0)     5771 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/session.py
+-rw-r--r--   0 root         (0) root         (0)     4131 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/file_comment_reaction.py
+-rw-r--r--   0 root         (0) root         (0)    15591 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/api_key.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/user_cipher_use.py
+-rw-r--r--   0 root         (0) root         (0)    16874 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/behavior.py
+-rw-r--r--   0 root         (0) root         (0)     8059 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/group_user.py
+-rw-r--r--   0 root         (0) root         (0)     7832 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/public_key.py
+-rw-r--r--   0 root         (0) root         (0)     6037 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/message_comment_reaction.py
+-rw-r--r--   0 root         (0) root         (0)     8052 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/as2_key.py
+-rw-r--r--   0 root         (0) root         (0)     1547 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/invoice_line_item.py
+-rw-r--r--   0 root         (0) root         (0)     6648 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/file_comment.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/form_field.py
+-rw-r--r--   0 root         (0) root         (0)     2525 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/inbox_upload.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/style.py
+-rw-r--r--   0 root         (0) root         (0)     8649 2021-03-02 22:59:09.000000 Files.com-1.0.99/files_sdk/models/file_action.py
```

### Comparing `Files.com-1.0.98/README.md` & `Files.com-1.0.99/README.md`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/Files.com.egg-info/SOURCES.txt` & `Files.com-1.0.99/Files.com.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/__init__.py` & `Files.com-1.0.99/files_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/api.py` & `Files.com-1.0.99/files_sdk/api.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/api_client.py` & `Files.com-1.0.99/files_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/list_obj.py` & `Files.com-1.0.99/files_sdk/list_obj.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/util.py` & `Files.com-1.0.99/files_sdk/util.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/exceptions.py` & `Files.com-1.0.99/files_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/message.py` & `Files.com-1.0.99/files_sdk/models/message.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/__init__.py` & `Files.com-1.0.99/files_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/action.py` & `Files.com-1.0.99/files_sdk/models/action.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/project.py` & `Files.com-1.0.99/files_sdk/models/project.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/folder.py` & `Files.com-1.0.99/files_sdk/models/folder.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/file_upload_part.py` & `Files.com-1.0.99/files_sdk/models/file_upload_part.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/errors.py` & `Files.com-1.0.99/files_sdk/models/errors.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/bundle_registration.py` & `Files.com-1.0.99/files_sdk/models/bundle_registration.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/ip_address.py` & `Files.com-1.0.99/files_sdk/models/ip_address.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/history.py` & `Files.com-1.0.99/files_sdk/models/history.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/user_request.py` & `Files.com-1.0.99/files_sdk/models/user_request.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/preview.py` & `Files.com-1.0.99/files_sdk/models/preview.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/remote_server.py` & `Files.com-1.0.99/files_sdk/models/remote_server.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/message_reaction.py` & `Files.com-1.0.99/files_sdk/models/message_reaction.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/payment_line_item.py` & `Files.com-1.0.99/files_sdk/models/payment_line_item.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/auto.py` & `Files.com-1.0.99/files_sdk/models/auto.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/dns_record.py` & `Files.com-1.0.99/files_sdk/models/dns_record.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/user.py` & `Files.com-1.0.99/files_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/notification.py` & `Files.com-1.0.99/files_sdk/models/notification.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/inbox_registration.py` & `Files.com-1.0.99/files_sdk/models/inbox_registration.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/group.py` & `Files.com-1.0.99/files_sdk/models/group.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/permission.py` & `Files.com-1.0.99/files_sdk/models/permission.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/app.py` & `Files.com-1.0.99/files_sdk/models/app.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/file.py` & `Files.com-1.0.99/files_sdk/models/file.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/status.py` & `Files.com-1.0.99/files_sdk/models/status.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/bundle_download.py` & `Files.com-1.0.99/files_sdk/models/bundle_download.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/bundle_recipient.py` & `Files.com-1.0.99/files_sdk/models/bundle_recipient.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/message_comment.py` & `Files.com-1.0.99/files_sdk/models/message_comment.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/image.py` & `Files.com-1.0.99/files_sdk/models/image.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/automation.py` & `Files.com-1.0.99/files_sdk/models/automation.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/public_ip_address.py` & `Files.com-1.0.99/files_sdk/models/public_ip_address.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/history_export_result.py` & `Files.com-1.0.99/files_sdk/models/history_export_result.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/usage_snapshot.py` & `Files.com-1.0.99/files_sdk/models/usage_snapshot.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/invoice.py` & `Files.com-1.0.99/files_sdk/models/invoice.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/bundle.py` & `Files.com-1.0.99/files_sdk/models/bundle.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/account_line_item.py` & `Files.com-1.0.99/files_sdk/models/account_line_item.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/payment.py` & `Files.com-1.0.99/files_sdk/models/payment.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/request.py` & `Files.com-1.0.99/files_sdk/models/request.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/sso_strategy.py` & `Files.com-1.0.99/files_sdk/models/sso_strategy.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/history_export.py` & `Files.com-1.0.99/files_sdk/models/history_export.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/form_field_set.py` & `Files.com-1.0.99/files_sdk/models/form_field_set.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/site.py` & `Files.com-1.0.99/files_sdk/models/site.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/inbox_recipient.py` & `Files.com-1.0.99/files_sdk/models/inbox_recipient.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/settings_change.py` & `Files.com-1.0.99/files_sdk/models/settings_change.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/external_event.py` & `Files.com-1.0.99/files_sdk/models/external_event.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/usage_daily_snapshot.py` & `Files.com-1.0.99/files_sdk/models/usage_daily_snapshot.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/bandwidth_snapshot.py` & `Files.com-1.0.99/files_sdk/models/bandwidth_snapshot.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/lock.py` & `Files.com-1.0.99/files_sdk/models/lock.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/clickwrap.py` & `Files.com-1.0.99/files_sdk/models/clickwrap.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/session.py` & `Files.com-1.0.99/files_sdk/models/session.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/file_comment_reaction.py` & `Files.com-1.0.99/files_sdk/models/file_comment_reaction.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/api_key.py` & `Files.com-1.0.99/files_sdk/models/api_key.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/user_cipher_use.py` & `Files.com-1.0.99/files_sdk/models/user_cipher_use.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/behavior.py` & `Files.com-1.0.99/files_sdk/models/behavior.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/group_user.py` & `Files.com-1.0.99/files_sdk/models/group_user.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/public_key.py` & `Files.com-1.0.99/files_sdk/models/public_key.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/message_comment_reaction.py` & `Files.com-1.0.99/files_sdk/models/message_comment_reaction.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/as2_key.py` & `Files.com-1.0.99/files_sdk/models/as2_key.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/invoice_line_item.py` & `Files.com-1.0.99/files_sdk/models/invoice_line_item.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/file_comment.py` & `Files.com-1.0.99/files_sdk/models/file_comment.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/form_field.py` & `Files.com-1.0.99/files_sdk/models/form_field.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/inbox_upload.py` & `Files.com-1.0.99/files_sdk/models/inbox_upload.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/style.py` & `Files.com-1.0.99/files_sdk/models/style.py`

 * *Files identical despite different names*

### Comparing `Files.com-1.0.98/files_sdk/models/file_action.py` & `Files.com-1.0.99/files_sdk/models/file_action.py`

 * *Files identical despite different names*

