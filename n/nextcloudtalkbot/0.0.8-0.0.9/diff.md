# Comparing `tmp/nextcloudtalkbot-0.0.8.tar.gz` & `tmp/nextcloudtalkbot-0.0.9.tar.gz`

## Comparing `nextcloudtalkbot-0.0.8.tar` & `nextcloudtalkbot-0.0.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/.readthedocs.yaml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/mkdocs.yml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/docs/FirstRunSetup.md
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/docs/NextcloudFileOperations.md
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/docs/NextcloudTalkExtractor.md
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/docs/NextcloudUser.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/docs/index.md
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/docs/requirements.txt
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/nextcloud_talk_bot/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/nextcloud_talk_bot/check_local_user_enviroment.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/nextcloud_talk_bot/constants.py
--rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/nextcloud_talk_bot/first_run_setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/nextcloud_talk_bot/headers.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/nextcloud_talk_bot/nextcloud_activities.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/nextcloud_talk_bot/nextcloud_file_operations.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/nextcloud_talk_bot/nextcloud_requests.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/nextcloud_talk_bot/nextcloud_talk_extractor.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/nextcloud_talk_bot/nextcloud_user.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/nextcloud_talk_bot/nextcloudtalkbot.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/nextcloud_talk_bot/permissions_map.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/nextcloud_talk_bot/read_data.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/nextcloud_talk_bot/send_message.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/nextcloud_talk_bot/translations.py
--rw-r--r--   0        0        0     4171 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/404.html
--rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/index.html
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/requirements.txt
--rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/search.html
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/sitemap.xml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/sitemap.xml.gz
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/FirstRunSetup/index.html
--rw-r--r--   0        0        0     7056 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/NextcloudFileOperations/index.html
--rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/NextcloudTalkExtractor/index.html
--rw-r--r--   0        0        0     7863 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/NextcloudUser/index.html
--rw-r--r--   0        0        0   129978 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/theme.css
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/theme_extra.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/img/favicon.ico
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/js/html5shiv.min.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/js/theme.js
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/js/theme_extra.js
--rw-r--r--   0        0        0    99805 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/search/lunr.js
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/search/main.js
--rw-r--r--   0        0        0    15361 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/search/search_index.json
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/site/search/worker.js
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/tests/test_encrypt_password
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/LICENSE
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/README.md
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/.readthedocs.yaml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/mkdocs.yml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/docs/FirstRunSetup.md
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/docs/NextcloudFileOperations.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/docs/NextcloudTalkExtractor.md
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/docs/NextcloudUser.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/docs/index.md
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/docs/requirements.txt
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/nextcloud_talk_bot/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/nextcloud_talk_bot/check_local_user_enviroment.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/nextcloud_talk_bot/constants.py
+-rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/nextcloud_talk_bot/first_run_setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/nextcloud_talk_bot/headers.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/nextcloud_talk_bot/nextcloud_activities.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/nextcloud_talk_bot/nextcloud_file_operations.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/nextcloud_talk_bot/nextcloud_requests.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/nextcloud_talk_bot/nextcloud_talk_extractor.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/nextcloud_talk_bot/nextcloud_user.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/nextcloud_talk_bot/nextcloudtalkbot.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/nextcloud_talk_bot/permissions_map.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/nextcloud_talk_bot/read_data.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/nextcloud_talk_bot/send_message.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/nextcloud_talk_bot/translations.py
+-rw-r--r--   0        0        0     4171 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/404.html
+-rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/index.html
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/requirements.txt
+-rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/search.html
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/sitemap.xml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/sitemap.xml.gz
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/FirstRunSetup/index.html
+-rw-r--r--   0        0        0     7056 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/NextcloudFileOperations/index.html
+-rw-r--r--   0        0        0     7915 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/NextcloudTalkExtractor/index.html
+-rw-r--r--   0        0        0     7863 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/NextcloudUser/index.html
+-rw-r--r--   0        0        0   129978 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/theme.css
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/theme_extra.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/img/favicon.ico
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/js/html5shiv.min.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/js/theme.js
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/js/theme_extra.js
+-rw-r--r--   0        0        0    99805 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/search/lunr.js
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/search/main.js
+-rw-r--r--   0        0        0    15361 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/search/search_index.json
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/site/search/worker.js
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/tests/test_encrypt_password
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/LICENSE
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/README.md
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 nextcloudtalkbot-0.0.9/PKG-INFO
```

### Comparing `nextcloudtalkbot-0.0.8/docs/FirstRunSetup.md` & `nextcloudtalkbot-0.0.9/docs/FirstRunSetup.md`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/docs/NextcloudFileOperations.md` & `nextcloudtalkbot-0.0.9/docs/NextcloudFileOperations.md`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/docs/NextcloudTalkExtractor.md` & `nextcloudtalkbot-0.0.9/docs/NextcloudTalkExtractor.md`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/docs/NextcloudUser.md` & `nextcloudtalkbot-0.0.9/docs/NextcloudUser.md`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/docs/requirements.txt` & `nextcloudtalkbot-0.0.9/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/nextcloud_talk_bot/check_local_user_enviroment.py` & `nextcloudtalkbot-0.0.9/nextcloud_talk_bot/check_local_user_enviroment.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/nextcloud_talk_bot/first_run_setup.py` & `nextcloudtalkbot-0.0.9/nextcloud_talk_bot/first_run_setup.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/nextcloud_talk_bot/headers.py` & `nextcloudtalkbot-0.0.9/nextcloud_talk_bot/headers.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/nextcloud_talk_bot/nextcloud_activities.py` & `nextcloudtalkbot-0.0.9/nextcloud_talk_bot/nextcloud_activities.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/nextcloud_talk_bot/nextcloud_file_operations.py` & `nextcloudtalkbot-0.0.9/nextcloud_talk_bot/nextcloud_file_operations.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/nextcloud_talk_bot/nextcloud_requests.py` & `nextcloudtalkbot-0.0.9/nextcloud_talk_bot/nextcloud_requests.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/nextcloud_talk_bot/nextcloud_talk_extractor.py` & `nextcloudtalkbot-0.0.9/nextcloud_talk_bot/nextcloud_talk_extractor.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/nextcloud_talk_bot/nextcloud_user.py` & `nextcloudtalkbot-0.0.9/nextcloud_talk_bot/nextcloud_user.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/nextcloud_talk_bot/read_data.py` & `nextcloudtalkbot-0.0.9/nextcloud_talk_bot/read_data.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/nextcloud_talk_bot/send_message.py` & `nextcloudtalkbot-0.0.9/nextcloud_talk_bot/send_message.py`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/404.html` & `nextcloudtalkbot-0.0.9/site/404.html`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/index.html` & `nextcloudtalkbot-0.0.9/site/index.html`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/requirements.txt` & `nextcloudtalkbot-0.0.9/site/requirements.txt`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/search.html` & `nextcloudtalkbot-0.0.9/site/search.html`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/sitemap.xml` & `nextcloudtalkbot-0.0.9/site/sitemap.xml`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/FirstRunSetup/index.html` & `nextcloudtalkbot-0.0.9/site/FirstRunSetup/index.html`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/NextcloudFileOperations/index.html` & `nextcloudtalkbot-0.0.9/site/NextcloudFileOperations/index.html`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/NextcloudTalkExtractor/index.html` & `nextcloudtalkbot-0.0.9/site/NextcloudTalkExtractor/index.html`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/NextcloudUser/index.html` & `nextcloudtalkbot-0.0.9/site/NextcloudUser/index.html`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/theme.css` & `nextcloudtalkbot-0.0.9/site/css/theme.css`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/theme_extra.css` & `nextcloudtalkbot-0.0.9/site/css/theme_extra.css`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/Roboto-Slab-Bold.woff` & `nextcloudtalkbot-0.0.9/site/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/Roboto-Slab-Bold.woff2` & `nextcloudtalkbot-0.0.9/site/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/Roboto-Slab-Regular.woff` & `nextcloudtalkbot-0.0.9/site/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/Roboto-Slab-Regular.woff2` & `nextcloudtalkbot-0.0.9/site/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/fontawesome-webfont.eot` & `nextcloudtalkbot-0.0.9/site/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/fontawesome-webfont.svg` & `nextcloudtalkbot-0.0.9/site/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/fontawesome-webfont.ttf` & `nextcloudtalkbot-0.0.9/site/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/fontawesome-webfont.woff` & `nextcloudtalkbot-0.0.9/site/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/fontawesome-webfont.woff2` & `nextcloudtalkbot-0.0.9/site/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/lato-bold-italic.woff` & `nextcloudtalkbot-0.0.9/site/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/lato-bold-italic.woff2` & `nextcloudtalkbot-0.0.9/site/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/lato-bold.woff` & `nextcloudtalkbot-0.0.9/site/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/lato-bold.woff2` & `nextcloudtalkbot-0.0.9/site/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/lato-normal-italic.woff` & `nextcloudtalkbot-0.0.9/site/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/lato-normal-italic.woff2` & `nextcloudtalkbot-0.0.9/site/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/lato-normal.woff` & `nextcloudtalkbot-0.0.9/site/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/css/fonts/lato-normal.woff2` & `nextcloudtalkbot-0.0.9/site/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/img/favicon.ico` & `nextcloudtalkbot-0.0.9/site/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/js/html5shiv.min.js` & `nextcloudtalkbot-0.0.9/site/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/js/jquery-3.6.0.min.js` & `nextcloudtalkbot-0.0.9/site/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/js/theme.js` & `nextcloudtalkbot-0.0.9/site/js/theme.js`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/search/lunr.js` & `nextcloudtalkbot-0.0.9/site/search/lunr.js`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/search/main.js` & `nextcloudtalkbot-0.0.9/site/search/main.js`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/search/search_index.json` & `nextcloudtalkbot-0.0.9/site/search/search_index.json`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/site/search/worker.js` & `nextcloudtalkbot-0.0.9/site/search/worker.js`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/tests/test_encrypt_password` & `nextcloudtalkbot-0.0.9/tests/test_encrypt_password`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/LICENSE` & `nextcloudtalkbot-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/README.md` & `nextcloudtalkbot-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nextcloudtalkbot-0.0.8/pyproject.toml` & `nextcloudtalkbot-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nextcloudtalkbot"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Massoud Ahmed", email="okko@okxo.de", homepage="https://okxo.de"},
 ]
 homepage = "https://okxo.de"
 description = "Python3 library for creating a Nextcloud Talk bot."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+dependencies = [
+    "cryptography",
+    "requests",
+]
+
 keywords = ["nextcloud", "nextcloud talk", "bot"]
 
 [project.urls]
 "Homepage" = "https://github.com/sowoi/nextcloud-talk-bot"
 "Bug Tracker" = "https://github.com/sowoi/nextcloud-talk-bot/issues"
 "Documentation" = "https://nextcloud-talk-bot.readthedocs.io"
```

### Comparing `nextcloudtalkbot-0.0.8/PKG-INFO` & `nextcloudtalkbot-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: nextcloudtalkbot
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python3 library for creating a Nextcloud Talk bot.
 Project-URL: Homepage, https://github.com/sowoi/nextcloud-talk-bot
 Project-URL: Bug Tracker, https://github.com/sowoi/nextcloud-talk-bot/issues
 Project-URL: Documentation, https://nextcloud-talk-bot.readthedocs.io
 Author-email: Massoud Ahmed <okko@okxo.de>
 License-File: LICENSE
 Keywords: bot,nextcloud,nextcloud talk
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: cryptography
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 ## Nextcloud Talk Bot
 
 *Not ready for production, yet.*
 
 Python3 library for creating a Nextcloud Talk bot.
```

