# Comparing `tmp/feedcrawler-18.0.4.tar.gz` & `tmp/feedcrawler-18.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedcrawler-18.0.4.tar", last modified: Sun Apr 16 13:23:50 2023, max compression
+gzip compressed data, was "feedcrawler-18.0.5.tar", last modified: Mon Apr 17 19:30:00 2023, max compression
```

## Comparing `feedcrawler-18.0.4.tar` & `feedcrawler-18.0.5.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.439161 feedcrawler-18.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-16 13:23:50.439161 feedcrawler-18.0.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7047 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.423161 feedcrawler-18.0.4/feedcrawler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.427161 feedcrawler-18.0.4/feedcrawler/external_sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.427161 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/content_all.py
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/content_shows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.427161 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_dw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_ff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_nk.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_nx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_ww.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.427161 feedcrawler-18.0.4/feedcrawler/external_sites/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/metadata/imdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.427161 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/content_all.py
--rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/content_shows.py
--rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.427161 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_dw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_nk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_nx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.431161 feedcrawler-18.0.4/feedcrawler/external_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42357 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_tools/myjd_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_tools/ombi_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_tools/overseerr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_tools/plex_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.431161 feedcrawler-18.0.4/feedcrawler/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/jobs/feed_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/jobs/package_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.431161 feedcrawler-18.0.4/feedcrawler/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20929 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.431161 feedcrawler-18.0.4/feedcrawler/providers/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/http_requests/cache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/http_requests/cloudflare_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/http_requests/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    44206 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/myjd_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/url_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.431161 feedcrawler-18.0.4/feedcrawler/web_interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/web_interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.423161 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.431161 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.435161 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    82113 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js
--rw-r--r--   0 runner    (1001) docker     (123)    20729 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js
--rw-r--r--   0 runner    (1001) docker     (123)    63885 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js
--rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js
--rw-r--r--   0 runner    (1001) docker     (123)    60695 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js
--rw-r--r--   0 runner    (1001) docker     (123)   194314 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css
--rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
--rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    79982 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css
--rw-r--r--   0 runner    (1001) docker     (123)   144763 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-44ade789.js
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js
--rw-r--r--   0 runner    (1001) docker     (123)    50726 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js
--rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js
--rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    82905 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/web_interface/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.423161 feedcrawler-18.0.4/feedcrawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-16 13:23:50.000000 feedcrawler-18.0.4/feedcrawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-16 13:23:50.000000 feedcrawler-18.0.4/feedcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:23:50.000000 feedcrawler-18.0.4/feedcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-16 13:23:50.000000 feedcrawler-18.0.4/feedcrawler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:23:50.000000 feedcrawler-18.0.4/feedcrawler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-16 13:23:50.000000 feedcrawler-18.0.4/feedcrawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 13:23:50.000000 feedcrawler-18.0.4/feedcrawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 13:23:50.439161 feedcrawler-18.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.604563 feedcrawler-18.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-17 19:30:00.604563 feedcrawler-18.0.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7047 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.596563 feedcrawler-18.0.5/feedcrawler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.596563 feedcrawler-18.0.5/feedcrawler/external_sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.596563 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/content_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20326 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/content_shows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.596563 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_ff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_nk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_nx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_ww.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.596563 feedcrawler-18.0.5/feedcrawler/external_sites/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/metadata/imdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.596563 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/content_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/content_shows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.600563 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_nk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_nx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.600563 feedcrawler-18.0.5/feedcrawler/external_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42357 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_tools/myjd_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_tools/ombi_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_tools/overseerr_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/external_tools/plex_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.600563 feedcrawler-18.0.5/feedcrawler/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/jobs/feed_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20733 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/jobs/package_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.600563 feedcrawler-18.0.5/feedcrawler/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20929 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.600563 feedcrawler-18.0.5/feedcrawler/providers/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/http_requests/cache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/http_requests/cloudflare_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/http_requests/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44206 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/myjd_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/url_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/providers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.600563 feedcrawler-18.0.5/feedcrawler/web_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/web_interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.596563 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.600563 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.604563 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    82113 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20729 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    63885 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js
+-rw-r--r--   0 runner    (1001) docker     (123)    60695 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   194314 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css
+-rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    79982 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css
+-rw-r--r--   0 runner    (1001) docker     (123)   144900 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-ffd92ad0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js
+-rw-r--r--   0 runner    (1001) docker     (123)    50726 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-04-17 19:29:59.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    82956 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/feedcrawler/web_interface/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 19:30:00.596563 feedcrawler-18.0.5/feedcrawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-17 19:30:00.000000 feedcrawler-18.0.5/feedcrawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 19:30:00.604563 feedcrawler-18.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-17 19:29:38.000000 feedcrawler-18.0.5/setup.py
```

### Comparing `feedcrawler-18.0.4/LICENSE.md` & `feedcrawler-18.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/PKG-INFO` & `feedcrawler-18.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedcrawler
-Version: 18.0.4
+Version: 18.0.5
 Summary: Automate downloads using predefined sites and the My JDownloader API
 Home-page: https://github.com/rix1337/FeedCrawler
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `feedcrawler-18.0.4/README.md` & `feedcrawler-18.0.5/README.md`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/crawler.py` & `feedcrawler-18.0.5/feedcrawler/crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 version = "v." + version.get_version()
 
 
 def start_feedcrawler():
     with multiprocessing.Manager() as manager:
         shared_state_dict = manager.dict()
-        shared_state.set_shared_dict(shared_state_dict)
+        shared_state_lock = manager.Lock()
+        shared_state.set_state(shared_state_dict, shared_state_lock)
 
         if gui.enabled:
             window = gui.create_main_window()
             sys.stdout = gui.PrintToConsoleAndGui(window)
         else:
             window = False
             sys.stdout = Unbuffered(sys.stdout)
@@ -70,15 +71,15 @@
         shared_state.set_files(config_path)
 
         print('Nutze das Verzeichnis "' + config_path + '" für Einstellungen/Logs')
 
         log_level = logging.__dict__[
             arguments.log_level] if arguments.log_level in logging.__dict__ else logging.INFO
 
-        shared_state.set_log_level(log_level)
+        shared_state.update("log_level", log_level)
         shared_state.set_logger()
 
         hostnames = CrawlerConfig('Hostnames')
 
         def clean_up_hostname(host, string):
             if string and '/' in string:
                 string = string.replace('https://', '').replace('http://', '')
@@ -188,31 +189,33 @@
         remove_redundant_db_tables(shared_state.values["dbfile"])
 
         if arguments.keep_cdc:
             print("CDC-Tabelle nicht geleert!")
         else:
             FeedDb('cdc').reset()
 
-        process_web_server = multiprocessing.Process(target=web_server, args=(shared_state_dict,))
+        process_web_server = multiprocessing.Process(target=web_server, args=(shared_state_dict, shared_state_lock,))
         process_web_server.start()
 
         if arguments.delay:
             delay = int(arguments.delay)
             print("Verzögere den ersten Suchlauf um " + str(delay) + " Sekunden")
             time.sleep(delay)
 
         if not shared_state.values["test_run"]:
-            process_feed_crawler = multiprocessing.Process(target=feed_crawler, args=(shared_state_dict,))
+            process_feed_crawler = multiprocessing.Process(target=feed_crawler,
+                                                           args=(shared_state_dict, shared_state_lock,))
             process_feed_crawler.start()
 
-            process_watch_packages = multiprocessing.Process(target=watch_packages, args=(shared_state_dict,))
+            process_watch_packages = multiprocessing.Process(target=watch_packages,
+                                                             args=(shared_state_dict, shared_state_lock,))
             process_watch_packages.start()
 
             if not arguments.docker and gui.enabled:
-                gui.main_gui(window, shared_state_dict)
+                gui.main_gui(window, shared_state_dict, shared_state_lock)
 
                 sys.stdout = sys.__stdout__
                 process_web_server.terminate()
                 process_feed_crawler.terminate()
                 process_watch_packages.terminate()
                 sys.exit(0)
 
@@ -228,14 +231,14 @@
                 try:
                     while True:
                         signal.pause()
                 except AttributeError:
                     while True:
                         time.sleep(1)
         else:
-            feed_crawler(shared_state_dict)
+            feed_crawler(shared_state_dict, shared_state_lock)
             process_web_server.terminate()
             sys.exit(0)
 
 
 if __name__ == "__main__":
     start_feedcrawler()
```

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/content_all.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/content_all.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/content_shows.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/content_shows.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
             first_post = feed.entries[0]
             concat = first_post.title + first_post.published + str(self.settings) + str(self.pattern)
             sha = hashlib.sha256(concat.encode(
                 'ascii', 'ignore')).hexdigest()
         else:
             if self._SITE == "SF" and not shared_state.values["sf_blocked"]:
                 print("SF hat den Feed-Anruf während der Feed-Suche blockiert.")
-                shared_state.values["sf_blocked"] = True
+                shared_state.update("sf_blocked", True)
             else:
                 shared_state.logger.debug("Feed ist leer - breche die Suche für diesen Feed ab!")
 
         if feed:
             for post in feed.entries:
                 concat = post.title + post.published + \
                          str(self.settings) + str(self.pattern)
```

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/shared.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/shared.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_by.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_by.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_dw.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_dw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_ff.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_ff.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_fx.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_fx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_hw.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_hw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_nk.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_nk.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_nx.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_nx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_ww.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_all_ww.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         data = payload[2]
         headers["Referer"] = referer
         response = post_url_headers(url, headers, data)
         if not response["text"] or response["status_code"] is not (200 or 304) or not '<span class="main-rls">' in \
                                                                                       response["text"]:
             if not shared_state.values["ww_blocked"]:
                 print("WW hat den Feed-Anruf während der Feed-Suche blockiert.")
-                shared_state.values["ww_blocked"] = True
+                shared_state.update("ww_blocked", True)
             return ""
         return response
     except:
         return ""
 
 
 def ww_get_download_links(self, content, title):
@@ -117,15 +117,15 @@
     download_links = []
     try:
         response = get_url(content)
         if not response or "NinjaFirewall 429" in response:
             if not shared_state.values["ww_blocked"]:
                 print(
                     "WW hat den Link-Abruf für " + title + " blockiert. Eine spätere Anfrage hat möglicherweise Erfolg!")
-                shared_state.values["ww_blocked"] = True
+                shared_state.update("ww_blocked", True)
             return False
         links = BeautifulSoup(response, "html.parser").findAll("div", {"id": "download-links"})
         for link in links:
             hoster = link.text
             if 'Direct Download 100 MBit/s' not in hoster:
                 url = base_url + link.find("a")["href"]
                 download_links.append('href="' + url + '" ' + hoster + '<')
```

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/metadata/imdb.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/metadata/imdb.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/content_all.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/content_all.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/content_shows.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/content_shows.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/shared.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/shared.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_by.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_by.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_dw.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_dw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_fx.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_fx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_hw.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_hw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_nk.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_nk.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_nx.py` & `feedcrawler-18.0.5/feedcrawler/external_sites/web_search/sites/content_all_nx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_tools/myjd_api.py` & `feedcrawler-18.0.5/feedcrawler/external_tools/myjd_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_tools/ombi_api.py` & `feedcrawler-18.0.5/feedcrawler/external_tools/ombi_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_tools/overseerr_api.py` & `feedcrawler-18.0.5/feedcrawler/external_tools/overseerr_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/external_tools/plex_api.py` & `feedcrawler-18.0.5/feedcrawler/external_tools/plex_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/jobs/feed_search.py` & `feedcrawler-18.0.5/feedcrawler/jobs/feed_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,21 +79,21 @@
         SJ(filename='List_ContentAll_Seasons'),
         DJ(filename='List_CustomDJ_Documentaries'),
         DJ(filename='List_CustomDJ_Documentaries_Regex'),
         DD(filename='List_CustomDD_Feeds')
     ]
 
 
-def feed_crawler(shared_state_dict):
+def feed_crawler(shared_state_dict, shared_state_lock):
     if gui.enabled:
-        sys.stdout = gui.AppendToPrintQueue(shared_state_dict)
+        sys.stdout = gui.AppendToPrintQueue(shared_state_dict, shared_state_lock)
     else:
         sys.stdout = Unbuffered(sys.stdout)
 
-    shared_state.set_shared_dict(shared_state_dict)
+    shared_state.set_state(shared_state_dict, shared_state_lock)
     shared_state.set_logger()
     logger = shared_state.logger
 
     request_management_first_run = True
     crawltimes = FeedDb("crawltimes")
     feedcrawler = CrawlerConfig('FeedCrawler')
```

### Comparing `feedcrawler-18.0.4/feedcrawler/jobs/package_watcher.py` & `feedcrawler-18.0.5/feedcrawler/jobs/package_watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 from feedcrawler.providers.myjd_connection import reset_in_downloads
 from feedcrawler.providers.myjd_connection import retry_decrypt
 from feedcrawler.providers.myjd_connection import set_device_from_config
 from feedcrawler.providers.notifications import notify
 from feedcrawler.providers.sqlite_database import FeedDb
 
 
-def watch_packages(shared_state_dict):
+def watch_packages(shared_state_dict, shared_state_lock):
     if gui.enabled:
-        sys.stdout = gui.AppendToPrintQueue(shared_state_dict)
+        sys.stdout = gui.AppendToPrintQueue(shared_state_dict, shared_state_lock)
     else:
         sys.stdout = Unbuffered(sys.stdout)
 
-    shared_state.set_shared_dict(shared_state_dict)
+    shared_state.set_state(shared_state_dict, shared_state_lock)
     shared_state.set_logger()
 
     crawljobs = CrawlerConfig('Crawljobs')
     autostart = crawljobs.get("autostart")
     db = FeedDb('crawldog')
 
     grabber_was_collecting = False
```

### Comparing `feedcrawler-18.0.4/feedcrawler/providers/common_functions.py` & `feedcrawler-18.0.5/feedcrawler/providers/common_functions.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/providers/config.py` & `feedcrawler-18.0.5/feedcrawler/providers/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from feedcrawler.providers import shared_state
 from feedcrawler.providers.sqlite_database import FeedDb
 
 
 class CrawlerConfig(object):
     _DEFAULT_CONFIG = {
         'FeedCrawler': [
-            ("auth_user", "str", ""),
+            ("auth_user", "secret", ""),
             ("auth_hash", "secret", ""),
-            ("myjd_user", "str", ""),
+            ("myjd_user", "secret", ""),
             ("myjd_pass", "secret", ""),
             ("myjd_device", "str", ""),
             ("myjd_auto_update", "bool", "False"),
             ("port", "int", "9090"),
             ("prefix", "str", ""),
             ("interval", "int", "60"),
             ("sponsors_helper", "str", ""),
@@ -196,14 +196,16 @@
             if value.startswith("secret|"):
                 crypt_key, crypt_iv = self._get_encryption_params()
                 cipher = AES.new(crypt_key, AES.MODE_CBC, crypt_iv)
                 decrypted_payload = cipher.decrypt(base64.b64decode(value[7:])).decode("utf-8").strip()
                 final_payload = "".join(filter(lambda c: c in string.printable, decrypted_payload))
                 return final_payload
             else:  ## Loaded value is not encrypted, return as is
+                if len(value) > 0:
+                    self.save(key, value)
                 return value
         elif [param for param in self._DEFAULT_CONFIG[self._section] if param[0] == key and param[1] == 'bool']:
             return True if len(res) and res[0].strip('\'"').lower() == 'true' else False
         else:
             return res[0].strip('\'"') if len(res) > 0 else False
 
     def save(self, key, value):
```

### Comparing `feedcrawler-18.0.4/feedcrawler/providers/gui.py` & `feedcrawler-18.0.5/feedcrawler/providers/gui.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     window.hide()
 
     return window
 
 
 @check_gui_enabled
-def main_gui(window, shared_state_dict):
+def main_gui(window, shared_state_dict, shared_state_lock):
     if not window:
         print("GUI-Fenster falsch initialisiert.")
         window = create_main_window()
     try:
         menu = ['', [title,
                      '---',
                      'GUI',
@@ -96,15 +96,15 @@
                 ]
         tray = SystemTray(menu, single_click_events=False, window=window, tooltip='Tooltip', icon=get_icon())
         tray.show_message(title, 'Gestartet und im Tray verfügbar.')
 
         while True:
             event, values = window.read(timeout=500)
 
-            print_from_queue(shared_state_dict)
+            print_from_queue(shared_state_dict, shared_state_lock)
 
             if event == tray.key:
                 event = values[event]  # use the System Tray's event as if was from the window
 
             if event in 'Beenden':
                 break
 
@@ -315,30 +315,41 @@
         self.terminal.write(message)
         self.gui.write(message)
 
     def flush(self):
         pass
 
 
+def update_shared_dict_with_lock(shared_dict, shared_lock, key, value):
+    shared_lock.acquire()
+    try:
+        shared_dict[key] = value
+    finally:
+        shared_lock.release()
+
+
 class AppendToPrintQueue(object):
-    def __init__(self, shared_state_dict):
+    def __init__(self, shared_state_dict, shared_state_lock):
         self.shared_state_dict = shared_state_dict
+        self.shared_state_lock = shared_state_lock
         try:
             self.shared_state_dict["print_queue"]
         except KeyError:
-            self.shared_state_dict["print_queue"] = ''
+            update_shared_dict_with_lock(self.shared_state_dict, self.shared_state_lock, "print_queue", '')
 
     def write(self, s):
-        self.shared_state_dict["print_queue"] += s
+        update_shared_dict_with_lock(self.shared_state_dict, self.shared_state_lock, "print_queue",
+                                     self.shared_state_dict["print_queue"] + s)
 
     def flush(self):
-        self.shared_state_dict["print_queue"] += ''
+        update_shared_dict_with_lock(self.shared_state_dict, self.shared_state_lock, "print_queue",
+                                     self.shared_state_dict["print_queue"] + '')
 
 
-def print_from_queue(shared_state_dict):
+def print_from_queue(shared_state_dict, shared_state_lock):
     try:
         output = shared_state_dict["print_queue"]
         if len(output) > 0:
             print(output)
-            shared_state_dict["print_queue"] = ''
+            update_shared_dict_with_lock(shared_state_dict, shared_state_lock, "print_queue", '')
     except KeyError:
         pass
```

### Comparing `feedcrawler-18.0.4/feedcrawler/providers/http_requests/cache_handler.py` & `feedcrawler-18.0.5/feedcrawler/providers/http_requests/cache_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 
         try:
             cached_response = shared_state.values["request_" + function_arguments_hash]
         except KeyError:
             cached_response = None
         if cached_response:
             try:
-                shared_state.values["request_cache_hits"] += 1
+                shared_state.update("request_cache_hits", shared_state.values["request_cache_hits"] + 1)
             except KeyError:
-                shared_state.values["request_cache_hits"] = 1
+                shared_state.update("request_cache_hits", 1)
             return cached_response
         else:
             #
             value = func(*args, **kwargs)
             if caching_allowed:
-                shared_state.values["request_" + function_arguments_hash] = value
+                shared_state.update("request_" + function_arguments_hash, value)
             return value
 
     return cache_returned_values
 
 
 @cache
 def cached_request(url, method='get', params=None, headers=None, redirect_url=False, dont_cache=False):
```

### Comparing `feedcrawler-18.0.4/feedcrawler/providers/http_requests/cloudflare_handlers.py` & `feedcrawler-18.0.5/feedcrawler/providers/http_requests/cloudflare_handlers.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/providers/http_requests/request_handler.py` & `feedcrawler-18.0.5/feedcrawler/providers/http_requests/request_handler.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/providers/myjd_connection.py` & `feedcrawler-18.0.5/feedcrawler/providers/myjd_connection.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/providers/notifications.py` & `feedcrawler-18.0.5/feedcrawler/providers/notifications.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/providers/shared_state.py` & `feedcrawler-18.0.5/feedcrawler/providers/shared_state.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,43 +10,49 @@
 from logging import handlers
 
 from feedcrawler.external_tools.myjd_api import Jddevice, Myjdapi
 from feedcrawler.external_tools.myjd_api import TokenExpiredException, RequestTimeoutException, MYJDException
 from feedcrawler.providers.config import CrawlerConfig
 
 values = {}
+lock = None
 logger = None
 
 
-def set_shared_dict(manager_dict):
+def set_state(manager_dict, manager_lock):
     global values
+    global lock
     values = manager_dict
+    lock = manager_lock
 
 
-def set_initial_values(test_run, remove_cloudflare_time):
+def update(key, value):
     global values
-    values["test_run"] = test_run
-    values["remove_cloudflare_time"] = remove_cloudflare_time
-    values["ww_blocked"] = False
-    values["sf_blocked"] = False
-    values["user_agent"] = 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) ' \
-                           'Chrome/111.0.0.0 Safari/537.36'
+    global lock
+    lock.acquire()
+    try:
+        values[key] = value
+    finally:
+        lock.release()
 
 
-def set_files(configpath):
-    global values
-    values["configfile"] = os.path.join(configpath, "FeedCrawler.ini")
-    values["dbfile"] = os.path.join(configpath, "FeedCrawler.db")
-    values["log_file"] = os.path.join(configpath, 'FeedCrawler.log')
-    values["log_file_debug"] = os.path.join(configpath, 'FeedCrawler_DEBUG.log')
+def set_initial_values(test_run, remove_cloudflare_time):
+    update("test_run", test_run)
+    update("remove_cloudflare_time", remove_cloudflare_time)
+    update("ww_blocked", False)
+    update("sf_blocked", False)
+    update("user_agent", 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) ' \
+                         'Chrome/111.0.0.0 Safari/537.36')
 
 
-def set_log_level(log_level):
-    global values
-    values["log_level"] = log_level
+def set_files(config_path):
+    update("configfile", os.path.join(config_path, "FeedCrawler.ini"))
+    update("dbfile", os.path.join(config_path, "FeedCrawler.db"))
+    update("log_file", os.path.join(config_path, 'FeedCrawler.log'))
+    update("log_file_debug", os.path.join(config_path, 'FeedCrawler_DEBUG.log'))
 
 
 def set_logger():
     global logger
 
     log_level = values["log_level"]
 
@@ -70,34 +76,30 @@
             logfile_debug = logging.handlers.RotatingFileHandler(values["log_file_debug"])
             logfile_debug.setFormatter(formatter)
             logfile_debug.setLevel(10)
             logger.addHandler(logfile_debug)
 
 
 def set_sites():
-    global values
-    values["sites"] = ["FX", "SF", "DW", "HW", "FF", "BY", "NK", "NX", "WW", "SJ", "DJ", "DD"]
+    update("sites", ["FX", "SF", "DW", "HW", "FF", "BY", "NK", "NX", "WW", "SJ", "DJ", "DD"])
 
 
 def set_device(new_device):
-    global values
-    values["device"] = new_device
+    update("device", new_device)
 
 
 def check_device(device):
     try:
         valid = isinstance(device, (type, Jddevice)) and device.downloadcontroller.get_current_state()
     except (AttributeError, KeyError, TokenExpiredException, RequestTimeoutException, MYJDException):
         valid = False
     return valid
 
 
 def connect_device():
-    global values
-
     device = False
     conf = CrawlerConfig('FeedCrawler')
     myjd_user = str(conf.get('myjd_user'))
     myjd_pass = str(conf.get('myjd_pass'))
     myjd_device = str(conf.get('myjd_device'))
 
     jd = Myjdapi()
@@ -108,52 +110,55 @@
             jd.connect(myjd_user, myjd_pass)
             jd.update_devices()
             device = jd.get_device(myjd_device)
         except (TokenExpiredException, RequestTimeoutException, MYJDException):
             pass
 
     if check_device(device):
-        values["device"] = device
+        update("device", device)
         return True
     else:
         return False
 
 
 def get_device():
-    global values
     attempts = 0
 
     while True:
         try:
             if check_device(values["device"]):
                 break
         except (AttributeError, KeyError, TokenExpiredException, RequestTimeoutException, MYJDException):
             pass
         attempts += 1
 
-        values["device"] = False
+        update("device", False)
 
         if attempts % 10 == 0:
             print(
                 f"WARNUNG: {attempts} aufeinanderfolgende My JDownloader Verbindungsfehler. Bitte prüfen und ggf. neu starten!")
         time.sleep(3)
 
         if connect_device():
             break
 
     return values["device"]
 
 
 def set_connection_info(local_address, port, prefix, docker):
-    global values
-    values["local_address"] = local_address
-    values["port"] = port
-    values["prefix"] = prefix
-    values["docker"] = docker
+    update("local_address", local_address)
+    update("port", port)
+    update("prefix", prefix)
+    update("docker", docker)
 
 
 def clear_request_cache():
     global values
-    for key in list(values.keys()):
-        if key.startswith('request_'):
-            values.pop(key)
-    values["request_cache_hits"] = 0
+    global lock
+    lock.acquire()
+    try:
+        for key in list(values.keys()):
+            if key.startswith('request_'):
+                values.pop(key)
+    finally:
+        lock.release()
+    update("request_cache_hits", 0)
```

### Comparing `feedcrawler-18.0.4/feedcrawler/providers/sqlite_database.py` & `feedcrawler-18.0.5/feedcrawler/providers/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/providers/url_functions.py` & `feedcrawler-18.0.5/feedcrawler/providers/url_functions.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/providers/version.py` & `feedcrawler-18.0.5/feedcrawler/providers/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import re
 from distutils.version import StrictVersion
 from urllib.request import urlopen
 
 
 def get_version():
-    return "18.0.4"
+    return "18.0.5"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub('[^\d\.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-44ade789.js` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-ffd92ad0.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -300,15 +300,15 @@
                 }, [e("button", {
                     "aria-controls": "offcanvasBottomLists",
                     class: "btn btn-outline-primary",
                     "data-bs-target": "#offcanvasBottomLists",
                     "data-bs-toggle": "offcanvas",
                     type: "button",
                     onClick: d
-                }, [bt, r(" Suchlisten ")])]), e("div", {
+                }, [bt, r(" Feed-Suche ")])]), e("div", {
                     class: "col-md-auto p-1"
                 }, [e("button", {
                     "aria-controls": "offcanvasBottomSettings",
                     class: "btn btn-outline-primary",
                     "data-bs-target": "#offcanvasBottomSettings",
                     "data-bs-toggle": "offcanvas",
                     type: "button",
@@ -1787,15 +1787,15 @@
                         "messages-class": "text-danger",
                         placeholder: "Film- oder Serien-Titel eingeben",
                         type: "text",
                         validation: "required|length:3"
                     }, null, 8, ["modelValue"])]),
                     _: 1
                 })])), [
-                    [R, "Bequeme Suchfunktion für " + s(t).state.hostnames.search + ". Bei hellblau hinterlegten Serien werden alle verfügbaren Staffeln/Folgen hinzugefügt. Komplette Serien landen auch in der Suchliste. Alternativ kann eine einzelne Staffel/Folge per Komma am Titel ergänzt werden: 'Serien Titel,S01' oder 'Serien Titel,S01E01'. Die für die Feed-Suche gesetzte Auflösung und Filterliste werden berücksichtigt, aber nicht forciert. Bereits geladene Releases werden hier nicht ignoriert!"]
+                    [R, "Bequeme Suchfunktion für " + s(t).state.hostnames.search + ". Bei hellblau hinterlegten Serien werden alle verfügbaren Staffeln/Folgen hinzugefügt. Komplette Serien landen auch in der Suchliste für die Feed-Suche. Alternativ kann eine einzelne Staffel/Folge per Komma am Titel ergänzt werden: 'Serien Titel,S01' oder 'Serien Titel,S01E01'. Die für die Feed-Suche gesetzte Auflösung und Filterliste werden berücksichtigt, aber nicht forciert. Bereits geladene Releases werden hier nicht ignoriert!"]
                 ]), e("div", jn, [e("div", Hn, [h(e("input", {
                     class: "form-check-input",
                     type: "checkbox",
                     id: "flexSwitchMovies",
                     "onUpdate:modelValue": w[3] || (w[3] = P => f.value = P)
                 }, null, 512), [
                     [ke, f.value]
@@ -1850,15 +1850,15 @@
     io = e("div", {
         class: "offcanvas-header"
     }, [e("h3", {
         id: "offcanvasBottomListsLabel",
         class: "offcanvas-title"
     }, [e("i", {
         class: "bi bi-text-left"
-    }), r(" Suchlisten ")]), e("button", {
+    }), r(" Listen für die Feed-Suche ")]), e("button", {
         "aria-label": "Close",
         class: "btn-close text-reset",
         "data-bs-dismiss": "offcanvas",
         type: "button"
     })], -1),
     ro = {
         class: "offcanvas-body"
@@ -2080,15 +2080,15 @@
                     "incomplete-message": "Es müssen alle Felder korrekt ausgefüllt werden! Fehler sind rot markiert.",
                     "messages-class": "text-danger",
                     type: "form",
                     onSubmit: V[10] || (V[10] = o => _())
                 }, {
                     default: M(({
                         value: o
-                    }) => [s(t).state.misc.loaded_lists ? i("", !0) : (l(), a("h4", co, "Suchlisten werden geladen...")), s(t).state.misc.loaded_lists ? (l(), a("div", uo, [s(t).state.hostnames.bl !== "Nicht gesetzt!" ? (l(), a("div", ho, [e("h2", mo, [e("button", go, " Filme (" + p(s(t).state.hostnames.bl) + ") ", 1)]), e("div", po, [e("div", bo, [h((l(), a("div", null, [u(y, {
+                    }) => [s(t).state.misc.loaded_lists ? i("", !0) : (l(), a("h4", co, "Listen werden geladen...")), s(t).state.misc.loaded_lists ? (l(), a("div", uo, [s(t).state.hostnames.bl !== "Nicht gesetzt!" ? (l(), a("div", ho, [e("h2", mo, [e("button", go, " Filme (" + p(s(t).state.hostnames.bl) + ") ", 1)]), e("div", po, [e("div", bo, [h((l(), a("div", null, [u(y, {
                         modelValue: s(t).state.lists.mb.filme,
                         "onUpdate:modelValue": V[0] || (V[0] = d => s(t).state.lists.mb.filme = d),
                         validation: [
                             ["?matches", /^[a-zA-Z0-9ÄäÖöÜüß\-+&\s]+$/]
                         ],
                         "validation-messages": {
                             matches: "Bitte nur Buchstaben, Zahlen, Leerzeichen oder folgende Sonderzeichen eingeben: - + &"
@@ -3519,15 +3519,15 @@
                         label: "Ombi API-Key",
                         "messages-class": "text-danger",
                         name: "ombi_api",
                         "outer-class": "mb-4",
                         placeholder: "Bspw. UQ6oVaEuPR3CyyhEfi2uT32PrRJfitfv3WG",
                         type: "text",
                         "validation-visibility": "live"
-                    }, null, 8, ["modelValue", "validation", "validation-messages"])])])]), s(t).state.hostnames.bl !== "Nicht gesetzt!" ? (l(), a("div", Lr, [e("h2", Br, [e("button", jr, p(s(t).state.hostnames.bl), 1)]), e("div", Hr, [e("div", Fr, [u(d, {
+                    }, null, 8, ["modelValue", "validation", "validation-messages"])])])]), s(t).state.hostnames.bl !== "Nicht gesetzt!" ? (l(), a("div", Lr, [e("h2", Br, [e("button", jr, " Filme (" + p(s(t).state.hostnames.bl) + ") ", 1)]), e("div", Hr, [e("div", Fr, [u(d, {
                         modelValue: s(t).state.settings.mb.quality,
                         "onUpdate:modelValue": o[43] || (o[43] = n => s(t).state.settings.mb.quality = n),
                         help: "Die Release-Auflösung, nach der gesucht wird.",
                         "help-class": "text-muted",
                         "input-class": "form-control bg-light mb-2",
                         label: "Auflösung",
                         "messages-class": "text-danger",
@@ -3690,15 +3690,15 @@
                         "outer-class": "mb-4",
                         type: "select"
                     }, {
                         default: M(() => [(l(), a(E, null, T(v, n => e("option", {
                             value: n.value
                         }, p(n.label), 9, tc)), 64))]),
                         _: 2
-                    }, 1032, ["modelValue"])])) : i("", !0)])])])) : i("", !0), s(t).state.hostnames.s !== "Nicht gesetzt!" ? (l(), a("div", sc, [e("h2", lc, [e("button", ac, p(s(t).state.hostnames.s), 1)]), e("div", nc, [e("div", oc, [u(d, {
+                    }, 1032, ["modelValue"])])) : i("", !0)])])])) : i("", !0), s(t).state.hostnames.s !== "Nicht gesetzt!" ? (l(), a("div", sc, [e("h2", lc, [e("button", ac, " Folgen (" + p(s(t).state.hostnames.s) + ") ", 1)]), e("div", nc, [e("div", oc, [u(d, {
                         modelValue: s(t).state.settings.sj.quality,
                         "onUpdate:modelValue": o[58] || (o[58] = n => s(t).state.settings.sj.quality = n),
                         help: "Die Release-Auflösung, nach der gesucht wird.",
                         "help-class": "text-muted",
                         "input-class": "form-control bg-light mb-2",
                         label: "Auflösung",
                         "messages-class": "text-danger",
@@ -3813,15 +3813,15 @@
                         label: "Suchtiefe",
                         "messages-class": "text-danger",
                         "outer-class": "mb-4",
                         placeholder: "Bspw. 3",
                         type: "number",
                         validation: "required|between:1,7",
                         "validation-visibility": "live"
-                    }, null, 8, ["modelValue"])])) : i("", !0)])) : i("", !0)])])])) : i("", !0), s(t).state.hostnames.sjbl !== "Nicht gesetzt!" && s(t).state.settings.mbsj.enabled && s(t).state.misc.sjbl_enabled ? (l(), a("div", xc, [e("h2", Sc, [e("button", Vc, p(s(t).state.hostnames.sjbl), 1)]), e("div", Cc, [e("div", Dc, [zc, e("label", Lc, [u(d, {
+                    }, null, 8, ["modelValue"])])) : i("", !0)])) : i("", !0)])])])) : i("", !0), s(t).state.hostnames.sjbl !== "Nicht gesetzt!" && s(t).state.settings.mbsj.enabled && s(t).state.misc.sjbl_enabled ? (l(), a("div", xc, [e("h2", Sc, [e("button", Vc, " Staffeln (" + p(s(t).state.hostnames.sjbl) + ") ", 1)]), e("div", Cc, [e("div", Dc, [zc, e("label", Lc, [u(d, {
                         modelValue: s(t).state.settings.mbsj.enabled,
                         "onUpdate:modelValue": o[69] || (o[69] = n => s(t).state.settings.mbsj.enabled = n),
                         help: "Wenn aktiviert, werden komplette Staffeln entsprechend der Staffel-Liste gesucht.",
                         "help-class": "text-muted",
                         "input-class": "form-check-input",
                         "messages-class": "text-danger",
                         "outer-class": "mb-4",
@@ -3874,15 +3874,15 @@
                         label: "Suchtiefe",
                         "messages-class": "text-danger",
                         "outer-class": "mb-4",
                         placeholder: "Bspw. 3",
                         type: "number",
                         validation: "required|between:1,7",
                         "validation-visibility": "live"
-                    }, null, 8, ["modelValue"])])) : i("", !0)])])])) : i("", !0), s(t).state.hostnames.dj !== "Nicht gesetzt!" ? (l(), a("div", Uc, [e("h2", Pc, [e("button", Nc, p(s(t).state.hostnames.dj), 1)]), e("div", Ec, [e("div", Tc, [u(d, {
+                    }, null, 8, ["modelValue"])])) : i("", !0)])])])) : i("", !0), s(t).state.hostnames.dj !== "Nicht gesetzt!" ? (l(), a("div", Uc, [e("h2", Pc, [e("button", Nc, " Dokus (" + p(s(t).state.hostnames.dj) + ") ", 1)]), e("div", Ec, [e("div", Tc, [u(d, {
                         modelValue: s(t).state.settings.dj.quality,
                         "onUpdate:modelValue": o[74] || (o[74] = n => s(t).state.settings.dj.quality = n),
                         help: "Die Release-Auflösung, nach der gesucht wird.",
                         "help-class": "text-muted",
                         "input-class": "form-control bg-light mb-2",
                         label: "Auflösung",
                         "messages-class": "text-danger",
@@ -3918,24 +3918,24 @@
                         "onUpdate:modelValue": o[77] || (o[77] = n => s(t).state.settings.dj.hoster_fallback = n),
                         help: "Wenn aktiviert, und sofern kein anderer Link gefunden werden konnte, werden alle gefundenen Hoster akzeptiert!",
                         "help-class": "text-muted",
                         "input-class": "form-check-input",
                         "messages-class": "text-danger",
                         "outer-class": "mb-4",
                         type: "checkbox"
-                    }, null, 8, ["modelValue"])])])])])) : i("", !0), s(t).state.hostnames.dd !== "Nicht gesetzt!" ? (l(), a("div", Mc, [e("h2", Ic, [e("button", Zc, p(s(t).state.hostnames.dd), 1)]), e("div", Oc, [e("div", Gc, [Xc, e("label", Qc, [u(d, {
+                    }, null, 8, ["modelValue"])])])])])) : i("", !0), s(t).state.hostnames.dd !== "Nicht gesetzt!" ? (l(), a("div", Mc, [e("h2", Ic, [e("button", Zc, " Folgen (" + p(s(t).state.hostnames.dd) + ") ", 1)]), e("div", Oc, [e("div", Gc, [Xc, e("label", Qc, [u(d, {
                         modelValue: s(t).state.settings.dd.hoster_fallback,
                         "onUpdate:modelValue": o[78] || (o[78] = n => s(t).state.settings.dd.hoster_fallback = n),
                         help: "Wenn aktiviert, und sofern kein anderer Link gefunden werden konnte, werden alle gefundenen Hoster akzeptiert!",
                         "help-class": "text-muted",
                         "input-class": "form-check-input",
                         "messages-class": "text-danger",
                         "outer-class": "mb-4",
                         type: "checkbox"
-                    }, null, 8, ["modelValue"])])])])])) : i("", !0), s(t).state.hostnames.f !== "Nicht gesetzt!" && s(t).state.hostnames.f !== s(t).state.hostnames.sjbl ? (l(), a("div", Yc, [e("h2", ed, [e("button", td, p(s(t).state.hostnames.f), 1)]), e("div", sd, [e("div", ld, [u(d, {
+                    }, null, 8, ["modelValue"])])])])])) : i("", !0), s(t).state.hostnames.f !== "Nicht gesetzt!" && s(t).state.hostnames.f !== s(t).state.hostnames.sjbl ? (l(), a("div", Yc, [e("h2", ed, [e("button", td, " Sonstiges (" + p(s(t).state.hostnames.f) + ") ", 1)]), e("div", sd, [e("div", ld, [u(d, {
                         modelValue: s(t).state.settings.f.search,
                         "onUpdate:modelValue": o[79] || (o[79] = n => s(t).state.settings.f.search = n),
                         help: "Die Suchtiefe in Tagen sollte nicht zu hoch angesetzt werden, um keinen Ban zu riskieren.",
                         "help-class": "text-muted",
                         "input-class": " form-control bg-light mb-2",
                         label: "Suchtiefe",
                         "messages-class": "text-danger",
```

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/index.html` & `feedcrawler-18.0.5/feedcrawler/web_interface/vuejs_frontend/dist/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <head>
     <meta charset="UTF-8">
     <meta content="width=device-width, initial-scale=1, shrink-to-fit=no" name="viewport">
 
     <link href="./favicon.ico" rel="icon" type="image/x-icon">
 
     <title>FeedCrawler</title>
-  <script type="module" crossorigin src="./assets/index-44ade789.js"></script>
+  <script type="module" crossorigin src="./assets/index-ffd92ad0.js"></script>
   <link rel="modulepreload" crossorigin href="./assets/@vue-d42f3502.js">
   <link rel="modulepreload" crossorigin href="./assets/vuex-c2e7db49.js">
   <link rel="modulepreload" crossorigin href="./assets/axios-707ed124.js">
   <link rel="modulepreload" crossorigin href="./assets/vue-router-4bccd9ac.js">
   <link rel="modulepreload" crossorigin href="./assets/@popperjs-9847b28c.js">
   <link rel="modulepreload" crossorigin href="./assets/bootstrap-163e1b4f.js">
   <link rel="modulepreload" crossorigin href="./assets/vue-toastification-2a2137d8.js">
```

### Comparing `feedcrawler-18.0.4/feedcrawler/web_interface/web_server.py` & `feedcrawler-18.0.5/feedcrawler/web_interface/web_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -2019,17 +2019,17 @@
         updateversion = version.update_check()[1]
         print('Update steht bereit (' + updateversion +
               ')! Weitere Informationen unter https://github.com/rix1337/FeedCrawler/releases/latest')
 
     app_container()
 
 
-def web_server(shared_state_dict):
+def web_server(shared_state_dict, shared_state_lock):
     if gui.enabled:
-        sys.stdout = gui.AppendToPrintQueue(shared_state_dict)
+        sys.stdout = gui.AppendToPrintQueue(shared_state_dict, shared_state_lock)
     else:
         sys.stdout = Unbuffered(sys.stdout)
 
-    shared_state.set_shared_dict(shared_state_dict)
+    shared_state.set_state(shared_state_dict, shared_state_lock)
     shared_state.set_logger()
 
     start()
```

### Comparing `feedcrawler-18.0.4/feedcrawler.egg-info/PKG-INFO` & `feedcrawler-18.0.5/feedcrawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedcrawler
-Version: 18.0.4
+Version: 18.0.5
 Summary: Automate downloads using predefined sites and the My JDownloader API
 Home-page: https://github.com/rix1337/FeedCrawler
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `feedcrawler-18.0.4/feedcrawler.egg-info/SOURCES.txt` & `feedcrawler-18.0.5/feedcrawler.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js
 feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js
 feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css
 feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
 feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
 feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css
 feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css
-feedcrawler/web_interface/vuejs_frontend/dist/assets/index-44ade789.js
+feedcrawler/web_interface/vuejs_frontend/dist/assets/index-ffd92ad0.js
 feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
 feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
 feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js
 feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js
 feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js
 feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
 feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js
```

### Comparing `feedcrawler-18.0.4/setup.py` & `feedcrawler-18.0.5/setup.py`

 * *Files identical despite different names*

