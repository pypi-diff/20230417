# Comparing `tmp/smart_app_framework-2.0.1rc6-py3-none-any.whl.zip` & `tmp/smart_app_framework-2.0.1rc7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 297089 bytes, number of entries: 327
+Zip file size: 297101 bytes, number of entries: 327
 -rw-r--r--  2.0 unx      113 b- defN 80-Jan-01 00:00 core/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/actions/__init__.py
 -rw-r--r--  2.0 unx    10756 b- defN 80-Jan-01 00:00 core/basic_models/actions/basic_actions.py
 -rw-r--r--  2.0 unx     6265 b- defN 80-Jan-01 00:00 core/basic_models/actions/client_profile_actions.py
 -rw-r--r--  2.0 unx     1203 b- defN 80-Jan-01 00:00 core/basic_models/actions/command.py
 -rw-r--r--  2.0 unx     3083 b- defN 80-Jan-01 00:00 core/basic_models/actions/counter_actions.py
@@ -123,15 +123,15 @@
 -rw-r--r--  2.0 unx      486 b- defN 80-Jan-01 00:00 core/unified_template/pan2service.py
 -rw-r--r--  2.0 unx     3391 b- defN 80-Jan-01 00:00 core/unified_template/unified_template.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/utils/__init__.py
 -rw-r--r--  2.0 unx      690 b- defN 80-Jan-01 00:00 core/utils/delay_runner.py
 -rw-r--r--  2.0 unx     1885 b- defN 80-Jan-01 00:00 core/utils/exception_handlers.py
 -rw-r--r--  2.0 unx     1358 b- defN 80-Jan-01 00:00 core/utils/fallback.py
 -rw-r--r--  2.0 unx      344 b- defN 80-Jan-01 00:00 core/utils/loader.py
--rw-r--r--  2.0 unx     7321 b- defN 80-Jan-01 00:00 core/utils/masking_message.py
+-rw-r--r--  2.0 unx     7347 b- defN 80-Jan-01 00:00 core/utils/masking_message.py
 -rw-r--r--  2.0 unx     1568 b- defN 80-Jan-01 00:00 core/utils/memstats.py
 -rw-r--r--  2.0 unx    32149 b- defN 80-Jan-01 00:00 core/utils/period_determiner.py
 -rw-r--r--  2.0 unx      529 b- defN 80-Jan-01 00:00 core/utils/pickle_copy.py
 -rw-r--r--  2.0 unx     1640 b- defN 80-Jan-01 00:00 core/utils/rerunable.py
 -rw-r--r--  2.0 unx      241 b- defN 80-Jan-01 00:00 core/utils/singleton.py
 -rw-r--r--  2.0 unx      293 b- defN 80-Jan-01 00:00 core/utils/stats_timer.py
 -rw-r--r--  2.0 unx     3673 b- defN 80-Jan-01 00:00 core/utils/utils.py
@@ -319,11 +319,11 @@
 -rw-r--r--  2.0 unx      486 b- defN 80-Jan-01 00:00 smart_kit/utils/__init__.py
 -rw-r--r--  2.0 unx     1325 b- defN 80-Jan-01 00:00 smart_kit/utils/cache.py
 -rw-r--r--  2.0 unx     2899 b- defN 80-Jan-01 00:00 smart_kit/utils/diff.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/__init__.py
 -rw-r--r--  2.0 unx     1504 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/logger_formatter.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/monitoring.py
 -rw-r--r--  2.0 unx      320 b- defN 80-Jan-01 00:00 smart_kit/utils/picklable_mock.py
--rw-r--r--  2.0 unx    10442 b- defN 80-Jan-01 00:00 smart_app_framework-2.0.1rc6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.0.1rc6.dist-info/WHEEL
-?rw-r--r--  2.0 unx    31543 b- defN 16-Jan-01 00:00 smart_app_framework-2.0.1rc6.dist-info/RECORD
-327 files, 964964 bytes uncompressed, 245707 bytes compressed:  74.5%
+-rw-r--r--  2.0 unx    10391 b- defN 80-Jan-01 00:00 smart_app_framework-2.0.1rc7.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.0.1rc7.dist-info/WHEEL
+?rw-r--r--  2.0 unx    31543 b- defN 16-Jan-01 00:00 smart_app_framework-2.0.1rc7.dist-info/RECORD
+327 files, 964939 bytes uncompressed, 245719 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -966,17 +966,17 @@
 
 Filename: smart_kit/utils/monitoring.py
 Comment: 
 
 Filename: smart_kit/utils/picklable_mock.py
 Comment: 
 
-Filename: smart_app_framework-2.0.1rc6.dist-info/METADATA
+Filename: smart_app_framework-2.0.1rc7.dist-info/METADATA
 Comment: 
 
-Filename: smart_app_framework-2.0.1rc6.dist-info/WHEEL
+Filename: smart_app_framework-2.0.1rc7.dist-info/WHEEL
 Comment: 
 
-Filename: smart_app_framework-2.0.1rc6.dist-info/RECORD
+Filename: smart_app_framework-2.0.1rc7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## core/utils/masking_message.py

```diff
@@ -1,12 +1,14 @@
 from typing import Optional, Union, Match, Dict, List
 import re
 
 MASK = "***"
-DEFAULT_MASKING_FIELDS = {"token": 0, "access_token": 0, "refresh_token": 0, "epkId": 0, "profileId": 0}
+DEFAULT_MASKING_FIELDS = {
+    "token": 0, "access_token": 0, "refresh_token": 0, "epkId": 0, "profileId": 0, "searchResult": 0,
+}
 CARD_MASKING_FIELDS = ["message", "debug_info", "normalizedMessage", "incoming_text", "annotations", "inner_entities",
                        "preprocess_result", "original_message", "original_tokenized_elements"]
 
 card_regular = re.compile(r"(?:(\d{18})|(\d{16})|(?:\d{4} ){3}(\d{4})(\s?\d{2})?)")
 
 
 class Counter(object):
```

## Comparing `smart_app_framework-2.0.1rc6.dist-info/METADATA` & `smart_app_framework-2.0.1rc7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: smart-app-framework
-Version: 2.0.1rc6
+Version: 2.0.1rc7
 Summary: Python-фреймворк, который позволяет создавать смартапы для виртуальных ассистентов Салют.
 Author: Salute Developers
 Author-email: developer@sberdevices.ru
-Requires-Python: >=3.8.1,<3.11
+Requires-Python: >=3.8.1,<3.10
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Jinja2 (==3.0.3)
 Requires-Dist: PyYAML (==5.3)
 Requires-Dist: Twisted (==22.8.0)
 Requires-Dist: aiohttp (==3.7.4)
 Requires-Dist: aioredis (==2.0.0)
 Requires-Dist: boto (==2.49.0)
 Requires-Dist: confluent_kafka (==1.9.2)
@@ -41,15 +40,15 @@
 Requires-Dist: rusenttokenize (==0.0.5)
 Requires-Dist: scikit-learn (==1.1.2)
 Requires-Dist: setuptools (==62.3.2)
 Requires-Dist: tabulate (==0.9.0)
 Requires-Dist: tatsu (==5.6.1)
 Requires-Dist: tensorflow (==2.8.0) ; sys_platform == "darwin" and platform_machine == "x86_64"
 Requires-Dist: tensorflow (==2.8.0) ; sys_platform == "linux" and platform_machine == "x86_64"
-Requires-Dist: tensorflow-aarch64 (==2.8.0) ; sys_platform == "linux" and platform_machine == "aarch64"
+Requires-Dist: tensorflow-aarch64 (==2.8.4) ; sys_platform == "linux" and platform_machine == "aarch64"
 Requires-Dist: tensorflow-macos (==2.8.0) ; sys_platform == "darwin" and platform_machine == "arm64"
 Requires-Dist: timeout-decorator (==0.4.1)
 Requires-Dist: tqdm (==4.64.1)
 Description-Content-Type: text/markdown
 
 # SmartApp Framework
```

## Comparing `smart_app_framework-2.0.1rc6.dist-info/RECORD` & `smart_app_framework-2.0.1rc7.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 core/unified_template/pan2service.py,sha256=pCAGWHP4OeYUKRJz7GHYWleCx4nJYacciRbTZdCqy4s,486
 core/unified_template/unified_template.py,sha256=3o85TTdlvrWFPyzBrna-aEErk6JMJE6uSVBT73RcFkY,3391
 core/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/utils/delay_runner.py,sha256=6utD0P4mlmjn8k-gs5BvfrWFkHwUxg0uRA6SEUw9TEg,690
 core/utils/exception_handlers.py,sha256=PPWsUpsOjzpXl4veOnJ8zsnnR_sryUa3Yv1wAGJp3Ts,1885
 core/utils/fallback.py,sha256=W09Fe4gXp-brLRA-e-pPKF5K_4uTCH9aesfjp4gafjI,1358
 core/utils/loader.py,sha256=4qTkjNxGVC8x9db4bMGvPivZ5yqWUiywZ_pmqqZBHnc,344
-core/utils/masking_message.py,sha256=GLOY3RbbGkdouqTu6s76qc_Hvp7rBzyqFfVJHs7f-HA,7321
+core/utils/masking_message.py,sha256=nkqG9fSN_VfAZiQgkO5jMQeo4I5bPGnWj5abRsmHRwY,7347
 core/utils/memstats.py,sha256=zf_pkw2rcJHU9weNNAV6-ts2Ta8UWgXY-NjS8sylEsE,1568
 core/utils/period_determiner.py,sha256=LCzZMRbJ2oYJ8hrjbSeNaajsjUzz4DKvptT1UnJvgbA,32149
 core/utils/pickle_copy.py,sha256=GSnMppL1P2JIh0jGoJbOztFk1fT2IB3oM7PKKWY4A1M,529
 core/utils/rerunable.py,sha256=nODhE7kbNMEgbdem2_TYNkW-My4L9WYQdVw4nEJl3jY,1640
 core/utils/singleton.py,sha256=HHb_IUEKnjLUyIpm193WICjkIW9cthjiKbgFFPrhNg0,241
 core/utils/stats_timer.py,sha256=lr2NH97NVo5H3lHQfz98oQtpUyxFpW8TP1DkjJqCIzE,293
 core/utils/utils.py,sha256=Hc-7qqLulz6krDKRYhnyi3YsuWqdeadN4yb4vIVZB3I,3673
@@ -318,10 +318,10 @@
 smart_kit/utils/__init__.py,sha256=CpZK3Ygk7w6USZDlrTu1GNjNlqboIm-Za_6eoGTbWuQ,486
 smart_kit/utils/cache.py,sha256=Lut5HMkfoeiRwCCnZoSHw7srWYn3Y0fD-hUJWckDBf8,1325
 smart_kit/utils/diff.py,sha256=rUdzi6f8mtXacNL6HvVYVoOnXD_M3FEMHFsMhPo0YL0,2899
 smart_kit/utils/logger_writer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/logger_writer/logger_formatter.py,sha256=Xkum0YisA1jYcEh3MHIAfvJttmp3hwxnyhWK5UV12Pc,1504
 smart_kit/utils/monitoring.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/picklable_mock.py,sha256=PxrgnKue58GFpVZMBGIQq36LPnITFzfNA21euCbfViE,320
-smart_app_framework-2.0.1rc6.dist-info/METADATA,sha256=e_z1WVf-3nZrLLQlDxoyduFipnQZzZfcHs4M1h9uPng,10442
-smart_app_framework-2.0.1rc6.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-smart_app_framework-2.0.1rc6.dist-info/RECORD,,
+smart_app_framework-2.0.1rc7.dist-info/METADATA,sha256=mlAREpZkx8QJkET-98JXFNn80Yul_Fe_GG8tE5AiaG0,10391
+smart_app_framework-2.0.1rc7.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+smart_app_framework-2.0.1rc7.dist-info/RECORD,,
```

